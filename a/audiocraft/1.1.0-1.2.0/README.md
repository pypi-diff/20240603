# Comparing `tmp/audiocraft-1.1.0.tar.gz` & `tmp/audiocraft-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audiocraft-1.1.0.tar", last modified: Tue Nov  7 12:54:21 2023, max compression
+gzip compressed data, was "audiocraft-1.2.0.tar", last modified: Mon Jan 15 16:55:28 2024, max compression
```

## Comparing `audiocraft-1.1.0.tar` & `audiocraft-1.2.0.tar`

### file list

```diff
@@ -1,266 +1,267 @@
-drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-11-07 12:54:21.930072 audiocraft-1.1.0/
--rw-r--r--   0 defossez   (501) staff       (20)     1981 2023-11-07 12:46:52.000000 audiocraft-1.1.0/CHANGELOG.md
--rw-r--r--   0 defossez   (501) staff       (20)     3535 2023-10-13 09:02:02.000000 audiocraft-1.1.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 defossez   (501) staff       (20)     1377 2023-11-06 13:30:18.000000 audiocraft-1.1.0/CONTRIBUTING.md
--rw-r--r--   0 defossez   (501) staff       (20)     1088 2023-07-03 08:49:34.000000 audiocraft-1.1.0/LICENSE
--rw-r--r--   0 defossez   (501) staff       (20)    19333 2023-11-06 13:30:18.000000 audiocraft-1.1.0/LICENSE_weights
--rw-r--r--   0 defossez   (501) staff       (20)      368 2023-11-06 13:30:18.000000 audiocraft-1.1.0/MANIFEST.in
--rw-r--r--   0 defossez   (501) staff       (20)     1464 2023-11-06 13:30:18.000000 audiocraft-1.1.0/Makefile
--rw-r--r--   0 defossez   (501) staff       (20)     5375 2023-11-07 12:54:21.930702 audiocraft-1.1.0/PKG-INFO
--rw-r--r--   0 defossez   (501) staff       (20)     4140 2023-11-06 13:30:18.000000 audiocraft-1.1.0/README.md
-drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-11-07 12:54:21.396678 audiocraft-1.1.0/assets/
--rw-r--r--   0 defossez   (501) staff       (20)    15228 2023-11-06 13:30:18.000000 audiocraft-1.1.0/assets/a_duck_quacking_as_birds_chirp_and_a_pigeon_cooing.mp3
--rw-r--r--   0 defossez   (501) staff       (20)   160496 2023-07-03 08:49:34.000000 audiocraft-1.1.0/assets/bach.mp3
--rw-r--r--   0 defossez   (501) staff       (20)   161280 2023-10-13 09:02:02.000000 audiocraft-1.1.0/assets/bolero_ravel.mp3
--rw-r--r--   0 defossez   (501) staff       (20)    15228 2023-11-06 13:30:18.000000 audiocraft-1.1.0/assets/sirens_and_a_humming_engine_approach_and_pass.mp3
-drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-11-07 12:54:21.427529 audiocraft-1.1.0/audiocraft/
--rw-r--r--   0 defossez   (501) staff       (20)     1247 2023-11-07 12:46:52.000000 audiocraft-1.1.0/audiocraft/__init__.py
-drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-11-07 12:54:21.465448 audiocraft-1.1.0/audiocraft/adversarial/
--rw-r--r--   0 defossez   (501) staff       (20)      570 2023-11-06 13:30:18.000000 audiocraft-1.1.0/audiocraft/adversarial/__init__.py
-drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-11-07 12:54:21.484361 audiocraft-1.1.0/audiocraft/adversarial/discriminators/
--rw-r--r--   0 defossez   (501) staff       (20)      346 2023-11-06 13:30:18.000000 audiocraft-1.1.0/audiocraft/adversarial/discriminators/__init__.py
--rw-r--r--   0 defossez   (501) staff       (20)      894 2023-11-06 13:30:18.000000 audiocraft-1.1.0/audiocraft/adversarial/discriminators/base.py
--rw-r--r--   0 defossez   (501) staff       (20)     4176 2023-11-06 13:30:18.000000 audiocraft-1.1.0/audiocraft/adversarial/discriminators/mpd.py
--rw-r--r--   0 defossez   (501) staff       (20)     5926 2023-11-06 13:30:18.000000 audiocraft-1.1.0/audiocraft/adversarial/discriminators/msd.py
--rw-r--r--   0 defossez   (501) staff       (20)     6331 2023-11-06 13:30:18.000000 audiocraft-1.1.0/audiocraft/adversarial/discriminators/msstftd.py
--rw-r--r--   0 defossez   (501) staff       (20)     9126 2023-11-06 13:30:18.000000 audiocraft-1.1.0/audiocraft/adversarial/losses.py
-drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-11-07 12:54:21.520792 audiocraft-1.1.0/audiocraft/data/
--rw-r--r--   0 defossez   (501) staff       (20)      396 2023-11-06 13:30:18.000000 audiocraft-1.1.0/audiocraft/data/__init__.py
--rw-r--r--   0 defossez   (501) staff       (20)     9811 2023-11-06 13:30:18.000000 audiocraft-1.1.0/audiocraft/data/audio.py
--rw-r--r--   0 defossez   (501) staff       (20)    25464 2023-11-06 13:30:18.000000 audiocraft-1.1.0/audiocraft/data/audio_dataset.py
--rw-r--r--   0 defossez   (501) staff       (20)     7752 2023-11-06 13:30:18.000000 audiocraft-1.1.0/audiocraft/data/audio_utils.py
--rw-r--r--   0 defossez   (501) staff       (20)     3902 2023-11-06 13:30:18.000000 audiocraft-1.1.0/audiocraft/data/info_audio_dataset.py
--rw-r--r--   0 defossez   (501) staff       (20)    11575 2023-11-06 13:30:18.000000 audiocraft-1.1.0/audiocraft/data/music_dataset.py
--rw-r--r--   0 defossez   (501) staff       (20)    13381 2023-11-06 13:30:18.000000 audiocraft-1.1.0/audiocraft/data/sound_dataset.py
--rw-r--r--   0 defossez   (501) staff       (20)     2202 2023-11-06 13:30:18.000000 audiocraft-1.1.0/audiocraft/data/zip.py
--rw-r--r--   0 defossez   (501) staff       (20)     6741 2023-11-06 13:30:18.000000 audiocraft-1.1.0/audiocraft/environment.py
-drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-11-07 12:54:21.524112 audiocraft-1.1.0/audiocraft/grids/
--rw-r--r--   0 defossez   (501) staff       (20)      216 2023-11-06 13:30:18.000000 audiocraft-1.1.0/audiocraft/grids/__init__.py
--rw-r--r--   0 defossez   (501) staff       (20)     2639 2023-11-06 13:30:18.000000 audiocraft-1.1.0/audiocraft/grids/_base_explorers.py
-drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-11-07 12:54:21.529829 audiocraft-1.1.0/audiocraft/grids/audiogen/
--rw-r--r--   0 defossez   (501) staff       (20)      220 2023-11-06 13:30:18.000000 audiocraft-1.1.0/audiocraft/grids/audiogen/__init__.py
--rw-r--r--   0 defossez   (501) staff       (20)      776 2023-11-06 13:30:18.000000 audiocraft-1.1.0/audiocraft/grids/audiogen/audiogen_base_16khz.py
--rw-r--r--   0 defossez   (501) staff       (20)     2483 2023-11-06 13:30:18.000000 audiocraft-1.1.0/audiocraft/grids/audiogen/audiogen_pretrained_16khz_eval.py
-drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-11-07 12:54:21.540605 audiocraft-1.1.0/audiocraft/grids/compression/
--rw-r--r--   0 defossez   (501) staff       (20)      219 2023-11-06 13:30:18.000000 audiocraft-1.1.0/audiocraft/grids/compression/__init__.py
--rw-r--r--   0 defossez   (501) staff       (20)     1601 2023-11-06 13:30:18.000000 audiocraft-1.1.0/audiocraft/grids/compression/_explorers.py
--rw-r--r--   0 defossez   (501) staff       (20)     1117 2023-11-06 13:30:18.000000 audiocraft-1.1.0/audiocraft/grids/compression/debug.py
--rw-r--r--   0 defossez   (501) staff       (20)     1100 2023-11-06 13:30:18.000000 audiocraft-1.1.0/audiocraft/grids/compression/encodec_audiogen_16khz.py
--rw-r--r--   0 defossez   (501) staff       (20)      956 2023-11-06 13:30:18.000000 audiocraft-1.1.0/audiocraft/grids/compression/encodec_base_24khz.py
--rw-r--r--   0 defossez   (501) staff       (20)     1262 2023-11-06 13:30:18.000000 audiocraft-1.1.0/audiocraft/grids/compression/encodec_musicgen_32khz.py
-drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-11-07 12:54:21.546557 audiocraft-1.1.0/audiocraft/grids/diffusion/
--rw-r--r--   0 defossez   (501) staff       (20)     1073 2023-11-06 13:30:18.000000 audiocraft-1.1.0/audiocraft/grids/diffusion/4_bands_base_32khz.py
--rw-r--r--   0 defossez   (501) staff       (20)      221 2023-11-06 13:30:18.000000 audiocraft-1.1.0/audiocraft/grids/diffusion/__init__.py
--rw-r--r--   0 defossez   (501) staff       (20)     2066 2023-11-06 13:30:18.000000 audiocraft-1.1.0/audiocraft/grids/diffusion/_explorers.py
-drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-11-07 12:54:21.573401 audiocraft-1.1.0/audiocraft/grids/musicgen/
--rw-r--r--   0 defossez   (501) staff       (20)      220 2023-11-06 13:30:18.000000 audiocraft-1.1.0/audiocraft/grids/musicgen/__init__.py
--rw-r--r--   0 defossez   (501) staff       (20)     3092 2023-11-06 13:30:18.000000 audiocraft-1.1.0/audiocraft/grids/musicgen/_explorers.py
--rw-r--r--   0 defossez   (501) staff       (20)     1413 2023-11-06 13:30:18.000000 audiocraft-1.1.0/audiocraft/grids/musicgen/musicgen_base_32khz.py
--rw-r--r--   0 defossez   (501) staff       (20)     2311 2023-11-06 13:30:18.000000 audiocraft-1.1.0/audiocraft/grids/musicgen/musicgen_base_cached_32khz.py
--rw-r--r--   0 defossez   (501) staff       (20)     1193 2023-11-06 13:30:18.000000 audiocraft-1.1.0/audiocraft/grids/musicgen/musicgen_clapemb_32khz.py
--rw-r--r--   0 defossez   (501) staff       (20)     2251 2023-11-06 13:30:18.000000 audiocraft-1.1.0/audiocraft/grids/musicgen/musicgen_melody_32khz.py
--rw-r--r--   0 defossez   (501) staff       (20)     3880 2023-11-06 13:30:18.000000 audiocraft-1.1.0/audiocraft/grids/musicgen/musicgen_pretrained_32khz_eval.py
-drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-11-07 12:54:21.578849 audiocraft-1.1.0/audiocraft/losses/
--rw-r--r--   0 defossez   (501) staff       (20)      585 2023-11-06 13:30:18.000000 audiocraft-1.1.0/audiocraft/losses/__init__.py
--rw-r--r--   0 defossez   (501) staff       (20)     6612 2023-11-06 13:30:18.000000 audiocraft-1.1.0/audiocraft/losses/balancer.py
--rw-r--r--   0 defossez   (501) staff       (20)     3263 2023-11-06 13:30:18.000000 audiocraft-1.1.0/audiocraft/losses/sisnr.py
--rw-r--r--   0 defossez   (501) staff       (20)     6531 2023-11-06 13:30:18.000000 audiocraft-1.1.0/audiocraft/losses/specloss.py
--rw-r--r--   0 defossez   (501) staff       (20)     8202 2023-11-06 13:30:18.000000 audiocraft-1.1.0/audiocraft/losses/stftloss.py
-drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-11-07 12:54:21.585057 audiocraft-1.1.0/audiocraft/metrics/
--rw-r--r--   0 defossez   (501) staff       (20)      592 2023-11-06 13:30:18.000000 audiocraft-1.1.0/audiocraft/metrics/__init__.py
--rw-r--r--   0 defossez   (501) staff       (20)     3674 2023-11-06 13:30:18.000000 audiocraft-1.1.0/audiocraft/metrics/chroma_cosinesim.py
--rw-r--r--   0 defossez   (501) staff       (20)     4525 2023-11-06 13:30:18.000000 audiocraft-1.1.0/audiocraft/metrics/clap_consistency.py
--rw-r--r--   0 defossez   (501) staff       (20)    17724 2023-11-06 13:30:18.000000 audiocraft-1.1.0/audiocraft/metrics/fad.py
--rw-r--r--   0 defossez   (501) staff       (20)    10211 2023-11-06 13:30:18.000000 audiocraft-1.1.0/audiocraft/metrics/kld.py
--rw-r--r--   0 defossez   (501) staff       (20)     6107 2023-11-06 13:30:18.000000 audiocraft-1.1.0/audiocraft/metrics/rvm.py
--rw-r--r--   0 defossez   (501) staff       (20)     9694 2023-11-06 13:30:18.000000 audiocraft-1.1.0/audiocraft/metrics/visqol.py
-drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-11-07 12:54:21.618759 audiocraft-1.1.0/audiocraft/models/
--rw-r--r--   0 defossez   (501) staff       (20)      605 2023-11-06 13:30:18.000000 audiocraft-1.1.0/audiocraft/models/__init__.py
--rw-r--r--   0 defossez   (501) staff       (20)    12444 2023-11-06 13:30:18.000000 audiocraft-1.1.0/audiocraft/models/audiogen.py
--rw-r--r--   0 defossez   (501) staff       (20)     9854 2023-11-06 13:30:18.000000 audiocraft-1.1.0/audiocraft/models/builders.py
--rw-r--r--   0 defossez   (501) staff       (20)    13569 2023-11-06 13:30:18.000000 audiocraft-1.1.0/audiocraft/models/encodec.py
--rw-r--r--   0 defossez   (501) staff       (20)    27199 2023-11-06 13:30:18.000000 audiocraft-1.1.0/audiocraft/models/lm.py
--rw-r--r--   0 defossez   (501) staff       (20)     5581 2023-11-07 12:46:52.000000 audiocraft-1.1.0/audiocraft/models/loaders.py
--rw-r--r--   0 defossez   (501) staff       (20)     8895 2023-11-06 13:30:18.000000 audiocraft-1.1.0/audiocraft/models/multibanddiffusion.py
--rw-r--r--   0 defossez   (501) staff       (20)    19997 2023-11-06 13:30:18.000000 audiocraft-1.1.0/audiocraft/models/musicgen.py
--rw-r--r--   0 defossez   (501) staff       (20)     8340 2023-11-06 13:30:18.000000 audiocraft-1.1.0/audiocraft/models/unet.py
-drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-11-07 12:54:21.639207 audiocraft-1.1.0/audiocraft/modules/
--rw-r--r--   0 defossez   (501) staff       (20)      586 2023-11-06 13:30:18.000000 audiocraft-1.1.0/audiocraft/modules/__init__.py
--rw-r--r--   0 defossez   (501) staff       (20)     3266 2023-11-06 13:30:18.000000 audiocraft-1.1.0/audiocraft/modules/activations.py
--rw-r--r--   0 defossez   (501) staff       (20)     3023 2023-11-06 13:30:18.000000 audiocraft-1.1.0/audiocraft/modules/chroma.py
--rw-r--r--   0 defossez   (501) staff       (20)    27943 2023-11-06 13:30:18.000000 audiocraft-1.1.0/audiocraft/modules/codebooks_patterns.py
--rw-r--r--   0 defossez   (501) staff       (20)    64783 2023-11-06 13:30:18.000000 audiocraft-1.1.0/audiocraft/modules/conditioners.py
--rw-r--r--   0 defossez   (501) staff       (20)    10496 2023-11-06 13:30:18.000000 audiocraft-1.1.0/audiocraft/modules/conv.py
--rw-r--r--   0 defossez   (501) staff       (20)    12018 2023-11-06 13:30:18.000000 audiocraft-1.1.0/audiocraft/modules/diffusion_schedule.py
--rw-r--r--   0 defossez   (501) staff       (20)      759 2023-07-03 08:49:34.000000 audiocraft-1.1.0/audiocraft/modules/lstm.py
--rw-r--r--   0 defossez   (501) staff       (20)     5649 2023-11-06 13:30:18.000000 audiocraft-1.1.0/audiocraft/modules/rope.py
--rw-r--r--   0 defossez   (501) staff       (20)    13868 2023-07-03 08:49:34.000000 audiocraft-1.1.0/audiocraft/modules/seanet.py
--rw-r--r--   0 defossez   (501) staff       (20)     4494 2023-11-06 13:30:18.000000 audiocraft-1.1.0/audiocraft/modules/streaming.py
--rw-r--r--   0 defossez   (501) staff       (20)    37020 2023-11-06 13:30:18.000000 audiocraft-1.1.0/audiocraft/modules/transformer.py
-drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-11-07 12:54:21.668587 audiocraft-1.1.0/audiocraft/optim/
--rw-r--r--   0 defossez   (501) staff       (20)      638 2023-11-06 13:30:18.000000 audiocraft-1.1.0/audiocraft/optim/__init__.py
--rw-r--r--   0 defossez   (501) staff       (20)     1730 2023-11-06 13:30:18.000000 audiocraft-1.1.0/audiocraft/optim/cosine_lr_scheduler.py
--rw-r--r--   0 defossez   (501) staff       (20)     8910 2023-11-06 13:30:18.000000 audiocraft-1.1.0/audiocraft/optim/dadam.py
--rw-r--r--   0 defossez   (501) staff       (20)     3196 2023-11-06 13:30:18.000000 audiocraft-1.1.0/audiocraft/optim/ema.py
--rw-r--r--   0 defossez   (501) staff       (20)     7316 2023-11-06 13:30:18.000000 audiocraft-1.1.0/audiocraft/optim/fsdp.py
--rw-r--r--   0 defossez   (501) staff       (20)     1390 2023-11-06 13:30:18.000000 audiocraft-1.1.0/audiocraft/optim/inverse_sqrt_lr_scheduler.py
--rw-r--r--   0 defossez   (501) staff       (20)     1272 2023-11-06 13:30:18.000000 audiocraft-1.1.0/audiocraft/optim/linear_warmup_lr_scheduler.py
--rw-r--r--   0 defossez   (501) staff       (20)     2012 2023-11-06 13:30:18.000000 audiocraft-1.1.0/audiocraft/optim/polynomial_decay_lr_scheduler.py
--rw-r--r--   0 defossez   (501) staff       (20)        0 2023-07-03 08:49:34.000000 audiocraft-1.1.0/audiocraft/py.typed
-drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-11-07 12:54:21.673376 audiocraft-1.1.0/audiocraft/quantization/
--rw-r--r--   0 defossez   (501) staff       (20)      329 2023-11-06 13:30:18.000000 audiocraft-1.1.0/audiocraft/quantization/__init__.py
--rw-r--r--   0 defossez   (501) staff       (20)     3314 2023-11-06 13:30:18.000000 audiocraft-1.1.0/audiocraft/quantization/base.py
--rw-r--r--   0 defossez   (501) staff       (20)    14357 2023-11-06 13:30:18.000000 audiocraft-1.1.0/audiocraft/quantization/core_vq.py
--rw-r--r--   0 defossez   (501) staff       (20)     4649 2023-11-06 13:30:18.000000 audiocraft-1.1.0/audiocraft/quantization/vq.py
-drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-11-07 12:54:21.683848 audiocraft-1.1.0/audiocraft/solvers/
--rw-r--r--   0 defossez   (501) staff       (20)      574 2023-11-06 13:30:18.000000 audiocraft-1.1.0/audiocraft/solvers/__init__.py
--rw-r--r--   0 defossez   (501) staff       (20)      655 2023-11-06 13:30:18.000000 audiocraft-1.1.0/audiocraft/solvers/audiogen.py
--rw-r--r--   0 defossez   (501) staff       (20)    31355 2023-11-06 13:30:18.000000 audiocraft-1.1.0/audiocraft/solvers/base.py
--rw-r--r--   0 defossez   (501) staff       (20)    13937 2023-11-06 13:30:18.000000 audiocraft-1.1.0/audiocraft/solvers/builders.py
--rw-r--r--   0 defossez   (501) staff       (20)    14774 2023-11-06 13:30:18.000000 audiocraft-1.1.0/audiocraft/solvers/compression.py
--rw-r--r--   0 defossez   (501) staff       (20)    11336 2023-11-06 13:30:18.000000 audiocraft-1.1.0/audiocraft/solvers/diffusion.py
--rw-r--r--   0 defossez   (501) staff       (20)    35147 2023-11-06 13:30:18.000000 audiocraft-1.1.0/audiocraft/solvers/musicgen.py
--rw-r--r--   0 defossez   (501) staff       (20)     6724 2023-11-06 13:30:18.000000 audiocraft-1.1.0/audiocraft/train.py
-drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-11-07 12:54:21.721488 audiocraft-1.1.0/audiocraft/utils/
--rw-r--r--   0 defossez   (501) staff       (20)      215 2023-11-06 13:30:18.000000 audiocraft-1.1.0/audiocraft/utils/__init__.py
--rw-r--r--   0 defossez   (501) staff       (20)     1377 2023-07-03 08:49:34.000000 audiocraft-1.1.0/audiocraft/utils/autocast.py
--rw-r--r--   0 defossez   (501) staff       (20)     3694 2023-11-06 13:30:18.000000 audiocraft-1.1.0/audiocraft/utils/best_state.py
--rw-r--r--   0 defossez   (501) staff       (20)    14294 2023-11-06 13:30:18.000000 audiocraft-1.1.0/audiocraft/utils/cache.py
--rw-r--r--   0 defossez   (501) staff       (20)     6129 2023-11-06 13:30:18.000000 audiocraft-1.1.0/audiocraft/utils/checkpoint.py
--rw-r--r--   0 defossez   (501) staff       (20)     2044 2023-11-06 13:30:18.000000 audiocraft-1.1.0/audiocraft/utils/cluster.py
--rw-r--r--   0 defossez   (501) staff       (20)     1710 2023-11-06 13:30:18.000000 audiocraft-1.1.0/audiocraft/utils/deadlock.py
--rw-r--r--   0 defossez   (501) staff       (20)     2677 2023-11-06 13:30:18.000000 audiocraft-1.1.0/audiocraft/utils/export.py
--rw-r--r--   0 defossez   (501) staff       (20)     1906 2023-11-06 13:30:18.000000 audiocraft-1.1.0/audiocraft/utils/export_legacy.py
--rw-r--r--   0 defossez   (501) staff       (20)      885 2023-10-13 09:02:02.000000 audiocraft-1.1.0/audiocraft/utils/notebook.py
--rw-r--r--   0 defossez   (501) staff       (20)     1209 2023-11-06 13:30:18.000000 audiocraft-1.1.0/audiocraft/utils/profiler.py
-drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-11-07 12:54:21.723388 audiocraft-1.1.0/audiocraft/utils/samples/
--rw-r--r--   0 defossez   (501) staff       (20)      198 2023-11-06 13:30:18.000000 audiocraft-1.1.0/audiocraft/utils/samples/__init__.py
--rw-r--r--   0 defossez   (501) staff       (20)    19385 2023-11-06 13:30:18.000000 audiocraft-1.1.0/audiocraft/utils/samples/manager.py
--rw-r--r--   0 defossez   (501) staff       (20)    10607 2023-11-06 13:30:18.000000 audiocraft-1.1.0/audiocraft/utils/utils.py
-drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-11-07 12:54:21.443242 audiocraft-1.1.0/audiocraft.egg-info/
--rw-r--r--   0 defossez   (501) staff       (20)     5375 2023-11-07 12:54:21.000000 audiocraft-1.1.0/audiocraft.egg-info/PKG-INFO
--rw-r--r--   0 defossez   (501) staff       (20)     7060 2023-11-07 12:54:21.000000 audiocraft-1.1.0/audiocraft.egg-info/SOURCES.txt
--rw-r--r--   0 defossez   (501) staff       (20)        1 2023-11-07 12:54:21.000000 audiocraft-1.1.0/audiocraft.egg-info/dependency_links.txt
--rw-r--r--   0 defossez   (501) staff       (20)      280 2023-11-07 12:54:21.000000 audiocraft-1.1.0/audiocraft.egg-info/requires.txt
--rw-r--r--   0 defossez   (501) staff       (20)       25 2023-11-07 12:54:21.000000 audiocraft-1.1.0/audiocraft.egg-info/top_level.txt
-drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-11-07 12:54:21.724727 audiocraft-1.1.0/config/
-drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-11-07 12:54:21.731024 audiocraft-1.1.0/config/conditioner/
--rw-r--r--   0 defossez   (501) staff       (20)      817 2023-11-06 13:30:18.000000 audiocraft-1.1.0/config/conditioner/chroma2music.yaml
--rw-r--r--   0 defossez   (501) staff       (20)      922 2023-11-06 13:30:18.000000 audiocraft-1.1.0/config/conditioner/clapemb2music.yaml
--rw-r--r--   0 defossez   (501) staff       (20)      239 2023-11-06 13:30:18.000000 audiocraft-1.1.0/config/conditioner/none.yaml
--rw-r--r--   0 defossez   (501) staff       (20)      496 2023-11-06 13:30:18.000000 audiocraft-1.1.0/config/conditioner/text2music.yaml
--rw-r--r--   0 defossez   (501) staff       (20)      411 2023-11-06 13:30:18.000000 audiocraft-1.1.0/config/conditioner/text2sound.yaml
--rw-r--r--   0 defossez   (501) staff       (20)     2733 2023-11-06 13:30:18.000000 audiocraft-1.1.0/config/config.yaml
-drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-11-07 12:54:21.732333 audiocraft-1.1.0/config/dset/
-drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-11-07 12:54:21.739185 audiocraft-1.1.0/config/dset/audio/
--rw-r--r--   0 defossez   (501) staff       (20)      281 2023-11-06 13:30:18.000000 audiocraft-1.1.0/config/dset/audio/audiocaps_16khz.yaml
--rw-r--r--   0 defossez   (501) staff       (20)      138 2023-11-06 13:30:18.000000 audiocraft-1.1.0/config/dset/audio/default.yaml
--rw-r--r--   0 defossez   (501) staff       (20)      169 2023-11-06 13:30:18.000000 audiocraft-1.1.0/config/dset/audio/example.yaml
--rw-r--r--   0 defossez   (501) staff       (20)      358 2023-11-06 13:30:18.000000 audiocraft-1.1.0/config/dset/audio/musiccaps_32khz.yaml
--rw-r--r--   0 defossez   (501) staff       (20)      300 2023-11-06 13:30:18.000000 audiocraft-1.1.0/config/dset/default.yaml
-drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-11-07 12:54:21.745306 audiocraft-1.1.0/config/dset/internal/
--rw-r--r--   0 defossez   (501) staff       (20)      338 2023-11-06 13:30:18.000000 audiocraft-1.1.0/config/dset/internal/music_10k_32khz.yaml
--rw-r--r--   0 defossez   (501) staff       (20)      275 2023-11-06 13:30:18.000000 audiocraft-1.1.0/config/dset/internal/music_400k_32khz.yaml
--rw-r--r--   0 defossez   (501) staff       (20)      344 2023-11-06 13:30:18.000000 audiocraft-1.1.0/config/dset/internal/sounds_16khz.yaml
-drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-11-07 12:54:21.747531 audiocraft-1.1.0/config/model/
-drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-11-07 12:54:21.770435 audiocraft-1.1.0/config/model/encodec/
--rw-r--r--   0 defossez   (501) staff       (20)     1112 2023-11-06 13:30:18.000000 audiocraft-1.1.0/config/model/encodec/default.yaml
--rw-r--r--   0 defossez   (501) staff       (20)      112 2023-11-06 13:30:18.000000 audiocraft-1.1.0/config/model/encodec/encodec_base_causal.yaml
--rw-r--r--   0 defossez   (501) staff       (20)      161 2023-11-06 13:30:18.000000 audiocraft-1.1.0/config/model/encodec/encodec_large_nq4_s320.yaml
--rw-r--r--   0 defossez   (501) staff       (20)      148 2023-11-06 13:30:18.000000 audiocraft-1.1.0/config/model/encodec/encodec_large_nq4_s640.yaml
-drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-11-07 12:54:21.773710 audiocraft-1.1.0/config/model/lm/
--rw-r--r--   0 defossez   (501) staff       (20)      738 2023-11-06 13:30:18.000000 audiocraft-1.1.0/config/model/lm/audiogen_lm.yaml
--rw-r--r--   0 defossez   (501) staff       (20)     1992 2023-11-06 13:30:18.000000 audiocraft-1.1.0/config/model/lm/default.yaml
-drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-11-07 12:54:21.778946 audiocraft-1.1.0/config/model/lm/model_scale/
--rw-r--r--   0 defossez   (501) staff       (20)      102 2023-11-06 13:30:18.000000 audiocraft-1.1.0/config/model/lm/model_scale/base.yaml
--rw-r--r--   0 defossez   (501) staff       (20)      126 2023-11-06 13:30:18.000000 audiocraft-1.1.0/config/model/lm/model_scale/large.yaml
--rw-r--r--   0 defossez   (501) staff       (20)      109 2023-11-06 13:30:18.000000 audiocraft-1.1.0/config/model/lm/model_scale/medium.yaml
--rw-r--r--   0 defossez   (501) staff       (20)       97 2023-11-06 13:30:18.000000 audiocraft-1.1.0/config/model/lm/model_scale/small.yaml
--rw-r--r--   0 defossez   (501) staff       (20)      181 2023-11-06 13:30:18.000000 audiocraft-1.1.0/config/model/lm/model_scale/xsmall.yaml
--rw-r--r--   0 defossez   (501) staff       (20)      738 2023-11-06 13:30:18.000000 audiocraft-1.1.0/config/model/lm/musicgen_lm.yaml
--rw-r--r--   0 defossez   (501) staff       (20)      157 2023-11-06 13:30:18.000000 audiocraft-1.1.0/config/model/none.yaml
-drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-11-07 12:54:21.779897 audiocraft-1.1.0/config/model/score/
--rw-r--r--   0 defossez   (501) staff       (20)      269 2023-11-06 13:30:18.000000 audiocraft-1.1.0/config/model/score/basic.yaml
-drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-11-07 12:54:21.780958 audiocraft-1.1.0/config/solver/
-drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-11-07 12:54:21.783525 audiocraft-1.1.0/config/solver/audiogen/
--rw-r--r--   0 defossez   (501) staff       (20)     1772 2023-11-06 13:30:18.000000 audiocraft-1.1.0/config/solver/audiogen/audiogen_base_16khz.yaml
--rw-r--r--   0 defossez   (501) staff       (20)      972 2023-11-06 13:30:18.000000 audiocraft-1.1.0/config/solver/audiogen/debug.yaml
--rw-r--r--   0 defossez   (501) staff       (20)      769 2023-11-06 13:30:18.000000 audiocraft-1.1.0/config/solver/audiogen/default.yaml
-drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-11-07 12:54:21.785136 audiocraft-1.1.0/config/solver/audiogen/evaluation/
--rw-r--r--   0 defossez   (501) staff       (20)       67 2023-11-06 13:30:18.000000 audiocraft-1.1.0/config/solver/audiogen/evaluation/none.yaml
--rw-r--r--   0 defossez   (501) staff       (20)      725 2023-11-06 13:30:18.000000 audiocraft-1.1.0/config/solver/audiogen/evaluation/objective_eval.yaml
-drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-11-07 12:54:21.792020 audiocraft-1.1.0/config/solver/compression/
--rw-r--r--   0 defossez   (501) staff       (20)      812 2023-11-06 13:30:18.000000 audiocraft-1.1.0/config/solver/compression/debug.yaml
--rw-r--r--   0 defossez   (501) staff       (20)     2955 2023-11-06 13:30:18.000000 audiocraft-1.1.0/config/solver/compression/default.yaml
--rw-r--r--   0 defossez   (501) staff       (20)      177 2023-11-06 13:30:18.000000 audiocraft-1.1.0/config/solver/compression/encodec_audiogen_16khz.yaml
--rw-r--r--   0 defossez   (501) staff       (20)      174 2023-11-06 13:30:18.000000 audiocraft-1.1.0/config/solver/compression/encodec_base_24khz.yaml
--rw-r--r--   0 defossez   (501) staff       (20)      177 2023-11-06 13:30:18.000000 audiocraft-1.1.0/config/solver/compression/encodec_musicgen_32khz.yaml
--rw-r--r--   0 defossez   (501) staff       (20)     2534 2023-11-06 13:30:18.000000 audiocraft-1.1.0/config/solver/default.yaml
-drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-11-07 12:54:21.795747 audiocraft-1.1.0/config/solver/diffusion/
--rw-r--r--   0 defossez   (501) staff       (20)     1677 2023-11-06 13:30:18.000000 audiocraft-1.1.0/config/solver/diffusion/debug.yaml
--rw-r--r--   0 defossez   (501) staff       (20)     1690 2023-11-06 13:30:18.000000 audiocraft-1.1.0/config/solver/diffusion/default.yaml
--rw-r--r--   0 defossez   (501) staff       (20)      197 2023-11-06 13:30:18.000000 audiocraft-1.1.0/config/solver/diffusion/encodec_24khz.yaml
-drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-11-07 12:54:21.817746 audiocraft-1.1.0/config/solver/musicgen/
--rw-r--r--   0 defossez   (501) staff       (20)     1004 2023-11-06 13:30:18.000000 audiocraft-1.1.0/config/solver/musicgen/debug.yaml
--rw-r--r--   0 defossez   (501) staff       (20)     2343 2023-11-06 13:30:18.000000 audiocraft-1.1.0/config/solver/musicgen/default.yaml
-drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-11-07 12:54:21.820582 audiocraft-1.1.0/config/solver/musicgen/evaluation/
--rw-r--r--   0 defossez   (501) staff       (20)       67 2023-11-06 13:30:18.000000 audiocraft-1.1.0/config/solver/musicgen/evaluation/none.yaml
--rw-r--r--   0 defossez   (501) staff       (20)      619 2023-11-06 13:30:18.000000 audiocraft-1.1.0/config/solver/musicgen/evaluation/objective_eval.yaml
--rw-r--r--   0 defossez   (501) staff       (20)     1125 2023-11-06 13:30:18.000000 audiocraft-1.1.0/config/solver/musicgen/musicgen_base_32khz.yaml
--rw-r--r--   0 defossez   (501) staff       (20)     1174 2023-11-06 13:30:18.000000 audiocraft-1.1.0/config/solver/musicgen/musicgen_melody_32khz.yaml
-drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-11-07 12:54:21.823654 audiocraft-1.1.0/config/teams/
--rw-r--r--   0 defossez   (501) staff       (20)      324 2023-11-06 13:30:18.000000 audiocraft-1.1.0/config/teams/default.yaml
--rw-r--r--   0 defossez   (501) staff       (20)      836 2023-11-06 13:30:18.000000 audiocraft-1.1.0/config/teams/labs.yaml
-drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-11-07 12:54:21.828460 audiocraft-1.1.0/demos/
--rw-r--r--   0 defossez   (501) staff       (20)     5463 2023-11-06 13:30:18.000000 audiocraft-1.1.0/demos/audiogen_demo.ipynb
--rw-r--r--   0 defossez   (501) staff       (20)    18223 2023-11-06 13:30:18.000000 audiocraft-1.1.0/demos/musicgen_app.py
--rw-r--r--   0 defossez   (501) staff       (20)     7843 2023-11-06 13:30:18.000000 audiocraft-1.1.0/demos/musicgen_demo.ipynb
-drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-11-07 12:54:21.840938 audiocraft-1.1.0/docs/
--rw-r--r--   0 defossez   (501) staff       (20)     6557 2023-11-06 13:30:18.000000 audiocraft-1.1.0/docs/AUDIOGEN.md
--rw-r--r--   0 defossez   (501) staff       (20)     7369 2023-11-06 13:30:18.000000 audiocraft-1.1.0/docs/CONDITIONING.md
--rw-r--r--   0 defossez   (501) staff       (20)     3073 2023-11-06 13:30:18.000000 audiocraft-1.1.0/docs/DATASETS.md
--rw-r--r--   0 defossez   (501) staff       (20)     6804 2023-11-06 13:30:18.000000 audiocraft-1.1.0/docs/ENCODEC.md
--rw-r--r--   0 defossez   (501) staff       (20)     5102 2023-11-06 13:30:18.000000 audiocraft-1.1.0/docs/MBD.md
--rw-r--r--   0 defossez   (501) staff       (20)     5769 2023-11-06 13:30:18.000000 audiocraft-1.1.0/docs/METRICS.md
--rw-r--r--   0 defossez   (501) staff       (20)    16516 2023-11-06 13:30:18.000000 audiocraft-1.1.0/docs/MUSICGEN.md
--rw-r--r--   0 defossez   (501) staff       (20)    14423 2023-11-06 13:30:18.000000 audiocraft-1.1.0/docs/TRAINING.md
-drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-11-07 12:54:21.844939 audiocraft-1.1.0/model_cards/
--rw-r--r--   0 defossez   (501) staff       (20)     5788 2023-11-06 13:30:18.000000 audiocraft-1.1.0/model_cards/AUDIOGEN_MODEL_CARD.md
--rw-r--r--   0 defossez   (501) staff       (20)     6760 2023-11-06 13:30:18.000000 audiocraft-1.1.0/model_cards/MUSICGEN_MODEL_CARD.md
--rw-r--r--   0 defossez   (501) staff       (20)      169 2023-11-06 13:30:18.000000 audiocraft-1.1.0/mypy.ini
--rw-r--r--   0 defossez   (501) staff       (20)      337 2023-11-06 13:30:18.000000 audiocraft-1.1.0/requirements.txt
-drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-11-07 12:54:21.868306 audiocraft-1.1.0/scripts/
--rw-r--r--   0 defossez   (501) staff       (20)      198 2023-11-06 13:30:18.000000 audiocraft-1.1.0/scripts/__init__.py
--rw-r--r--   0 defossez   (501) staff       (20)     9641 2023-11-06 13:30:18.000000 audiocraft-1.1.0/scripts/mos.py
--rw-r--r--   0 defossez   (501) staff       (20)     7478 2023-11-06 13:30:18.000000 audiocraft-1.1.0/scripts/resample_dataset.py
--rw-r--r--   0 defossez   (501) staff       (20)      270 2023-11-07 12:54:21.932121 audiocraft-1.1.0/setup.cfg
--rw-r--r--   0 defossez   (501) staff       (20)     1807 2023-11-06 13:30:18.000000 audiocraft-1.1.0/setup.py
-drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-11-07 12:54:21.870381 audiocraft-1.1.0/tests/
--rw-r--r--   0 defossez   (501) staff       (20)      198 2023-07-03 08:49:34.000000 audiocraft-1.1.0/tests/__init__.py
-drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-11-07 12:54:21.876027 audiocraft-1.1.0/tests/adversarial/
--rw-r--r--   0 defossez   (501) staff       (20)      198 2023-11-06 13:30:18.000000 audiocraft-1.1.0/tests/adversarial/__init__.py
--rw-r--r--   0 defossez   (501) staff       (20)     2295 2023-11-06 13:30:18.000000 audiocraft-1.1.0/tests/adversarial/test_discriminators.py
--rw-r--r--   0 defossez   (501) staff       (20)     5284 2023-11-06 13:30:18.000000 audiocraft-1.1.0/tests/adversarial/test_losses.py
-drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-11-07 12:54:21.881361 audiocraft-1.1.0/tests/common_utils/
--rw-r--r--   0 defossez   (501) staff       (20)      323 2023-07-03 08:49:34.000000 audiocraft-1.1.0/tests/common_utils/__init__.py
--rw-r--r--   0 defossez   (501) staff       (20)     1745 2023-11-06 13:30:18.000000 audiocraft-1.1.0/tests/common_utils/temp_utils.py
--rw-r--r--   0 defossez   (501) staff       (20)      860 2023-11-06 13:30:18.000000 audiocraft-1.1.0/tests/common_utils/wav_utils.py
-drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-11-07 12:54:21.890749 audiocraft-1.1.0/tests/data/
--rw-r--r--   0 defossez   (501) staff       (20)      198 2023-07-03 08:49:34.000000 audiocraft-1.1.0/tests/data/__init__.py
--rw-r--r--   0 defossez   (501) staff       (20)    10518 2023-07-03 08:49:34.000000 audiocraft-1.1.0/tests/data/test_audio.py
--rw-r--r--   0 defossez   (501) staff       (20)    15058 2023-11-06 13:30:18.000000 audiocraft-1.1.0/tests/data/test_audio_dataset.py
--rw-r--r--   0 defossez   (501) staff       (20)     3738 2023-07-03 08:49:34.000000 audiocraft-1.1.0/tests/data/test_audio_utils.py
-drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-11-07 12:54:21.895266 audiocraft-1.1.0/tests/losses/
--rw-r--r--   0 defossez   (501) staff       (20)      198 2023-11-06 13:30:18.000000 audiocraft-1.1.0/tests/losses/__init__.py
--rw-r--r--   0 defossez   (501) staff       (20)     1811 2023-11-06 13:30:18.000000 audiocraft-1.1.0/tests/losses/test_losses.py
-drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-11-07 12:54:21.927707 audiocraft-1.1.0/tests/modules/
--rw-r--r--   0 defossez   (501) staff       (20)      198 2023-07-03 08:49:34.000000 audiocraft-1.1.0/tests/modules/__init__.py
--rw-r--r--   0 defossez   (501) staff       (20)      827 2023-11-06 13:30:18.000000 audiocraft-1.1.0/tests/modules/test_activations.py
--rw-r--r--   0 defossez   (501) staff       (20)    10986 2023-07-03 08:49:34.000000 audiocraft-1.1.0/tests/modules/test_codebooks_patterns.py
--rw-r--r--   0 defossez   (501) staff       (20)     7383 2023-07-03 08:49:34.000000 audiocraft-1.1.0/tests/modules/test_conv.py
--rw-r--r--   0 defossez   (501) staff       (20)      781 2023-07-03 08:49:34.000000 audiocraft-1.1.0/tests/modules/test_lstm.py
--rw-r--r--   0 defossez   (501) staff       (20)     5112 2023-11-06 13:30:18.000000 audiocraft-1.1.0/tests/modules/test_rope.py
--rw-r--r--   0 defossez   (501) staff       (20)     4874 2023-07-03 08:49:34.000000 audiocraft-1.1.0/tests/modules/test_seanet.py
--rw-r--r--   0 defossez   (501) staff       (20)     9169 2023-11-06 13:30:18.000000 audiocraft-1.1.0/tests/modules/test_transformer.py
-drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-11-07 12:54:21.928969 audiocraft-1.1.0/tests/utils/
--rw-r--r--   0 defossez   (501) staff       (20)      198 2023-07-03 08:49:34.000000 audiocraft-1.1.0/tests/utils/__init__.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-01-15 16:55:28.693855 audiocraft-1.2.0/
+-rw-r--r--   0 alex       (501) staff       (20)     2266 2024-01-15 16:55:20.000000 audiocraft-1.2.0/CHANGELOG.md
+-rw-r--r--   0 alex       (501) staff       (20)     3535 2023-12-11 15:36:43.000000 audiocraft-1.2.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 alex       (501) staff       (20)     1377 2023-12-11 15:36:43.000000 audiocraft-1.2.0/CONTRIBUTING.md
+-rw-r--r--   0 alex       (501) staff       (20)     1088 2023-12-11 15:36:43.000000 audiocraft-1.2.0/LICENSE
+-rw-r--r--   0 alex       (501) staff       (20)    19333 2023-12-11 15:36:43.000000 audiocraft-1.2.0/LICENSE_weights
+-rw-r--r--   0 alex       (501) staff       (20)      368 2023-12-11 15:36:43.000000 audiocraft-1.2.0/MANIFEST.in
+-rw-r--r--   0 alex       (501) staff       (20)     1464 2023-12-11 15:36:43.000000 audiocraft-1.2.0/Makefile
+-rw-r--r--   0 alex       (501) staff       (20)     5667 2024-01-15 16:55:28.693793 audiocraft-1.2.0/PKG-INFO
+-rw-r--r--   0 alex       (501) staff       (20)     4333 2024-01-15 16:55:20.000000 audiocraft-1.2.0/README.md
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-01-15 16:55:28.655240 audiocraft-1.2.0/assets/
+-rw-r--r--   0 alex       (501) staff       (20)    15228 2023-12-11 15:36:43.000000 audiocraft-1.2.0/assets/a_duck_quacking_as_birds_chirp_and_a_pigeon_cooing.mp3
+-rw-r--r--   0 alex       (501) staff       (20)   160496 2023-12-11 15:36:43.000000 audiocraft-1.2.0/assets/bach.mp3
+-rw-r--r--   0 alex       (501) staff       (20)   161280 2023-12-11 15:36:43.000000 audiocraft-1.2.0/assets/bolero_ravel.mp3
+-rw-r--r--   0 alex       (501) staff       (20)    15228 2023-12-11 15:36:43.000000 audiocraft-1.2.0/assets/sirens_and_a_humming_engine_approach_and_pass.mp3
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-01-15 16:55:28.656029 audiocraft-1.2.0/audiocraft/
+-rw-r--r--   0 alex       (501) staff       (20)     1247 2024-01-15 16:55:20.000000 audiocraft-1.2.0/audiocraft/__init__.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-01-15 16:55:28.657036 audiocraft-1.2.0/audiocraft/adversarial/
+-rw-r--r--   0 alex       (501) staff       (20)      570 2023-12-11 15:36:43.000000 audiocraft-1.2.0/audiocraft/adversarial/__init__.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-01-15 16:55:28.657987 audiocraft-1.2.0/audiocraft/adversarial/discriminators/
+-rw-r--r--   0 alex       (501) staff       (20)      346 2023-12-11 15:36:43.000000 audiocraft-1.2.0/audiocraft/adversarial/discriminators/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)      894 2023-12-11 15:36:43.000000 audiocraft-1.2.0/audiocraft/adversarial/discriminators/base.py
+-rw-r--r--   0 alex       (501) staff       (20)     4176 2023-12-11 15:36:43.000000 audiocraft-1.2.0/audiocraft/adversarial/discriminators/mpd.py
+-rw-r--r--   0 alex       (501) staff       (20)     5926 2023-12-11 15:36:43.000000 audiocraft-1.2.0/audiocraft/adversarial/discriminators/msd.py
+-rw-r--r--   0 alex       (501) staff       (20)     6331 2023-12-11 15:36:43.000000 audiocraft-1.2.0/audiocraft/adversarial/discriminators/msstftd.py
+-rw-r--r--   0 alex       (501) staff       (20)     9126 2023-12-11 15:36:43.000000 audiocraft-1.2.0/audiocraft/adversarial/losses.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-01-15 16:55:28.659580 audiocraft-1.2.0/audiocraft/data/
+-rw-r--r--   0 alex       (501) staff       (20)      396 2023-12-11 15:36:43.000000 audiocraft-1.2.0/audiocraft/data/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)     9811 2023-12-11 15:36:43.000000 audiocraft-1.2.0/audiocraft/data/audio.py
+-rw-r--r--   0 alex       (501) staff       (20)    25464 2023-12-11 15:36:43.000000 audiocraft-1.2.0/audiocraft/data/audio_dataset.py
+-rw-r--r--   0 alex       (501) staff       (20)     7752 2023-12-11 15:36:43.000000 audiocraft-1.2.0/audiocraft/data/audio_utils.py
+-rw-r--r--   0 alex       (501) staff       (20)     3902 2023-12-11 15:36:43.000000 audiocraft-1.2.0/audiocraft/data/info_audio_dataset.py
+-rw-r--r--   0 alex       (501) staff       (20)    11575 2023-12-11 15:36:43.000000 audiocraft-1.2.0/audiocraft/data/music_dataset.py
+-rw-r--r--   0 alex       (501) staff       (20)    13381 2023-12-11 15:36:43.000000 audiocraft-1.2.0/audiocraft/data/sound_dataset.py
+-rw-r--r--   0 alex       (501) staff       (20)     2202 2023-12-11 15:36:43.000000 audiocraft-1.2.0/audiocraft/data/zip.py
+-rw-r--r--   0 alex       (501) staff       (20)     6741 2023-12-11 15:36:43.000000 audiocraft-1.2.0/audiocraft/environment.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-01-15 16:55:28.659984 audiocraft-1.2.0/audiocraft/grids/
+-rw-r--r--   0 alex       (501) staff       (20)      216 2023-12-11 15:36:43.000000 audiocraft-1.2.0/audiocraft/grids/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)     2639 2023-12-11 15:36:43.000000 audiocraft-1.2.0/audiocraft/grids/_base_explorers.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-01-15 16:55:28.660558 audiocraft-1.2.0/audiocraft/grids/audiogen/
+-rw-r--r--   0 alex       (501) staff       (20)      220 2023-12-11 15:36:43.000000 audiocraft-1.2.0/audiocraft/grids/audiogen/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)      776 2023-12-11 15:36:43.000000 audiocraft-1.2.0/audiocraft/grids/audiogen/audiogen_base_16khz.py
+-rw-r--r--   0 alex       (501) staff       (20)     2483 2023-12-11 15:36:43.000000 audiocraft-1.2.0/audiocraft/grids/audiogen/audiogen_pretrained_16khz_eval.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-01-15 16:55:28.661590 audiocraft-1.2.0/audiocraft/grids/compression/
+-rw-r--r--   0 alex       (501) staff       (20)      219 2023-12-11 15:36:43.000000 audiocraft-1.2.0/audiocraft/grids/compression/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)     1601 2023-12-11 15:36:43.000000 audiocraft-1.2.0/audiocraft/grids/compression/_explorers.py
+-rw-r--r--   0 alex       (501) staff       (20)     1117 2023-12-11 15:36:43.000000 audiocraft-1.2.0/audiocraft/grids/compression/debug.py
+-rw-r--r--   0 alex       (501) staff       (20)     1100 2023-12-11 15:36:43.000000 audiocraft-1.2.0/audiocraft/grids/compression/encodec_audiogen_16khz.py
+-rw-r--r--   0 alex       (501) staff       (20)      956 2023-12-11 15:36:43.000000 audiocraft-1.2.0/audiocraft/grids/compression/encodec_base_24khz.py
+-rw-r--r--   0 alex       (501) staff       (20)     1262 2023-12-11 15:36:43.000000 audiocraft-1.2.0/audiocraft/grids/compression/encodec_musicgen_32khz.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-01-15 16:55:28.662134 audiocraft-1.2.0/audiocraft/grids/diffusion/
+-rw-r--r--   0 alex       (501) staff       (20)     1073 2023-12-11 15:36:43.000000 audiocraft-1.2.0/audiocraft/grids/diffusion/4_bands_base_32khz.py
+-rw-r--r--   0 alex       (501) staff       (20)      221 2023-12-11 15:36:43.000000 audiocraft-1.2.0/audiocraft/grids/diffusion/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)     2066 2023-12-11 15:36:43.000000 audiocraft-1.2.0/audiocraft/grids/diffusion/_explorers.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-01-15 16:55:28.663715 audiocraft-1.2.0/audiocraft/grids/musicgen/
+-rw-r--r--   0 alex       (501) staff       (20)      220 2023-12-11 15:36:43.000000 audiocraft-1.2.0/audiocraft/grids/musicgen/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)     3092 2023-12-11 15:36:43.000000 audiocraft-1.2.0/audiocraft/grids/musicgen/_explorers.py
+-rw-r--r--   0 alex       (501) staff       (20)     1413 2023-12-11 15:36:43.000000 audiocraft-1.2.0/audiocraft/grids/musicgen/musicgen_base_32khz.py
+-rw-r--r--   0 alex       (501) staff       (20)     2311 2023-12-11 15:36:43.000000 audiocraft-1.2.0/audiocraft/grids/musicgen/musicgen_base_cached_32khz.py
+-rw-r--r--   0 alex       (501) staff       (20)     1193 2023-12-11 15:36:43.000000 audiocraft-1.2.0/audiocraft/grids/musicgen/musicgen_clapemb_32khz.py
+-rw-r--r--   0 alex       (501) staff       (20)     2251 2023-12-11 15:36:43.000000 audiocraft-1.2.0/audiocraft/grids/musicgen/musicgen_melody_32khz.py
+-rw-r--r--   0 alex       (501) staff       (20)     3880 2023-12-11 15:36:43.000000 audiocraft-1.2.0/audiocraft/grids/musicgen/musicgen_pretrained_32khz_eval.py
+-rw-r--r--   0 alex       (501) staff       (20)     2139 2023-12-11 15:36:43.000000 audiocraft-1.2.0/audiocraft/grids/musicgen/musicgen_stereo_finetune_32khz.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-01-15 16:55:28.664704 audiocraft-1.2.0/audiocraft/losses/
+-rw-r--r--   0 alex       (501) staff       (20)      585 2023-12-11 15:36:43.000000 audiocraft-1.2.0/audiocraft/losses/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)     6612 2023-12-11 15:36:43.000000 audiocraft-1.2.0/audiocraft/losses/balancer.py
+-rw-r--r--   0 alex       (501) staff       (20)     3263 2023-12-11 15:36:43.000000 audiocraft-1.2.0/audiocraft/losses/sisnr.py
+-rw-r--r--   0 alex       (501) staff       (20)     6531 2023-12-11 15:36:43.000000 audiocraft-1.2.0/audiocraft/losses/specloss.py
+-rw-r--r--   0 alex       (501) staff       (20)     8202 2023-12-11 15:36:43.000000 audiocraft-1.2.0/audiocraft/losses/stftloss.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-01-15 16:55:28.666257 audiocraft-1.2.0/audiocraft/metrics/
+-rw-r--r--   0 alex       (501) staff       (20)      592 2023-12-11 15:36:43.000000 audiocraft-1.2.0/audiocraft/metrics/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)     3674 2023-12-11 15:36:43.000000 audiocraft-1.2.0/audiocraft/metrics/chroma_cosinesim.py
+-rw-r--r--   0 alex       (501) staff       (20)     4525 2023-12-11 15:36:43.000000 audiocraft-1.2.0/audiocraft/metrics/clap_consistency.py
+-rw-r--r--   0 alex       (501) staff       (20)    17724 2023-12-11 15:36:43.000000 audiocraft-1.2.0/audiocraft/metrics/fad.py
+-rw-r--r--   0 alex       (501) staff       (20)    10211 2023-12-11 15:36:43.000000 audiocraft-1.2.0/audiocraft/metrics/kld.py
+-rw-r--r--   0 alex       (501) staff       (20)     6107 2023-12-11 15:36:43.000000 audiocraft-1.2.0/audiocraft/metrics/rvm.py
+-rw-r--r--   0 alex       (501) staff       (20)     9694 2023-12-11 15:36:43.000000 audiocraft-1.2.0/audiocraft/metrics/visqol.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-01-15 16:55:28.667484 audiocraft-1.2.0/audiocraft/models/
+-rw-r--r--   0 alex       (501) staff       (20)      605 2024-01-15 16:55:20.000000 audiocraft-1.2.0/audiocraft/models/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)    12444 2024-01-15 16:55:20.000000 audiocraft-1.2.0/audiocraft/models/audiogen.py
+-rw-r--r--   0 alex       (501) staff       (20)    10334 2024-01-15 16:55:20.000000 audiocraft-1.2.0/audiocraft/models/builders.py
+-rw-r--r--   0 alex       (501) staff       (20)    18018 2024-01-15 16:55:20.000000 audiocraft-1.2.0/audiocraft/models/encodec.py
+-rw-r--r--   0 alex       (501) staff       (20)    27199 2024-01-15 16:55:20.000000 audiocraft-1.2.0/audiocraft/models/lm.py
+-rw-r--r--   0 alex       (501) staff       (20)     5581 2024-01-15 16:55:20.000000 audiocraft-1.2.0/audiocraft/models/loaders.py
+-rw-r--r--   0 alex       (501) staff       (20)     8737 2024-01-15 16:54:28.000000 audiocraft-1.2.0/audiocraft/models/multibanddiffusion.py
+-rw-r--r--   0 alex       (501) staff       (20)    20463 2024-01-15 16:55:20.000000 audiocraft-1.2.0/audiocraft/models/musicgen.py
+-rw-r--r--   0 alex       (501) staff       (20)     8340 2023-12-11 15:36:43.000000 audiocraft-1.2.0/audiocraft/models/unet.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-01-15 16:55:28.671135 audiocraft-1.2.0/audiocraft/modules/
+-rw-r--r--   0 alex       (501) staff       (20)      586 2023-12-11 15:36:43.000000 audiocraft-1.2.0/audiocraft/modules/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)     3266 2023-12-11 15:36:43.000000 audiocraft-1.2.0/audiocraft/modules/activations.py
+-rw-r--r--   0 alex       (501) staff       (20)     3023 2023-12-11 15:36:43.000000 audiocraft-1.2.0/audiocraft/modules/chroma.py
+-rw-r--r--   0 alex       (501) staff       (20)    27943 2024-01-15 16:55:20.000000 audiocraft-1.2.0/audiocraft/modules/codebooks_patterns.py
+-rw-r--r--   0 alex       (501) staff       (20)    65008 2023-12-11 15:36:43.000000 audiocraft-1.2.0/audiocraft/modules/conditioners.py
+-rw-r--r--   0 alex       (501) staff       (20)    10496 2023-12-11 15:36:43.000000 audiocraft-1.2.0/audiocraft/modules/conv.py
+-rw-r--r--   0 alex       (501) staff       (20)    12018 2023-12-11 15:36:43.000000 audiocraft-1.2.0/audiocraft/modules/diffusion_schedule.py
+-rw-r--r--   0 alex       (501) staff       (20)      759 2023-12-11 15:36:43.000000 audiocraft-1.2.0/audiocraft/modules/lstm.py
+-rw-r--r--   0 alex       (501) staff       (20)     5649 2023-12-11 15:36:43.000000 audiocraft-1.2.0/audiocraft/modules/rope.py
+-rw-r--r--   0 alex       (501) staff       (20)    13868 2023-12-11 15:36:43.000000 audiocraft-1.2.0/audiocraft/modules/seanet.py
+-rw-r--r--   0 alex       (501) staff       (20)     4494 2023-12-11 15:36:43.000000 audiocraft-1.2.0/audiocraft/modules/streaming.py
+-rw-r--r--   0 alex       (501) staff       (20)    36933 2024-01-15 16:55:20.000000 audiocraft-1.2.0/audiocraft/modules/transformer.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-01-15 16:55:28.672692 audiocraft-1.2.0/audiocraft/optim/
+-rw-r--r--   0 alex       (501) staff       (20)      638 2023-12-11 15:36:43.000000 audiocraft-1.2.0/audiocraft/optim/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)     1730 2023-12-11 15:36:43.000000 audiocraft-1.2.0/audiocraft/optim/cosine_lr_scheduler.py
+-rw-r--r--   0 alex       (501) staff       (20)     8910 2023-12-11 15:36:43.000000 audiocraft-1.2.0/audiocraft/optim/dadam.py
+-rw-r--r--   0 alex       (501) staff       (20)     3196 2023-12-11 15:36:43.000000 audiocraft-1.2.0/audiocraft/optim/ema.py
+-rw-r--r--   0 alex       (501) staff       (20)     7316 2023-12-11 15:36:43.000000 audiocraft-1.2.0/audiocraft/optim/fsdp.py
+-rw-r--r--   0 alex       (501) staff       (20)     1390 2023-12-11 15:36:43.000000 audiocraft-1.2.0/audiocraft/optim/inverse_sqrt_lr_scheduler.py
+-rw-r--r--   0 alex       (501) staff       (20)     1272 2023-12-11 15:36:43.000000 audiocraft-1.2.0/audiocraft/optim/linear_warmup_lr_scheduler.py
+-rw-r--r--   0 alex       (501) staff       (20)     2012 2023-12-11 15:36:43.000000 audiocraft-1.2.0/audiocraft/optim/polynomial_decay_lr_scheduler.py
+-rw-r--r--   0 alex       (501) staff       (20)        0 2023-12-11 15:36:43.000000 audiocraft-1.2.0/audiocraft/py.typed
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-01-15 16:55:28.673224 audiocraft-1.2.0/audiocraft/quantization/
+-rw-r--r--   0 alex       (501) staff       (20)      329 2023-12-11 15:36:43.000000 audiocraft-1.2.0/audiocraft/quantization/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)     3314 2023-12-11 15:36:43.000000 audiocraft-1.2.0/audiocraft/quantization/base.py
+-rw-r--r--   0 alex       (501) staff       (20)    14593 2024-01-15 16:54:28.000000 audiocraft-1.2.0/audiocraft/quantization/core_vq.py
+-rw-r--r--   0 alex       (501) staff       (20)     4649 2023-12-11 15:36:43.000000 audiocraft-1.2.0/audiocraft/quantization/vq.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-01-15 16:55:28.674560 audiocraft-1.2.0/audiocraft/solvers/
+-rw-r--r--   0 alex       (501) staff       (20)      574 2023-12-11 15:36:43.000000 audiocraft-1.2.0/audiocraft/solvers/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)      655 2023-12-11 15:36:43.000000 audiocraft-1.2.0/audiocraft/solvers/audiogen.py
+-rw-r--r--   0 alex       (501) staff       (20)    31355 2023-12-11 15:36:43.000000 audiocraft-1.2.0/audiocraft/solvers/base.py
+-rw-r--r--   0 alex       (501) staff       (20)    13937 2024-01-15 16:55:20.000000 audiocraft-1.2.0/audiocraft/solvers/builders.py
+-rw-r--r--   0 alex       (501) staff       (20)    14774 2023-12-11 15:36:43.000000 audiocraft-1.2.0/audiocraft/solvers/compression.py
+-rw-r--r--   0 alex       (501) staff       (20)    11336 2023-12-11 15:36:43.000000 audiocraft-1.2.0/audiocraft/solvers/diffusion.py
+-rw-r--r--   0 alex       (501) staff       (20)    36228 2024-01-15 16:54:28.000000 audiocraft-1.2.0/audiocraft/solvers/musicgen.py
+-rw-r--r--   0 alex       (501) staff       (20)     6724 2023-12-11 15:36:43.000000 audiocraft-1.2.0/audiocraft/train.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-01-15 16:55:28.676616 audiocraft-1.2.0/audiocraft/utils/
+-rw-r--r--   0 alex       (501) staff       (20)      215 2023-12-11 15:36:43.000000 audiocraft-1.2.0/audiocraft/utils/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)     1377 2023-12-11 15:36:43.000000 audiocraft-1.2.0/audiocraft/utils/autocast.py
+-rw-r--r--   0 alex       (501) staff       (20)     3694 2023-12-11 15:36:43.000000 audiocraft-1.2.0/audiocraft/utils/best_state.py
+-rw-r--r--   0 alex       (501) staff       (20)    14356 2023-12-11 15:36:43.000000 audiocraft-1.2.0/audiocraft/utils/cache.py
+-rw-r--r--   0 alex       (501) staff       (20)     6129 2023-12-11 15:36:43.000000 audiocraft-1.2.0/audiocraft/utils/checkpoint.py
+-rw-r--r--   0 alex       (501) staff       (20)     2044 2023-12-11 15:36:43.000000 audiocraft-1.2.0/audiocraft/utils/cluster.py
+-rw-r--r--   0 alex       (501) staff       (20)     1710 2023-12-11 15:36:43.000000 audiocraft-1.2.0/audiocraft/utils/deadlock.py
+-rw-r--r--   0 alex       (501) staff       (20)     2677 2023-12-11 15:36:43.000000 audiocraft-1.2.0/audiocraft/utils/export.py
+-rw-r--r--   0 alex       (501) staff       (20)     2403 2023-12-11 15:36:43.000000 audiocraft-1.2.0/audiocraft/utils/export_legacy.py
+-rw-r--r--   0 alex       (501) staff       (20)      885 2023-12-11 15:36:43.000000 audiocraft-1.2.0/audiocraft/utils/notebook.py
+-rw-r--r--   0 alex       (501) staff       (20)     1209 2023-12-11 15:36:43.000000 audiocraft-1.2.0/audiocraft/utils/profiler.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-01-15 16:55:28.677056 audiocraft-1.2.0/audiocraft/utils/samples/
+-rw-r--r--   0 alex       (501) staff       (20)      198 2023-12-11 15:36:43.000000 audiocraft-1.2.0/audiocraft/utils/samples/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)    19385 2023-12-11 15:36:43.000000 audiocraft-1.2.0/audiocraft/utils/samples/manager.py
+-rw-r--r--   0 alex       (501) staff       (20)    10611 2023-12-11 15:36:43.000000 audiocraft-1.2.0/audiocraft/utils/utils.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-01-15 16:55:28.656741 audiocraft-1.2.0/audiocraft.egg-info/
+-rw-r--r--   0 alex       (501) staff       (20)     5667 2024-01-15 16:55:28.000000 audiocraft-1.2.0/audiocraft.egg-info/PKG-INFO
+-rw-r--r--   0 alex       (501) staff       (20)     7120 2024-01-15 16:55:28.000000 audiocraft-1.2.0/audiocraft.egg-info/SOURCES.txt
+-rw-r--r--   0 alex       (501) staff       (20)        1 2024-01-15 16:55:28.000000 audiocraft-1.2.0/audiocraft.egg-info/dependency_links.txt
+-rw-r--r--   0 alex       (501) staff       (20)      280 2024-01-15 16:55:28.000000 audiocraft-1.2.0/audiocraft.egg-info/requires.txt
+-rw-r--r--   0 alex       (501) staff       (20)       25 2024-01-15 16:55:28.000000 audiocraft-1.2.0/audiocraft.egg-info/top_level.txt
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-01-15 16:55:28.677596 audiocraft-1.2.0/config/
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-01-15 16:55:28.678215 audiocraft-1.2.0/config/conditioner/
+-rw-r--r--   0 alex       (501) staff       (20)      817 2023-12-11 15:36:43.000000 audiocraft-1.2.0/config/conditioner/chroma2music.yaml
+-rw-r--r--   0 alex       (501) staff       (20)      922 2023-12-11 15:36:43.000000 audiocraft-1.2.0/config/conditioner/clapemb2music.yaml
+-rw-r--r--   0 alex       (501) staff       (20)      239 2023-12-11 15:36:43.000000 audiocraft-1.2.0/config/conditioner/none.yaml
+-rw-r--r--   0 alex       (501) staff       (20)      496 2023-12-11 15:36:43.000000 audiocraft-1.2.0/config/conditioner/text2music.yaml
+-rw-r--r--   0 alex       (501) staff       (20)      411 2023-12-11 15:36:43.000000 audiocraft-1.2.0/config/conditioner/text2sound.yaml
+-rw-r--r--   0 alex       (501) staff       (20)     2733 2023-12-11 15:36:43.000000 audiocraft-1.2.0/config/config.yaml
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-01-15 16:55:28.678344 audiocraft-1.2.0/config/dset/
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-01-15 16:55:28.678956 audiocraft-1.2.0/config/dset/audio/
+-rw-r--r--   0 alex       (501) staff       (20)      281 2023-12-11 15:36:43.000000 audiocraft-1.2.0/config/dset/audio/audiocaps_16khz.yaml
+-rw-r--r--   0 alex       (501) staff       (20)      138 2023-12-11 15:36:43.000000 audiocraft-1.2.0/config/dset/audio/default.yaml
+-rw-r--r--   0 alex       (501) staff       (20)      169 2023-12-11 15:36:43.000000 audiocraft-1.2.0/config/dset/audio/example.yaml
+-rw-r--r--   0 alex       (501) staff       (20)      358 2023-12-11 15:36:43.000000 audiocraft-1.2.0/config/dset/audio/musiccaps_32khz.yaml
+-rw-r--r--   0 alex       (501) staff       (20)      300 2023-12-11 15:36:43.000000 audiocraft-1.2.0/config/dset/default.yaml
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-01-15 16:55:28.679547 audiocraft-1.2.0/config/dset/internal/
+-rw-r--r--   0 alex       (501) staff       (20)      338 2023-12-11 15:36:43.000000 audiocraft-1.2.0/config/dset/internal/music_10k_32khz.yaml
+-rw-r--r--   0 alex       (501) staff       (20)      275 2023-12-11 15:36:43.000000 audiocraft-1.2.0/config/dset/internal/music_400k_32khz.yaml
+-rw-r--r--   0 alex       (501) staff       (20)      344 2023-12-11 15:36:43.000000 audiocraft-1.2.0/config/dset/internal/sounds_16khz.yaml
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-01-15 16:55:28.679687 audiocraft-1.2.0/config/model/
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-01-15 16:55:28.680238 audiocraft-1.2.0/config/model/encodec/
+-rw-r--r--   0 alex       (501) staff       (20)     1112 2023-12-11 15:36:43.000000 audiocraft-1.2.0/config/model/encodec/default.yaml
+-rw-r--r--   0 alex       (501) staff       (20)      112 2023-12-11 15:36:43.000000 audiocraft-1.2.0/config/model/encodec/encodec_base_causal.yaml
+-rw-r--r--   0 alex       (501) staff       (20)      161 2023-12-11 15:36:43.000000 audiocraft-1.2.0/config/model/encodec/encodec_large_nq4_s320.yaml
+-rw-r--r--   0 alex       (501) staff       (20)      148 2023-12-11 15:36:43.000000 audiocraft-1.2.0/config/model/encodec/encodec_large_nq4_s640.yaml
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-01-15 16:55:28.680632 audiocraft-1.2.0/config/model/lm/
+-rw-r--r--   0 alex       (501) staff       (20)      738 2023-12-11 15:36:43.000000 audiocraft-1.2.0/config/model/lm/audiogen_lm.yaml
+-rw-r--r--   0 alex       (501) staff       (20)     1992 2023-12-11 15:36:43.000000 audiocraft-1.2.0/config/model/lm/default.yaml
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-01-15 16:55:28.681280 audiocraft-1.2.0/config/model/lm/model_scale/
+-rw-r--r--   0 alex       (501) staff       (20)      102 2023-12-11 15:36:43.000000 audiocraft-1.2.0/config/model/lm/model_scale/base.yaml
+-rw-r--r--   0 alex       (501) staff       (20)      126 2023-12-11 15:36:43.000000 audiocraft-1.2.0/config/model/lm/model_scale/large.yaml
+-rw-r--r--   0 alex       (501) staff       (20)      109 2023-12-11 15:36:43.000000 audiocraft-1.2.0/config/model/lm/model_scale/medium.yaml
+-rw-r--r--   0 alex       (501) staff       (20)       97 2023-12-11 15:36:43.000000 audiocraft-1.2.0/config/model/lm/model_scale/small.yaml
+-rw-r--r--   0 alex       (501) staff       (20)      181 2023-12-11 15:36:43.000000 audiocraft-1.2.0/config/model/lm/model_scale/xsmall.yaml
+-rw-r--r--   0 alex       (501) staff       (20)      738 2023-12-11 15:36:43.000000 audiocraft-1.2.0/config/model/lm/musicgen_lm.yaml
+-rw-r--r--   0 alex       (501) staff       (20)      157 2023-12-11 15:36:43.000000 audiocraft-1.2.0/config/model/none.yaml
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-01-15 16:55:28.681409 audiocraft-1.2.0/config/model/score/
+-rw-r--r--   0 alex       (501) staff       (20)      269 2023-12-11 15:36:43.000000 audiocraft-1.2.0/config/model/score/basic.yaml
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-01-15 16:55:28.681542 audiocraft-1.2.0/config/solver/
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-01-15 16:55:28.681927 audiocraft-1.2.0/config/solver/audiogen/
+-rw-r--r--   0 alex       (501) staff       (20)     1772 2023-12-11 15:36:43.000000 audiocraft-1.2.0/config/solver/audiogen/audiogen_base_16khz.yaml
+-rw-r--r--   0 alex       (501) staff       (20)      972 2023-12-11 15:36:43.000000 audiocraft-1.2.0/config/solver/audiogen/debug.yaml
+-rw-r--r--   0 alex       (501) staff       (20)      769 2023-12-11 15:36:43.000000 audiocraft-1.2.0/config/solver/audiogen/default.yaml
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-01-15 16:55:28.682201 audiocraft-1.2.0/config/solver/audiogen/evaluation/
+-rw-r--r--   0 alex       (501) staff       (20)       67 2023-12-11 15:36:43.000000 audiocraft-1.2.0/config/solver/audiogen/evaluation/none.yaml
+-rw-r--r--   0 alex       (501) staff       (20)      725 2023-12-11 15:36:43.000000 audiocraft-1.2.0/config/solver/audiogen/evaluation/objective_eval.yaml
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-01-15 16:55:28.683059 audiocraft-1.2.0/config/solver/compression/
+-rw-r--r--   0 alex       (501) staff       (20)      812 2023-12-11 15:36:43.000000 audiocraft-1.2.0/config/solver/compression/debug.yaml
+-rw-r--r--   0 alex       (501) staff       (20)     2955 2023-12-11 15:36:43.000000 audiocraft-1.2.0/config/solver/compression/default.yaml
+-rw-r--r--   0 alex       (501) staff       (20)      177 2023-12-11 15:36:43.000000 audiocraft-1.2.0/config/solver/compression/encodec_audiogen_16khz.yaml
+-rw-r--r--   0 alex       (501) staff       (20)      174 2023-12-11 15:36:43.000000 audiocraft-1.2.0/config/solver/compression/encodec_base_24khz.yaml
+-rw-r--r--   0 alex       (501) staff       (20)      177 2023-12-11 15:36:43.000000 audiocraft-1.2.0/config/solver/compression/encodec_musicgen_32khz.yaml
+-rw-r--r--   0 alex       (501) staff       (20)     2534 2023-12-11 15:36:43.000000 audiocraft-1.2.0/config/solver/default.yaml
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-01-15 16:55:28.683507 audiocraft-1.2.0/config/solver/diffusion/
+-rw-r--r--   0 alex       (501) staff       (20)     1677 2023-12-11 15:36:43.000000 audiocraft-1.2.0/config/solver/diffusion/debug.yaml
+-rw-r--r--   0 alex       (501) staff       (20)     1690 2023-12-11 15:36:43.000000 audiocraft-1.2.0/config/solver/diffusion/default.yaml
+-rw-r--r--   0 alex       (501) staff       (20)      197 2023-12-11 15:36:43.000000 audiocraft-1.2.0/config/solver/diffusion/encodec_24khz.yaml
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-01-15 16:55:28.684021 audiocraft-1.2.0/config/solver/musicgen/
+-rw-r--r--   0 alex       (501) staff       (20)     1004 2023-12-11 15:36:43.000000 audiocraft-1.2.0/config/solver/musicgen/debug.yaml
+-rw-r--r--   0 alex       (501) staff       (20)     2737 2023-12-11 15:36:43.000000 audiocraft-1.2.0/config/solver/musicgen/default.yaml
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-01-15 16:55:28.684290 audiocraft-1.2.0/config/solver/musicgen/evaluation/
+-rw-r--r--   0 alex       (501) staff       (20)       67 2023-12-11 15:36:43.000000 audiocraft-1.2.0/config/solver/musicgen/evaluation/none.yaml
+-rw-r--r--   0 alex       (501) staff       (20)      619 2023-12-11 15:36:43.000000 audiocraft-1.2.0/config/solver/musicgen/evaluation/objective_eval.yaml
+-rw-r--r--   0 alex       (501) staff       (20)     1125 2023-12-11 15:36:43.000000 audiocraft-1.2.0/config/solver/musicgen/musicgen_base_32khz.yaml
+-rw-r--r--   0 alex       (501) staff       (20)     1174 2023-12-11 15:36:43.000000 audiocraft-1.2.0/config/solver/musicgen/musicgen_melody_32khz.yaml
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-01-15 16:55:28.684553 audiocraft-1.2.0/config/teams/
+-rw-r--r--   0 alex       (501) staff       (20)      324 2023-12-11 15:36:43.000000 audiocraft-1.2.0/config/teams/default.yaml
+-rw-r--r--   0 alex       (501) staff       (20)      836 2023-12-11 15:36:43.000000 audiocraft-1.2.0/config/teams/labs.yaml
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-01-15 16:55:28.687354 audiocraft-1.2.0/demos/
+-rw-r--r--   0 alex       (501) staff       (20)     5469 2023-12-11 15:36:43.000000 audiocraft-1.2.0/demos/audiogen_demo.ipynb
+-rw-r--r--   0 alex       (501) staff       (20)    22463 2023-12-11 15:36:43.000000 audiocraft-1.2.0/demos/musicgen_app.py
+-rw-r--r--   0 alex       (501) staff       (20)     7843 2023-12-11 15:36:43.000000 audiocraft-1.2.0/demos/musicgen_demo.ipynb
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-01-15 16:55:28.689005 audiocraft-1.2.0/docs/
+-rw-r--r--   0 alex       (501) staff       (20)     6557 2023-12-11 15:36:43.000000 audiocraft-1.2.0/docs/AUDIOGEN.md
+-rw-r--r--   0 alex       (501) staff       (20)     7377 2024-01-15 16:54:28.000000 audiocraft-1.2.0/docs/CONDITIONING.md
+-rw-r--r--   0 alex       (501) staff       (20)     3073 2023-12-11 15:36:43.000000 audiocraft-1.2.0/docs/DATASETS.md
+-rw-r--r--   0 alex       (501) staff       (20)     6809 2024-01-15 16:54:28.000000 audiocraft-1.2.0/docs/ENCODEC.md
+-rw-r--r--   0 alex       (501) staff       (20)     5076 2023-12-11 15:36:43.000000 audiocraft-1.2.0/docs/MBD.md
+-rw-r--r--   0 alex       (501) staff       (20)     5769 2023-12-11 15:36:43.000000 audiocraft-1.2.0/docs/METRICS.md
+-rw-r--r--   0 alex       (501) staff       (20)    19365 2023-12-11 15:36:43.000000 audiocraft-1.2.0/docs/MUSICGEN.md
+-rw-r--r--   0 alex       (501) staff       (20)    14426 2024-01-15 16:54:28.000000 audiocraft-1.2.0/docs/TRAINING.md
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-01-15 16:55:28.689302 audiocraft-1.2.0/model_cards/
+-rw-r--r--   0 alex       (501) staff       (20)     5788 2023-12-11 15:36:43.000000 audiocraft-1.2.0/model_cards/AUDIOGEN_MODEL_CARD.md
+-rw-r--r--   0 alex       (501) staff       (20)     7484 2023-12-11 15:36:43.000000 audiocraft-1.2.0/model_cards/MUSICGEN_MODEL_CARD.md
+-rw-r--r--   0 alex       (501) staff       (20)      169 2023-12-11 15:36:43.000000 audiocraft-1.2.0/mypy.ini
+-rw-r--r--   0 alex       (501) staff       (20)      338 2023-12-11 15:36:43.000000 audiocraft-1.2.0/requirements.txt
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-01-15 16:55:28.689960 audiocraft-1.2.0/scripts/
+-rw-r--r--   0 alex       (501) staff       (20)      198 2023-12-11 15:36:43.000000 audiocraft-1.2.0/scripts/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)     9641 2023-12-11 15:36:43.000000 audiocraft-1.2.0/scripts/mos.py
+-rw-r--r--   0 alex       (501) staff       (20)     7478 2023-12-11 15:36:43.000000 audiocraft-1.2.0/scripts/resample_dataset.py
+-rw-r--r--   0 alex       (501) staff       (20)      270 2024-01-15 16:55:28.694118 audiocraft-1.2.0/setup.cfg
+-rw-r--r--   0 alex       (501) staff       (20)     1807 2023-12-11 15:36:43.000000 audiocraft-1.2.0/setup.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-01-15 16:55:28.690103 audiocraft-1.2.0/tests/
+-rw-r--r--   0 alex       (501) staff       (20)      198 2023-12-11 15:36:43.000000 audiocraft-1.2.0/tests/__init__.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-01-15 16:55:28.690557 audiocraft-1.2.0/tests/adversarial/
+-rw-r--r--   0 alex       (501) staff       (20)      198 2023-12-11 15:36:43.000000 audiocraft-1.2.0/tests/adversarial/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)     2295 2023-12-11 15:36:43.000000 audiocraft-1.2.0/tests/adversarial/test_discriminators.py
+-rw-r--r--   0 alex       (501) staff       (20)     5284 2023-12-11 15:36:43.000000 audiocraft-1.2.0/tests/adversarial/test_losses.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-01-15 16:55:28.691006 audiocraft-1.2.0/tests/common_utils/
+-rw-r--r--   0 alex       (501) staff       (20)      323 2023-12-11 15:36:43.000000 audiocraft-1.2.0/tests/common_utils/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)     1745 2023-12-11 15:36:43.000000 audiocraft-1.2.0/tests/common_utils/temp_utils.py
+-rw-r--r--   0 alex       (501) staff       (20)      860 2023-12-11 15:36:43.000000 audiocraft-1.2.0/tests/common_utils/wav_utils.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-01-15 16:55:28.691766 audiocraft-1.2.0/tests/data/
+-rw-r--r--   0 alex       (501) staff       (20)      198 2023-12-11 15:36:43.000000 audiocraft-1.2.0/tests/data/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)    10518 2023-12-11 15:36:43.000000 audiocraft-1.2.0/tests/data/test_audio.py
+-rw-r--r--   0 alex       (501) staff       (20)    15058 2023-12-11 15:36:43.000000 audiocraft-1.2.0/tests/data/test_audio_dataset.py
+-rw-r--r--   0 alex       (501) staff       (20)     3738 2023-12-11 15:36:43.000000 audiocraft-1.2.0/tests/data/test_audio_utils.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-01-15 16:55:28.692009 audiocraft-1.2.0/tests/losses/
+-rw-r--r--   0 alex       (501) staff       (20)      198 2023-12-11 15:36:43.000000 audiocraft-1.2.0/tests/losses/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)     1811 2023-12-11 15:36:43.000000 audiocraft-1.2.0/tests/losses/test_losses.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-01-15 16:55:28.693036 audiocraft-1.2.0/tests/modules/
+-rw-r--r--   0 alex       (501) staff       (20)      198 2023-12-11 15:36:43.000000 audiocraft-1.2.0/tests/modules/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)      827 2023-12-11 15:36:43.000000 audiocraft-1.2.0/tests/modules/test_activations.py
+-rw-r--r--   0 alex       (501) staff       (20)    10986 2023-12-11 15:36:43.000000 audiocraft-1.2.0/tests/modules/test_codebooks_patterns.py
+-rw-r--r--   0 alex       (501) staff       (20)     7383 2023-12-11 15:36:43.000000 audiocraft-1.2.0/tests/modules/test_conv.py
+-rw-r--r--   0 alex       (501) staff       (20)      781 2023-12-11 15:36:43.000000 audiocraft-1.2.0/tests/modules/test_lstm.py
+-rw-r--r--   0 alex       (501) staff       (20)     5112 2023-12-11 15:36:43.000000 audiocraft-1.2.0/tests/modules/test_rope.py
+-rw-r--r--   0 alex       (501) staff       (20)     4874 2023-12-11 15:36:43.000000 audiocraft-1.2.0/tests/modules/test_seanet.py
+-rw-r--r--   0 alex       (501) staff       (20)     9169 2023-12-11 15:36:43.000000 audiocraft-1.2.0/tests/modules/test_transformer.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-01-15 16:55:28.693174 audiocraft-1.2.0/tests/utils/
+-rw-r--r--   0 alex       (501) staff       (20)      198 2023-12-11 15:36:43.000000 audiocraft-1.2.0/tests/utils/__init__.py
```

### Comparing `audiocraft-1.1.0/CHANGELOG.md` & `audiocraft-1.2.0/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,22 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/).
 
+## [1.2.0] - 2024-01-11
+
+Adding stereo models.
+
+Fixed the commitment loss, which was until now only applied to the first RVQ layer.
+
+Removed compression model state from the LM checkpoints, for consistency, it
+should always be loaded from the original `compression_model_checkpoint`.
+
 
 ## [1.1.0] - 2023-11-06
 
 Not using torchaudio anymore when writing audio files, relying instead directly on the commandline ffmpeg. Also not using it anymore for reading audio files, for similar reasons.
 
 Fixed DAC support with non default number of codebooks.
```

### Comparing `audiocraft-1.1.0/CODE_OF_CONDUCT.md` & `audiocraft-1.2.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/CONTRIBUTING.md` & `audiocraft-1.2.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/LICENSE` & `audiocraft-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/LICENSE_weights` & `audiocraft-1.2.0/LICENSE_weights`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/Makefile` & `audiocraft-1.2.0/Makefile`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/PKG-INFO` & `audiocraft-1.2.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,101 +1,86 @@
-Metadata-Version: 2.1
-Name: audiocraft
-Version: 1.1.0
-Summary: Audio generation research library for PyTorch
-Home-page: https://github.com/facebookresearch/audiocraft
-Author: FAIR Speech & Audio
-Author-email: defossez@meta.com, jadecopet@meta.com
-License: MIT License
-Description: 
-        # AudioCraft
-        ![docs badge](https://github.com/facebookresearch/audiocraft/workflows/audiocraft_docs/badge.svg)
-        ![linter badge](https://github.com/facebookresearch/audiocraft/workflows/audiocraft_linter/badge.svg)
-        ![tests badge](https://github.com/facebookresearch/audiocraft/workflows/audiocraft_tests/badge.svg)
-        
-        AudioCraft is a PyTorch library for deep learning research on audio generation. AudioCraft contains inference and training code
-        for two state-of-the-art AI generative models producing high-quality audio: AudioGen and MusicGen.
-        
-        
-        ## Installation
-        AudioCraft requires Python 3.9, PyTorch 2.0.0. To install AudioCraft, you can run the following:
-        
-        ```shell
-        # Best to make sure you have torch installed first, in particular before installing xformers.
-        # Don't run this if you already have PyTorch installed.
-        pip install 'torch>=2.0'
-        # Then proceed to one of the following
-        pip install -U audiocraft  # stable release
-        pip install -U git+https://git@github.com/facebookresearch/audiocraft#egg=audiocraft  # bleeding edge
-        pip install -e .  # or if you cloned the repo locally (mandatory if you want to train).
-        ```
-        
-        We also recommend having `ffmpeg` installed, either through your system or Anaconda:
-        ```bash
-        sudo apt-get install ffmpeg
-        # Or if you are using Anaconda or Miniconda
-        conda install "ffmpeg<5" -c conda-forge
-        ```
-        
-        ## Models
-        
-        At the moment, AudioCraft contains the training code and inference code for:
-        * [MusicGen](./docs/MUSICGEN.md): A state-of-the-art controllable text-to-music model.
-        * [AudioGen](./docs/AUDIOGEN.md): A state-of-the-art text-to-sound model.
-        * [EnCodec](./docs/ENCODEC.md): A state-of-the-art high fidelity neural audio codec.
-        * [Multi Band Diffusion](./docs/MBD.md): An EnCodec compatible decoder using diffusion.
-        
-        ## Training code
-        
-        AudioCraft contains PyTorch components for deep learning research in audio and training pipelines for the developed models.
-        For a general introduction of AudioCraft design principles and instructions to develop your own training pipeline, refer to
-        the [AudioCraft training documentation](./docs/TRAINING.md).
-        
-        For reproducing existing work and using the developed training pipelines, refer to the instructions for each specific model
-        that provides pointers to configuration, example grids and model/task-specific information and FAQ.
-        
-        
-        ## API documentation
-        
-        We provide some [API documentation](https://facebookresearch.github.io/audiocraft/api_docs/audiocraft/index.html) for AudioCraft.
-        
-        
-        ## FAQ
-        
-        #### Is the training code available?
-        
-        Yes! We provide the training code for [EnCodec](./docs/ENCODEC.md), [MusicGen](./docs/MUSICGEN.md) and [Multi Band Diffusion](./docs/MBD.md).
-        
-        #### Where are the models stored?
-        
-        Hugging Face stored the model in a specific location, which can be overriden by setting the `AUDIOCRAFT_CACHE_DIR` environment variable for the AudioCraft models.
-        In order to change the cache location of the other Hugging Face models, please check out the [Hugging Face Transformers documentation for the cache setup](https://huggingface.co/docs/transformers/installation#cache-setup).
-        Finally, if you use a model that relies on Demucs (e.g. `musicgen-melody`) and want to change the download location for Demucs, refer to the [Torch Hub documentation](https://pytorch.org/docs/stable/hub.html#where-are-my-downloaded-models-saved).
-        
-        
-        ## License
-        * The code in this repository is released under the MIT license as found in the [LICENSE file](LICENSE).
-        * The models weights in this repository are released under the CC-BY-NC 4.0 license as found in the [LICENSE_weights file](LICENSE_weights).
-        
-        
-        ## Citation
-        
-        For the general framework of AudioCraft, please cite the following.
-        ```
-        @article{copet2023simple,
-            title={Simple and Controllable Music Generation},
-            author={Jade Copet and Felix Kreuk and Itai Gat and Tal Remez and David Kant and Gabriel Synnaeve and Yossi Adi and Alexandre Défossez},
-            year={2023},
-            journal={arXiv preprint arXiv:2306.05284},
-        }
-        ```
-        
-        When referring to a specific model, please cite as mentioned in the model specific README, e.g
-        [./docs/MUSICGEN.md](./docs/MUSICGEN.md), [./docs/AUDIOGEN.md](./docs/AUDIOGEN.md), etc.
-        
-Platform: UNKNOWN
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Topic :: Multimedia :: Sound/Audio
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.8.0
-Description-Content-Type: text/markdown
-Provides-Extra: dev
+# AudioCraft
+![docs badge](https://github.com/facebookresearch/audiocraft/workflows/audiocraft_docs/badge.svg)
+![linter badge](https://github.com/facebookresearch/audiocraft/workflows/audiocraft_linter/badge.svg)
+![tests badge](https://github.com/facebookresearch/audiocraft/workflows/audiocraft_tests/badge.svg)
+
+AudioCraft is a PyTorch library for deep learning research on audio generation. AudioCraft contains inference and training code
+for two state-of-the-art AI generative models producing high-quality audio: AudioGen and MusicGen.
+
+
+## Installation
+AudioCraft requires Python 3.9, PyTorch 2.1.0. To install AudioCraft, you can run the following:
+
+```shell
+# Best to make sure you have torch installed first, in particular before installing xformers.
+# Don't run this if you already have PyTorch installed.
+python -m pip install 'torch==2.1.0'
+# You might need the following before trying to install the packages
+python -m pip install setuptools wheel
+# Then proceed to one of the following
+python -m pip install -U audiocraft  # stable release
+python -m pip install -U git+https://git@github.com/facebookresearch/audiocraft#egg=audiocraft  # bleeding edge
+python -m pip install -e .  # or if you cloned the repo locally (mandatory if you want to train).
+```
+
+We also recommend having `ffmpeg` installed, either through your system or Anaconda:
+```bash
+sudo apt-get install ffmpeg
+# Or if you are using Anaconda or Miniconda
+conda install "ffmpeg<5" -c conda-forge
+```
+
+## Models
+
+At the moment, AudioCraft contains the training code and inference code for:
+* [MusicGen](./docs/MUSICGEN.md): A state-of-the-art controllable text-to-music model.
+* [AudioGen](./docs/AUDIOGEN.md): A state-of-the-art text-to-sound model.
+* [EnCodec](./docs/ENCODEC.md): A state-of-the-art high fidelity neural audio codec.
+* [Multi Band Diffusion](./docs/MBD.md): An EnCodec compatible decoder using diffusion.
+
+## Training code
+
+AudioCraft contains PyTorch components for deep learning research in audio and training pipelines for the developed models.
+For a general introduction of AudioCraft design principles and instructions to develop your own training pipeline, refer to
+the [AudioCraft training documentation](./docs/TRAINING.md).
+
+For reproducing existing work and using the developed training pipelines, refer to the instructions for each specific model
+that provides pointers to configuration, example grids and model/task-specific information and FAQ.
+
+
+## API documentation
+
+We provide some [API documentation](https://facebookresearch.github.io/audiocraft/api_docs/audiocraft/index.html) for AudioCraft.
+
+
+## FAQ
+
+#### Is the training code available?
+
+Yes! We provide the training code for [EnCodec](./docs/ENCODEC.md), [MusicGen](./docs/MUSICGEN.md) and [Multi Band Diffusion](./docs/MBD.md).
+
+#### Where are the models stored?
+
+Hugging Face stored the model in a specific location, which can be overriden by setting the `AUDIOCRAFT_CACHE_DIR` environment variable for the AudioCraft models.
+In order to change the cache location of the other Hugging Face models, please check out the [Hugging Face Transformers documentation for the cache setup](https://huggingface.co/docs/transformers/installation#cache-setup).
+Finally, if you use a model that relies on Demucs (e.g. `musicgen-melody`) and want to change the download location for Demucs, refer to the [Torch Hub documentation](https://pytorch.org/docs/stable/hub.html#where-are-my-downloaded-models-saved).
+
+
+## License
+* The code in this repository is released under the MIT license as found in the [LICENSE file](LICENSE).
+* The models weights in this repository are released under the CC-BY-NC 4.0 license as found in the [LICENSE_weights file](LICENSE_weights).
+
+
+## Citation
+
+For the general framework of AudioCraft, please cite the following.
+```
+@inproceedings{copet2023simple,
+    title={Simple and Controllable Music Generation},
+    author={Jade Copet and Felix Kreuk and Itai Gat and Tal Remez and David Kant and Gabriel Synnaeve and Yossi Adi and Alexandre Défossez},
+    booktitle={Thirty-seventh Conference on Neural Information Processing Systems},
+    year={2023},
+}
+```
+
+When referring to a specific model, please cite as mentioned in the model specific README, e.g
+[./docs/MUSICGEN.md](./docs/MUSICGEN.md), [./docs/AUDIOGEN.md](./docs/AUDIOGEN.md), etc.
```

### Comparing `audiocraft-1.1.0/assets/a_duck_quacking_as_birds_chirp_and_a_pigeon_cooing.mp3` & `audiocraft-1.2.0/assets/a_duck_quacking_as_birds_chirp_and_a_pigeon_cooing.mp3`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/assets/bach.mp3` & `audiocraft-1.2.0/assets/bach.mp3`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/assets/bolero_ravel.mp3` & `audiocraft-1.2.0/assets/bolero_ravel.mp3`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/assets/sirens_and_a_humming_engine_approach_and_pass.mp3` & `audiocraft-1.2.0/assets/sirens_and_a_humming_engine_approach_and_pass.mp3`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/audiocraft/__init__.py` & `audiocraft-1.2.0/audiocraft/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,8 +19,8 @@
 - [MultiBandDiffusion](TODO), alternative diffusion-based decoder compatible with EnCodec that
     improves the perceived quality and reduces the artifacts coming from adversarial decoders.
 """
 
 # flake8: noqa
 from . import data, modules, models
 
-__version__ = '1.1.0'
+__version__ = '1.2.0'
```

### Comparing `audiocraft-1.1.0/audiocraft/adversarial/__init__.py` & `audiocraft-1.2.0/audiocraft/adversarial/__init__.py`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/audiocraft/adversarial/discriminators/base.py` & `audiocraft-1.2.0/audiocraft/adversarial/discriminators/base.py`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/audiocraft/adversarial/discriminators/mpd.py` & `audiocraft-1.2.0/audiocraft/adversarial/discriminators/mpd.py`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/audiocraft/adversarial/discriminators/msd.py` & `audiocraft-1.2.0/audiocraft/adversarial/discriminators/msd.py`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/audiocraft/adversarial/discriminators/msstftd.py` & `audiocraft-1.2.0/audiocraft/adversarial/discriminators/msstftd.py`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/audiocraft/adversarial/losses.py` & `audiocraft-1.2.0/audiocraft/adversarial/losses.py`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/audiocraft/data/audio.py` & `audiocraft-1.2.0/audiocraft/data/audio.py`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/audiocraft/data/audio_dataset.py` & `audiocraft-1.2.0/audiocraft/data/audio_dataset.py`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/audiocraft/data/audio_utils.py` & `audiocraft-1.2.0/audiocraft/data/audio_utils.py`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/audiocraft/data/info_audio_dataset.py` & `audiocraft-1.2.0/audiocraft/data/info_audio_dataset.py`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/audiocraft/data/music_dataset.py` & `audiocraft-1.2.0/audiocraft/data/music_dataset.py`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/audiocraft/data/sound_dataset.py` & `audiocraft-1.2.0/audiocraft/data/sound_dataset.py`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/audiocraft/data/zip.py` & `audiocraft-1.2.0/audiocraft/data/zip.py`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/audiocraft/environment.py` & `audiocraft-1.2.0/audiocraft/environment.py`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/audiocraft/grids/_base_explorers.py` & `audiocraft-1.2.0/audiocraft/grids/_base_explorers.py`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/audiocraft/grids/audiogen/audiogen_base_16khz.py` & `audiocraft-1.2.0/audiocraft/grids/audiogen/audiogen_base_16khz.py`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/audiocraft/grids/audiogen/audiogen_pretrained_16khz_eval.py` & `audiocraft-1.2.0/audiocraft/grids/audiogen/audiogen_pretrained_16khz_eval.py`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/audiocraft/grids/compression/_explorers.py` & `audiocraft-1.2.0/audiocraft/grids/compression/_explorers.py`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/audiocraft/grids/compression/debug.py` & `audiocraft-1.2.0/audiocraft/grids/compression/debug.py`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/audiocraft/grids/compression/encodec_audiogen_16khz.py` & `audiocraft-1.2.0/audiocraft/grids/compression/encodec_audiogen_16khz.py`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/audiocraft/grids/compression/encodec_base_24khz.py` & `audiocraft-1.2.0/audiocraft/grids/compression/encodec_base_24khz.py`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/audiocraft/grids/compression/encodec_musicgen_32khz.py` & `audiocraft-1.2.0/audiocraft/grids/compression/encodec_musicgen_32khz.py`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/audiocraft/grids/diffusion/4_bands_base_32khz.py` & `audiocraft-1.2.0/audiocraft/grids/diffusion/4_bands_base_32khz.py`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/audiocraft/grids/diffusion/_explorers.py` & `audiocraft-1.2.0/audiocraft/grids/diffusion/_explorers.py`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/audiocraft/grids/musicgen/_explorers.py` & `audiocraft-1.2.0/audiocraft/grids/musicgen/_explorers.py`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/audiocraft/grids/musicgen/musicgen_base_32khz.py` & `audiocraft-1.2.0/audiocraft/grids/musicgen/musicgen_base_32khz.py`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/audiocraft/grids/musicgen/musicgen_base_cached_32khz.py` & `audiocraft-1.2.0/audiocraft/grids/musicgen/musicgen_base_cached_32khz.py`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/audiocraft/grids/musicgen/musicgen_clapemb_32khz.py` & `audiocraft-1.2.0/audiocraft/grids/musicgen/musicgen_clapemb_32khz.py`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/audiocraft/grids/musicgen/musicgen_melody_32khz.py` & `audiocraft-1.2.0/audiocraft/grids/musicgen/musicgen_melody_32khz.py`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/audiocraft/grids/musicgen/musicgen_pretrained_32khz_eval.py` & `audiocraft-1.2.0/audiocraft/grids/musicgen/musicgen_pretrained_32khz_eval.py`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/audiocraft/losses/__init__.py` & `audiocraft-1.2.0/audiocraft/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/audiocraft/losses/balancer.py` & `audiocraft-1.2.0/audiocraft/losses/balancer.py`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/audiocraft/losses/sisnr.py` & `audiocraft-1.2.0/audiocraft/losses/sisnr.py`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/audiocraft/losses/specloss.py` & `audiocraft-1.2.0/audiocraft/losses/specloss.py`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/audiocraft/losses/stftloss.py` & `audiocraft-1.2.0/audiocraft/losses/stftloss.py`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/audiocraft/metrics/__init__.py` & `audiocraft-1.2.0/audiocraft/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/audiocraft/metrics/chroma_cosinesim.py` & `audiocraft-1.2.0/audiocraft/metrics/chroma_cosinesim.py`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/audiocraft/metrics/clap_consistency.py` & `audiocraft-1.2.0/audiocraft/metrics/clap_consistency.py`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/audiocraft/metrics/fad.py` & `audiocraft-1.2.0/audiocraft/metrics/fad.py`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/audiocraft/metrics/kld.py` & `audiocraft-1.2.0/audiocraft/metrics/kld.py`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/audiocraft/metrics/rvm.py` & `audiocraft-1.2.0/audiocraft/metrics/rvm.py`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/audiocraft/metrics/visqol.py` & `audiocraft-1.2.0/audiocraft/metrics/visqol.py`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/audiocraft/models/__init__.py` & `audiocraft-1.2.0/audiocraft/models/__init__.py`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/audiocraft/models/audiogen.py` & `audiocraft-1.2.0/audiocraft/models/audiogen.py`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/audiocraft/models/builders.py` & `audiocraft-1.2.0/audiocraft/models/builders.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 import typing as tp
 
 import audiocraft
 import omegaconf
 import torch
 
-from .encodec import CompressionModel, EncodecModel
+from .encodec import CompressionModel, EncodecModel, InterleaveStereoCompressionModel
 from .lm import LMModel
 from ..modules.codebooks_patterns import (
     CodebooksPatternProvider,
     DelayedPatternProvider,
     MusicLMPattern,
     ParallelPatternProvider,
     UnrolledPatternProvider,
@@ -243,9 +243,16 @@
         cross_attention=True, causal=True)
     return lm.to(device).eval()
 
 
 def get_wrapped_compression_model(
         compression_model: CompressionModel,
         cfg: omegaconf.DictConfig) -> CompressionModel:
-    # more to come.
+    if hasattr(cfg, 'interleave_stereo_codebooks'):
+        if cfg.interleave_stereo_codebooks.use:
+            kwargs = dict_from_config(cfg.interleave_stereo_codebooks)
+            kwargs.pop('use')
+            compression_model = InterleaveStereoCompressionModel(compression_model, **kwargs)
+    if hasattr(cfg, 'compression_model_n_q'):
+        if cfg.compression_model_n_q is not None:
+            compression_model.set_num_codebooks(cfg.compression_model_n_q)
     return compression_model
```

### Comparing `audiocraft-1.1.0/audiocraft/models/encodec.py` & `audiocraft-1.2.0/audiocraft/models/encodec.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,27 +9,28 @@
 
 from abc import ABC, abstractmethod
 import logging
 import math
 from pathlib import Path
 import typing as tp
 
+from einops import rearrange
 import numpy as np
 import torch
 from torch import nn
 from transformers import EncodecModel as HFEncodecModel
 
 from .. import quantization as qt
 
 
 logger = logging.getLogger()
 
 
 class CompressionModel(ABC, nn.Module):
-    """Base API for all compression model that aim at being used as audio tokenizers
+    """Base API for all compression models that aim at being used as audio tokenizers
     with a language model.
     """
 
     @abstractmethod
     def forward(self, x: torch.Tensor) -> qt.QuantizedResult:
         ...
 
@@ -107,15 +108,15 @@
             model_type = name.split('_')[1]
             logger.info("Getting pretrained compression model from DAC %s", model_type)
             model = DAC(model_type)
         elif name in ['debug_compression_model']:
             logger.info("Getting pretrained compression model for debug")
             model = builders.get_debug_compression_model()
         elif Path(name).exists():
-            # We assume here if the paths exist that it is in fact an AC checkpoint
+            # We assume here if the path exists that it is in fact an AC checkpoint
             # that was exported using `audiocraft.utils.export` functions.
             model = loaders.load_compression_model(name, device=device)
         else:
             logger.info("Getting pretrained compression model from HF %s", name)
             hf_model = HFEncodecModel.from_pretrained(name)
             model = HFEncodecCompressionModel(hf_model).to(device)
         return model.to(device).eval()
@@ -223,16 +224,16 @@
         """Encode the given input tensor to quantized representation along with scale parameter.
 
         Args:
             x (torch.Tensor): Float tensor of shape [B, C, T]
 
         Returns:
             codes, scale (tuple of torch.Tensor, torch.Tensor): Tuple composed of:
-                codes a float tensor of shape [B, K, T] with K the number of codebooks used and T the timestep.
-                scale a float tensor containing the scale for audio renormalizealization.
+                codes: a float tensor of shape [B, K, T] with K the number of codebooks used and T the timestep.
+                scale: a float tensor containing the scale for audio renormalization.
         """
         assert x.dim() == 3
         x, scale = self.preprocess(x)
         emb = self.encoder(x)
         codes = self.quantizer.encode(emb)
         return codes, scale
 
@@ -387,7 +388,119 @@
 
     def set_num_codebooks(self, n: int):
         """Set the active number of codebooks used by the quantizer.
         """
         if n not in self.possible_num_codebooks:
             raise ValueError(f"Allowed values for num codebooks: {self.possible_num_codebooks}")
         self._num_codebooks = n
+
+
+class InterleaveStereoCompressionModel(CompressionModel):
+    """Wraps a CompressionModel to support stereo inputs. The wrapped model
+    will be applied independently to the left and right channels, and both codebooks
+    will be interleaved. If the wrapped model returns a representation `[B, K ,T]` per
+    channel, then the output will be `[B, K * 2, T]`  or `[B, K, T * 2]` depending on
+    `per_timestep`.
+
+    Args:
+        model (CompressionModel): Compression model to wrap.
+        per_timestep (bool): Whether to interleave on the timestep dimension
+            or on the codebooks dimension.
+    """
+    def __init__(self, model: CompressionModel, per_timestep: bool = False):
+        super().__init__()
+        self.model = model
+        self.per_timestep = per_timestep
+        assert self.model.channels == 1, "Wrapped model is expected to be for monophonic audio"
+
+    @property
+    def total_codebooks(self):
+        return self.model.total_codebooks
+
+    @property
+    def num_codebooks(self):
+        """Active number of codebooks used by the quantizer.
+
+        ..Warning:: this reports the number of codebooks after the interleaving
+        of the codebooks!
+        """
+        return self.model.num_codebooks if self.per_timestep else self.model.num_codebooks * 2
+
+    def set_num_codebooks(self, n: int):
+        """Set the active number of codebooks used by the quantizer.
+
+        ..Warning:: this sets the number of codebooks before the interleaving!
+        """
+        self.model.set_num_codebooks(n)
+
+    @property
+    def num_virtual_steps(self) -> float:
+        """Return the number of virtual steps, e.g. one real step
+        will be split into that many steps.
+        """
+        return 2 if self.per_timestep else 1
+
+    @property
+    def frame_rate(self) -> float:
+        return self.model.frame_rate * self.num_virtual_steps
+
+    @property
+    def sample_rate(self) -> int:
+        return self.model.sample_rate
+
+    @property
+    def channels(self) -> int:
+        return 2
+
+    @property
+    def cardinality(self):
+        """Cardinality of each codebook.
+        """
+        return self.model.cardinality
+
+    def forward(self, x: torch.Tensor) -> qt.QuantizedResult:
+        raise NotImplementedError("Not supported, use encode and decode.")
+
+    def encode(self, x: torch.Tensor) -> tp.Tuple[torch.Tensor, tp.Optional[torch.Tensor]]:
+        B, C, T = x.shape
+        assert C == self.channels, f"Expecting stereo audio but audio num channels is {C}"
+
+        indices_c0, scales_c0 = self.model.encode(x[:, 0, ...].unsqueeze(1))
+        indices_c1, scales_c1 = self.model.encode(x[:, 1, ...].unsqueeze(1))
+        indices = torch.stack([indices_c0, indices_c1], dim=0)
+        scales: tp.Optional[torch.Tensor] = None
+        if scales_c0 is not None and scales_c1 is not None:
+            scales = torch.stack([scales_c0, scales_c1], dim=1)
+
+        if self.per_timestep:
+            indices = rearrange(indices, 'c b k t -> b k (t c)', c=2)
+        else:
+            indices = rearrange(indices, 'c b k t -> b (k c) t', c=2)
+
+        return (indices, scales)
+
+    def get_left_right_codes(self, codes: torch.Tensor) -> tp.Tuple[torch.Tensor, torch.Tensor]:
+        if self.per_timestep:
+            codes = rearrange(codes, 'b k (t c) -> c b k t', c=2)
+        else:
+            codes = rearrange(codes, 'b (k c) t -> c b k t', c=2)
+        return codes[0], codes[1]
+
+    def decode(self, codes: torch.Tensor, scale: tp.Optional[torch.Tensor] = None):
+        B, K, T = codes.shape
+        assert T % self.num_virtual_steps == 0, "Provided codes' number of timesteps does not match"
+        assert K == self.num_codebooks, "Provided codes' number of codebooks does not match"
+
+        scale_c0, scale_c1 = None, None
+        if scale is not None:
+            assert scale.size(0) == B and scale.size(1) == 2, f"Scale has unexpected shape: {scale.shape}"
+            scale_c0 = scale[0, ...]
+            scale_c1 = scale[1, ...]
+
+        codes_c0, codes_c1 = self.get_left_right_codes(codes)
+        audio_c0 = self.model.decode(codes_c0, scale_c0)
+        audio_c1 = self.model.decode(codes_c1, scale_c1)
+        return torch.cat([audio_c0, audio_c1], dim=1)
+
+    def decode_latent(self, codes: torch.Tensor):
+        """Decode from the discrete codes to continuous latent space."""
+        raise NotImplementedError("Not supported by interleaved stereo wrapped models.")
```

### Comparing `audiocraft-1.1.0/audiocraft/models/lm.py` & `audiocraft-1.2.0/audiocraft/models/lm.py`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/audiocraft/models/loaders.py` & `audiocraft-1.2.0/audiocraft/models/loaders.py`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/audiocraft/models/multibanddiffusion.py` & `audiocraft-1.2.0/audiocraft/models/multibanddiffusion.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,26 +26,24 @@
     """Sampling for a diffusion Model.
 
     Args:
         model (DiffusionUnet): Diffusion U-Net model.
         noise_schedule (NoiseSchedule): Noise schedule for diffusion process.
     """
     def __init__(self, model: DiffusionUnet, noise_schedule: NoiseSchedule) -> None:
-        """
-        """
         self.model = model
         self.schedule = noise_schedule
 
     def generate(self, condition: torch.Tensor, initial_noise: torch.Tensor,
                  step_list: tp.Optional[tp.List[int]] = None):
         """Perform one diffusion process to generate one of the bands.
 
         Args:
-            condition (tensor): The embeddings form the compression model.
-            initial_noise (tensor): The initial noise to start the process/
+            condition (torch.Tensor): The embeddings from the compression model.
+            initial_noise (torch.Tensor): The initial noise to start the process.
         """
         return self.schedule.generate_subsampled(model=self.model, initial=initial_noise, step_list=step_list,
                                                  condition=condition)
 
 
 class MultiBandDiffusion:
     """Sample from multiple diffusion models.
@@ -76,22 +74,21 @@
         DPs = []
         for i in range(len(models)):
             schedule = NoiseSchedule(**cfgs[i].schedule, sample_processor=processors[i], device=device)
             DPs.append(DiffusionProcess(model=models[i], noise_schedule=schedule))
         return MultiBandDiffusion(DPs=DPs, codec_model=codec_model)
 
     @staticmethod
-    def get_mbd_24khz(bw: float = 3.0, pretrained: bool = True,
+    def get_mbd_24khz(bw: float = 3.0,
                       device: tp.Optional[tp.Union[torch.device, str]] = None,
                       n_q: tp.Optional[int] = None):
         """Get the pretrained Models for MultibandDiffusion.
 
         Args:
             bw (float): Bandwidth of the compression model.
-            pretrained (bool): Whether to use / download if necessary the models.
             device (torch.device or str, optional): Device on which the models are loaded.
             n_q (int, optional): Number of quantizers to use within the compression model.
         """
         if device is None:
             device = 'cuda' if torch.cuda.is_available() else 'cpu'
         assert bw in [1.5, 3.0, 6.0], f"bandwidth {bw} not available"
         if n_q is not None:
@@ -108,89 +105,87 @@
         models, processors, cfgs = load_diffusion_models(path, filename=filename, device=device)
         DPs = []
         for i in range(len(models)):
             schedule = NoiseSchedule(**cfgs[i].schedule, sample_processor=processors[i], device=device)
             DPs.append(DiffusionProcess(model=models[i], noise_schedule=schedule))
         return MultiBandDiffusion(DPs=DPs, codec_model=codec_model)
 
-        return MultiBandDiffusion(DPs, codec_model)
-
     @torch.no_grad()
     def get_condition(self, wav: torch.Tensor, sample_rate: int) -> torch.Tensor:
-        """Get the conditioning (i.e. latent reprentatios of the compression model) from a waveform.
+        """Get the conditioning (i.e. latent representations of the compression model) from a waveform.
         Args:
-            wav (torch.Tensor): The audio that we want to extract the conditioning from
-            sample_rate (int): sample rate of the audio"""
+            wav (torch.Tensor): The audio that we want to extract the conditioning from.
+            sample_rate (int): Sample rate of the audio."""
         if sample_rate != self.sample_rate:
             wav = julius.resample_frac(wav, sample_rate, self.sample_rate)
         codes, scale = self.codec_model.encode(wav)
         assert scale is None, "Scaled compression models not supported."
         emb = self.get_emb(codes)
         return emb
 
     @torch.no_grad()
     def get_emb(self, codes: torch.Tensor):
-        """Get latent representation from the discrete codes
-        Argrs:
-            codes (torch.Tensor): discrete tokens"""
+        """Get latent representation from the discrete codes.
+        Args:
+            codes (torch.Tensor): Discrete tokens."""
         emb = self.codec_model.decode_latent(codes)
         return emb
 
     def generate(self, emb: torch.Tensor, size: tp.Optional[torch.Size] = None,
                  step_list: tp.Optional[tp.List[int]] = None):
-        """Generate Wavform audio from the latent embeddings of the compression model
+        """Generate waveform audio from the latent embeddings of the compression model.
         Args:
-            emb (torch.Tensor): Conditioning embeddinds
-            size (none torch.Size): size of the output
-                if None this is computed from the typical upsampling of the model
-            step_list (optional list[int]): list of Markov chain steps, defaults to 50 linearly spaced step.
+            emb (torch.Tensor): Conditioning embeddings
+            size (None, torch.Size): Size of the output
+                if None this is computed from the typical upsampling of the model.
+            step_list (list[int], optional): list of Markov chain steps, defaults to 50 linearly spaced step.
         """
         if size is None:
             upsampling = int(self.codec_model.sample_rate / self.codec_model.frame_rate)
             size = torch.Size([emb.size(0), self.codec_model.channels, emb.size(-1) * upsampling])
         assert size[0] == emb.size(0)
         out = torch.zeros(size).to(self.device)
         for DP in self.DPs:
             out += DP.generate(condition=emb, step_list=step_list, initial_noise=torch.randn_like(out))
         return out
 
     def re_eq(self, wav: torch.Tensor, ref: torch.Tensor, n_bands: int = 32, strictness: float = 1):
-        """match the eq to the encodec output by matching the standard deviation of some frequency bands
+        """Match the eq to the encodec output by matching the standard deviation of some frequency bands.
         Args:
-            wav (torch.Tensor): audio to equalize
-            ref (torch.Tensor):refenrence audio from which we match the spectrogram.
-            n_bands (int): number of bands of the eq
-            strictness (float): how strict the the matching. 0 is no matching, 1 is exact matching.
+            wav (torch.Tensor): Audio to equalize.
+            ref (torch.Tensor): Reference audio from which we match the spectrogram.
+            n_bands (int): Number of bands of the eq.
+            strictness (float): How strict the matching. 0 is no matching, 1 is exact matching.
         """
         split = julius.SplitBands(n_bands=n_bands, sample_rate=self.codec_model.sample_rate).to(wav.device)
         bands = split(wav)
         bands_ref = split(ref)
         out = torch.zeros_like(ref)
         for i in range(n_bands):
             out += bands[i] * (bands_ref[i].std() / bands[i].std()) ** strictness
         return out
 
     def regenerate(self, wav: torch.Tensor, sample_rate: int):
-        """Regenerate a wavform through compression and diffusion regeneration.
+        """Regenerate a waveform through compression and diffusion regeneration.
         Args:
-            wav (torch.Tensor): Original 'ground truth' audio
-            sample_rate (int): sample rate of the input (and output) wav
+            wav (torch.Tensor): Original 'ground truth' audio.
+            sample_rate (int): Sample rate of the input (and output) wav.
         """
         if sample_rate != self.codec_model.sample_rate:
             wav = julius.resample_frac(wav, sample_rate, self.codec_model.sample_rate)
         emb = self.get_condition(wav, sample_rate=self.codec_model.sample_rate)
         size = wav.size()
         out = self.generate(emb, size=size)
         if sample_rate != self.codec_model.sample_rate:
             out = julius.resample_frac(out, self.codec_model.sample_rate, sample_rate)
         return out
 
     def tokens_to_wav(self, tokens: torch.Tensor, n_bands: int = 32):
         """Generate Waveform audio with diffusion from the discrete codes.
         Args:
-            tokens (torch.Tensor): discrete codes
-            n_bands (int): bands for the eq matching.
+            tokens (torch.Tensor): Discrete codes.
+            n_bands (int): Bands for the eq matching.
         """
         wav_encodec = self.codec_model.decode(tokens)
         condition = self.get_emb(tokens)
         wav_diffusion = self.generate(emb=condition, size=wav_encodec.size())
         return self.re_eq(wav=wav_diffusion, ref=wav_encodec, n_bands=n_bands)
```

### Comparing `audiocraft-1.1.0/audiocraft/models/musicgen.py` & `audiocraft-1.2.0/audiocraft/models/musicgen.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,19 +8,20 @@
 Main model for using MusicGen. This will combine all the required components
 and provide easy access to the generation API.
 """
 
 import typing as tp
 import warnings
 
+import omegaconf
 import torch
 
 from .encodec import CompressionModel
 from .lm import LMModel
-from .builders import get_debug_compression_model, get_debug_lm_model
+from .builders import get_debug_compression_model, get_debug_lm_model, get_wrapped_compression_model
 from .loaders import load_compression_model, load_lm_model
 from ..data.audio_utils import convert_audio
 from ..modules.conditioners import ConditioningAttributes, WavCondition
 from ..utils.autocast import TorchAutocast
 
 
 MelodyList = tp.List[tp.Optional[torch.Tensor]]
@@ -48,26 +49,36 @@
             otherwise, inferred from the training params.
     """
     def __init__(self, name: str, compression_model: CompressionModel, lm: LMModel,
                  max_duration: tp.Optional[float] = None):
         self.name = name
         self.compression_model = compression_model
         self.lm = lm
+        self.cfg: tp.Optional[omegaconf.DictConfig] = None
         # Just to be safe, let's put everything in eval mode.
         self.compression_model.eval()
         self.lm.eval()
 
+        if hasattr(lm, 'cfg'):
+            cfg = lm.cfg
+            assert isinstance(cfg, omegaconf.DictConfig)
+            self.cfg = cfg
+
+        if self.cfg is not None:
+            self.compression_model = get_wrapped_compression_model(self.compression_model, self.cfg)
+
         if max_duration is None:
-            if hasattr(lm, 'cfg'):
+            if self.cfg is not None:
                 max_duration = lm.cfg.dataset.segment_duration  # type: ignore
             else:
                 raise ValueError("You must provide max_duration when building directly MusicGen")
         assert max_duration is not None
         self.max_duration: float = max_duration
         self.device = next(iter(lm.parameters())).device
+
         self.generation_params: dict = {}
         self.set_generation_params(duration=15)  # 15 seconds by default
         self._progress_callback: tp.Optional[tp.Callable[[int, int], None]] = None
         if self.device.type == 'cpu':
             self.autocast = TorchAutocast(enabled=False)
         else:
             self.autocast = TorchAutocast(
@@ -118,14 +129,15 @@
                 f"Please use full pre-trained id instead: facebook/musicgen-{name}")
             name = _HF_MODEL_CHECKPOINTS_MAP[name]
 
         lm = load_lm_model(name, device=device)
         compression_model = load_compression_model(name, device=device)
         if 'self_wav' in lm.condition_provider.conditioners:
             lm.condition_provider.conditioners['self_wav'].match_len_on_eval = True
+            lm.condition_provider.conditioners['self_wav']._use_masking = False
 
         return MusicGen(name, compression_model, lm)
 
     def set_generation_params(self, use_sampling: bool = True, top_k: int = 250,
                               top_p: float = 0.0, temperature: float = 1.0,
                               duration: float = 30.0, cfg_coef: float = 3.0,
                               two_step_cfg: bool = False, extend_stride: float = 18):
```

### Comparing `audiocraft-1.1.0/audiocraft/models/unet.py` & `audiocraft-1.2.0/audiocraft/models/unet.py`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/audiocraft/modules/__init__.py` & `audiocraft-1.2.0/audiocraft/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/audiocraft/modules/activations.py` & `audiocraft-1.2.0/audiocraft/modules/activations.py`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/audiocraft/modules/chroma.py` & `audiocraft-1.2.0/audiocraft/modules/chroma.py`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/audiocraft/modules/codebooks_patterns.py` & `audiocraft-1.2.0/audiocraft/modules/codebooks_patterns.py`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/audiocraft/modules/conditioners.py` & `audiocraft-1.2.0/audiocraft/modules/conditioners.py`

 * *Files 1% similar despite different names*

```diff
@@ -465,14 +465,16 @@
         dim (int): The internal representation dimension.
         output_dim (int): Output dimension.
         device (tp.Union[torch.device, str]): Device.
     """
     def __init__(self, dim: int, output_dim: int, device: tp.Union[torch.device, str]):
         super().__init__(dim, output_dim)
         self.device = device
+        # if False no masking is done, used in ChromaStemConditioner when completing by periodicity a sample.
+        self._use_masking = True
 
     def tokenize(self, x: WavCondition) -> WavCondition:
         wav, length, sample_rate, path, seek_time = x
         assert length is not None
         return WavCondition(wav.to(self.device), length.to(self.device), sample_rate, path, seek_time)
 
     def _get_wav_embedding(self, x: WavCondition) -> torch.Tensor:
@@ -492,21 +494,20 @@
         """
         wav, lengths, *_ = x
         with torch.no_grad():
             embeds = self._get_wav_embedding(x)
         embeds = embeds.to(self.output_proj.weight)
         embeds = self.output_proj(embeds)
 
-        if lengths is not None:
+        if lengths is not None and self._use_masking:
             lengths = lengths / self._downsampling_factor()
             mask = length_to_mask(lengths, max_len=embeds.shape[1]).int()  # type: ignore
         else:
-            mask = torch.ones_like(embeds)
-        embeds = (embeds * mask.unsqueeze(2).to(self.device))
-
+            mask = torch.ones_like(embeds[..., 0])
+        embeds = (embeds * mask.unsqueeze(-1))
         return embeds, mask
 
 
 class ChromaStemConditioner(WaveformConditioner):
     """Chroma conditioner based on stems.
     The ChromaStemConditioner uses DEMUCS to first filter out drums and bass, as
     the drums and bass often dominate the chroma leading to the chroma features
@@ -533,14 +534,16 @@
                  n_eval_wavs: int = 0, cache_path: tp.Optional[tp.Union[str, Path]] = None,
                  device: tp.Union[torch.device, str] = 'cpu', **kwargs):
         from demucs import pretrained
         super().__init__(dim=n_chroma, output_dim=output_dim, device=device)
         self.autocast = TorchAutocast(enabled=device != 'cpu', device_type=self.device, dtype=torch.float32)
         self.sample_rate = sample_rate
         self.match_len_on_eval = match_len_on_eval
+        if match_len_on_eval:
+            self._use_masking = False
         self.duration = duration
         self.__dict__['demucs'] = pretrained.get_model('htdemucs').to(device)
         stem_sources: list = self.demucs.sources  # type: ignore
         self.stem_indices = torch.LongTensor([stem_sources.index('vocals'), stem_sources.index('other')]).to(device)
         self.chroma = ChromaExtractor(sample_rate=sample_rate, n_chroma=n_chroma,
                                       radix2_exp=radix2_exp, **kwargs).to(device)
         self.chroma_len = self._get_chroma_len()
```

### Comparing `audiocraft-1.1.0/audiocraft/modules/conv.py` & `audiocraft-1.2.0/audiocraft/modules/conv.py`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/audiocraft/modules/diffusion_schedule.py` & `audiocraft-1.2.0/audiocraft/modules/diffusion_schedule.py`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/audiocraft/modules/lstm.py` & `audiocraft-1.2.0/audiocraft/modules/lstm.py`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/audiocraft/modules/rope.py` & `audiocraft-1.2.0/audiocraft/modules/rope.py`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/audiocraft/modules/seanet.py` & `audiocraft-1.2.0/audiocraft/modules/seanet.py`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/audiocraft/modules/streaming.py` & `audiocraft-1.2.0/audiocraft/modules/streaming.py`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/audiocraft/modules/transformer.py` & `audiocraft-1.2.0/audiocraft/modules/transformer.py`

 * *Files 1% similar despite different names*

```diff
@@ -644,15 +644,14 @@
                     device=device, dtype=dtype, **kwargs))
 
         if self.checkpointing != 'none':
             for layer in self.layers:
                 # see audiocraft/optim/fsdp.py, magic signal to indicate this requires fixing the
                 # backward hook inside of FSDP...
                 layer._magma_checkpointed = True  # type: ignore
-                assert layer.layer_drop == 0., "Need further checking"  # type: ignore
 
     def _apply_layer(self, layer, *args, **kwargs):
         method = self.checkpointing
         if method == 'none':
             return layer(*args, **kwargs)
         elif method == 'torch':
             return torch_checkpoint(layer, *args, use_reentrant=False, **kwargs)
```

### Comparing `audiocraft-1.1.0/audiocraft/optim/__init__.py` & `audiocraft-1.2.0/audiocraft/optim/__init__.py`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/audiocraft/optim/cosine_lr_scheduler.py` & `audiocraft-1.2.0/audiocraft/optim/cosine_lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/audiocraft/optim/dadam.py` & `audiocraft-1.2.0/audiocraft/optim/dadam.py`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/audiocraft/optim/ema.py` & `audiocraft-1.2.0/audiocraft/optim/ema.py`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/audiocraft/optim/fsdp.py` & `audiocraft-1.2.0/audiocraft/optim/fsdp.py`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/audiocraft/optim/inverse_sqrt_lr_scheduler.py` & `audiocraft-1.2.0/audiocraft/optim/inverse_sqrt_lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/audiocraft/optim/linear_warmup_lr_scheduler.py` & `audiocraft-1.2.0/audiocraft/optim/linear_warmup_lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/audiocraft/optim/polynomial_decay_lr_scheduler.py` & `audiocraft-1.2.0/audiocraft/optim/polynomial_decay_lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/audiocraft/quantization/base.py` & `audiocraft-1.2.0/audiocraft/quantization/base.py`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/audiocraft/quantization/core_vq.py` & `audiocraft-1.2.0/audiocraft/quantization/core_vq.py`

 * *Files 5% similar despite different names*

```diff
@@ -367,19 +367,24 @@
         all_losses = []
         all_indices = []
 
         n_q = n_q or len(self.layers)
 
         for i, layer in enumerate(self.layers[:n_q]):
             quantized, indices, loss = layer(residual)
+            quantized = quantized.detach()
             residual = residual - quantized
             quantized_out = quantized_out + quantized
             all_indices.append(indices)
             all_losses.append(loss)
 
+        if self.training:
+            # Solving subtle bug with STE and RVQ: https://github.com/facebookresearch/encodec/issues/25
+            quantized_out = x + (quantized_out - x).detach()
+
         out_losses, out_indices = map(torch.stack, (all_losses, all_indices))
         return quantized_out, out_indices, out_losses
 
     def encode(self, x: torch.Tensor, n_q: tp.Optional[int] = None) -> torch.Tensor:
         residual = x
         all_indices = []
         n_q = n_q or len(self.layers)
```

### Comparing `audiocraft-1.1.0/audiocraft/quantization/vq.py` & `audiocraft-1.2.0/audiocraft/quantization/vq.py`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/audiocraft/solvers/__init__.py` & `audiocraft-1.2.0/audiocraft/solvers/__init__.py`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/audiocraft/solvers/audiogen.py` & `audiocraft-1.2.0/audiocraft/solvers/audiogen.py`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/audiocraft/solvers/base.py` & `audiocraft-1.2.0/audiocraft/solvers/base.py`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/audiocraft/solvers/builders.py` & `audiocraft-1.2.0/audiocraft/solvers/builders.py`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/audiocraft/solvers/compression.py` & `audiocraft-1.2.0/audiocraft/solvers/compression.py`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/audiocraft/solvers/diffusion.py` & `audiocraft-1.2.0/audiocraft/solvers/diffusion.py`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/audiocraft/solvers/musicgen.py` & `audiocraft-1.2.0/audiocraft/solvers/musicgen.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from .. import models
 from ..data.audio_dataset import AudioDataset
 from ..data.music_dataset import MusicDataset, MusicInfo, AudioInfo
 from ..data.audio_utils import normalize_audio
 from ..modules.conditioners import JointEmbedCondition, SegmentWithAttributes, WavCondition
 from ..utils.cache import CachedBatchWriter, CachedBatchLoader
 from ..utils.samples.manager import SampleManager
-from ..utils.utils import get_dataset_from_loader, is_jsonable, warn_once
+from ..utils.utils import get_dataset_from_loader, is_jsonable, warn_once, model_hash
 
 
 class MusicGenSolver(base.StandardSolver):
     """Solver for MusicGen training task.
 
     Used in: https://arxiv.org/abs/2306.05284
     """
@@ -139,15 +139,15 @@
         if self.cfg.fsdp.use:
             assert not self.cfg.autocast, "Cannot use autocast with fsdp"
             self.model = self.wrap_with_fsdp(self.model)
         self.register_ema('model')
         # initialize optimization
         self.optimizer = builders.get_optimizer(builders.get_optim_parameter_groups(self.model), self.cfg.optim)
         self.lr_scheduler = builders.get_lr_scheduler(self.optimizer, self.cfg.schedule, self.total_updates)
-        self.register_stateful('compression_model', 'model', 'optimizer', 'lr_scheduler')
+        self.register_stateful('model', 'optimizer', 'lr_scheduler')
         self.register_best_state('model')
         self.autocast_dtype = {
             'float16': torch.float16, 'bfloat16': torch.bfloat16
         }[self.cfg.autocast_dtype]
         self.scaler: tp.Optional[torch.cuda.amp.GradScaler] = None
         if self.cfg.fsdp.use:
             need_scaler = self.cfg.fsdp.param_dtype == 'float16'
@@ -177,14 +177,30 @@
             model_state = state['model']
             condition_provider_state = state.pop('condition_provider')
             prefix = 'condition_provider.'
             for key, value in condition_provider_state.items():
                 key = prefix + key
                 assert key not in model_state
                 model_state[key] = value
+        if 'compression_model' in state:
+            # We used to store the `compression_model` state in the checkpoint, however
+            # this is in general not needed, as the compression model should always be readable
+            # from the original `cfg.compression_model_checkpoint` location.
+            compression_model_state = state.pop('compression_model')
+            before_hash = model_hash(self.compression_model)
+            self.compression_model.load_state_dict(compression_model_state)
+            after_hash = model_hash(self.compression_model)
+            if before_hash != after_hash:
+                raise RuntimeError(
+                    "The compression model state inside the checkpoint is different"
+                    " from the one obtained from compression_model_checkpoint..."
+                    "We do not support altering the compression model inside the LM "
+                    "checkpoint as parts of the code, in particular for running eval post-training "
+                    "will use the compression_model_checkpoint as the source of truth.")
+
         super().load_state_dict(state)
 
     def load_from_pretrained(self, name: str):
         # TODO: support native HF versions of MusicGen.
         lm_pkg = models.loaders.load_lm_model_ckpt(name)
         state: dict = {
             'best_state': {
```

### Comparing `audiocraft-1.1.0/audiocraft/train.py` & `audiocraft-1.2.0/audiocraft/train.py`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/audiocraft/utils/autocast.py` & `audiocraft-1.2.0/audiocraft/utils/autocast.py`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/audiocraft/utils/best_state.py` & `audiocraft-1.2.0/audiocraft/utils/best_state.py`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/audiocraft/utils/cache.py` & `audiocraft-1.2.0/audiocraft/utils/cache.py`

 * *Files 0% similar despite different names*

```diff
@@ -283,14 +283,15 @@
                 transposed = zip(*entries)
                 out = []
                 for part in transposed:
                     assert len(part) > 0
                     if isinstance(part[0], torch.Tensor):
                         out.append(torch.stack(part))
                     else:
+                        assert isinstance(part, torch.Tensor)
                         out.append(part)
                 return out
         except Exception:
             logger.error("Error when reading zip path %s", zip_path)
             raise
 
     def __iter__(self):
```

### Comparing `audiocraft-1.1.0/audiocraft/utils/checkpoint.py` & `audiocraft-1.2.0/audiocraft/utils/checkpoint.py`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/audiocraft/utils/cluster.py` & `audiocraft-1.2.0/audiocraft/utils/cluster.py`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/audiocraft/utils/deadlock.py` & `audiocraft-1.2.0/audiocraft/utils/deadlock.py`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/audiocraft/utils/export.py` & `audiocraft-1.2.0/audiocraft/utils/export.py`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/audiocraft/utils/export_legacy.py` & `audiocraft-1.2.0/audiocraft/utils/export_legacy.py`

 * *Files 24% similar despite different names*

```diff
@@ -10,47 +10,61 @@
 
 from pathlib import Path
 import typing as tp
 
 from omegaconf import OmegaConf, DictConfig
 import torch
 
+from audiocraft import __version__
+
 
 def _clean_lm_cfg(cfg: DictConfig):
     OmegaConf.set_struct(cfg, False)
     # This used to be set automatically in the LM solver, need a more robust solution
     # for the future.
     cfg['transformer_lm']['card'] = 2048
-    cfg['transformer_lm']['n_q'] = 4
+    n_q = 4
+    stereo_cfg = getattr(cfg, 'interleave_stereo_codebooks', None)
+    if stereo_cfg is not None and stereo_cfg.use:
+        if 'downsample' in stereo_cfg:
+            del stereo_cfg['downsample']
+        n_q = 8
+    cfg['transformer_lm']['n_q'] = n_q
     # Experimental params no longer supported.
     bad_params = ['spectral_norm_attn_iters', 'spectral_norm_ff_iters',
                   'residual_balancer_attn', 'residual_balancer_ff', 'layer_drop']
     for name in bad_params:
         del cfg['transformer_lm'][name]
     OmegaConf.set_struct(cfg, True)
     return cfg
 
 
-def export_encodec(checkpoint_path: tp.Union[Path, str], out_folder: tp.Union[Path, str]):
-    sig = Path(checkpoint_path).parent.name
-    assert len(sig) == 8, "Not a valid Dora signature"
+def export_encodec(checkpoint_path: tp.Union[Path, str], out_file: tp.Union[Path, str]):
     pkg = torch.load(checkpoint_path, 'cpu')
     new_pkg = {
         'best_state': pkg['ema']['state']['model'],
         'xp.cfg': OmegaConf.to_yaml(pkg['xp.cfg']),
+        # The following params were NOT exported for the first release of MusicGen.
+        'version': __version__,
+        'exported': True,
     }
-    out_file = Path(out_folder) / f'{sig}.th'
+    Path(out_file).parent.mkdir(exist_ok=True, parents=True)
     torch.save(new_pkg, out_file)
     return out_file
 
 
-def export_lm(checkpoint_path: tp.Union[Path, str], out_folder: tp.Union[Path, str]):
-    sig = Path(checkpoint_path).parent.name
-    assert len(sig) == 8, "Not a valid Dora signature"
+def export_lm(checkpoint_path: tp.Union[Path, str], out_file: tp.Union[Path, str]):
     pkg = torch.load(checkpoint_path, 'cpu')
+    if pkg['fsdp_best_state']:
+        best_state = pkg['fsdp_best_state']['model']
+    else:
+        best_state = pkg['best_state']['model']
     new_pkg = {
-        'best_state': pkg['fsdp_best_state']['model'],
-        'xp.cfg': OmegaConf.to_yaml(_clean_lm_cfg(pkg['xp.cfg']))
+        'best_state': best_state,
+        'xp.cfg': OmegaConf.to_yaml(_clean_lm_cfg(pkg['xp.cfg'])),
+        # The following params were NOT exported for the first release of MusicGen.
+        'version': __version__,
+        'exported': True,
     }
-    out_file = Path(out_folder) / f'{sig}.th'
+    Path(out_file).parent.mkdir(exist_ok=True, parents=True)
     torch.save(new_pkg, out_file)
     return out_file
```

### Comparing `audiocraft-1.1.0/audiocraft/utils/notebook.py` & `audiocraft-1.2.0/audiocraft/utils/notebook.py`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/audiocraft/utils/profiler.py` & `audiocraft-1.2.0/audiocraft/utils/profiler.py`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/audiocraft/utils/samples/manager.py` & `audiocraft-1.2.0/audiocraft/utils/samples/manager.py`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/audiocraft/utils/utils.py` & `audiocraft-1.2.0/audiocraft/utils/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -181,15 +181,15 @@
         max_len (int): can set the max length manually. Defaults to None.
     Returns:
         torch.Tensor: mask with 0s where there is pad tokens else 1s
     """
     assert len(lengths.shape) == 1, "Length shape should be 1 dimensional."
     final_length = lengths.max().item() if not max_len else max_len
     final_length = max(final_length, 1)  # if all seqs are of len zero we don't want a zero-size tensor
-    return torch.arange(final_length)[None, :].to(lengths.device) < lengths[:, None]
+    return torch.arange(final_length, device=lengths.device)[None, :] < lengths[:, None]
 
 
 def hash_trick(word: str, vocab_size: int) -> int:
     """Hash trick to pair each word with an index
 
     Args:
         word (str): word we wish to convert to an index
```

### Comparing `audiocraft-1.1.0/audiocraft.egg-info/SOURCES.txt` & `audiocraft-1.2.0/audiocraft.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -55,14 +55,15 @@
 audiocraft/grids/musicgen/__init__.py
 audiocraft/grids/musicgen/_explorers.py
 audiocraft/grids/musicgen/musicgen_base_32khz.py
 audiocraft/grids/musicgen/musicgen_base_cached_32khz.py
 audiocraft/grids/musicgen/musicgen_clapemb_32khz.py
 audiocraft/grids/musicgen/musicgen_melody_32khz.py
 audiocraft/grids/musicgen/musicgen_pretrained_32khz_eval.py
+audiocraft/grids/musicgen/musicgen_stereo_finetune_32khz.py
 audiocraft/losses/__init__.py
 audiocraft/losses/balancer.py
 audiocraft/losses/sisnr.py
 audiocraft/losses/specloss.py
 audiocraft/losses/stftloss.py
 audiocraft/metrics/__init__.py
 audiocraft/metrics/chroma_cosinesim.py
```

### Comparing `audiocraft-1.1.0/config/conditioner/chroma2music.yaml` & `audiocraft-1.2.0/config/conditioner/chroma2music.yaml`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/config/conditioner/clapemb2music.yaml` & `audiocraft-1.2.0/config/conditioner/clapemb2music.yaml`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/config/config.yaml` & `audiocraft-1.2.0/config/config.yaml`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/config/model/encodec/default.yaml` & `audiocraft-1.2.0/config/model/encodec/default.yaml`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/config/model/lm/audiogen_lm.yaml` & `audiocraft-1.2.0/config/model/lm/audiogen_lm.yaml`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/config/model/lm/default.yaml` & `audiocraft-1.2.0/config/model/lm/default.yaml`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/config/model/lm/musicgen_lm.yaml` & `audiocraft-1.2.0/config/model/lm/musicgen_lm.yaml`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/config/solver/audiogen/audiogen_base_16khz.yaml` & `audiocraft-1.2.0/config/solver/audiogen/audiogen_base_16khz.yaml`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/config/solver/audiogen/debug.yaml` & `audiocraft-1.2.0/config/solver/audiogen/debug.yaml`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/config/solver/audiogen/default.yaml` & `audiocraft-1.2.0/config/solver/audiogen/default.yaml`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/config/solver/audiogen/evaluation/objective_eval.yaml` & `audiocraft-1.2.0/config/solver/audiogen/evaluation/objective_eval.yaml`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/config/solver/compression/debug.yaml` & `audiocraft-1.2.0/config/solver/compression/debug.yaml`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/config/solver/compression/default.yaml` & `audiocraft-1.2.0/config/solver/compression/default.yaml`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/config/solver/default.yaml` & `audiocraft-1.2.0/config/solver/default.yaml`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/config/solver/diffusion/debug.yaml` & `audiocraft-1.2.0/config/solver/diffusion/debug.yaml`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/config/solver/diffusion/default.yaml` & `audiocraft-1.2.0/config/solver/diffusion/default.yaml`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/config/solver/musicgen/debug.yaml` & `audiocraft-1.2.0/config/solver/musicgen/debug.yaml`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/config/solver/musicgen/default.yaml` & `audiocraft-1.2.0/config/solver/musicgen/default.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -10,18 +10,28 @@
 autocast: true
 autocast_dtype: float16
 
 solver: musicgen
 sample_rate: ???
 channels: ???
 compression_model_checkpoint: ???
+# The following will set the num codebooks on the underlying
+# model, this might be different from the actual value for n_q
+# given to the transformer, when the model output is postprocessed, for instance
+# for stereo channels. If not provided, default value for the compression model
+# will be used.
+compression_model_n_q: null
 
 tokens:
   padding_with_special_token: false
 
+interleave_stereo_codebooks:
+  use: false
+  per_timestep: false
+
 cache:
   path:
   write: false
   write_shard: 0
   write_num_shards: 1
```

### Comparing `audiocraft-1.1.0/config/solver/musicgen/evaluation/objective_eval.yaml` & `audiocraft-1.2.0/config/solver/musicgen/evaluation/objective_eval.yaml`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/config/solver/musicgen/musicgen_base_32khz.yaml` & `audiocraft-1.2.0/config/solver/musicgen/musicgen_base_32khz.yaml`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/config/solver/musicgen/musicgen_melody_32khz.yaml` & `audiocraft-1.2.0/config/solver/musicgen/musicgen_melody_32khz.yaml`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/config/teams/labs.yaml` & `audiocraft-1.2.0/config/teams/labs.yaml`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/demos/audiogen_demo.ipynb` & `audiocraft-1.2.0/demos/audiogen_demo.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998611111111111%*

 * *Differences: {"'cells'": "{6: {'source': {insert: [(10, '    wav = torch.cos(2 * math.pi * frequency * "*

 * *            "t)[None]\\n')], delete: [10]}}}"}*

```diff
@@ -79,15 +79,15 @@
                 "from audiocraft.utils.notebook import display_audio\n",
                 "\n",
                 "def get_bip_bip(bip_duration=0.125, frequency=440,\n",
                 "                duration=0.5, sample_rate=16000, device=\"cuda\"):\n",
                 "    \"\"\"Generates a series of bip bip at the given frequency.\"\"\"\n",
                 "    t = torch.arange(\n",
                 "        int(duration * sample_rate), device=\"cuda\", dtype=torch.float) / sample_rate\n",
-                "    wav = torch.cos(2 * math.pi * 440 * t)[None]\n",
+                "    wav = torch.cos(2 * math.pi * frequency * t)[None]\n",
                 "    tp = (t % (2 * bip_duration)) / (2 * bip_duration)\n",
                 "    envelope = (tp >= 0.5).float()\n",
                 "    return wav * envelope"
             ]
         },
         {
             "cell_type": "code",
```

### Comparing `audiocraft-1.1.0/demos/musicgen_app.py` & `audiocraft-1.2.0/demos/musicgen_app.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,32 +5,37 @@
 # LICENSE file in the root directory of this source tree.
 
 # Updated to account for UI changes from https://github.com/rkfg/audiocraft/blob/long/app.py
 # also released under the MIT license.
 
 import argparse
 from concurrent.futures import ProcessPoolExecutor
+import logging
 import os
 from pathlib import Path
 import subprocess as sp
+import sys
 from tempfile import NamedTemporaryFile
 import time
 import typing as tp
 import warnings
 
+from einops import rearrange
 import torch
 import gradio as gr
 
 from audiocraft.data.audio_utils import convert_audio
 from audiocraft.data.audio import audio_write
+from audiocraft.models.encodec import InterleaveStereoCompressionModel
 from audiocraft.models import MusicGen, MultiBandDiffusion
 
 
 MODEL = None  # Last used model
-IS_BATCHED = "facebook/MusicGen" in os.environ.get('SPACE_ID', '')
+SPACE_ID = os.environ.get('SPACE_ID', '')
+IS_BATCHED = "facebook/MusicGen" in SPACE_ID or 'musicgen-internal/musicgen_dev' in SPACE_ID
 print(IS_BATCHED)
 MAX_BATCH_SIZE = 12
 BATCHED_DURATION = 15
 INTERRUPTING = False
 MBD = None
 # We have to wrap subprocess call to clean a bit the log when using gr.make_waveform
 _old_call = sp.call
@@ -68,16 +73,15 @@
         for time_added, path in list(self.files):
             if now - time_added > self.file_lifetime:
                 if path.exists():
                     path.unlink()
                 self.files.pop(0)
             else:
                 break
-
-
+                
 file_cleaner = FileCleaner()
 
 
 def make_waveform(*args, **kwargs):
     # Further remove some warnings.
     be = time.time()
     with warnings.catch_warnings():
@@ -87,25 +91,29 @@
         return out
 
 
 def load_model(version='facebook/musicgen-melody'):
     global MODEL
     print("Loading model", version)
     if MODEL is None or MODEL.name != version:
+        # Clear PyTorch CUDA cache and delete model
+        del MODEL
+        torch.cuda.empty_cache()
+        MODEL = None  # in case loading would crash
         MODEL = MusicGen.get_pretrained(version)
 
 
 def load_diffusion():
     global MBD
     if MBD is None:
         print("loading MBD")
         MBD = MultiBandDiffusion.get_mbd_musicgen()
 
 
-def _do_predictions(texts, melodies, duration, progress=False, **gen_kwargs):
+def _do_predictions(texts, melodies, duration, progress=False, gradio_progress=None, **gen_kwargs):
     MODEL.set_generation_params(duration=duration, **gen_kwargs)
     print("new batch", len(texts), texts, [None if m is None else (m[0], m[1].shape) for m in melodies])
     be = time.time()
     processed_melodies = []
     target_sr = 32000
     target_ac = 1
     for melody in melodies:
@@ -115,26 +123,38 @@
             sr, melody = melody[0], torch.from_numpy(melody[1]).to(MODEL.device).float().t()
             if melody.dim() == 1:
                 melody = melody[None]
             melody = melody[..., :int(sr * duration)]
             melody = convert_audio(melody, sr, target_sr, target_ac)
             processed_melodies.append(melody)
 
-    if any(m is not None for m in processed_melodies):
-        outputs = MODEL.generate_with_chroma(
-            descriptions=texts,
-            melody_wavs=processed_melodies,
-            melody_sample_rate=target_sr,
-            progress=progress,
-            return_tokens=USE_DIFFUSION
-        )
-    else:
-        outputs = MODEL.generate(texts, progress=progress, return_tokens=USE_DIFFUSION)
+    try:
+        if any(m is not None for m in processed_melodies):
+            outputs = MODEL.generate_with_chroma(
+                descriptions=texts,
+                melody_wavs=processed_melodies,
+                melody_sample_rate=target_sr,
+                progress=progress,
+                return_tokens=USE_DIFFUSION
+            )
+        else:
+            outputs = MODEL.generate(texts, progress=progress, return_tokens=USE_DIFFUSION)
+    except RuntimeError as e:
+        raise gr.Error("Error while generating " + e.args[0])
     if USE_DIFFUSION:
-        outputs_diffusion = MBD.tokens_to_wav(outputs[1])
+        if gradio_progress is not None:
+            gradio_progress(1, desc='Running MultiBandDiffusion...')
+        tokens = outputs[1]
+        if isinstance(MODEL.compression_model, InterleaveStereoCompressionModel):
+            left, right = MODEL.compression_model.get_left_right_codes(tokens)
+            tokens = torch.cat([left, right])
+        outputs_diffusion = MBD.tokens_to_wav(tokens)
+        if isinstance(MODEL.compression_model, InterleaveStereoCompressionModel):
+            assert outputs_diffusion.shape[1] == 1  # output is mono
+            outputs_diffusion = rearrange(outputs_diffusion, '(s b) c t -> b (s c) t', s=2)
         outputs = torch.cat([outputs[0], outputs_diffusion], dim=0)
     outputs = outputs.detach().cpu().float()
     pending_videos = []
     out_wavs = []
     for output in outputs:
         with NamedTemporaryFile("wb", suffix=".wav", delete=False) as file:
             audio_write(
@@ -150,47 +170,62 @@
     print("Tempfiles currently stored: ", len(file_cleaner.files))
     return out_videos, out_wavs
 
 
 def predict_batched(texts, melodies):
     max_text_length = 512
     texts = [text[:max_text_length] for text in texts]
-    load_model('facebook/musicgen-melody')
+    load_model('facebook/musicgen-stereo-melody')
     res = _do_predictions(texts, melodies, BATCHED_DURATION)
     return res
 
 
-def predict_full(model, decoder, text, melody, duration, topk, topp, temperature, cfg_coef, progress=gr.Progress()):
+def predict_full(model, model_path, decoder, text, melody, duration, topk, topp, temperature, cfg_coef, progress=gr.Progress()):
     global INTERRUPTING
     global USE_DIFFUSION
     INTERRUPTING = False
+    progress(0, desc="Loading model...")
+    model_path = model_path.strip()
+    if model_path:
+        if not Path(model_path).exists():
+            raise gr.Error(f"Model path {model_path} doesn't exist.")
+        if not Path(model_path).is_dir():
+            raise gr.Error(f"Model path {model_path} must be a folder containing "
+                           "state_dict.bin and compression_state_dict_.bin.")
+        model = model_path
     if temperature < 0:
         raise gr.Error("Temperature must be >= 0.")
     if topk < 0:
         raise gr.Error("Topk must be non-negative.")
     if topp < 0:
         raise gr.Error("Topp must be non-negative.")
 
     topk = int(topk)
     if decoder == "MultiBand_Diffusion":
         USE_DIFFUSION = True
+        progress(0, desc="Loading diffusion model...")
         load_diffusion()
     else:
         USE_DIFFUSION = False
     load_model(model)
 
+    max_generated = 0
+
     def _progress(generated, to_generate):
-        progress((min(generated, to_generate), to_generate))
+        nonlocal max_generated
+        max_generated = max(generated, max_generated)
+        progress((min(max_generated, to_generate), to_generate))
         if INTERRUPTING:
             raise gr.Error("Interrupted.")
     MODEL.set_custom_progress_callback(_progress)
 
     videos, wavs = _do_predictions(
         [text], [melody], duration, progress=True,
-        top_k=topk, top_p=topp, temperature=temperature, cfg_coef=cfg_coef)
+        top_k=topk, top_p=topp, temperature=temperature, cfg_coef=cfg_coef,
+        gradio_progress=progress)
     if USE_DIFFUSION:
         return videos[0], wavs[0], videos[1], wavs[1]
     return videos[0], wavs[0], None, None
 
 
 def toggle_audio_src(choice):
     if choice == "mic":
@@ -219,24 +254,28 @@
         with gr.Row():
             with gr.Column():
                 with gr.Row():
                     text = gr.Text(label="Input Text", interactive=True)
                     with gr.Column():
                         radio = gr.Radio(["file", "mic"], value="file",
                                          label="Condition on a melody (optional) File or Mic")
-                        melody = gr.Audio(source="upload", type="numpy", label="File",
+                        melody = gr.Audio(sources=["upload"], type="numpy", label="File",
                                           interactive=True, elem_id="melody-input")
                 with gr.Row():
                     submit = gr.Button("Submit")
                     # Adapted from https://github.com/rkfg/audiocraft/blob/long/app.py, MIT license.
                     _ = gr.Button("Interrupt").click(fn=interrupt, queue=False)
                 with gr.Row():
                     model = gr.Radio(["facebook/musicgen-melody", "facebook/musicgen-medium", "facebook/musicgen-small",
-                                      "facebook/musicgen-large"],
-                                     label="Model", value="facebook/musicgen-melody", interactive=True)
+                                      "facebook/musicgen-large", "facebook/musicgen-melody-large",
+                                      "facebook/musicgen-stereo-small", "facebook/musicgen-stereo-medium",
+                                      "facebook/musicgen-stereo-melody", "facebook/musicgen-stereo-large",
+                                      "facebook/musicgen-stereo-melody-large"],
+                                     label="Model", value="facebook/musicgen-stereo-melody", interactive=True)
+                    model_path = gr.Text(label="Model Path (custom models)")
                 with gr.Row():
                     decoder = gr.Radio(["Default", "MultiBand_Diffusion"],
                                        label="Decoder", value="Default", interactive=True)
                 with gr.Row():
                     duration = gr.Slider(minimum=1, maximum=120, value=10, label="Duration", interactive=True)
                 with gr.Row():
                     topk = gr.Number(label="Top-k", value=250, interactive=True)
@@ -245,107 +284,117 @@
                     cfg_coef = gr.Number(label="Classifier Free Guidance", value=3.0, interactive=True)
             with gr.Column():
                 output = gr.Video(label="Generated Music")
                 audio_output = gr.Audio(label="Generated Music (wav)", type='filepath')
                 diffusion_output = gr.Video(label="MultiBand Diffusion Decoder")
                 audio_diffusion = gr.Audio(label="MultiBand Diffusion Decoder (wav)", type='filepath')
         submit.click(toggle_diffusion, decoder, [diffusion_output, audio_diffusion], queue=False,
-                     show_progress=False).then(predict_full, inputs=[model, decoder, text, melody, duration, topk, topp,
+                     show_progress=False).then(predict_full, inputs=[model, model_path, decoder, text, melody, duration, topk, topp,
                                                                      temperature, cfg_coef],
                                                outputs=[output, audio_output, diffusion_output, audio_diffusion])
         radio.change(toggle_audio_src, radio, [melody], queue=False, show_progress=False)
 
         gr.Examples(
             fn=predict_full,
             examples=[
                 [
                     "An 80s driving pop song with heavy drums and synth pads in the background",
                     "./assets/bach.mp3",
-                    "facebook/musicgen-melody",
+                    "facebook/musicgen-stereo-melody",
                     "Default"
                 ],
                 [
                     "A cheerful country song with acoustic guitars",
                     "./assets/bolero_ravel.mp3",
-                    "facebook/musicgen-melody",
+                    "facebook/musicgen-stereo-melody",
                     "Default"
                 ],
                 [
                     "90s rock song with electric guitar and heavy drums",
                     None,
-                    "facebook/musicgen-medium",
+                    "facebook/musicgen-stereo-medium",
                     "Default"
                 ],
                 [
                     "a light and cheerly EDM track, with syncopated drums, aery pads, and strong emotions",
                     "./assets/bach.mp3",
-                    "facebook/musicgen-melody",
+                    "facebook/musicgen-stereo-melody",
                     "Default"
                 ],
                 [
                     "lofi slow bpm electro chill with organic samples",
                     None,
-                    "facebook/musicgen-medium",
+                    "facebook/musicgen-stereo-medium",
                     "Default"
                 ],
                 [
                     "Punk rock with loud drum and power guitar",
                     None,
-                    "facebook/musicgen-medium",
+                    "facebook/musicgen-stereo-medium",
                     "MultiBand_Diffusion"
                 ],
             ],
             inputs=[text, melody, model, decoder],
             outputs=[output]
         )
         gr.Markdown(
             """
             ### More details
 
             The model will generate a short music extract based on the description you provided.
-            The model can generate up to 30 seconds of audio in one pass. It is now possible
-            to extend the generation by feeding back the end of the previous chunk of audio.
+            The model can generate up to 30 seconds of audio in one pass.
+
+            The model was trained with description from a stock music catalog, descriptions that will work best
+            should include some level of details on the instruments present, along with some intended use case
+            (e.g. adding "perfect for a commercial" can somehow help).
+
+            Using one of the `melody` model (e.g. `musicgen-melody-*`), you can optionally provide a reference audio
+            from which a broad melody will be extracted.
+            The model will then try to follow both the description and melody provided.
+            For best results, the melody should be 30 seconds long (I know, the samples we provide are not...)
+
+            It is now possible to extend the generation by feeding back the end of the previous chunk of audio.
             This can take a long time, and the model might lose consistency. The model might also
             decide at arbitrary positions that the song ends.
 
             **WARNING:** Choosing long durations will take a long time to generate (2min might take ~10min).
             An overlap of 12 seconds is kept with the previously generated chunk, and 18 "new" seconds
             are generated each time.
 
-            We present 4 model variations:
+            We present 10 model variations:
             1. facebook/musicgen-melody -- a music generation model capable of generating music condition
                 on text and melody inputs. **Note**, you can also use text only.
             2. facebook/musicgen-small -- a 300M transformer decoder conditioned on text only.
             3. facebook/musicgen-medium -- a 1.5B transformer decoder conditioned on text only.
             4. facebook/musicgen-large -- a 3.3B transformer decoder conditioned on text only.
+            5. facebook/musicgen-melody-large -- a 3.3B transformer decoder conditioned on and melody.
+            6. facebook/musicgen-stereo-*: same as the previous models but fine tuned to output stereo audio.
 
             We also present two way of decoding the audio tokens
-            1. Use the default GAN based compression model
-            2. Use MultiBand Diffusion from (paper linknano )
-
-            When using `facebook/musicgen-melody`, you can optionally provide a reference audio from
-            which a broad melody will be extracted. The model will then try to follow both
-            the description and melody provided.
+            1. Use the default GAN based compression model. It can suffer from artifacts especially
+                for crashes, snares etc.
+            2. Use [MultiBand Diffusion](https://arxiv.org/abs/2308.02560). Should improve the audio quality,
+                at an extra computational cost. When this is selected, we provide both the GAN based decoded
+                audio, and the one obtained with MBD.
 
-            You can also use your own GPU or a Google Colab by following the instructions on our repo.
-            See [github.com/facebookresearch/audiocraft](https://github.com/facebookresearch/audiocraft)
+            See [github.com/facebookresearch/audiocraft](https://github.com/facebookresearch/audiocraft/blob/main/docs/MUSICGEN.md)
             for more details.
             """
         )
 
         interface.queue().launch(**launch_kwargs)
 
 
 def ui_batched(launch_kwargs):
     with gr.Blocks() as demo:
         gr.Markdown(
             """
             # MusicGen
 
-            This is the demo for [MusicGen](https://github.com/facebookresearch/audiocraft),
+            This is the demo for [MusicGen](https://github.com/facebookresearch/audiocraft/blob/main/docs/MUSICGEN.md),
             a simple and controllable model for music generation
             presented at: ["Simple and Controllable Music Generation"](https://huggingface.co/papers/2306.05284).
             <br/>
             <a href="https://huggingface.co/spaces/facebook/MusicGen?duplicate=true"
                 style="display: inline-block;margin-top: .5em;margin-right: .25em;" target="_blank">
             <img style="margin-bottom: 0em;display: inline;margin-top: -.25em;"
                 src="https://bit.ly/3gLdBN6" alt="Duplicate Space"></a>
@@ -395,23 +444,35 @@
             ],
             inputs=[text, melody],
             outputs=[output]
         )
         gr.Markdown("""
         ### More details
 
-        The model will generate 12 seconds of audio based on the description you provided.
+        The model will generate 15 seconds of audio based on the description you provided.
+        The model was trained with description from a stock music catalog, descriptions that will work best
+        should include some level of details on the instruments present, along with some intended use case
+        (e.g. adding "perfect for a commercial" can somehow help).
+
         You can optionally provide a reference audio from which a broad melody will be extracted.
         The model will then try to follow both the description and melody provided.
-        All samples are generated with the `melody` model.
+        For best results, the melody should be 30 seconds long (I know, the samples we provide are not...)
 
-        You can also use your own GPU or a Google Colab by following the instructions on our repo.
+        You can access more control (longer generation, more models etc.) by clicking
+        the <a href="https://huggingface.co/spaces/facebook/MusicGen?duplicate=true"
+                style="display: inline-block;margin-top: .5em;margin-right: .25em;" target="_blank">
+            <img style="margin-bottom: 0em;display: inline;margin-top: -.25em;"
+                src="https://bit.ly/3gLdBN6" alt="Duplicate Space"></a>
+        (you will then need a paid GPU from HuggingFace).
+        If you have a GPU, you can run the gradio demo locally (click the link to our repo below for more info).
+        Finally, you can get a GPU for free from Google
+        and run the demo in [a Google Colab.](https://ai.honu.io/red/musicgen-colab).
 
-        See [github.com/facebookresearch/audiocraft](https://github.com/facebookresearch/audiocraft)
-        for more details.
+        See [github.com/facebookresearch/audiocraft](https://github.com/facebookresearch/audiocraft/blob/main/docs/MUSICGEN.md)
+        for more details. All samples are generated with the `stereo-melody` model.
         """)
 
         demo.queue(max_size=8 * 4).launch(**launch_kwargs)
 
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser()
@@ -450,14 +511,16 @@
     if args.server_port:
         launch_kwargs['server_port'] = args.server_port
     if args.inbrowser:
         launch_kwargs['inbrowser'] = args.inbrowser
     if args.share:
         launch_kwargs['share'] = args.share
 
+    logging.basicConfig(level=logging.INFO, stream=sys.stderr)
+
     # Show the interface
     if IS_BATCHED:
         global USE_DIFFUSION
         USE_DIFFUSION = False
         ui_batched(launch_kwargs)
     else:
         ui_full(launch_kwargs)
```

### Comparing `audiocraft-1.1.0/demos/musicgen_demo.ipynb` & `audiocraft-1.2.0/demos/musicgen_demo.ipynb`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/docs/AUDIOGEN.md` & `audiocraft-1.2.0/docs/AUDIOGEN.md`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/docs/CONDITIONING.md` & `audiocraft-1.2.0/docs/CONDITIONING.md`

 * *Files 6% similar despite different names*

```diff
@@ -11,29 +11,29 @@
 
 For now, we support 3 main types of conditioning within AudioCraft:
 * Text-based conditioning methods
 * Waveform-based conditioning methods
 * Joint embedding conditioning methods for text and audio projected in a shared latent space.
 
 The Language Model relies on 2 core components that handle processing information:
-* The `ConditionProvider` class, that maps metadata to processed conditions leveraging
+* The `ConditionProvider` class, that maps metadata to processed conditions, leveraging
 all the defined conditioners for the given task.
 * The `ConditionFuser` class, that takes preprocessed conditions and properly fuse the
 conditioning embedding to the language model inputs following a given fusing strategy.
 
 Different conditioners (for text, waveform, joint embeddings...) are provided as torch
 modules in AudioCraft and are used internally in the language model to process the
 conditioning signals and feed them to the language model.
 
 
 ## Core concepts
 
 ### Conditioners
 
-The `BaseConditioner` torch module is the base implementation for all conditioners in audiocraft.
+The `BaseConditioner` torch module is the base implementation for all conditioners in AudioCraft.
 
 Each conditioner is expected to implement 2 methods:
 * The `tokenize` method that is used as a preprocessing method that contains all processing
 that can lead to synchronization points (e.g. BPE tokenization with transfer to the GPU).
 The output of the tokenize method will then be used to feed the forward method.
 * The `forward` method that takes the output of the tokenize method and contains the core computation
 to obtain the conditioning embedding along with a mask indicating valid indices (e.g. padding tokens).
@@ -41,18 +41,18 @@
 ### ConditionProvider
 
 The ConditionProvider prepares and provides conditions given a dictionary of conditioners.
 
 Conditioners are specified as a dictionary of attributes and the corresponding conditioner
 providing the processing logic for the given attribute.
 
-Similarly to the conditioners, the condition provider works in two steps to avoid sychronization points:
+Similarly to the conditioners, the condition provider works in two steps to avoid synchronization points:
 * A `tokenize` method that takes a list of conditioning attributes for the batch,
-and run all tokenize steps for the set of conditioners.
-* A `forward` method that takes the output of the tokenize step and run all the forward steps
+and runs all tokenize steps for the set of conditioners.
+* A `forward` method that takes the output of the tokenize step and runs all the forward steps
 for the set of conditioners.
 
 The list of conditioning attributes is passed as a list of `ConditioningAttributes`
 that is presented just below.
 
 ### ConditionFuser
 
@@ -107,23 +107,23 @@
 * The `T5Conditioner` that relies on a
 [pre-trained T5 model](https://huggingface.co/docs/transformers/model_doc/t5)
 frozen or fine-tuned at train time to extract the text embeddings.
 
 ### Waveform conditioners
 
 All waveform conditioners are expected to inherit from the `WaveformConditioner` class and
-consists of conditioning method that takes a waveform as input. The waveform conditioner
+consist of a conditioning method that takes a waveform as input. The waveform conditioner
 must implement the logic to extract the embedding from the waveform and define the downsampling
 factor from the waveform to the resulting embedding.
 
 The `ChromaStemConditioner` conditioner is a waveform conditioner for the chroma features
-conditioning used by MusicGen. It takes a given waveform, extract relevant stems for melody
+conditioning used by MusicGen. It takes a given waveform, extracts relevant stems for melody
 (namely all non drums and bass stems) using a
 [pre-trained Demucs model](https://github.com/facebookresearch/demucs)
-and then extract the chromagram bins from the remaining mix of stems.
+and then extracts the chromagram bins from the remaining mix of stems.
 
 ### Joint embeddings conditioners
 
 We finally provide support for conditioning based on joint text and audio embeddings through
 the `JointEmbeddingConditioner` class and the `CLAPEmbeddingConditioner` that implements such
 a conditioning method relying on a [pretrained CLAP model](https://github.com/LAION-AI/CLAP).
 
@@ -139,8 +139,8 @@
 not to expect all conditioning signals to be provided at once.
 
 ## Faster computation of conditions
 
 Conditioners that require some heavy computation on the waveform can be cached, in particular
 the `ChromaStemConditioner` or `CLAPEmbeddingConditioner`. You just need to provide the
 `cache_path` parameter to them. We recommend running dummy jobs for filling up the cache quickly.
-An example is provied in the [musicgen.musicgen_melody_32khz grid](../audiocraft/grids/musicgen/musicgen_melody_32khz.py).
+An example is provided in the [musicgen.musicgen_melody_32khz grid](../audiocraft/grids/musicgen/musicgen_melody_32khz.py).
```

### Comparing `audiocraft-1.1.0/docs/DATASETS.md` & `audiocraft-1.2.0/docs/DATASETS.md`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/docs/ENCODEC.md` & `audiocraft-1.2.0/docs/ENCODEC.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # EnCodec: High Fidelity Neural Audio Compression
 
 AudioCraft provides the training code for EnCodec, a state-of-the-art deep learning
-based audio codec supporting both mono stereo audio, presented in the
+based audio codec supporting both mono and stereo audio, presented in the
 [High Fidelity Neural Audio Compression][arxiv] paper.
 Check out our [sample page][encodec_samples].
 
 ## Original EnCodec models
 
 The EnCodec models presented in High Fidelity Neural Audio Compression can be accessed
 and used with the [EnCodec repository](https://github.com/facebookresearch/encodec).
@@ -22,15 +22,15 @@
 ## Training
 
 The [CompressionSolver](../audiocraft/solvers/compression.py) implements the audio reconstruction
 task to train an EnCodec model. Specifically, it trains an encoder-decoder with a quantization
 bottleneck - a SEANet encoder-decoder with Residual Vector Quantization bottleneck for EnCodec -
 using a combination of objective and perceptual losses in the forms of discriminators.
 
-The default configuration matches a causal EnCodec training with at a single bandwidth.
+The default configuration matches a causal EnCodec training at a single bandwidth.
 
 ### Example configuration and grids
 
 We provide sample configuration and grids for training EnCodec models.
 
 The compression configuration are defined in
 [config/solver/compression](../config/solver/compression).
@@ -41,24 +41,24 @@
 ```shell
 # base causal encodec on monophonic audio sampled at 24 khz
 dora grid compression.encodec_base_24khz
 # encodec model used for MusicGen on monophonic audio sampled at 32 khz
 dora grid compression.encodec_musicgen_32khz
 ```
 
-### Training and valid stages
+### Training and validation stages
 
 The model is trained using a combination of objective and perceptual losses.
 More specifically, EnCodec is trained with the MS-STFT discriminator along with
 objective losses through the use of a loss balancer to effectively weight
 the different losses, in an intuitive manner.
 
 ### Evaluation stage
 
-Evaluations metrics for audio generation:
+Evaluation metrics for audio generation:
 * SI-SNR: Scale-Invariant Signal-to-Noise Ratio.
 * ViSQOL: Virtual Speech Quality Objective Listener.
 
 Note: Path to the ViSQOL binary (compiled with bazel) needs to be provided in
 order to run the ViSQOL metric on the reference and degraded signals.
 The metric is disabled by default.
 Please refer to the [metrics documentation](../METRICS.md) to learn more.
@@ -106,34 +106,35 @@
 # Finally, you can also retrieve the full Solver object, with its dataloader etc.
 from audiocraft import train
 from pathlib import Path
 import logging
 import os
 import sys
 
-# uncomment the following line if you want some detailed logs when loading a Solver.
-logging.basicConfig(stream=sys.stderr, level=logging.INFO)
+# Uncomment the following line if you want some detailed logs when loading a Solver.
+# logging.basicConfig(stream=sys.stderr, level=logging.INFO)
+
 # You must always run the following function from the root directory.
 os.chdir(Path(train.__file__).parent.parent)
 
 
 # You can also get the full solver (only for your own experiments).
 # You can provide some overrides to the parameters to make things more convenient.
 solver = train.get_solver_from_sig('SIG', {'device': 'cpu', 'dataset': {'batch_size': 8}})
 solver.model
 solver.dataloaders
 ```
 
 ### Importing / Exporting models
 
 At the moment we do not have a definitive workflow for exporting EnCodec models, for
-instance to Hugging Face (HF). We are working on supporting automatic convertion between
+instance to Hugging Face (HF). We are working on supporting automatic conversion between
 AudioCraft and Hugging Face implementations.
 
-We still have some support for fine tuning an EnCodec model coming from HF in AudioCraft,
+We still have some support for fine-tuning an EnCodec model coming from HF in AudioCraft,
 using for instance `continue_from=//pretrained/facebook/encodec_32k`.
 
 An AudioCraft checkpoint can be exported in a more compact format (excluding the optimizer etc.)
 using `audiocraft.utils.export.export_encodec`. For instance, you could run
 
 ```python
 from audiocraft.utils import export
@@ -144,19 +145,19 @@
     '/checkpoints/my_audio_lm/compression_state_dict.bin')
 
 
 from audiocraft.models import CompressionModel
 model = CompressionModel.get_pretrained('/checkpoints/my_audio_lm/compression_state_dict.bin')
 
 from audiocraft.solvers import CompressionSolver
-# The two are strictly equivalent, but this function supports also loading from non already exported models.
+# The two are strictly equivalent, but this function supports also loading from non-already exported models.
 model = CompressionSolver.model_from_checkpoint('//pretrained//checkpoints/my_audio_lm/compression_state_dict.bin')
 ```
 
-We will see then how to use this model as a tokenizer for MusicGen/Audio gen in the
+We will see then how to use this model as a tokenizer for MusicGen/AudioGen in the
 [MusicGen documentation](./MUSICGEN.md).
 
 ### Learn more
 
 Learn more about AudioCraft training pipelines in the [dedicated section](./TRAINING.md).
```

### Comparing `audiocraft-1.1.0/docs/MBD.md` & `audiocraft-1.2.0/docs/MBD.md`

 * *Files 3% similar despite different names*

```diff
@@ -109,9 +109,9 @@
 
 
 ## License
 
 See license information in the [README](../README.md).
 
 
-[arxiv]: https://dl.fbaipublicfiles.com/encodec/Diffusion/paper.pdf
+[arxiv]: https://arxiv.org/abs/2308.02560
 [mbd_samples]: https://ai.honu.io/papers/mbd/
```

#### html2text {}

```diff
@@ -55,9 +55,9 @@
 bands MBD trainning dora grid diffusion.4_bands_base_32khz ``` ### Learn more
 Learn more about AudioCraft training pipelines in the [dedicated section](./
 TRAINING.md). ## Citation ``` @article{sanroman2023fromdi, title={From Discrete
 Tokens to High-Fidelity Audio Using Multi-Band Diffusion}, author={San Roman,
 Robin and Adi, Yossi and Deleforge, Antoine and Serizel, Romain and Synnaeve,
 Gabriel and DÃ©fossez, Alexandre}, journal={arXiv preprint arXiv:}, year={2023}
 } ``` ## License See license information in the [README](../README.md).
-[arxiv]: https://dl.fbaipublicfiles.com/encodec/Diffusion/paper.pdf
-[mbd_samples]: https://ai.honu.io/papers/mbd/
+[arxiv]: https://arxiv.org/abs/2308.02560 [mbd_samples]: https://ai.honu.io/
+papers/mbd/
```

### Comparing `audiocraft-1.1.0/docs/METRICS.md` & `audiocraft-1.2.0/docs/METRICS.md`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/docs/MUSICGEN.md` & `audiocraft-1.2.0/docs/MUSICGEN.md`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 <a href="https://github.com/facebookresearch/encodec">EnCodec tokenizer</a> with 4 codebooks sampled at 50 Hz.
 Unlike existing methods like [MusicLM](https://arxiv.org/abs/2301.11325), MusicGen doesn't require
 a self-supervised semantic representation, and it generates all 4 codebooks in one pass. By introducing
 a small delay between the codebooks, we show we can predict them in parallel, thus having only 50 auto-regressive
 steps per second of audio.
 Check out our [sample page][musicgen_samples] or test the available demo!
 
-<a target="_blank" href="https://colab.research.google.com/drive/1JlTOjB-G0A2Hz3h8PK63vLZk4xdCI5QB?usp=sharing">
+<a target="_blank" href="https://ai.honu.io/red/musicgen-colab">
   <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
 </a>
 <a target="_blank" href="https://huggingface.co/spaces/facebook/MusicGen">
   <img src="https://huggingface.co/datasets/huggingface/badges/raw/main/open-in-hf-spaces-sm.svg" alt="Open in HugginFace"/>
 </a>
 <br>
 
@@ -34,28 +34,35 @@
 
 ## Usage
 
 We offer a number of way to interact with MusicGen:
 1. A demo is also available on the [`facebook/MusicGen` Hugging Face Space](https://huggingface.co/spaces/facebook/MusicGen)
 (huge thanks to all the HF team for their support).
 2. You can run the extended demo on a Colab:
-[colab notebook](https://colab.research.google.com/drive/1JlTOjB-G0A2Hz3h8PK63vLZk4xdCI5QB?usp=sharing)
+[colab notebook](https://ai.honu.io/red/musicgen-colab)
 3. You can use the gradio demo locally by running [`python -m demos.musicgen_app --share`](../demos/musicgen_app.py).
 4. You can play with MusicGen by running the jupyter notebook at [`demos/musicgen_demo.ipynb`](../demos/musicgen_demo.ipynb) locally (if you have a GPU).
 5. Finally, checkout [@camenduru Colab page](https://github.com/camenduru/MusicGen-colab)
 which is regularly updated with contributions from @camenduru and the community.
 
 
 ## API
 
-We provide a simple API and 4 pre-trained models. The pre trained models are:
+We provide a simple API and 10 pre-trained models. The pre trained models are:
 - `facebook/musicgen-small`: 300M model, text to music only - [🤗 Hub](https://huggingface.co/facebook/musicgen-small)
 - `facebook/musicgen-medium`: 1.5B model, text to music only - [🤗 Hub](https://huggingface.co/facebook/musicgen-medium)
 - `facebook/musicgen-melody`: 1.5B model, text to music and text+melody to music - [🤗 Hub](https://huggingface.co/facebook/musicgen-melody)
 - `facebook/musicgen-large`: 3.3B model, text to music only - [🤗 Hub](https://huggingface.co/facebook/musicgen-large)
+- `facebook/musicgen-melody-large`: 3.3B model, text to music and text+melody to music - [🤗 Hub](https://huggingface.co/facebook/musicgen-melody-large)
+- `facebook/musicgen-stereo-*`: All the previous models fine tuned for stereo generation -
+    [small](https://huggingface.co/facebook/musicgen-stereo-small),
+    [medium](https://huggingface.co/facebook/musicgen-stereo-medium),
+    [large](https://huggingface.co/facebook/musicgen-stereo-large),
+    [melody](https://huggingface.co/facebook/musicgen-stereo-melody),
+    [melody large](https://huggingface.co/facebook/musicgen-stereo-melody-large).
 
 We observe the best trade-off between quality and compute with the `facebook/musicgen-medium` or `facebook/musicgen-melody` model.
 In order to use MusicGen locally **you must have a GPU**. We recommend 16GB of memory, but smaller
 GPUs will be able to generate short sequences, or longer sequences with the `facebook/musicgen-small` model.
 
 See after a quick example for using the API.
 
@@ -205,14 +212,27 @@
     compression_model_checkpoint=//sig/SIG \ # where SIG is the Dora signature of the EnCodec XP.
     transformer_lm.n_q=... transformer_lm.card=...
 ```
 
 **Warning:** you are responsible for setting the proper value for `transformer_lm.n_q` and `transformer_lm.card` (cardinality of the codebooks). You also have to update the codebook_pattern to match `n_q` as shown in the example for using DAC. .
 
 
+### Training stereo models
+
+Use the option `interleave_stereo_codebooks.use` set to `True` to activate stereo training along with `channels=2`. Left and right channels will be
+encoded separately by the compression model, then their codebook will be interleaved, e.g. order of codebook is
+`[1_L, 1_R, 2_L, 2_R, ...]`. You will also need to update the delays for the codebook patterns to match the number of codebooks, and the `n_q` value passed to the transformer LM:
+```
+dora run solver=musicgen/debug \
+    compression_model_checkpoint=//pretrained/facebook/encodec_32khz \
+    channels=2 interleave_stereo_codebooks.use=True \
+    transformer_lm.n_q=8 transformer_lm.card=2048 \
+    codebooks_pattern.delay.delays='[0, 0, 1, 1, 2, 2, 3, 3]'
+```
+
 ### Fine tuning existing models
 
 You can initialize your model to one of the pretrained models by using the `continue_from` argument, in particular
 
 ```bash
 # Using pretrained MusicGen model.
 dora run solver=musicgen/musicgen_base_32khz model/lm/model_scale=medium continue_from=//pretrained/facebook/musicgen-medium conditioner=text2music
@@ -228,14 +248,47 @@
     with the model you are fine tuning. Configuration is NOT automatically inherited from the model you continue from. In particular make sure to select the proper `conditioner` and `model/lm/model_scale`.
 
 **Warning:** We currently do not support fine tuning a model with slightly different layers. If you decide
  to change some parts, like the conditioning or some other parts of the model, you are responsible for manually crafting a checkpoint file from which we can safely run `load_state_dict`.
  If you decide to do so, make sure your checkpoint is saved with `torch.save` and contains a dict
     `{'best_state': {'model': model_state_dict_here}}`. Directly give the path to `continue_from` without a `//pretrained/` prefix.
 
+
+#### Fine tuning mono model to stereo
+
+You will not be able to `continue_from` a mono model with stereo training, as the shape of the embeddings and output linears
+would not match. You can use the following snippet to prepare a proper finetuning checkpoint.
+
+```python
+from pathlib import Path
+import torch
+
+# Download the pretrained model, e.g. from
+# https://huggingface.co/facebook/musicgen-melody/blob/main/state_dict.bin
+
+model_name = 'musicgen-melody'
+root = Path.home() / 'checkpoints'
+# You are responsible for downloading the following checkpoint in the proper location
+input_state_dict_path = root / model_name / 'state_dict.bin'
+state = torch.load(input_state_dict_path, 'cpu')
+bs = state['best_state']
+# there is a slight different in format between training checkpoints and exported public checkpoints.
+# If you want to use your own mono models from one of your training checkpont, following the instructions
+# for exporting a model explained later on this page.
+assert 'model' not in bs, 'The following code is for using an exported pretrained model'
+nbs = dict(bs)
+for k in range(8):
+    # We will just copy mono embeddings and linears twice, once for left and right channels.
+    nbs[f'linears.{k}.weight'] = bs[f'linears.{k//2}.weight']
+    nbs[f'emb.{k}.weight'] = bs[f'emb.{k//2}.weight']
+torch.save({'best_state': {'model': nbs}}, root / f'stereo_finetune_{model_name}.th')
+```
+
+Now, you can use `$HOME/checkpoints/stereo_finetune_musicgen-melody.th` as a `continue_from` target (without a `//pretrained` prefix!).
+
 ### Caching of EnCodec tokens
 
 It is possible to precompute the EnCodec tokens and other metadata.
 An example of generating and using this cache provided in the [musicgen.musicgen_base_cached_32khz grid](../audiocraft/grids/musicgen/musicgen_base_cached_32khz.py).
 
 ### Evaluation stage
 
@@ -283,17 +336,17 @@
 
 ### Playing with the model
 
 Once you have launched some experiments, you can easily get access
 to the Solver with the latest trained model using the following snippet.
 
 ```python
-from audiocraft.solvers.musicgen import MusicGen
+from audiocraft.solvers.musicgen import MusicGenSolver
 
-solver = MusicGen.get_eval_solver_from_sig('SIG', device='cpu', batch_size=8)
+solver = MusicGenSolver.get_eval_solver_from_sig('SIG', device='cpu', batch_size=8)
 solver.model
 solver.dataloaders
 ```
 
 ### Importing / Exporting models
 
 We do not support currently loading a model from the Hugging Face implementation or exporting to it.
@@ -344,19 +397,19 @@
 The two are mutually exclusive (because FSDP does autocast on its own).
 You can use autocast up to 1.5B (medium), if you have enough RAM on your GPU.
 FSDP makes everything more complex but will free up some memory for the actual
 activations by sharding the optimizer state.
 
 ## Citation
 ```
-@article{copet2023simple,
+@inproceedings{copet2023simple,
     title={Simple and Controllable Music Generation},
     author={Jade Copet and Felix Kreuk and Itai Gat and Tal Remez and David Kant and Gabriel Synnaeve and Yossi Adi and Alexandre Défossez},
+    booktitle={Thirty-seventh Conference on Neural Information Processing Systems},
     year={2023},
-    journal={arXiv preprint arXiv:2306.05284},
 }
 ```
 
 
 ## License
 
 See license information in the [model card](../model_cards/MUSICGEN_MODEL_CARD.md).
```

#### html2text {}

```diff
@@ -15,35 +15,42 @@
 MUSICGEN_MODEL_CARD.md). ## Installation Please follow the AudioCraft
 installation instructions from the [README](../README.md). AudioCraft requires
 a GPU with at least 16 GB of memory for running inference with the medium-sized
 models (~1.5B parameters). ## Usage We offer a number of way to interact with
 MusicGen: 1. A demo is also available on the [`facebook/MusicGen` Hugging Face
 Space](https://huggingface.co/spaces/facebook/MusicGen) (huge thanks to all the
 HF team for their support). 2. You can run the extended demo on a Colab: [colab
-notebook](https://colab.research.google.com/drive/1JlTOjB-
-G0A2Hz3h8PK63vLZk4xdCI5QB?usp=sharing) 3. You can use the gradio demo locally
-by running [`python -m demos.musicgen_app --share`](../demos/musicgen_app.py).
-4. You can play with MusicGen by running the jupyter notebook at [`demos/
-musicgen_demo.ipynb`](../demos/musicgen_demo.ipynb) locally (if you have a
-GPU). 5. Finally, checkout [@camenduru Colab page](https://github.com/
+notebook](https://ai.honu.io/red/musicgen-colab) 3. You can use the gradio demo
+locally by running [`python -m demos.musicgen_app --share`](../demos/
+musicgen_app.py). 4. You can play with MusicGen by running the jupyter notebook
+at [`demos/musicgen_demo.ipynb`](../demos/musicgen_demo.ipynb) locally (if you
+have a GPU). 5. Finally, checkout [@camenduru Colab page](https://github.com/
 camenduru/MusicGen-colab) which is regularly updated with contributions from
-@camenduru and the community. ## API We provide a simple API and 4 pre-trained
+@camenduru and the community. ## API We provide a simple API and 10 pre-trained
 models. The pre trained models are: - `facebook/musicgen-small`: 300M model,
 text to music only - [ð¤ Hub](https://huggingface.co/facebook/musicgen-small)
 - `facebook/musicgen-medium`: 1.5B model, text to music only - [ð¤ Hub]
 (https://huggingface.co/facebook/musicgen-medium) - `facebook/musicgen-melody`:
 1.5B model, text to music and text+melody to music - [ð¤ Hub](https://
 huggingface.co/facebook/musicgen-melody) - `facebook/musicgen-large`: 3.3B
 model, text to music only - [ð¤ Hub](https://huggingface.co/facebook/
-musicgen-large) We observe the best trade-off between quality and compute with
-the `facebook/musicgen-medium` or `facebook/musicgen-melody` model. In order to
-use MusicGen locally **you must have a GPU**. We recommend 16GB of memory, but
-smaller GPUs will be able to generate short sequences, or longer sequences with
-the `facebook/musicgen-small` model. See after a quick example for using the
-API. ```python import torchaudio from audiocraft.models import MusicGen from
+musicgen-large) - `facebook/musicgen-melody-large`: 3.3B model, text to music
+and text+melody to music - [ð¤ Hub](https://huggingface.co/facebook/musicgen-
+melody-large) - `facebook/musicgen-stereo-*`: All the previous models fine
+tuned for stereo generation - [small](https://huggingface.co/facebook/musicgen-
+stereo-small), [medium](https://huggingface.co/facebook/musicgen-stereo-
+medium), [large](https://huggingface.co/facebook/musicgen-stereo-large),
+[melody](https://huggingface.co/facebook/musicgen-stereo-melody), [melody
+large](https://huggingface.co/facebook/musicgen-stereo-melody-large). We
+observe the best trade-off between quality and compute with the `facebook/
+musicgen-medium` or `facebook/musicgen-melody` model. In order to use MusicGen
+locally **you must have a GPU**. We recommend 16GB of memory, but smaller GPUs
+will be able to generate short sequences, or longer sequences with the
+`facebook/musicgen-small` model. See after a quick example for using the API.
+```python import torchaudio from audiocraft.models import MusicGen from
 audiocraft.data.audio import audio_write model = MusicGen.get_pretrained
 ('facebook/musicgen-melody') model.set_generation_params(duration=8) # generate
 8 seconds. wav = model.generate_unconditional(4) # generates 4 unconditional
 audio samples descriptions = ['happy rock', 'energetic EDM', 'sad jazz'] wav =
 model.generate(descriptions) # generates 3 samples. melody, sr =
 torchaudio.load('./assets/bach.mp3') # generates using the melody from the
 given audio and the provided descriptions. wav = model.generate_with_chroma
@@ -116,74 +123,104 @@
 compression_state_dict.bin \ transformer_lm.n_q=... transformer_lm.card=... #
 Using your own model from its training checkpoint. dora run solver=musicgen/
 debug \ compression_model_checkpoint=//sig/SIG \ # where SIG is the Dora
 signature of the EnCodec XP. transformer_lm.n_q=... transformer_lm.card=... ```
 **Warning:** you are responsible for setting the proper value for
 `transformer_lm.n_q` and `transformer_lm.card` (cardinality of the codebooks).
 You also have to update the codebook_pattern to match `n_q` as shown in the
-example for using DAC. . ### Fine tuning existing models You can initialize
-your model to one of the pretrained models by using the `continue_from`
-argument, in particular ```bash # Using pretrained MusicGen model. dora run
-solver=musicgen/musicgen_base_32khz model/lm/model_scale=medium continue_from=/
-/pretrained/facebook/musicgen-medium conditioner=text2music # Using another
-model you already trained with a Dora signature SIG. dora run solver=musicgen/
+example for using DAC. . ### Training stereo models Use the option
+`interleave_stereo_codebooks.use` set to `True` to activate stereo training
+along with `channels=2`. Left and right channels will be encoded separately by
+the compression model, then their codebook will be interleaved, e.g. order of
+codebook is `[1_L, 1_R, 2_L, 2_R, ...]`. You will also need to update the
+delays for the codebook patterns to match the number of codebooks, and the
+`n_q` value passed to the transformer LM: ``` dora run solver=musicgen/debug \
+compression_model_checkpoint=//pretrained/facebook/encodec_32khz \ channels=2
+interleave_stereo_codebooks.use=True \ transformer_lm.n_q=8
+transformer_lm.card=2048 \ codebooks_pattern.delay.delays='[0, 0, 1, 1, 2, 2,
+3, 3]' ``` ### Fine tuning existing models You can initialize your model to one
+of the pretrained models by using the `continue_from` argument, in particular
+```bash # Using pretrained MusicGen model. dora run solver=musicgen/
+musicgen_base_32khz model/lm/model_scale=medium continue_from=//pretrained/
+facebook/musicgen-medium conditioner=text2music # Using another model you
+already trained with a Dora signature SIG. dora run solver=musicgen/
 musicgen_base_32khz model/lm/model_scale=medium continue_from=//sig/SIG
 conditioner=text2music # Or providing manually a path dora run solver=musicgen/
 musicgen_base_32khz model/lm/model_scale=medium continue_from=/checkpoints/
 my_other_xp/checkpoint.th ``` **Warning:** You are responsible for selecting
 the other parameters accordingly, in a way that make it compatible with the
 model you are fine tuning. Configuration is NOT automatically inherited from
 the model you continue from. In particular make sure to select the proper
 `conditioner` and `model/lm/model_scale`. **Warning:** We currently do not
 support fine tuning a model with slightly different layers. If you decide to
 change some parts, like the conditioning or some other parts of the model, you
 are responsible for manually crafting a checkpoint file from which we can
 safely run `load_state_dict`. If you decide to do so, make sure your checkpoint
 is saved with `torch.save` and contains a dict `{'best_state': {'model':
 model_state_dict_here}}`. Directly give the path to `continue_from` without a
-`//pretrained/` prefix. ### Caching of EnCodec tokens It is possible to
-precompute the EnCodec tokens and other metadata. An example of generating and
-using this cache provided in the [musicgen.musicgen_base_cached_32khz grid](../
-audiocraft/grids/musicgen/musicgen_base_cached_32khz.py). ### Evaluation stage
-By default, evaluation stage is also computing the cross-entropy and the
-perplexity over the evaluation dataset. Indeed the objective metrics used for
-evaluation can be costly to run or require some extra dependencies. Please
-refer to the [metrics documentation](./METRICS.md) for more details on the
-requirements for each metric. We provide an off-the-shelf configuration to
-enable running the objective metrics for audio generation in [config/solver/
-musicgen/evaluation/objective_eval](../config/solver/musicgen/evaluation/
-objective_eval.yaml). One can then activate evaluation the following way:
-```shell # using the configuration dora run solver=musicgen/debug solver/
-musicgen/evaluation=objective_eval # specifying each of the fields, e.g. to
-activate KL computation dora run solver=musicgen/debug
-evaluate.metrics.kld=true ``` See [an example evaluation grid](../audiocraft/
-grids/musicgen/musicgen_pretrained_32khz_eval.py). ### Generation stage The
-generation stage allows to generate samples conditionally and/or
-unconditionally and to perform audio continuation (from a prompt). We currently
-support greedy sampling (argmax), sampling from softmax with a given
-temperature, top-K and top-P (nucleus) sampling. The number of samples
-generated and the batch size used are controlled by the `dataset.generate`
-configuration while the other generation parameters are defined in
-`generate.lm`. ```shell # control sampling parameters dora run solver=musicgen/
-debug generate.lm.gen_duration=10 generate.lm.use_sampling=true
-generate.lm.top_k=15 ``` #### Listening to samples Note that generation happens
-automatically every 25 epochs. You can easily access and compare samples
-between models (as long as they are trained) on the same dataset using the MOS
-tool. For that first `pip install Flask gunicorn`. Then ``` gunicorn -w 4 -
-b 127.0.0.1:8895 -t 120 'scripts.mos:app' --access-logfile - ``` And access the
-tool at [https://127.0.0.1:8895](https://127.0.0.1:8895). ### Playing with the
-model Once you have launched some experiments, you can easily get access to the
-Solver with the latest trained model using the following snippet. ```python
-from audiocraft.solvers.musicgen import MusicGen solver =
-MusicGen.get_eval_solver_from_sig('SIG', device='cpu', batch_size=8)
-solver.model solver.dataloaders ``` ### Importing / Exporting models We do not
-support currently loading a model from the Hugging Face implementation or
-exporting to it. If you want to export your model in a way that is compatible
-with `audiocraft.models.MusicGen` API, you can run: ```python from
-audiocraft.utils import export from audiocraft import train xp =
+`//pretrained/` prefix. #### Fine tuning mono model to stereo You will not be
+able to `continue_from` a mono model with stereo training, as the shape of the
+embeddings and output linears would not match. You can use the following
+snippet to prepare a proper finetuning checkpoint. ```python from pathlib
+import Path import torch # Download the pretrained model, e.g. from # https://
+huggingface.co/facebook/musicgen-melody/blob/main/state_dict.bin model_name =
+'musicgen-melody' root = Path.home() / 'checkpoints' # You are responsible for
+downloading the following checkpoint in the proper location
+input_state_dict_path = root / model_name / 'state_dict.bin' state = torch.load
+(input_state_dict_path, 'cpu') bs = state['best_state'] # there is a slight
+different in format between training checkpoints and exported public
+checkpoints. # If you want to use your own mono models from one of your
+training checkpont, following the instructions # for exporting a model
+explained later on this page. assert 'model' not in bs, 'The following code is
+for using an exported pretrained model' nbs = dict(bs) for k in range(8): # We
+will just copy mono embeddings and linears twice, once for left and right
+channels. nbs[f'linears.{k}.weight'] = bs[f'linears.{k//2}.weight'] nbs[f'emb.
+{k}.weight'] = bs[f'emb.{k//2}.weight'] torch.save({'best_state': {'model':
+nbs}}, root / f'stereo_finetune_{model_name}.th') ``` Now, you can use `$HOME/
+checkpoints/stereo_finetune_musicgen-melody.th` as a `continue_from` target
+(without a `//pretrained` prefix!). ### Caching of EnCodec tokens It is
+possible to precompute the EnCodec tokens and other metadata. An example of
+generating and using this cache provided in the
+[musicgen.musicgen_base_cached_32khz grid](../audiocraft/grids/musicgen/
+musicgen_base_cached_32khz.py). ### Evaluation stage By default, evaluation
+stage is also computing the cross-entropy and the perplexity over the
+evaluation dataset. Indeed the objective metrics used for evaluation can be
+costly to run or require some extra dependencies. Please refer to the [metrics
+documentation](./METRICS.md) for more details on the requirements for each
+metric. We provide an off-the-shelf configuration to enable running the
+objective metrics for audio generation in [config/solver/musicgen/evaluation/
+objective_eval](../config/solver/musicgen/evaluation/objective_eval.yaml). One
+can then activate evaluation the following way: ```shell # using the
+configuration dora run solver=musicgen/debug solver/musicgen/
+evaluation=objective_eval # specifying each of the fields, e.g. to activate KL
+computation dora run solver=musicgen/debug evaluate.metrics.kld=true ``` See
+[an example evaluation grid](../audiocraft/grids/musicgen/
+musicgen_pretrained_32khz_eval.py). ### Generation stage The generation stage
+allows to generate samples conditionally and/or unconditionally and to perform
+audio continuation (from a prompt). We currently support greedy sampling
+(argmax), sampling from softmax with a given temperature, top-K and top-P
+(nucleus) sampling. The number of samples generated and the batch size used are
+controlled by the `dataset.generate` configuration while the other generation
+parameters are defined in `generate.lm`. ```shell # control sampling parameters
+dora run solver=musicgen/debug generate.lm.gen_duration=10
+generate.lm.use_sampling=true generate.lm.top_k=15 ``` #### Listening to
+samples Note that generation happens automatically every 25 epochs. You can
+easily access and compare samples between models (as long as they are trained)
+on the same dataset using the MOS tool. For that first `pip install Flask
+gunicorn`. Then ``` gunicorn -w 4 -b 127.0.0.1:8895 -t 120 'scripts.mos:app' --
+access-logfile - ``` And access the tool at [https://127.0.0.1:8895](https://
+127.0.0.1:8895). ### Playing with the model Once you have launched some
+experiments, you can easily get access to the Solver with the latest trained
+model using the following snippet. ```python from audiocraft.solvers.musicgen
+import MusicGenSolver solver = MusicGenSolver.get_eval_solver_from_sig('SIG',
+device='cpu', batch_size=8) solver.model solver.dataloaders ``` ### Importing /
+Exporting models We do not support currently loading a model from the Hugging
+Face implementation or exporting to it. If you want to export your model in a
+way that is compatible with `audiocraft.models.MusicGen` API, you can run:
+```python from audiocraft.utils import export from audiocraft import train xp =
 train.main.get_xp_from_sig('SIG_OF_LM') export.export_lm(xp.folder /
 'checkpoint.th', '/checkpoints/my_audio_lm/state_dict.bin') # You also need to
 bundle the EnCodec model you used !! ## Case 1) you trained your own xp_encodec
 = train.main.get_xp_from_sig('SIG_OF_ENCODEC') export.export_encodec
 (xp_encodec.folder / 'checkpoint.th', '/checkpoints/my_audio_lm/
 compression_state_dict.bin') ## Case 2) you used a pretrained model. Give the
 name you used without the //pretrained/ prefix. ## This will actually not dump
@@ -201,14 +238,15 @@
 [@FurkanGozukara tutorial](https://github.com/FurkanGozukara/Stable-Diffusion/
 blob/main/Tutorials/AI-Music-Generation-Audiocraft-Tutorial.md#more-info-about-
 top-k-top-p-temperature-and-classifier-free-guidance-from-chatgpt). #### Should
 I use FSDP or autocast ? The two are mutually exclusive (because FSDP does
 autocast on its own). You can use autocast up to 1.5B (medium), if you have
 enough RAM on your GPU. FSDP makes everything more complex but will free up
 some memory for the actual activations by sharding the optimizer state. ##
-Citation ``` @article{copet2023simple, title={Simple and Controllable Music
-Generation}, author={Jade Copet and Felix Kreuk and Itai Gat and Tal Remez and
-David Kant and Gabriel Synnaeve and Yossi Adi and Alexandre DÃ©fossez}, year=
-{2023}, journal={arXiv preprint arXiv:2306.05284}, } ``` ## License See license
-information in the [model card](../model_cards/MUSICGEN_MODEL_CARD.md).
-[arxiv]: https://arxiv.org/abs/2306.05284 [musicgen_samples]: https://
-ai.honu.io/papers/musicgen/
+Citation ``` @inproceedings{copet2023simple, title={Simple and Controllable
+Music Generation}, author={Jade Copet and Felix Kreuk and Itai Gat and Tal
+Remez and David Kant and Gabriel Synnaeve and Yossi Adi and Alexandre
+DÃ©fossez}, booktitle={Thirty-seventh Conference on Neural Information
+Processing Systems}, year={2023}, } ``` ## License See license information in
+the [model card](../model_cards/MUSICGEN_MODEL_CARD.md). [arxiv]: https://
+arxiv.org/abs/2306.05284 [musicgen_samples]: https://ai.honu.io/papers/
+musicgen/
```

### Comparing `audiocraft-1.1.0/docs/TRAINING.md` & `audiocraft-1.2.0/docs/TRAINING.md`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 and [Dora](https://github.com/facebookresearch/dora) as our experiment manager.
 AudioCraft training pipelines are designed to be research and experiment-friendly.
 
 
 ## Environment setup
 
 For the base installation, follow the instructions from the [README.md](../README.md).
-Below are some additional instructions for setting up environment to train new models.
+Below are some additional instructions for setting up the environment to train new models.
 
 ### Team and cluster configuration
 
 In order to support multiple teams and clusters, AudioCraft uses an environment configuration.
 The team configuration allows to specify cluster-specific configurations (e.g. SLURM configuration),
 or convenient mapping of paths between the supported environments.
 
@@ -43,15 +43,15 @@
 
 **Important:** The default output dir for trained models and checkpoints is under `/tmp/`. This is suitable
 only for quick testing. If you are doing anything serious you MUST edit the file `default.yaml` and
 properly set the `dora_dir` entries.
 
 #### Overriding environment configurations
 
-You can set the following environmet variables to bypass the team's environment configuration:
+You can set the following environment variables to bypass the team's environment configuration:
 * `AUDIOCRAFT_CONFIG`: absolute path to a team config yaml file.
 * `AUDIOCRAFT_DORA_DIR`: absolute path to a custom dora directory.
 * `AUDIOCRAFT_REFERENCE_DIR`: absolute path to the shared reference directory.
 
 ## Training pipelines
 
 Each task supported in AudioCraft has its own training pipeline and dedicated solver.
@@ -195,15 +195,15 @@
 and compose configurations. Updating the root default configuration files will then have
 an impact on all solvers and tasks.
 **One should never change the default configuration files. Instead they should use Hydra config groups in order to store custom configuration.**
 Once this configuration is created and used for running experiments, you should not edit it anymore.
 
 Note that as we are using Dora as our experiment manager, all our experiment tracking is based on
 signatures computed from delta between configurations.
-**One must therefore ensure backward compatibilty of the configuration at all time.**
+**One must therefore ensure backward compatibility of the configuration at all time.**
 See [Dora's README](https://github.com/facebookresearch/dora) and the
 [section below introduction Dora](#running-experiments-with-dora).
 
 ##### Configuration structure
 
 The configuration is organized in config groups:
 * `conditioner`: default values for conditioning modules.
@@ -251,15 +251,15 @@
 [Dora](https://github.com/facebookresearch/dora) is the experiment manager tool used in AudioCraft.
 Check out the README to learn how Dora works. Here is a quick summary of what to know:
 * An XP is a unique set of hyper-parameters with a given signature. The signature is a hash
 of those hyper-parameters. We always refer to an XP with its signature, e.g. 9357e12e. We will see
 after that one can retrieve the hyper-params and re-rerun it in a single command.
 * In fact, the hash is defined as a delta between the base config and the one obtained
 with the config overrides you passed from the command line. This means you must never change
-the `conf/**.yaml` files directly., except for editing things like paths. Changing the default values
+the `conf/**.yaml` files directly, except for editing things like paths. Changing the default values
 in the config files means the XP signature won't reflect that change, and wrong checkpoints might be reused.
 I know, this is annoying, but the reason is that otherwise, any change to the config file would mean
 that all XPs ran so far would see their signature change.
 
 #### Dora commands
 
 ```shell
@@ -272,31 +272,31 @@
 
 dora run -d -f 81de367c dataset.batch_size=32  # start from the config of XP 81de367c but change some hyper-params.
                                                # This will give you a new XP with a new signature (e.g. 3fe9c332).
 
 dora info -f SIG -t    # will tail the log (if the XP has scheduled).
 # if you need to access the logs of the process for rank > 0, in particular because a crash didn't happen in the main
 # process, then use `dora info -f SIG` to get the main log name (finished into something like `/5037674_0_0_log.out`)
-# and worker K can accessed as `/5037674_0_{K}_log.out`.
+# and worker K can be accessed as `/5037674_0_{K}_log.out`.
 # This is only for scheduled jobs, for local distributed runs with `-d`, then you should go into the XP folder,
 # and look for `worker_{K}.log` logs.
 ```
 
 An XP runs from a specific folder based on its signature, under the
 `<cluster_specific_path>/<user>/experiments/audiocraft/outputs/` folder.
 You can safely interrupt a training and resume it, it will reuse any existing checkpoint,
 as it will reuse the same folder. If you made some change to the code and need to ignore
 a previous checkpoint you can use `dora run --clear [RUN ARGS]`.
 
 If you have a Slurm cluster, you can also use the dora grid command, e.g.
 
 ```shell
-# run a dummy grid located at `audiocraft/grids/my_grid_folder/my_grid_name.py`
+# Run a dummy grid located at `audiocraft/grids/my_grid_folder/my_grid_name.py`
 dora grid my_grid_folder.my_grid_name
-# Run the following will simply display the grid and also initialized the Dora experiments database.
+# The following will simply display the grid and also initialize the Dora experiments database.
 # You can then simply refer to a config using its signature (e.g. as `dora run -f SIG`).
 dora grid my_grid_folder.my_grid_name --dry_run --init
 ```
 
 Please refer to the [Dora documentation](https://github.com/facebookresearch/dora) for more information.
```

### Comparing `audiocraft-1.1.0/model_cards/AUDIOGEN_MODEL_CARD.md` & `audiocraft-1.2.0/model_cards/AUDIOGEN_MODEL_CARD.md`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/model_cards/MUSICGEN_MODEL_CARD.md` & `audiocraft-1.2.0/model_cards/MUSICGEN_MODEL_CARD.md`

 * *Files 11% similar despite different names*

```diff
@@ -83,8 +83,23 @@
 
 **Biases:** The source of data is potentially lacking diversity and all music cultures are not equally represented in the dataset. The model may not perform equally well on the wide variety of music genres that exists. The generated samples from the model will reflect the biases from the training data. Further work on this model should include methods for balanced and just representations of cultures, for example, by scaling the training data to be both diverse and inclusive.
 
 **Risks and harms:** Biases and limitations of the model may lead to generation of samples that may be considered as biased, inappropriate or offensive. We believe that providing the code to reproduce the research and train new models will allow to broaden the application to new and more representative data.
 
 **Use cases:** Users must be aware of the biases, limitations and risks of the model. MusicGen is a model developed for artificial intelligence research on controllable music generation. As such, it should not be used for downstream applications without further investigation and mitigation of risks.
 
+## Update: stereo models and large melody.
+
+We further release a set of stereophonic capable models. Those were fine tuned for 200k updates starting
+from the mono models. The training data is otherwise identical and capabilities and limitations are shared with the base modes. The stereo models work by getting 2 streams of tokens from the EnCodec model, and interleaving those using
+the delay pattern. We also release a mono large model with melody conditioning capabilities. The list of new models
+is as follow:
+
+- facebook/musicgen-stereo-small
+- facebook/musicgen-stereo-medium
+- facebook/musicgen-stereo-large
+- facebook/musicgen-stereo-melody
+- facebook/musicgen-melody-large
+- facebook/musicgen-stereo-melody-large
+
+
 [arxiv]: https://arxiv.org/abs/2306.05284
```

### Comparing `audiocraft-1.1.0/scripts/mos.py` & `audiocraft-1.2.0/scripts/mos.py`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/scripts/resample_dataset.py` & `audiocraft-1.2.0/scripts/resample_dataset.py`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/setup.py` & `audiocraft-1.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/tests/adversarial/test_discriminators.py` & `audiocraft-1.2.0/tests/adversarial/test_discriminators.py`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/tests/adversarial/test_losses.py` & `audiocraft-1.2.0/tests/adversarial/test_losses.py`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/tests/common_utils/temp_utils.py` & `audiocraft-1.2.0/tests/common_utils/temp_utils.py`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/tests/common_utils/wav_utils.py` & `audiocraft-1.2.0/tests/common_utils/wav_utils.py`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/tests/data/test_audio.py` & `audiocraft-1.2.0/tests/data/test_audio.py`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/tests/data/test_audio_dataset.py` & `audiocraft-1.2.0/tests/data/test_audio_dataset.py`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/tests/data/test_audio_utils.py` & `audiocraft-1.2.0/tests/data/test_audio_utils.py`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/tests/losses/test_losses.py` & `audiocraft-1.2.0/tests/losses/test_losses.py`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/tests/modules/test_activations.py` & `audiocraft-1.2.0/tests/modules/test_activations.py`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/tests/modules/test_codebooks_patterns.py` & `audiocraft-1.2.0/tests/modules/test_codebooks_patterns.py`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/tests/modules/test_conv.py` & `audiocraft-1.2.0/tests/modules/test_conv.py`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/tests/modules/test_lstm.py` & `audiocraft-1.2.0/tests/modules/test_lstm.py`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/tests/modules/test_rope.py` & `audiocraft-1.2.0/tests/modules/test_rope.py`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/tests/modules/test_seanet.py` & `audiocraft-1.2.0/tests/modules/test_seanet.py`

 * *Files identical despite different names*

### Comparing `audiocraft-1.1.0/tests/modules/test_transformer.py` & `audiocraft-1.2.0/tests/modules/test_transformer.py`

 * *Files identical despite different names*

