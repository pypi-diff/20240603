# Comparing `tmp/phonexia_speaker_diarization_client-1.1.0.tar.gz` & `tmp/phonexia_speaker_diarization_client-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phonexia_speaker_diarization_client-1.1.0.tar", max compression
+gzip compressed data, was "phonexia_speaker_diarization_client-1.2.0.tar", max compression
```

## Comparing `phonexia_speaker_diarization_client-1.1.0.tar` & `phonexia_speaker_diarization_client-1.2.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     9289 2024-02-26 08:06:54.464982 phonexia_speaker_diarization_client-1.1.0/phonexia_speaker_diarization_client.py
--rw-r--r--   0        0        0      749 2024-02-26 08:06:54.464982 phonexia_speaker_diarization_client-1.1.0/pypi-README.md
--rw-r--r--   0        0        0     2050 2024-02-26 08:07:09.621235 phonexia_speaker_diarization_client-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     1867 1970-01-01 00:00:00.000000 phonexia_speaker_diarization_client-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0    10159 2024-06-03 06:44:46.080577 phonexia_speaker_diarization_client-1.2.0/phonexia_speaker_diarization_client.py
+-rw-r--r--   0        0        0      749 2024-06-03 06:44:46.080577 phonexia_speaker_diarization_client-1.2.0/pypi-README.md
+-rw-r--r--   0        0        0     2050 2024-06-03 06:45:02.557856 phonexia_speaker_diarization_client-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1867 1970-01-01 00:00:00.000000 phonexia_speaker_diarization_client-1.2.0/PKG-INFO
```

### Comparing `phonexia_speaker_diarization_client-1.1.0/phonexia_speaker_diarization_client.py` & `phonexia_speaker_diarization_client-1.2.0/phonexia_speaker_diarization_client.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 #!/usr/bin/python3
 
 import argparse
 import fnmatch
 import logging
 import os
+import sys
 from pathlib import Path
 from typing import Iterator, Optional
 
 import google.protobuf.duration_pb2
 import grpc
 import phonexia.grpc.common.core_pb2 as phx_common
 import phonexia.grpc.technologies.speaker_diarization.v1.speaker_diarization_pb2 as diarization
 import phonexia.grpc.technologies.speaker_diarization.v1.speaker_diarization_pb2_grpc as diarization_grpc
+from google.protobuf.json_format import MessageToJson
 
 CHUNK_SIZE = 1024 * 1024
 
 
 class speaker_diarization_client:
     def __init__(
         self,
         host: str,
         use_ssl: bool,
         max_speakers: Optional[int] = None,
         total_speakers: Optional[int] = None,
         output_format="lab",
+        metadata: Optional[list] = None,
     ):
         if use_ssl:
             logging.info("Connecting to %s via secure channel", host)
             credentials = grpc.ssl_channel_credentials()
             self.channel = grpc.secure_channel(host, credentials)
         else:
             logging.info("Connecting to %s via insecure channel", host)
@@ -37,19 +40,20 @@
         self.total_speakers = total_speakers
         logging.info(
             "Using max_speakers=%s and total_speakers=%s",
             self.max_speakers,
             self.total_speakers,
         )
         self.diarize_stub = diarization_grpc.SpeakerDiarizationStub(self.channel)
-        if output_format not in {"lab", "rttm"}:
+        if output_format not in {"lab", "rttm", "json"}:
             raise ValueError("Unsupported output format")
         self.format = output_format
+        self.metadata = metadata
 
-    def time_to_duration(self, time: float) -> google.protobuf.duration_pb2.Duration | None:
+    def time_to_duration(self, time: float) -> Optional[google.protobuf.duration_pb2.Duration]:
         if time is None:
             return None
         duration = google.protobuf.duration_pb2.Duration()
         duration.seconds = int(time)
         duration.nanos = int((time - duration.seconds) * 1e9)
         return duration
 
@@ -75,86 +79,85 @@
                 request.audio.content = chunk
                 logging.debug("Sending chunk of size %d", len(chunk))
                 yield request
                 request.audio.ClearField("time_range")
                 request.config.ClearField("total_speakers")
                 request.config.ClearField("max_speakers")
 
-    def save_response_lab(self, response: diarization.DiarizeResponse, file: Path):
+    def save_response_lab(self, response: diarization.DiarizeResponse, output):
         def to_htk(sec: float):
             return int(round(sec * 10**7, ndigits=0))
 
-        with open(file, "w", encoding="utf8") as fd:
-            for segment in response.segments:
-                print(
-                    "{:d} {:d} {:d}".format(
-                        to_htk(segment.start_time.ToTimedelta().total_seconds()),
-                        to_htk(segment.end_time.ToTimedelta().total_seconds()),
-                        int(segment.speaker_id) + 1,
-                    ),
-                    file=fd,
+        for segment in response.segments:
+            output.write(
+                "{start:d} {end:d} {speaker:d}\n".format(  # noqa: UP032
+                    start=to_htk(segment.start_time.ToTimedelta().total_seconds()),
+                    end=to_htk(segment.end_time.ToTimedelta().total_seconds()),
+                    speaker=int(segment.speaker_id) + 1,
                 )
+            )
 
-    def save_response_rttm(self, response: diarization.DiarizeResponse, file: Path):
-        with open(file, "w", encoding="utf8") as fd:
-            for segment in response.segments:
-                beg = segment.start_time.ToTimedelta().total_seconds()
-                end = segment.end_time.ToTimedelta().total_seconds()
-                size = end - beg
-                print(
-                    f"SPEAKER {file.stem} 1 {beg:.2f} {size:.2f} <NA> <NA>"
-                    f" {int(segment.speaker_id) + 1} <NA>",
-                    file=fd,
-                )
+    def save_response_rttm(self, response: diarization.DiarizeResponse, file: Path, output):
+        for segment in response.segments:
+            beg = segment.start_time.ToTimedelta().total_seconds()
+            end = segment.end_time.ToTimedelta().total_seconds()
+            size = end - beg
+            output.write(
+                f"SPEAKER {file.stem} 1 {beg:.2f} {size:.2f} <NA> <NA>"
+                f" {int(segment.speaker_id) + 1} <NA>\n"
+            )
 
     def send_diarize_request(
         self, request: Iterator[diarization.DiarizeRequest]
     ) -> diarization.DiarizeResponse:
-        return self.diarize_stub.Diarize(request)
+        return self.diarize_stub.Diarize(request, metadata=self.metadata)
 
     def process_file(
         self,
         in_file: Path,
         start: Optional[float] = None,
         end: Optional[float] = None,
-        output: Optional[Path] = None,
+        output_file: Optional[Path] = None,
     ):
-        if output is None:
-            output = in_file.with_suffix("." + self.format)
-
-        logging.info("%s -> %s", in_file, output)
+        logging.info("%s -> %s", in_file, output_file if output_file else "stdout")
 
         response = self.send_diarize_request(self.file_to_request(in_file, start, end))
 
+        output = open(output_file, "w", encoding="utf8") if output_file else sys.stdout  # noqa: SIM115
+
         if self.format == "lab":
             self.save_response_lab(response, output)
-        if self.format == "rttm":
-            self.save_response_rttm(response, output)
+        elif self.format == "rttm":
+            self.save_response_rttm(response, in_file, output)
+        elif self.format == "json":
+            output.write(MessageToJson(response))
+
+        if output_file:
+            output.close()
 
     def process_dir(
         self,
         in_dir: Path,
         start: Optional[float] = None,
         end: Optional[float] = None,
         output: Optional[Path] = None,
         input_suffix: str = "wav",
     ):
-        if output is None:
-            output = in_dir
-
-        if not output.exists:
+        if output is not None and not output.exists:
             os.mkdir(output)
 
         logging.info("Scanning directory %s for *.%s", os.path.abspath(in_dir), input_suffix)
         files = os.listdir(in_dir)
         filtered_files = [f for f in files if fnmatch.fnmatch(f, f"*.{input_suffix}")]
         logging.info("Found %d files", len(filtered_files))
         for file in filtered_files:
             in_file = in_dir / file
-            out_file = (Path(output) / file).with_suffix("." + self.format)
+            out_file = (
+                None if output is None else (Path(output) / file).with_suffix("." + self.format)
+            )
             self.process_file(in_file, start, end, out_file)
 
 
 def main():
     parser = argparse.ArgumentParser(
         description=(
             "Speaker Diarization gRPC client. Identifies speakers in input audio and returns"
@@ -166,61 +169,68 @@
         "--host",
         default="localhost:8080",
         help="Phonexia Speech Engine gRPC API server host",
     )
     parser.add_argument("--use_ssl", action="store_true", default=False, help="Use SSL connection")
     parser.add_argument(
         "-F",
-        "--out-format",
+        "--out_format",
         default="lab",
-        choices=["lab", "rttm"],
+        choices=["lab", "rttm", "json"],
         help="Output format",
     )
     speakers = parser.add_mutually_exclusive_group(required=False)
     speakers.add_argument(
-        "--total-speakers",
+        "--total_speakers",
         type=int,
         help="Exact number of speakers in recording",
     )
     speakers.add_argument(
-        "--max-speakers",
+        "--max_speakers",
         type=int,
         help="Maximum number of speakers in recording",
     )
     parser.add_argument(
+        "--metadata",
+        metavar="key=value",
+        nargs="+",
+        type=lambda x: tuple(x.split("=")),
+        help="Custom client metadata",
+    )
+    parser.add_argument(
         "-l",
-        "--log-level",
+        "--log_level",
         type=str,
         default="info",
         choices=["critical", "error", "warning", "info", "debug"],
         help="Logging level",
     )
     input_options = parser.add_mutually_exclusive_group(required=True)
-    input_options.add_argument("-i", "--in-file", type=Path, help="Path to audio file")
+    input_options.add_argument("-i", "--in_file", type=Path, help="Path to audio file")
     input_options.add_argument(
-        "-d", "--in-dir", type=Path, help="Path to directory containing audio files"
+        "-d", "--in_dir", type=Path, help="Path to directory containing audio files"
     )
     parser.add_argument("--start", type=float, help="Audio start time")
     parser.add_argument("--end", type=float, help="Audio end time")
     parser.add_argument(
         "-e",
-        "--in-extension",
+        "--in_extension",
         default="wav",
         help="Input extension of files in directory.",
     )
     output_options = parser.add_mutually_exclusive_group(required=False)
     output_options.add_argument(
         "-o",
-        "--out-file",
+        "--out_file",
         type=Path,
         help="Location the output will be stored into.",
     )
     output_options.add_argument(
         "-D",
-        "--out-dir",
+        "--out_dir",
         type=Path,
         help="Directory in which the output will be stored.",
     )
 
     args = parser.parse_args()
 
     if args.start is not None and args.start < 0:
@@ -228,33 +238,43 @@
 
     if args.end is not None and args.end <= 0:
         raise ValueError("Parameter 'end' must be a positive float.\n")
 
     if args.start is not None and args.end is not None and args.start >= args.end:
         raise ValueError("Parameter 'end' must be larger than 'start'.\n")
 
+    if args.max_speakers is not None and args.max_speakers == 0:
+        raise ValueError("Option 'max_speakers' must be larger than 0.\n")
+
     if args.out_file and args.in_dir:
         raise ValueError("'-o' option can not be used with '-d'.\n")
 
     if args.out_dir and args.in_file:
         raise ValueError("'-D' option can not be used with '-i'.\n")
 
+    if args.in_file and not os.path.isfile(args.in_file):
+        raise ValueError(f"No such file or directory '{args.in_file}'.\n")
+
+    if args.in_dir and not os.path.isdir(args.in_dir):
+        raise ValueError(f"No such file or directory '{args.in_dir}'.\n")
+
     logging.basicConfig(
         level=args.log_level.upper(),
         format="[%(asctime)s.%(msecs)03d] [%(levelname)s] %(message)s",
         datefmt="%Y-%m-%d %H:%M:%S",
     )
 
     try:
         client = speaker_diarization_client(
             args.host,
             args.use_ssl,
             args.max_speakers,
             args.total_speakers,
             args.out_format,
+            args.metadata,
         )
 
         if args.in_file:
             client.process_file(args.in_file, args.start, args.end, args.out_file)
 
         elif args.in_dir:
             client.process_dir(args.in_dir, args.start, args.end, args.out_dir, args.in_extension)
```

### Comparing `phonexia_speaker_diarization_client-1.1.0/pypi-README.md` & `phonexia_speaker_diarization_client-1.2.0/pypi-README.md`

 * *Files identical despite different names*

### Comparing `phonexia_speaker_diarization_client-1.1.0/pyproject.toml` & `phonexia_speaker_diarization_client-1.2.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "phonexia-speaker-diarization-client"
-version = "1.1.0"
+version = "1.2.0"
 description = "Client script for communicationg with diarization microservice"
 readme = "pypi-README.md"
 keywords = ["grpc", "voice", "voice-biometry", "speech", "language", "diarization"]
 authors = ["Phonexia <info@phonexia.com>"]
 
 [tool.poetry.urls]
 Homepage = "https://phonexia.com"
@@ -13,15 +13,15 @@
 
 [tool.poetry.scripts]
 speaker_diarization_client = 'phonexia_speaker_diarization_client:main'
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
 grpcio = "^1.54.0"
-phonexia-grpc = {version="^1.0.0", source="pypi"}
+phonexia-grpc = {version="^2.0.0", source="pypi"}
 ConfigArgParse = "1.7"
 grpcio-reflection = "^1.54.0"
 grpcio-health-checking = "^1.54.0"
 tomlkit = "^0.12.0"
 
 [[tool.poetry.source]]
 name = "gitlab"
```

### Comparing `phonexia_speaker_diarization_client-1.1.0/PKG-INFO` & `phonexia_speaker_diarization_client-1.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phonexia-speaker-diarization-client
-Version: 1.1.0
+Version: 1.2.0
 Summary: Client script for communicationg with diarization microservice
 Keywords: grpc,voice,voice-biometry,speech,language,diarization
 Author: Phonexia
 Author-email: info@phonexia.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: ConfigArgParse (==1.7)
 Requires-Dist: grpcio (>=1.54.0,<2.0.0)
 Requires-Dist: grpcio-health-checking (>=1.54.0,<2.0.0)
 Requires-Dist: grpcio-reflection (>=1.54.0,<2.0.0)
-Requires-Dist: phonexia-grpc (>=1.0.0,<2.0.0)
+Requires-Dist: phonexia-grpc (>=2.0.0,<3.0.0)
 Requires-Dist: tomlkit (>=0.12.0,<0.13.0)
 Project-URL: Homepage, https://phonexia.com
 Project-URL: Issues, https://phonexia.atlassian.net/servicedesk/customer/portal/15/group/20/create/40
 Project-URL: protofiles, https://github.com/phonexia/protofiles
 Description-Content-Type: text/markdown
```

