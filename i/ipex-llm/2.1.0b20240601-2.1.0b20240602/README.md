# Comparing `tmp/ipex_llm-2.1.0b20240601-py3-none-win_amd64.whl.zip` & `tmp/ipex_llm-2.1.0b20240602-py3-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 3928702 bytes, number of entries: 195
+Zip file size: 3928720 bytes, number of entries: 195
 -rw-------  2.0 unx     1898 b- defN 24-Mar-25 11:36 ipex_llm/__init__.py
 -rw-------  2.0 unx     6816 b- defN 24-Mar-25 11:36 ipex_llm/convert_model.py
 -rw-------  2.0 unx     3232 b- defN 24-May-07 15:07 ipex_llm/llm_patching.py
 -rw-------  2.0 unx     1063 b- defN 24-May-31 15:04 ipex_llm/models.py
 -rw-------  2.0 unx    12466 b- defN 24-May-24 15:08 ipex_llm/optimize.py
 -rw-------  2.0 unx     2769 b- defN 24-Mar-25 11:36 ipex_llm/cli/llm-chat.ps1
 -rwx------  2.0 unx     3009 b- defN 24-Mar-25 11:36 ipex_llm/cli/llm-cli.ps1
@@ -37,43 +37,43 @@
 -rw-------  2.0 unx     7225 b- defN 24-Mar-25 11:36 ipex_llm/langchain/embeddings/transformersembeddings.py
 -rw-------  2.0 unx     1588 b- defN 24-May-31 15:04 ipex_llm/langchain/llms/__init__.py
 -rw-------  2.0 unx    24235 b- defN 24-May-31 15:04 ipex_llm/langchain/llms/bigdlllm.py
 -rw-------  2.0 unx    10576 b- defN 24-Apr-03 15:07 ipex_llm/langchain/llms/transformersllm.py
 -rw-------  2.0 unx     7379 b- defN 24-Mar-25 11:36 ipex_llm/langchain/llms/transformerspipelinellm.py
 -rw-------  2.0 unx      874 b- defN 24-May-24 15:08 ipex_llm/langchain/vllm/__init__.py
 -rw-------  2.0 unx     7793 b- defN 24-May-24 15:08 ipex_llm/langchain/vllm/vllm.py
--rw-------  2.0 unx        0 b- defN 24-Jun-01 15:05 ipex_llm/libs/__init__.py
--rw-------  2.0 unx    36352 b- defN 24-Jun-01 15:05 ipex_llm/libs/bloom-api.dll
--rw-------  2.0 unx   473088 b- defN 24-Jun-01 15:05 ipex_llm/libs/bloom.dll
--rw-------  2.0 unx    24576 b- defN 24-Jun-01 15:05 ipex_llm/libs/gptneox-api.dll
--rw-------  2.0 unx   532992 b- defN 24-Jun-01 15:05 ipex_llm/libs/gptneox.dll
--rw-------  2.0 unx   499712 b- defN 24-Jun-01 15:05 ipex_llm/libs/libbloom_avx.dll
--rw-------  2.0 unx   473600 b- defN 24-Jun-01 15:05 ipex_llm/libs/libbloom_vnni.dll
--rw-------  2.0 unx   559616 b- defN 24-Jun-01 15:05 ipex_llm/libs/libgptneox_avx.dll
--rw-------  2.0 unx   533504 b- defN 24-Jun-01 15:05 ipex_llm/libs/libgptneox_vnni.dll
--rw-------  2.0 unx   553472 b- defN 24-Jun-01 15:05 ipex_llm/libs/libllama_avx.dll
--rw-------  2.0 unx   527360 b- defN 24-Jun-01 15:05 ipex_llm/libs/libllama_vnni.dll
--rw-------  2.0 unx   590848 b- defN 24-Jun-01 15:05 ipex_llm/libs/libstarcoder_avx.dll
--rw-------  2.0 unx   564736 b- defN 24-Jun-01 15:05 ipex_llm/libs/libstarcoder_vnni.dll
--rw-------  2.0 unx    25088 b- defN 24-Jun-01 15:05 ipex_llm/libs/llama-api.dll
--rw-------  2.0 unx   527360 b- defN 24-Jun-01 15:05 ipex_llm/libs/llama.dll
--rw-------  2.0 unx   103424 b- defN 24-Jun-01 15:05 ipex_llm/libs/main-bloom.exe
--rw-------  2.0 unx    98816 b- defN 24-Jun-01 15:05 ipex_llm/libs/main-gptneox.exe
--rw-------  2.0 unx    99840 b- defN 24-Jun-01 15:05 ipex_llm/libs/main-llama.exe
--rw-------  2.0 unx   157696 b- defN 24-Jun-01 15:05 ipex_llm/libs/main-starcoder.exe
--rw-------  2.0 unx   126464 b- defN 24-Jun-01 15:05 ipex_llm/libs/quantize-bloom.exe
--rw-------  2.0 unx   127488 b- defN 24-Jun-01 15:05 ipex_llm/libs/quantize-bloom_vnni.exe
--rw-------  2.0 unx   103936 b- defN 24-Jun-01 15:05 ipex_llm/libs/quantize-gptneox.exe
--rw-------  2.0 unx   104448 b- defN 24-Jun-01 15:05 ipex_llm/libs/quantize-gptneox_vnni.exe
--rw-------  2.0 unx   109056 b- defN 24-Jun-01 15:05 ipex_llm/libs/quantize-llama.exe
--rw-------  2.0 unx   110080 b- defN 24-Jun-01 15:05 ipex_llm/libs/quantize-llama_vnni.exe
--rw-------  2.0 unx   126976 b- defN 24-Jun-01 15:05 ipex_llm/libs/quantize-starcoder.exe
--rw-------  2.0 unx   128512 b- defN 24-Jun-01 15:05 ipex_llm/libs/quantize-starcoder_vnni.exe
--rw-------  2.0 unx    21504 b- defN 24-Jun-01 15:05 ipex_llm/libs/starcoder-api.dll
--rw-------  2.0 unx   564224 b- defN 24-Jun-01 15:05 ipex_llm/libs/starcoder.dll
+-rw-------  2.0 unx        0 b- defN 24-Jun-02 15:05 ipex_llm/libs/__init__.py
+-rw-------  2.0 unx    36352 b- defN 24-Jun-02 15:05 ipex_llm/libs/bloom-api.dll
+-rw-------  2.0 unx   473088 b- defN 24-Jun-02 15:05 ipex_llm/libs/bloom.dll
+-rw-------  2.0 unx    24576 b- defN 24-Jun-02 15:05 ipex_llm/libs/gptneox-api.dll
+-rw-------  2.0 unx   532992 b- defN 24-Jun-02 15:05 ipex_llm/libs/gptneox.dll
+-rw-------  2.0 unx   499712 b- defN 24-Jun-02 15:05 ipex_llm/libs/libbloom_avx.dll
+-rw-------  2.0 unx   473600 b- defN 24-Jun-02 15:05 ipex_llm/libs/libbloom_vnni.dll
+-rw-------  2.0 unx   559616 b- defN 24-Jun-02 15:05 ipex_llm/libs/libgptneox_avx.dll
+-rw-------  2.0 unx   533504 b- defN 24-Jun-02 15:05 ipex_llm/libs/libgptneox_vnni.dll
+-rw-------  2.0 unx   553472 b- defN 24-Jun-02 15:05 ipex_llm/libs/libllama_avx.dll
+-rw-------  2.0 unx   527360 b- defN 24-Jun-02 15:05 ipex_llm/libs/libllama_vnni.dll
+-rw-------  2.0 unx   590848 b- defN 24-Jun-02 15:05 ipex_llm/libs/libstarcoder_avx.dll
+-rw-------  2.0 unx   564736 b- defN 24-Jun-02 15:05 ipex_llm/libs/libstarcoder_vnni.dll
+-rw-------  2.0 unx    25088 b- defN 24-Jun-02 15:05 ipex_llm/libs/llama-api.dll
+-rw-------  2.0 unx   527360 b- defN 24-Jun-02 15:05 ipex_llm/libs/llama.dll
+-rw-------  2.0 unx   103424 b- defN 24-Jun-02 15:05 ipex_llm/libs/main-bloom.exe
+-rw-------  2.0 unx    98816 b- defN 24-Jun-02 15:05 ipex_llm/libs/main-gptneox.exe
+-rw-------  2.0 unx    99840 b- defN 24-Jun-02 15:05 ipex_llm/libs/main-llama.exe
+-rw-------  2.0 unx   157696 b- defN 24-Jun-02 15:05 ipex_llm/libs/main-starcoder.exe
+-rw-------  2.0 unx   126464 b- defN 24-Jun-02 15:05 ipex_llm/libs/quantize-bloom.exe
+-rw-------  2.0 unx   127488 b- defN 24-Jun-02 15:05 ipex_llm/libs/quantize-bloom_vnni.exe
+-rw-------  2.0 unx   103936 b- defN 24-Jun-02 15:05 ipex_llm/libs/quantize-gptneox.exe
+-rw-------  2.0 unx   104448 b- defN 24-Jun-02 15:05 ipex_llm/libs/quantize-gptneox_vnni.exe
+-rw-------  2.0 unx   109056 b- defN 24-Jun-02 15:05 ipex_llm/libs/quantize-llama.exe
+-rw-------  2.0 unx   110080 b- defN 24-Jun-02 15:05 ipex_llm/libs/quantize-llama_vnni.exe
+-rw-------  2.0 unx   126976 b- defN 24-Jun-02 15:05 ipex_llm/libs/quantize-starcoder.exe
+-rw-------  2.0 unx   128512 b- defN 24-Jun-02 15:05 ipex_llm/libs/quantize-starcoder_vnni.exe
+-rw-------  2.0 unx    21504 b- defN 24-Jun-02 15:05 ipex_llm/libs/starcoder-api.dll
+-rw-------  2.0 unx   564224 b- defN 24-Jun-02 15:05 ipex_llm/libs/starcoder.dll
 -rw-------  2.0 unx      874 b- defN 24-Mar-25 11:36 ipex_llm/llamaindex/__init__.py
 -rw-------  2.0 unx     1139 b- defN 24-Apr-07 15:05 ipex_llm/llamaindex/llms/__init__.py
 -rw-------  2.0 unx    26314 b- defN 24-Apr-07 15:05 ipex_llm/llamaindex/llms/bigdlllm.py
 -rw-------  2.0 unx      586 b- defN 24-Mar-25 11:36 ipex_llm/serving/__init__.py
 -rw-------  2.0 unx      586 b- defN 24-Mar-25 11:36 ipex_llm/serving/fastchat/__init__.py
 -rw-------  2.0 unx    10084 b- defN 24-Mar-25 11:36 ipex_llm/serving/fastchat/bigdl_llm_model.py
 -rw-------  2.0 unx    19605 b- defN 24-May-20 15:06 ipex_llm/serving/fastchat/ipex_llm_worker.py
@@ -182,16 +182,16 @@
 -rw-------  2.0 unx     6944 b- defN 24-May-24 15:08 ipex_llm/vllm/cpu/entrypoints/openai/api_server.py
 -rw-------  2.0 unx      585 b- defN 24-May-24 15:08 ipex_llm/vllm/xpu/__init__.py
 -rw-------  2.0 unx    18506 b- defN 24-May-24 15:08 ipex_llm/vllm/xpu/ipex_llm_gpu_executor.py
 -rw-------  2.0 unx     7172 b- defN 24-May-24 15:08 ipex_llm/vllm/xpu/model_convert.py
 -rw-------  2.0 unx      747 b- defN 24-May-24 15:08 ipex_llm/vllm/xpu/engine/__init__.py
 -rw-------  2.0 unx     5953 b- defN 24-May-24 15:08 ipex_llm/vllm/xpu/engine/engine.py
 -rw-------  2.0 unx    10568 b- defN 24-May-24 15:08 ipex_llm/vllm/xpu/entrypoints/openai/api_server.py
--rwxr-xr-x  2.0 unx     2578 b- defN 24-May-24 15:08 ipex_llm-2.1.0b20240601.data/scripts/ipex-llm-init.bat
--rwxr-xr-x  2.0 unx     2769 b- defN 24-Mar-25 11:36 ipex_llm-2.1.0b20240601.data/scripts/llm-chat.ps1
--rwxr-xr-x  2.0 unx     3009 b- defN 24-Mar-25 11:36 ipex_llm-2.1.0b20240601.data/scripts/llm-cli.ps1
--rw-------  2.0 unx     5495 b- defN 24-Jun-01 15:05 ipex_llm-2.1.0b20240601.dist-info/METADATA
--rw-------  2.0 unx       98 b- defN 24-Jun-01 15:05 ipex_llm-2.1.0b20240601.dist-info/WHEEL
--rw-------  2.0 unx       61 b- defN 24-Jun-01 15:05 ipex_llm-2.1.0b20240601.dist-info/entry_points.txt
--rw-------  2.0 unx        9 b- defN 24-Jun-01 15:05 ipex_llm-2.1.0b20240601.dist-info/top_level.txt
--rw-rw-r--  2.0 unx    18478 b- defN 24-Jun-01 15:05 ipex_llm-2.1.0b20240601.dist-info/RECORD
-195 files, 10054173 bytes uncompressed, 3899168 bytes compressed:  61.2%
+-rwxr-xr-x  2.0 unx     2578 b- defN 24-May-24 15:08 ipex_llm-2.1.0b20240602.data/scripts/ipex-llm-init.bat
+-rwxr-xr-x  2.0 unx     2769 b- defN 24-Mar-25 11:36 ipex_llm-2.1.0b20240602.data/scripts/llm-chat.ps1
+-rwxr-xr-x  2.0 unx     3009 b- defN 24-Mar-25 11:36 ipex_llm-2.1.0b20240602.data/scripts/llm-cli.ps1
+-rw-------  2.0 unx     5495 b- defN 24-Jun-02 15:05 ipex_llm-2.1.0b20240602.dist-info/METADATA
+-rw-------  2.0 unx       98 b- defN 24-Jun-02 15:05 ipex_llm-2.1.0b20240602.dist-info/WHEEL
+-rw-------  2.0 unx       61 b- defN 24-Jun-02 15:05 ipex_llm-2.1.0b20240602.dist-info/entry_points.txt
+-rw-------  2.0 unx        9 b- defN 24-Jun-02 15:05 ipex_llm-2.1.0b20240602.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx    18478 b- defN 24-Jun-02 15:05 ipex_llm-2.1.0b20240602.dist-info/RECORD
+195 files, 10054173 bytes uncompressed, 3899186 bytes compressed:  61.2%
```

## zipnote {}

```diff
@@ -555,32 +555,32 @@
 
 Filename: ipex_llm/vllm/xpu/engine/engine.py
 Comment: 
 
 Filename: ipex_llm/vllm/xpu/entrypoints/openai/api_server.py
 Comment: 
 
-Filename: ipex_llm-2.1.0b20240601.data/scripts/ipex-llm-init.bat
+Filename: ipex_llm-2.1.0b20240602.data/scripts/ipex-llm-init.bat
 Comment: 
 
-Filename: ipex_llm-2.1.0b20240601.data/scripts/llm-chat.ps1
+Filename: ipex_llm-2.1.0b20240602.data/scripts/llm-chat.ps1
 Comment: 
 
-Filename: ipex_llm-2.1.0b20240601.data/scripts/llm-cli.ps1
+Filename: ipex_llm-2.1.0b20240602.data/scripts/llm-cli.ps1
 Comment: 
 
-Filename: ipex_llm-2.1.0b20240601.dist-info/METADATA
+Filename: ipex_llm-2.1.0b20240602.dist-info/METADATA
 Comment: 
 
-Filename: ipex_llm-2.1.0b20240601.dist-info/WHEEL
+Filename: ipex_llm-2.1.0b20240602.dist-info/WHEEL
 Comment: 
 
-Filename: ipex_llm-2.1.0b20240601.dist-info/entry_points.txt
+Filename: ipex_llm-2.1.0b20240602.dist-info/entry_points.txt
 Comment: 
 
-Filename: ipex_llm-2.1.0b20240601.dist-info/top_level.txt
+Filename: ipex_llm-2.1.0b20240602.dist-info/top_level.txt
 Comment: 
 
-Filename: ipex_llm-2.1.0b20240601.dist-info/RECORD
+Filename: ipex_llm-2.1.0b20240602.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ipex_llm/libs/bloom-api.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x00000001800036cc
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Sat Jun  1 15:02:42 2024
+Time/Date		Sun Jun  2 15:02:41 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000003200
 SizeOfInitializedData	0000000000005e00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000000036cc
@@ -6375,19 +6375,18 @@
    180005621:	push   %rdx
    180005622:	add    %al,0x1(%rax)
    180005628:	pop    %rax
    180005629:	push   %rdx
    18000562a:	add    %al,0x1(%rax)
    180005630:	add    %al,(%rax)
    180005632:	add    %al,(%rax)
-   180005634:	adc    (%rax),%bh
-   180005636:	pop    %rbx
-   180005637:	data16 add %al,(%rax)
-   18000563a:	add    %al,(%rax)
-   18000563c:	or     $0xe0000000,%eax
+   180005634:	xchg   %eax,%ecx
+   180005635:	mov    %ebx,0x0(%rsi,%riz,2)
+   180005639:	add    %al,(%rax)
+   18000563b:	add    %cl,-0x20000000(%rip)        # 0x160005641
    180005641:	add    (%rax),%al
    180005643:	add    %cl,(%rcx,%rbx,2)
    180005646:	add    %al,(%rax)
    180005648:	or     $0x3f,%al
 	...
    18000567e:	add    %al,(%rax)
    180005680:	add    %eax,(%rax)
```

## ipex_llm/libs/bloom.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180055a28
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Sat Jun  1 15:02:42 2024
+Time/Date		Sun Jun  2 15:02:41 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000056000
 SizeOfInitializedData	00000000000bf400
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000055a28
@@ -112439,19 +112439,17 @@
    18005e83a:	add    $0x180,%eax
    18005e83f:	add    %dh,0x76(%rax)
    18005e842:	add    $0x180,%eax
    18005e847:	add    %bh,0x76(%rax)
    18005e84a:	add    $0x180,%eax
    18005e84f:	add    %al,(%rax)
    18005e851:	add    %al,(%rax)
-   18005e853:	add    %dl,(%rdx)
-   18005e855:	cmp    %bl,0x66(%rbx)
-   18005e858:	add    %al,(%rax)
-   18005e85a:	add    %al,(%rax)
-   18005e85c:	or     $0x50000000,%eax
+   18005e853:	add    %dl,0x665c89(%rcx)
+   18005e859:	add    %al,(%rax)
+   18005e85b:	add    %cl,0x50000000(%rip)        # 0x1d005e861
    18005e861:	add    (%rax),%eax
    18005e863:	add    %ah,(%rax)
    18005e865:	repnz add $0x5e62000,%eax
 	...
    18005e87f:	add    %dl,0x18005f5(%rax)
    18005e885:	add    %al,(%rax)
    18005e887:	add    %bl,0x18005f5(%rax)
```

## ipex_llm/libs/gptneox-api.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180002cbc
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Sat Jun  1 15:02:42 2024
+Time/Date		Sun Jun  2 15:02:41 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000002600
 SizeOfInitializedData	0000000000003e00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000002cbc
@@ -5058,19 +5058,18 @@
    1800049c0:	cmp    %al,0x0(%rdx)
    1800049c3:	addb   $0x0,(%rcx)
    1800049c6:	add    %al,(%rax)
    1800049c8:	rex
    1800049c9:	rex.X add %al,0x1(%rax)
    1800049d0:	add    %al,(%rax)
    1800049d2:	add    %al,(%rax)
-   1800049d4:	adc    (%rax),%bh
-   1800049d6:	pop    %rbx
-   1800049d7:	data16 add %al,(%rax)
-   1800049da:	add    %al,(%rax)
-   1800049dc:	or     $0xe0000000,%eax
+   1800049d4:	xchg   %eax,%ecx
+   1800049d5:	mov    %ebx,0x0(%rsi,%riz,2)
+   1800049d9:	add    %al,(%rax)
+   1800049db:	add    %cl,-0x20000000(%rip)        # 0x1600049e1
    1800049e1:	add    (%rax),%al
    1800049e3:	add    %ah,0x0(%rsp,%rcx,2)
    1800049e7:	add    %ah,0x0(%rsi,%rsi,1)
 	...
    1800049ff:	add    %al,(%rcx)
 	...
    180004a09:	add    %al,(%rax)
```

## ipex_llm/libs/gptneox.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x000000018005d188
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Sat Jun  1 15:02:43 2024
+Time/Date		Sun Jun  2 15:02:42 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		000000000005da00
 SizeOfInitializedData	00000000000c6600
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000005d188
@@ -123761,19 +123761,18 @@
    1800660fd:	add    %al,(%rax)
    1800660ff:	add    %bh,0x18005f6(%rax)
    180066105:	add    %al,(%rax)
    180066107:	add    %al,%al
    180066109:	testb  $0x0,0x180(%rip)        # 0x180066290
    180066110:	add    %al,(%rax)
    180066112:	add    %al,(%rax)
-   180066114:	adc    (%rax),%edi
-   180066116:	pop    %rbx
-   180066117:	data16 add %al,(%rax)
-   18006611a:	add    %al,(%rax)
-   18006611c:	or     $0x50000000,%eax
+   180066114:	xchg   %eax,%edx
+   180066115:	mov    %ebx,0x0(%rsi,%riz,2)
+   180066119:	add    %al,(%rax)
+   18006611b:	add    %cl,0x50000000(%rip)        # 0x1d0066121
    180066121:	add    (%rax),%eax
    180066123:	add    %al,0x5b840006(%rbp,%rbp,2)
    18006612a:	(bad)
 	...
    18006617f:	add    %bh,%al
    180066181:	jo     0x180066189
    180066183:	addb   $0x0,(%rcx)
```

## ipex_llm/libs/libbloom_avx.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x000000018005bcb8
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Sat Jun  1 15:02:57 2024
+Time/Date		Sun Jun  2 15:03:45 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		000000000005c200
 SizeOfInitializedData	00000000000bfa00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000005bcb8
@@ -112468,30 +112468,32 @@
    180061eb9:	jae    0x180061ee8
    180061ebb:	jb     0x180061f32
    180061ebd:	outsb  %ds:(%rsi),(%dx)
    180061ebe:	outsb  %ds:(%rsi),(%dx)
    180061ebf:	gs jb  0x180061f1e
    180061ec2:	(bad)
    180061ec7:	sub    $0x6c697562,%eax
-   180061ecc:	fs sub $0x5c77656e,%eax
-   180061ed2:	pop    %rdi
-   180061ed3:	ja     0x180061f44
-   180061ed5:	jb     0x180061f42
-   180061ed7:	pop    %rsp
-   180061ed8:	imul   $0x6c6c2d78,0x65(%rax),%esi
-   180061edf:	insl   (%dx),%es:(%rdi)
-   180061ee0:	pop    %rsp
-   180061ee1:	imul   $0x6c6c2d78,0x65(%rax),%esi
-   180061ee8:	insl   (%dx),%es:(%rdi)
-   180061ee9:	pop    %rsp
-   180061eea:	jae    0x180061f5e
-   180061eec:	movsxd 0x67(%rdi,%riz,2),%ebx
-   180061ef0:	insl   (%dx),%es:(%rdi)
-   180061ef1:	insb   (%dx),%es:(%rdi)
-   180061ef2:	cs movsxd (%rax),%eax
+   180061ecc:	fs pop %rsp
+   180061ece:	pop    %rdi
+   180061ecf:	ja     0x180061f40
+   180061ed1:	jb     0x180061f3e
+   180061ed3:	pop    %rsp
+   180061ed4:	imul   $0x6c6c2d78,0x65(%rax),%esi
+   180061edb:	insl   (%dx),%es:(%rdi)
+   180061edc:	pop    %rsp
+   180061edd:	imul   $0x6c6c2d78,0x65(%rax),%esi
+   180061ee4:	insl   (%dx),%es:(%rdi)
+   180061ee5:	pop    %rsp
+   180061ee6:	jae    0x180061f5a
+   180061ee8:	movsxd 0x67(%rdi,%riz,2),%ebx
+   180061eec:	insl   (%dx),%es:(%rdi)
+   180061eed:	insb   (%dx),%es:(%rdi)
+   180061eee:	cs movsxd (%rax),%eax
+   180061ef1:	add    %al,(%rax)
+   180061ef3:	add    %al,(%rax)
    180061ef5:	add    %al,(%rax)
    180061ef7:	add    %al,0x47(%rdi)
    180061efa:	rex.WRB
    180061efb:	rex.WR pop %rdi
    180061efd:	push   %r11
    180061eff:	push   %rbx
    180061f00:	rex.RB push %r10
@@ -118004,19 +118006,18 @@
    18006576d:	add    %al,(%rax)
    18006576f:	add    %dh,-0x1a(%rax)
    180065772:	add    $0x180,%eax
    180065777:	add    %bh,-0x1a(%rax)
    18006577a:	add    $0x180,%eax
    18006577f:	add    %al,(%rax)
    180065781:	add    %al,(%rax)
-   180065783:	add    %ah,(%rcx)
-   180065785:	cmp    %bl,0x66(%rbx)
-   180065788:	add    %al,(%rax)
-   18006578a:	add    %al,(%rax)
-   18006578c:	or     $0x50000000,%eax
+   180065783:	add    %dl,%cl
+   180065785:	mov    %ebx,0x0(%rsi,%riz,2)
+   180065789:	add    %al,(%rax)
+   18006578b:	add    %cl,0x50000000(%rip)        # 0x1d0065791
    180065791:	add    (%rax),%eax
    180065793:	add    %ah,-0x5ffff99f(%rax)
    180065799:	rex.RXB (bad)
 	...
    1800657ff:	add    %dl,(%rax)
    180065801:	gs (bad)
    180065803:	addb   $0x0,(%rcx)
```

## ipex_llm/libs/libbloom_vnni.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180055c38
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Sat Jun  1 15:03:45 2024
+Time/Date		Sun Jun  2 15:02:54 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000056200
 SizeOfInitializedData	00000000000bf400
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000055c38
@@ -106894,32 +106894,30 @@
    18005beb9:	jae    0x18005bee8
    18005bebb:	jb     0x18005bf32
    18005bebd:	outsb  %ds:(%rsi),(%dx)
    18005bebe:	outsb  %ds:(%rsi),(%dx)
    18005bebf:	gs jb  0x18005bf1e
    18005bec2:	(bad)
    18005bec7:	sub    $0x6c697562,%eax
-   18005becc:	fs pop %rsp
-   18005bece:	pop    %rdi
-   18005becf:	ja     0x18005bf40
-   18005bed1:	jb     0x18005bf3e
-   18005bed3:	pop    %rsp
-   18005bed4:	imul   $0x6c6c2d78,0x65(%rax),%esi
-   18005bedb:	insl   (%dx),%es:(%rdi)
-   18005bedc:	pop    %rsp
-   18005bedd:	imul   $0x6c6c2d78,0x65(%rax),%esi
-   18005bee4:	insl   (%dx),%es:(%rdi)
-   18005bee5:	pop    %rsp
-   18005bee6:	jae    0x18005bf5a
-   18005bee8:	movsxd 0x67(%rdi,%riz,2),%ebx
-   18005beec:	insl   (%dx),%es:(%rdi)
-   18005beed:	insb   (%dx),%es:(%rdi)
-   18005beee:	cs movsxd (%rax),%eax
-   18005bef1:	add    %al,(%rax)
-   18005bef3:	add    %al,(%rax)
+   18005becc:	fs sub $0x5c77656e,%eax
+   18005bed2:	pop    %rdi
+   18005bed3:	ja     0x18005bf44
+   18005bed5:	jb     0x18005bf42
+   18005bed7:	pop    %rsp
+   18005bed8:	imul   $0x6c6c2d78,0x65(%rax),%esi
+   18005bedf:	insl   (%dx),%es:(%rdi)
+   18005bee0:	pop    %rsp
+   18005bee1:	imul   $0x6c6c2d78,0x65(%rax),%esi
+   18005bee8:	insl   (%dx),%es:(%rdi)
+   18005bee9:	pop    %rsp
+   18005beea:	jae    0x18005bf5e
+   18005beec:	movsxd 0x67(%rdi,%riz,2),%ebx
+   18005bef0:	insl   (%dx),%es:(%rdi)
+   18005bef1:	insb   (%dx),%es:(%rdi)
+   18005bef2:	cs movsxd (%rax),%eax
    18005bef5:	add    %al,(%rax)
    18005bef7:	add    %al,0x47(%rdi)
    18005befa:	rex.WRB
    18005befb:	rex.WR pop %rdi
    18005befd:	push   %r11
    18005beff:	push   %rbx
    18005bf00:	rex.RB push %r10
@@ -112506,19 +112504,17 @@
    18005f81a:	add    $0x180,%eax
    18005f81f:	add    %dh,-0x7a(%rax)
    18005f822:	add    $0x180,%eax
    18005f827:	add    %bh,-0x7a(%rax)
    18005f82a:	add    $0x180,%eax
    18005f82f:	add    %al,(%rax)
    18005f831:	add    %al,(%rax)
-   18005f833:	add    %dl,0x38(%rcx)
-   18005f836:	pop    %rbx
-   18005f837:	data16 add %al,(%rax)
-   18005f83a:	add    %al,(%rax)
-   18005f83c:	or     $0x50000000,%eax
+   18005f833:	add    %bl,0x665c89(%rsi)
+   18005f839:	add    %al,(%rax)
+   18005f83b:	add    %cl,0x50000000(%rip)        # 0x1d005f841
    18005f841:	add    (%rax),%eax
    18005f843:	add    %ah,(%rax)
    18005f845:	add    (%rsi),%al
    18005f847:	add    %ah,(%rax)
    18005f849:	call   0x18005f853
 	...
    18005f87e:	add    %al,(%rax)
```

## ipex_llm/libs/libgptneox_avx.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x00000001800634a8
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Sat Jun  1 15:02:58 2024
+Time/Date		Sun Jun  2 15:03:46 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000063e00
 SizeOfInitializedData	00000000000c6a00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000000634a8
@@ -25409,15 +25409,15 @@
    180007cf0:	xor    %rsp,%rax
    180007cf3:	mov    %rax,0x50(%rsp)
    180007cf8:	mov    %r9,%rbp
    180007cfb:	mov    %r8,%rsi
    180007cfe:	mov    %rdx,%rbx
    180007d01:	mov    %rcx,%rdi
    180007d04:	mov    %rcx,0x28(%rsp)
-   180007d09:	lea    0x5dfa4(%rip),%r8        # 0x180065cb4
+   180007d09:	lea    0x5dfa0(%rip),%r8        # 0x180065cb0
    180007d10:	call   0x180007b70
    180007d15:	nop
    180007d16:	movl   $0xc470,0x14(%rdi)
    180007d1d:	movl   $0x1000,0x18(%rdi)
    180007d24:	movl   $0x1400,0x1c(%rdi)
    180007d2b:	movl   $0x28,0x20(%rdi)
    180007d32:	movl   $0x24,0x24(%rdi)
@@ -42279,15 +42279,15 @@
    1800176e3:	sub    $0x80,%rsp
    1800176ea:	mov    0x6dd97(%rip),%rax        # 0x180085488
    1800176f1:	xor    %rsp,%rax
    1800176f4:	mov    %rax,-0x8(%rbp)
    1800176f8:	mov    0x60(%rbp),%r13
    1800176fc:	mov    %r8,%r12
    1800176ff:	mov    %rcx,%rdi
-   180017702:	lea    0x4e5ab(%rip),%r8        # 0x180065cb4
+   180017702:	lea    0x4e5a7(%rip),%r8        # 0x180065cb0
    180017709:	lea    -0x28(%rbp),%rcx
    18001770d:	mov    %r9,%r15
    180017710:	call   0x180007b70
    180017715:	call   *0x4de0d(%rip)        # 0x180065528
    18001771b:	mov    -0x28(%rbp),%rbx
    18001771f:	lea    -0x50(%rbp),%rcx
    180017723:	xor    %r14d,%r14d
@@ -119470,36 +119470,38 @@
    1800657d9:	jae    0x180065808
    1800657db:	jb     0x180065852
    1800657dd:	outsb  %ds:(%rsi),(%dx)
    1800657de:	outsb  %ds:(%rsi),(%dx)
    1800657df:	gs jb  0x18006583e
    1800657e2:	(bad)
    1800657e7:	sub    $0x6c697562,%eax
-   1800657ec:	fs sub $0x5c77656e,%eax
-   1800657f2:	pop    %rdi
-   1800657f3:	ja     0x180065864
-   1800657f5:	jb     0x180065862
-   1800657f7:	pop    %rsp
-   1800657f8:	imul   $0x6c6c2d78,0x65(%rax),%esi
-   1800657ff:	insl   (%dx),%es:(%rdi)
-   180065800:	pop    %rsp
-   180065801:	imul   $0x6c6c2d78,0x65(%rax),%esi
-   180065808:	insl   (%dx),%es:(%rdi)
-   180065809:	pop    %rsp
-   18006580a:	jae    0x18006587e
-   18006580c:	movsxd 0x70(%rdi,%riz,2),%ebx
-   180065810:	je     0x180065880
-   180065812:	outsl  %gs:(%rsi),(%dx)
-   180065814:	js     0x180065872
-   180065816:	addr32 jo 0x18006588d
-   180065819:	outsb  %ds:(%rsi),(%dx)
-   18006581a:	outsl  %gs:(%rsi),(%dx)
-   18006581c:	js     0x18006584b
-   18006581e:	jne    0x180065894
-   180065820:	imul   $0x0,0x68(%rsi,%rbp,1),%ebp
+   1800657ec:	fs pop %rsp
+   1800657ee:	pop    %rdi
+   1800657ef:	ja     0x180065860
+   1800657f1:	jb     0x18006585e
+   1800657f3:	pop    %rsp
+   1800657f4:	imul   $0x6c6c2d78,0x65(%rax),%esi
+   1800657fb:	insl   (%dx),%es:(%rdi)
+   1800657fc:	pop    %rsp
+   1800657fd:	imul   $0x6c6c2d78,0x65(%rax),%esi
+   180065804:	insl   (%dx),%es:(%rdi)
+   180065805:	pop    %rsp
+   180065806:	jae    0x18006587a
+   180065808:	movsxd 0x70(%rdi,%riz,2),%ebx
+   18006580c:	je     0x18006587c
+   18006580e:	outsl  %gs:(%rsi),(%dx)
+   180065810:	js     0x18006586e
+   180065812:	addr32 jo 0x180065889
+   180065815:	outsb  %ds:(%rsi),(%dx)
+   180065816:	outsl  %gs:(%rsi),(%dx)
+   180065818:	js     0x180065847
+   18006581a:	jne    0x180065890
+   18006581c:	imul   $0x0,0x68(%rsi,%rbp,1),%ebp
+   180065824:	add    %al,(%rax)
+   180065826:	add    %al,(%rax)
    180065828:	rex.RXB push %r8
    18006582a:	push   %rsp
    18006582b:	rex.WRX
    18006582c:	rex.RB
    18006582d:	rex.WRXB pop %r8
    18006582f:	pop    %rdi
    180065830:	push   %r11
@@ -119868,37 +119870,39 @@
    180065c69:	jae    0x180065c98
    180065c6b:	jb     0x180065ce2
    180065c6d:	outsb  %ds:(%rsi),(%dx)
    180065c6e:	outsb  %ds:(%rsi),(%dx)
    180065c6f:	gs jb  0x180065cce
    180065c72:	(bad)
    180065c77:	sub    $0x6c697562,%eax
-   180065c7c:	fs sub $0x5c77656e,%eax
-   180065c82:	pop    %rdi
-   180065c83:	ja     0x180065cf4
-   180065c85:	jb     0x180065cf2
-   180065c87:	pop    %rsp
-   180065c88:	imul   $0x6c6c2d78,0x65(%rax),%esi
-   180065c8f:	insl   (%dx),%es:(%rdi)
-   180065c90:	pop    %rsp
-   180065c91:	imul   $0x6c6c2d78,0x65(%rax),%esi
-   180065c98:	insl   (%dx),%es:(%rdi)
-   180065c99:	pop    %rsp
-   180065c9a:	jae    0x180065d0e
-   180065c9c:	movsxd 0x70(%rdi,%riz,2),%ebx
-   180065ca0:	je     0x180065d10
-   180065ca2:	outsl  %gs:(%rsi),(%dx)
-   180065ca4:	js     0x180065d02
-   180065ca6:	addr32 jo 0x180065d1d
-   180065ca9:	outsb  %ds:(%rsi),(%dx)
-   180065caa:	outsl  %gs:(%rsi),(%dx)
-   180065cac:	js     0x180065cdc
-   180065cae:	movsxd 0x70(%rax),%esi
-   180065cb1:	add    %al,(%rax)
-   180065cb3:	add    %dh,0x62(%rdx)
+   180065c7c:	fs pop %rsp
+   180065c7e:	pop    %rdi
+   180065c7f:	ja     0x180065cf0
+   180065c81:	jb     0x180065cee
+   180065c83:	pop    %rsp
+   180065c84:	imul   $0x6c6c2d78,0x65(%rax),%esi
+   180065c8b:	insl   (%dx),%es:(%rdi)
+   180065c8c:	pop    %rsp
+   180065c8d:	imul   $0x6c6c2d78,0x65(%rax),%esi
+   180065c94:	insl   (%dx),%es:(%rdi)
+   180065c95:	pop    %rsp
+   180065c96:	jae    0x180065d0a
+   180065c98:	movsxd 0x70(%rdi,%riz,2),%ebx
+   180065c9c:	je     0x180065d0c
+   180065c9e:	outsl  %gs:(%rsi),(%dx)
+   180065ca0:	js     0x180065cfe
+   180065ca2:	addr32 jo 0x180065d19
+   180065ca5:	outsb  %ds:(%rsi),(%dx)
+   180065ca6:	outsl  %gs:(%rsi),(%dx)
+   180065ca8:	js     0x180065cd8
+   180065caa:	movsxd 0x70(%rax),%esi
+   180065cad:	add    %al,(%rax)
+   180065caf:	add    %dh,0x62(%rdx)
+   180065cb2:	add    %al,(%rax)
+   180065cb4:	add    %al,(%rax)
    180065cb6:	add    %al,(%rax)
    180065cb8:	(bad)
    180065cbd:	sub    $0x3a6d6c6c,%eax
    180065cc2:	and    %ch,0x61(%rdi,%rbp,2)
    180065cc6:	imul   $0x646f6d20,%fs:0x67(%rsi),%ebp
    180065cce:	gs insb (%dx),%es:(%rdi)
    180065cd0:	and    %ah,0x72(%rsi)
@@ -126244,30 +126248,32 @@
    180069f99:	jae    0x180069fc8
    180069f9b:	jb     0x18006a012
    180069f9d:	outsb  %ds:(%rsi),(%dx)
    180069f9e:	outsb  %ds:(%rsi),(%dx)
    180069f9f:	gs jb  0x180069ffe
    180069fa2:	(bad)
    180069fa7:	sub    $0x6c697562,%eax
-   180069fac:	fs sub $0x5c77656e,%eax
-   180069fb2:	pop    %rdi
-   180069fb3:	ja     0x18006a024
-   180069fb5:	jb     0x18006a022
-   180069fb7:	pop    %rsp
-   180069fb8:	imul   $0x6c6c2d78,0x65(%rax),%esi
-   180069fbf:	insl   (%dx),%es:(%rdi)
-   180069fc0:	pop    %rsp
-   180069fc1:	imul   $0x6c6c2d78,0x65(%rax),%esi
-   180069fc8:	insl   (%dx),%es:(%rdi)
-   180069fc9:	pop    %rsp
-   180069fca:	jae    0x18006a03e
-   180069fcc:	movsxd 0x67(%rdi,%riz,2),%ebx
-   180069fd0:	insl   (%dx),%es:(%rdi)
-   180069fd1:	insb   (%dx),%es:(%rdi)
-   180069fd2:	cs movsxd (%rax),%eax
+   180069fac:	fs pop %rsp
+   180069fae:	pop    %rdi
+   180069faf:	ja     0x18006a020
+   180069fb1:	jb     0x18006a01e
+   180069fb3:	pop    %rsp
+   180069fb4:	imul   $0x6c6c2d78,0x65(%rax),%esi
+   180069fbb:	insl   (%dx),%es:(%rdi)
+   180069fbc:	pop    %rsp
+   180069fbd:	imul   $0x6c6c2d78,0x65(%rax),%esi
+   180069fc4:	insl   (%dx),%es:(%rdi)
+   180069fc5:	pop    %rsp
+   180069fc6:	jae    0x18006a03a
+   180069fc8:	movsxd 0x67(%rdi,%riz,2),%ebx
+   180069fcc:	insl   (%dx),%es:(%rdi)
+   180069fcd:	insb   (%dx),%es:(%rdi)
+   180069fce:	cs movsxd (%rax),%eax
+   180069fd1:	add    %al,(%rax)
+   180069fd3:	add    %al,(%rax)
    180069fd5:	add    %al,(%rax)
    180069fd7:	add    %al,0x47(%rdi)
    180069fda:	rex.WRB
    180069fdb:	rex.WR pop %rdi
    180069fdd:	push   %r11
    180069fdf:	push   %rbx
    180069fe0:	rex.RB push %r10
@@ -129468,17 +129474,15 @@
    18006c037:	add    %al,%al
    18006c039:	push   %rsi
    18006c03a:	(bad)
    18006c03b:	addb   $0x0,(%rcx)
    18006c03e:	add    %al,(%rax)
    18006c040:	add    %al,(%rax)
    18006c042:	add    %al,(%rax)
-   18006c044:	and    (%rax),%bh
-   18006c046:	pop    %rbx
-   18006c047:	data16 add %al,(%rax)
+   18006c044:	rorb   %cl,0x665c(%rcx)
    18006c04a:	add    %al,(%rax)
    18006c04c:	or     $0x50000000,%eax
    18006c051:	add    (%rax),%eax
    18006c053:	add    %al,-0x417bfffa(%rsp,%rcx,8)
    18006c05a:	(bad)
 	...
    18006c07f:	add    %bh,%al
```

## ipex_llm/libs/libgptneox_vnni.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x000000018005d398
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Sat Jun  1 15:03:45 2024
+Time/Date		Sun Jun  2 15:02:55 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		000000000005dc00
 SizeOfInitializedData	00000000000c6600
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000005d398
@@ -25024,15 +25024,15 @@
    180007cf0:	xor    %rsp,%rax
    180007cf3:	mov    %rax,0x50(%rsp)
    180007cf8:	mov    %r9,%rbp
    180007cfb:	mov    %r8,%rsi
    180007cfe:	mov    %rdx,%rbx
    180007d01:	mov    %rcx,%rdi
    180007d04:	mov    %rcx,0x28(%rsp)
-   180007d09:	lea    0x57fa0(%rip),%r8        # 0x18005fcb0
+   180007d09:	lea    0x57fa4(%rip),%r8        # 0x18005fcb4
    180007d10:	call   0x180007b70
    180007d15:	nop
    180007d16:	movl   $0xc470,0x14(%rdi)
    180007d1d:	movl   $0x1000,0x18(%rdi)
    180007d24:	movl   $0x1400,0x1c(%rdi)
    180007d2b:	movl   $0x28,0x20(%rdi)
    180007d32:	movl   $0x24,0x24(%rdi)
@@ -41895,15 +41895,15 @@
    180017743:	sub    $0x80,%rsp
    18001774a:	mov    0x67d37(%rip),%rax        # 0x18007f488
    180017751:	xor    %rsp,%rax
    180017754:	mov    %rax,-0x8(%rbp)
    180017758:	mov    0x60(%rbp),%r13
    18001775c:	mov    %r8,%r12
    18001775f:	mov    %rcx,%rdi
-   180017762:	lea    0x48547(%rip),%r8        # 0x18005fcb0
+   180017762:	lea    0x4854b(%rip),%r8        # 0x18005fcb4
    180017769:	lea    -0x28(%rbp),%rcx
    18001776d:	mov    %r9,%r15
    180017770:	call   0x180007b70
    180017775:	call   *0x47dad(%rip)        # 0x18005f528
    18001777b:	mov    -0x28(%rbp),%rbx
    18001777f:	lea    -0x50(%rbp),%rcx
    180017783:	xor    %r14d,%r14d
@@ -113855,38 +113855,36 @@
    18005f7d9:	jae    0x18005f808
    18005f7db:	jb     0x18005f852
    18005f7dd:	outsb  %ds:(%rsi),(%dx)
    18005f7de:	outsb  %ds:(%rsi),(%dx)
    18005f7df:	gs jb  0x18005f83e
    18005f7e2:	(bad)
    18005f7e7:	sub    $0x6c697562,%eax
-   18005f7ec:	fs pop %rsp
-   18005f7ee:	pop    %rdi
-   18005f7ef:	ja     0x18005f860
-   18005f7f1:	jb     0x18005f85e
-   18005f7f3:	pop    %rsp
-   18005f7f4:	imul   $0x6c6c2d78,0x65(%rax),%esi
-   18005f7fb:	insl   (%dx),%es:(%rdi)
-   18005f7fc:	pop    %rsp
-   18005f7fd:	imul   $0x6c6c2d78,0x65(%rax),%esi
-   18005f804:	insl   (%dx),%es:(%rdi)
-   18005f805:	pop    %rsp
-   18005f806:	jae    0x18005f87a
-   18005f808:	movsxd 0x70(%rdi,%riz,2),%ebx
-   18005f80c:	je     0x18005f87c
-   18005f80e:	outsl  %gs:(%rsi),(%dx)
-   18005f810:	js     0x18005f86e
-   18005f812:	addr32 jo 0x18005f889
-   18005f815:	outsb  %ds:(%rsi),(%dx)
-   18005f816:	outsl  %gs:(%rsi),(%dx)
-   18005f818:	js     0x18005f847
-   18005f81a:	jne    0x18005f890
-   18005f81c:	imul   $0x0,0x68(%rsi,%rbp,1),%ebp
-   18005f824:	add    %al,(%rax)
-   18005f826:	add    %al,(%rax)
+   18005f7ec:	fs sub $0x5c77656e,%eax
+   18005f7f2:	pop    %rdi
+   18005f7f3:	ja     0x18005f864
+   18005f7f5:	jb     0x18005f862
+   18005f7f7:	pop    %rsp
+   18005f7f8:	imul   $0x6c6c2d78,0x65(%rax),%esi
+   18005f7ff:	insl   (%dx),%es:(%rdi)
+   18005f800:	pop    %rsp
+   18005f801:	imul   $0x6c6c2d78,0x65(%rax),%esi
+   18005f808:	insl   (%dx),%es:(%rdi)
+   18005f809:	pop    %rsp
+   18005f80a:	jae    0x18005f87e
+   18005f80c:	movsxd 0x70(%rdi,%riz,2),%ebx
+   18005f810:	je     0x18005f880
+   18005f812:	outsl  %gs:(%rsi),(%dx)
+   18005f814:	js     0x18005f872
+   18005f816:	addr32 jo 0x18005f88d
+   18005f819:	outsb  %ds:(%rsi),(%dx)
+   18005f81a:	outsl  %gs:(%rsi),(%dx)
+   18005f81c:	js     0x18005f84b
+   18005f81e:	jne    0x18005f894
+   18005f820:	imul   $0x0,0x68(%rsi,%rbp,1),%ebp
    18005f828:	rex.RXB push %r8
    18005f82a:	push   %rsp
    18005f82b:	rex.WRX
    18005f82c:	rex.RB
    18005f82d:	rex.WRXB pop %r8
    18005f82f:	pop    %rdi
    18005f830:	push   %r11
@@ -114249,39 +114247,37 @@
    18005fc69:	jae    0x18005fc98
    18005fc6b:	jb     0x18005fce2
    18005fc6d:	outsb  %ds:(%rsi),(%dx)
    18005fc6e:	outsb  %ds:(%rsi),(%dx)
    18005fc6f:	gs jb  0x18005fcce
    18005fc72:	(bad)
    18005fc77:	sub    $0x6c697562,%eax
-   18005fc7c:	fs pop %rsp
-   18005fc7e:	pop    %rdi
-   18005fc7f:	ja     0x18005fcf0
-   18005fc81:	jb     0x18005fcee
-   18005fc83:	pop    %rsp
-   18005fc84:	imul   $0x6c6c2d78,0x65(%rax),%esi
-   18005fc8b:	insl   (%dx),%es:(%rdi)
-   18005fc8c:	pop    %rsp
-   18005fc8d:	imul   $0x6c6c2d78,0x65(%rax),%esi
-   18005fc94:	insl   (%dx),%es:(%rdi)
-   18005fc95:	pop    %rsp
-   18005fc96:	jae    0x18005fd0a
-   18005fc98:	movsxd 0x70(%rdi,%riz,2),%ebx
-   18005fc9c:	je     0x18005fd0c
-   18005fc9e:	outsl  %gs:(%rsi),(%dx)
-   18005fca0:	js     0x18005fcfe
-   18005fca2:	addr32 jo 0x18005fd19
-   18005fca5:	outsb  %ds:(%rsi),(%dx)
-   18005fca6:	outsl  %gs:(%rsi),(%dx)
-   18005fca8:	js     0x18005fcd8
-   18005fcaa:	movsxd 0x70(%rax),%esi
-   18005fcad:	add    %al,(%rax)
-   18005fcaf:	add    %dh,0x62(%rdx)
-   18005fcb2:	add    %al,(%rax)
-   18005fcb4:	add    %al,(%rax)
+   18005fc7c:	fs sub $0x5c77656e,%eax
+   18005fc82:	pop    %rdi
+   18005fc83:	ja     0x18005fcf4
+   18005fc85:	jb     0x18005fcf2
+   18005fc87:	pop    %rsp
+   18005fc88:	imul   $0x6c6c2d78,0x65(%rax),%esi
+   18005fc8f:	insl   (%dx),%es:(%rdi)
+   18005fc90:	pop    %rsp
+   18005fc91:	imul   $0x6c6c2d78,0x65(%rax),%esi
+   18005fc98:	insl   (%dx),%es:(%rdi)
+   18005fc99:	pop    %rsp
+   18005fc9a:	jae    0x18005fd0e
+   18005fc9c:	movsxd 0x70(%rdi,%riz,2),%ebx
+   18005fca0:	je     0x18005fd10
+   18005fca2:	outsl  %gs:(%rsi),(%dx)
+   18005fca4:	js     0x18005fd02
+   18005fca6:	addr32 jo 0x18005fd1d
+   18005fca9:	outsb  %ds:(%rsi),(%dx)
+   18005fcaa:	outsl  %gs:(%rsi),(%dx)
+   18005fcac:	js     0x18005fcdc
+   18005fcae:	movsxd 0x70(%rax),%esi
+   18005fcb1:	add    %al,(%rax)
+   18005fcb3:	add    %dh,0x62(%rdx)
    18005fcb6:	add    %al,(%rax)
    18005fcb8:	(bad)
    18005fcbd:	sub    $0x3a6d6c6c,%eax
    18005fcc2:	and    %ch,0x61(%rdi,%rbp,2)
    18005fcc6:	imul   $0x646f6d20,%fs:0x67(%rsi),%ebp
    18005fcce:	gs insb (%dx),%es:(%rdi)
    18005fcd0:	and    %ah,0x72(%rsi)
@@ -120623,32 +120619,30 @@
    180063f99:	jae    0x180063fc8
    180063f9b:	jb     0x180064012
    180063f9d:	outsb  %ds:(%rsi),(%dx)
    180063f9e:	outsb  %ds:(%rsi),(%dx)
    180063f9f:	gs jb  0x180063ffe
    180063fa2:	(bad)
    180063fa7:	sub    $0x6c697562,%eax
-   180063fac:	fs pop %rsp
-   180063fae:	pop    %rdi
-   180063faf:	ja     0x180064020
-   180063fb1:	jb     0x18006401e
-   180063fb3:	pop    %rsp
-   180063fb4:	imul   $0x6c6c2d78,0x65(%rax),%esi
-   180063fbb:	insl   (%dx),%es:(%rdi)
-   180063fbc:	pop    %rsp
-   180063fbd:	imul   $0x6c6c2d78,0x65(%rax),%esi
-   180063fc4:	insl   (%dx),%es:(%rdi)
-   180063fc5:	pop    %rsp
-   180063fc6:	jae    0x18006403a
-   180063fc8:	movsxd 0x67(%rdi,%riz,2),%ebx
-   180063fcc:	insl   (%dx),%es:(%rdi)
-   180063fcd:	insb   (%dx),%es:(%rdi)
-   180063fce:	cs movsxd (%rax),%eax
-   180063fd1:	add    %al,(%rax)
-   180063fd3:	add    %al,(%rax)
+   180063fac:	fs sub $0x5c77656e,%eax
+   180063fb2:	pop    %rdi
+   180063fb3:	ja     0x180064024
+   180063fb5:	jb     0x180064022
+   180063fb7:	pop    %rsp
+   180063fb8:	imul   $0x6c6c2d78,0x65(%rax),%esi
+   180063fbf:	insl   (%dx),%es:(%rdi)
+   180063fc0:	pop    %rsp
+   180063fc1:	imul   $0x6c6c2d78,0x65(%rax),%esi
+   180063fc8:	insl   (%dx),%es:(%rdi)
+   180063fc9:	pop    %rsp
+   180063fca:	jae    0x18006403e
+   180063fcc:	movsxd 0x67(%rdi,%riz,2),%ebx
+   180063fd0:	insl   (%dx),%es:(%rdi)
+   180063fd1:	insb   (%dx),%es:(%rdi)
+   180063fd2:	cs movsxd (%rax),%eax
    180063fd5:	add    %al,(%rax)
    180063fd7:	add    %al,0x47(%rdi)
    180063fda:	rex.WRB
    180063fdb:	rex.WR pop %rdi
    180063fdd:	push   %r11
    180063fdf:	push   %rbx
    180063fe0:	rex.RB push %r10
@@ -123918,19 +123912,18 @@
    1800660dd:	add    %al,(%rax)
    1800660df:	add    %bh,0x18005f6(%rax)
    1800660e5:	add    %al,(%rax)
    1800660e7:	add    %al,%al
    1800660e9:	testb  $0x0,0x180(%rip)        # 0x180066270
    1800660f0:	add    %al,(%rax)
    1800660f2:	add    %al,(%rax)
-   1800660f4:	push   %rcx
-   1800660f5:	cmp    %bl,0x66(%rbx)
-   1800660f8:	add    %al,(%rax)
-   1800660fa:	add    %al,(%rax)
-   1800660fc:	or     $0x50000000,%eax
+   1800660f4:	lahf
+   1800660f5:	mov    %ebx,0x0(%rsi,%riz,2)
+   1800660f9:	add    %al,(%rax)
+   1800660fb:	add    %cl,0x50000000(%rip)        # 0x1d0066101
    180066101:	add    (%rax),%eax
    180066103:	add    %al,0x5d840006(%rbp,%rbp,2)
    18006610a:	(bad)
 	...
    18006617f:	add    %bh,%al
    180066181:	jo     0x180066189
    180066183:	addb   $0x0,(%rcx)
```

## ipex_llm/libs/libllama_avx.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x00000001800621b8
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Sat Jun  1 15:02:58 2024
+Time/Date		Sun Jun  2 15:03:46 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000062800
 SizeOfInitializedData	00000000000c6800
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000000621b8
@@ -25082,52 +25082,52 @@
    18000795d:	mov    %rax,%rcx
    180007960:	call   *0x5ccd2(%rip)        # 0x180064638
    180007966:	test   %eax,%eax
    180007968:	je     0x1800079a4
    18000796a:	mov    $0x2,%ecx
    18000796f:	call   *0x5cc9b(%rip)        # 0x180064610
    180007975:	mov    %rax,%rcx
-   180007978:	lea    0x5cf41(%rip),%rax        # 0x1800648c0
+   180007978:	lea    0x5cf39(%rip),%rax        # 0x1800648b8
    18000797f:	mov    %rax,0x20(%rsp)
    180007984:	mov    $0x65,%r9d
    18000798a:	lea    0x5ce7f(%rip),%r8        # 0x180064810
-   180007991:	lea    0x5ced0(%rip),%rdx        # 0x180064868
+   180007991:	lea    0x5cec8(%rip),%rdx        # 0x180064860
    180007998:	call   0x180015760
    18000799d:	call   *0x5cbb5(%rip)        # 0x180064558
    1800079a3:	int3
    1800079a4:	mov    (%rbx),%rcx
    1800079a7:	call   *0x5cc83(%rip)        # 0x180064630
    1800079ad:	cmp    $0xffffffffffffffff,%rax
    1800079b1:	jne    0x1800079eb
    1800079b3:	lea    0x3(%rax),%ecx
    1800079b6:	call   *0x5cc54(%rip)        # 0x180064610
    1800079bc:	mov    %rax,%rcx
-   1800079bf:	lea    0x5ceea(%rip),%rax        # 0x1800648b0
+   1800079bf:	lea    0x5cee2(%rip),%rax        # 0x1800648a8
    1800079c6:	mov    %rax,0x20(%rsp)
    1800079cb:	mov    $0x5b,%r9d
    1800079d1:	lea    0x5ce38(%rip),%r8        # 0x180064810
-   1800079d8:	lea    0x5ce89(%rip),%rdx        # 0x180064868
+   1800079d8:	lea    0x5ce81(%rip),%rdx        # 0x180064860
    1800079df:	call   0x180015760
    1800079e4:	call   *0x5cb6e(%rip)        # 0x180064558
    1800079ea:	int3
    1800079eb:	mov    %rax,0x8(%rbx)
    1800079ef:	xor    %r8d,%r8d
    1800079f2:	xor    %edx,%edx
    1800079f4:	mov    (%rbx),%rcx
    1800079f7:	call   *0x5cc3b(%rip)        # 0x180064638
    1800079fd:	test   %eax,%eax
    1800079ff:	je     0x180007a3b
    180007a01:	mov    $0x2,%ecx
    180007a06:	call   *0x5cc04(%rip)        # 0x180064610
    180007a0c:	mov    %rax,%rcx
-   180007a0f:	lea    0x5ceaa(%rip),%rax        # 0x1800648c0
+   180007a0f:	lea    0x5cea2(%rip),%rax        # 0x1800648b8
    180007a16:	mov    %rax,0x20(%rsp)
    180007a1b:	mov    $0x65,%r9d
    180007a21:	lea    0x5cde8(%rip),%r8        # 0x180064810
-   180007a28:	lea    0x5ce39(%rip),%rdx        # 0x180064868
+   180007a28:	lea    0x5ce31(%rip),%rdx        # 0x180064860
    180007a2f:	call   0x180015760
    180007a34:	call   *0x5cb1e(%rip)        # 0x180064558
    180007a3a:	int3
    180007a3b:	mov    %rbx,%rax
    180007a3e:	mov    0x68(%rsp),%rcx
    180007a43:	xor    %rsp,%rcx
    180007a46:	call   0x180061bb0
@@ -25136,15 +25136,15 @@
    180007a57:	pop    %rdi
    180007a58:	ret
    180007a59:	call   *0x5cad9(%rip)        # 0x180064538
    180007a5f:	mov    (%rax),%ecx
    180007a61:	call   *0x5cae9(%rip)        # 0x180064550
    180007a67:	mov    %rax,%r9
    180007a6a:	mov    %rdi,%r8
-   180007a6d:	lea    0x5ce24(%rip),%rdx        # 0x180064898
+   180007a6d:	lea    0x5ce1c(%rip),%rdx        # 0x180064890
    180007a74:	lea    0x48(%rsp),%rcx
    180007a79:	call   0x18000c010
    180007a7e:	nop
    180007a7f:	mov    %rax,%rdx
    180007a82:	lea    0x30(%rsp),%rcx
    180007a87:	call   0x1800086c0
    180007a8c:	lea    0x6ac8d(%rip),%rdx        # 0x180072720
@@ -25162,15 +25162,15 @@
    180007ab0:	xor    %rsp,%rax
    180007ab3:	mov    %rax,0x50(%rsp)
    180007ab8:	mov    %r9,%rbp
    180007abb:	mov    %r8,%rsi
    180007abe:	mov    %rdx,%rbx
    180007ac1:	mov    %rcx,%rdi
    180007ac4:	mov    %rcx,0x28(%rsp)
-   180007ac9:	lea    0x5d200(%rip),%r8        # 0x180064cd0
+   180007ac9:	lea    0x5d1fc(%rip),%r8        # 0x180064ccc
    180007ad0:	call   0x180007920
    180007ad5:	nop
    180007ad6:	movl   $0x7d00,0x14(%rdi)
    180007add:	movl   $0x200,0x18(%rdi)
    180007ae4:	movl   $0x1000,0x1c(%rdi)
    180007aeb:	movl   $0x100,0x20(%rdi)
    180007af2:	movl   $0x20,0x24(%rdi)
@@ -25181,15 +25181,15 @@
    180007b15:	lea    0x38(%rdi),%rcx
    180007b19:	call   0x1800085f0
    180007b1e:	nop
    180007b1f:	mov    $0x2,%ecx
    180007b24:	call   *0x5cae6(%rip)        # 0x180064610
    180007b2a:	mov    %rax,%rcx
    180007b2d:	mov    %rbx,%r8
-   180007b30:	lea    0x5d1a1(%rip),%rdx        # 0x180064cd8
+   180007b30:	lea    0x5d199(%rip),%rdx        # 0x180064cd0
    180007b37:	call   0x180015760
    180007b3c:	mov    $0x4,%r8d
    180007b42:	lea    0x20(%rsp),%rdx
    180007b47:	mov    %rdi,%rcx
    180007b4a:	call   0x180012ee0
    180007b4f:	mov    0x20(%rsp),%ebx
    180007b53:	cmp    $0x67676d6c,%ebx
@@ -25363,15 +25363,15 @@
    180007df2:	cmpq   $0x10,0x18(%rax)
    180007df7:	jb     0x180007dfc
    180007df9:	mov    (%rax),%rbx
    180007dfc:	mov    $0x2,%ecx
    180007e01:	call   *0x5c809(%rip)        # 0x180064610
    180007e07:	mov    %rax,%rcx
    180007e0a:	mov    %rbx,%r8
-   180007e0d:	lea    0x5cb5c(%rip),%rdx        # 0x180064970
+   180007e0d:	lea    0x5cb54(%rip),%rdx        # 0x180064968
    180007e14:	call   0x180015760
    180007e19:	mov    0x60(%rsp),%rdx
    180007e1e:	cmp    $0x10,%rdx
    180007e22:	jb     0x180007e59
    180007e24:	inc    %rdx
    180007e27:	mov    0x48(%rsp),%rcx
    180007e2c:	mov    %rcx,%rax
@@ -25399,15 +25399,15 @@
    180007e7f:	mov    %ebp,%edx
    180007e81:	lea    0x68(%rsp),%rcx
    180007e86:	call   0x18000eef0
    180007e8b:	nop
    180007e8c:	mov    %rax,%rcx
    180007e8f:	call   0x18000b8d0
    180007e94:	mov    %rax,%r8
-   180007e97:	lea    0x5cab2(%rip),%rdx        # 0x180064950
+   180007e97:	lea    0x5caaa(%rip),%rdx        # 0x180064948
    180007e9e:	lea    0x48(%rsp),%rcx
    180007ea3:	call   0x18000c010
    180007ea8:	nop
    180007ea9:	mov    %rax,%rdx
    180007eac:	lea    0x30(%rsp),%rcx
    180007eb1:	call   0x1800086c0
    180007eb6:	lea    0x6a863(%rip),%rdx        # 0x180072720
@@ -25417,15 +25417,15 @@
    180007ec8:	mov    %eax,%edx
    180007eca:	lea    0x48(%rsp),%rcx
    180007ecf:	call   0x18000eef0
    180007ed4:	nop
    180007ed5:	mov    %rax,%rcx
    180007ed8:	call   0x18000b8d0
    180007edd:	mov    %rax,%r8
-   180007ee0:	lea    0x5ca49(%rip),%rdx        # 0x180064930
+   180007ee0:	lea    0x5ca41(%rip),%rdx        # 0x180064928
    180007ee7:	lea    0x68(%rsp),%rcx
    180007eec:	call   0x18000c010
    180007ef1:	nop
    180007ef2:	mov    %rax,%rdx
    180007ef5:	lea    0x30(%rsp),%rcx
    180007efa:	call   0x1800086c0
    180007eff:	lea    0x6a81a(%rip),%rdx        # 0x180072720
@@ -27614,15 +27614,15 @@
    180009ae7:	cmpq   $0x10,0x18(%rax)
    180009aec:	jb     0x180009af1
    180009aee:	mov    (%rax),%rbx
    180009af1:	mov    $0x2,%ecx
    180009af6:	call   *0x5ab14(%rip)        # 0x180064610
    180009afc:	mov    %rax,%rcx
    180009aff:	mov    %rbx,%r8
-   180009b02:	lea    0x5ae97(%rip),%rdx        # 0x1800649a0
+   180009b02:	lea    0x5ae8f(%rip),%rdx        # 0x180064998
    180009b09:	call   0x180015760
    180009b0e:	mov    0x38(%rsp),%rdx
    180009b13:	cmp    $0x10,%rdx
    180009b17:	jb     0x180009b4f
    180009b19:	inc    %rdx
    180009b1c:	mov    0x20(%rsp),%rcx
    180009b21:	mov    %rcx,%rax
@@ -29902,15 +29902,15 @@
    18000b9c6:	mov    $0x2,%ecx
    18000b9cb:	call   *0x58c3f(%rip)        # 0x180064610
    18000b9d1:	mov    %rax,%rcx
    18000b9d4:	lea    0x5927d(%rip),%rax        # 0x180064c58
    18000b9db:	mov    %rax,0x20(%rsp)
    18000b9e0:	mov    $0x187,%r9d
    18000b9e6:	lea    0x59293(%rip),%r8        # 0x180064c80
-   18000b9ed:	lea    0x58e74(%rip),%rdx        # 0x180064868
+   18000b9ed:	lea    0x58e6c(%rip),%rdx        # 0x180064860
    18000b9f4:	call   0x180015760
    18000b9f9:	call   *0x58b59(%rip)        # 0x180064558
    18000b9ff:	int3
    18000ba00:	mov    0x3c(%r14),%ecx
    18000ba04:	test   %ecx,%ecx
    18000ba06:	je     0x18000ba65
    18000ba08:	sub    $0x1,%ecx
@@ -30523,19 +30523,19 @@
    18000c124:	mov    %r14,%rcx
    18000c127:	call   0x180019950
    18000c12c:	cmp    %r15d,%eax
    18000c12f:	je     0x18000c16b
    18000c131:	mov    $0x2,%ecx
    18000c136:	call   *0x584d4(%rip)        # 0x180064610
    18000c13c:	mov    %rax,%rcx
-   18000c13f:	lea    0x58742(%rip),%rax        # 0x180064888
+   18000c13f:	lea    0x5873a(%rip),%rax        # 0x180064880
    18000c146:	mov    %rax,0x20(%rsp)
    18000c14b:	mov    $0x40,%r9d
    18000c151:	lea    0x586b8(%rip),%r8        # 0x180064810
-   18000c158:	lea    0x58709(%rip),%rdx        # 0x180064868
+   18000c158:	lea    0x58701(%rip),%rdx        # 0x180064860
    18000c15f:	call   0x180015760
    18000c164:	call   *0x583ee(%rip)        # 0x180064558
    18000c16a:	int3
    18000c16b:	vpxor  %xmm0,%xmm0,%xmm0
    18000c16f:	vmovups %xmm0,0x0(%rbp)
    18000c174:	mov    %r12,0x10(%rbp)
    18000c178:	mov    %r12,0x18(%rbp)
@@ -30575,15 +30575,15 @@
    18000c1da:	mov    $0x2,%ecx
    18000c1df:	call   *0x5842b(%rip)        # 0x180064610
    18000c1e5:	mov    %rax,%rcx
    18000c1e8:	lea    0x585f9(%rip),%rax        # 0x1800647e8
    18000c1ef:	mov    %rax,0x20(%rsp)
    18000c1f4:	mov    $0x3d,%r9d
    18000c1fa:	lea    0x5860f(%rip),%r8        # 0x180064810
-   18000c201:	lea    0x58660(%rip),%rdx        # 0x180064868
+   18000c201:	lea    0x58658(%rip),%rdx        # 0x180064860
    18000c208:	call   0x180015760
    18000c20d:	call   *0x58345(%rip)        # 0x180064558
    18000c213:	int3
    18000c214:	call   0x18000b0f0
    18000c219:	int3
    18000c21a:	call   0x18000b540
    18000c21f:	int3
@@ -30673,15 +30673,15 @@
    18000c360:	mov    $0x2,%ecx
    18000c365:	call   *0x582a5(%rip)        # 0x180064610
    18000c36b:	mov    %rax,%rcx
    18000c36e:	lea    0x58c43(%rip),%rax        # 0x180064fb8
    18000c375:	mov    %rax,0x20(%rsp)
    18000c37a:	mov    $0x2b2,%r9d
    18000c380:	lea    0x588f9(%rip),%r8        # 0x180064c80
-   18000c387:	lea    0x584da(%rip),%rdx        # 0x180064868
+   18000c387:	lea    0x584d2(%rip),%rdx        # 0x180064860
    18000c38e:	call   0x180015760
    18000c393:	call   *0x581bf(%rip)        # 0x180064558
    18000c399:	int3
    18000c39a:	mov    (%r14),%r8d
    18000c39d:	mov    0x38(%rdi),%edx
    18000c3a0:	mov    0x80(%rbx),%rcx
    18000c3a7:	call   0x18003efc0
@@ -30697,15 +30697,15 @@
    18000c3cc:	mov    $0x2,%ecx
    18000c3d1:	call   *0x58239(%rip)        # 0x180064610
    18000c3d7:	mov    %rax,%rcx
    18000c3da:	lea    0x58bef(%rip),%rax        # 0x180064fd0
    18000c3e1:	mov    %rax,0x20(%rsp)
    18000c3e6:	mov    $0x2b6,%r9d
    18000c3ec:	lea    0x5888d(%rip),%r8        # 0x180064c80
-   18000c3f3:	lea    0x5846e(%rip),%rdx        # 0x180064868
+   18000c3f3:	lea    0x58466(%rip),%rdx        # 0x180064860
    18000c3fa:	call   0x180015760
    18000c3ff:	call   *0x58153(%rip)        # 0x180064558
    18000c405:	int3
    18000c406:	mov    %r13d,0x4(%rsi)
    18000c40a:	mov    %rsi,0x60(%rdi)
    18000c40e:	incq   0x78(%rbx)
    18000c412:	mov    %rsi,%rax
@@ -30779,16 +30779,16 @@
    18000c501:	mov    %rcx,%rbx
    18000c504:	jne    0x18000c540
    18000c506:	mov    $0x2,%ecx
    18000c50b:	call   *0x580ff(%rip)        # 0x180064610
    18000c511:	mov    $0x114,%r9d
    18000c517:	lea    0x582f2(%rip),%r8        # 0x180064810
    18000c51e:	mov    %rax,%rcx
-   18000c521:	lea    0x58340(%rip),%rdx        # 0x180064868
-   18000c528:	lea    0x584b5(%rip),%rax        # 0x1800649e4
+   18000c521:	lea    0x58338(%rip),%rdx        # 0x180064860
+   18000c528:	lea    0x584ad(%rip),%rax        # 0x1800649dc
    18000c52f:	mov    %rax,0x20(%rsp)
    18000c534:	call   0x180015760
    18000c539:	call   *0x58019(%rip)        # 0x180064558
    18000c53f:	int3
    18000c540:	cmpb   $0x0,0x10(%rcx)
    18000c544:	jne    0x18000c598
    18000c546:	lea    0x30(%rsp),%rcx
@@ -31005,16 +31005,16 @@
    18000c834:	add    $0x38,%rsp
    18000c838:	ret
    18000c839:	mov    $0x2,%ecx
    18000c83e:	call   *0x57dcc(%rip)        # 0x180064610
    18000c844:	mov    $0x10f,%r9d
    18000c84a:	lea    0x57fbf(%rip),%r8        # 0x180064810
    18000c851:	mov    %rax,%rcx
-   18000c854:	lea    0x5800d(%rip),%rdx        # 0x180064868
-   18000c85b:	lea    0x58166(%rip),%rax        # 0x1800649c8
+   18000c854:	lea    0x58005(%rip),%rdx        # 0x180064860
+   18000c85b:	lea    0x5815e(%rip),%rax        # 0x1800649c0
    18000c862:	mov    %rax,0x20(%rsp)
    18000c867:	call   0x180015760
    18000c86c:	call   *0x57ce6(%rip)        # 0x180064558
    18000c872:	int3
    18000c873:	int3
    18000c874:	int3
    18000c875:	int3
@@ -32515,15 +32515,15 @@
    18000e280:	mov    %rax,-0x30(%rbp)
    18000e284:	jne    0x18000e2c0
    18000e286:	mov    $0x2,%ecx
    18000e28b:	call   *0x5637f(%rip)        # 0x180064610
    18000e291:	mov    $0x4e8,%r9d
    18000e297:	lea    0x569e2(%rip),%r8        # 0x180064c80
    18000e29e:	mov    %rax,%rcx
-   18000e2a1:	lea    0x565c0(%rip),%rdx        # 0x180064868
+   18000e2a1:	lea    0x565b8(%rip),%rdx        # 0x180064860
    18000e2a8:	lea    0x57351(%rip),%rax        # 0x180065600
    18000e2af:	mov    %rax,0x20(%rsp)
    18000e2b4:	call   0x180015760
    18000e2b9:	call   *0x56299(%rip)        # 0x180064558
    18000e2bf:	int3
    18000e2c0:	mov    0x13e0(%r14),%ecx
    18000e2c7:	mov    0x13e4(%r14),%eax
@@ -33271,19 +33271,19 @@
    18000ef51:	mov    %rdi,0x10(%rbx)
    18000ef55:	mov    %rbx,%rcx
    18000ef58:	movq   $0xf,0x18(%rbx)
    18000ef60:	call   0x18000b5a0
    18000ef65:	mov    %rax,(%rbx)
    18000ef68:	movq   $0x15,0x10(%rbx)
    18000ef70:	movq   $0x1f,0x18(%rbx)
-   18000ef78:	vmovups 0x55998(%rip),%xmm0        # 0x180064918
+   18000ef78:	vmovups 0x55990(%rip),%xmm0        # 0x180064910
    18000ef80:	vmovups %xmm0,(%rax)
-   18000ef84:	mov    0x5599e(%rip),%ecx        # 0x180064928
+   18000ef84:	mov    0x55996(%rip),%ecx        # 0x180064920
    18000ef8a:	mov    %ecx,0x10(%rax)
-   18000ef8d:	movzbl 0x55998(%rip),%ecx        # 0x18006492c
+   18000ef8d:	movzbl 0x55990(%rip),%ecx        # 0x180064924
    18000ef94:	mov    %cl,0x14(%rax)
    18000ef97:	mov    %dil,0x15(%rax)
    18000ef9b:	jmp    0x18000efd1
    18000ef9d:	mov    0x40(%rsp),%rdx
    18000efa2:	lea    0x50(%rsp),%rcx
    18000efa7:	vpxor  %xmm1,%xmm1,%xmm1
    18000efab:	vmovdqu %xmm1,0x60(%rsp)
@@ -34978,15 +34978,15 @@
    180010b9e:	mov    $0x2,%ecx
    180010ba3:	call   *0x53a67(%rip)        # 0x180064610
    180010ba9:	mov    %rax,%rcx
    180010bac:	lea    0x53fc1(%rip),%rax        # 0x180064b74
    180010bb3:	mov    %rax,0x20(%rsp)
    180010bb8:	mov    $0x39e,%r9d
    180010bbe:	lea    0x540bb(%rip),%r8        # 0x180064c80
-   180010bc5:	lea    0x53c9c(%rip),%rdx        # 0x180064868
+   180010bc5:	lea    0x53c94(%rip),%rdx        # 0x180064860
    180010bcc:	call   0x180015760
    180010bd1:	call   *0x53981(%rip)        # 0x180064558
    180010bd7:	int3
    180010bd8:	lea    0x554f1(%rip),%rcx        # 0x1800660d0
    180010bdf:	call   0x180061358
    180010be4:	int3
    180010be5:	lea    0x547f4(%rip),%rdx        # 0x1800653e0
@@ -35864,48 +35864,48 @@
    1800119a2:	mov    $0x2,%ecx
    1800119a7:	call   *0x52c63(%rip)        # 0x180064610
    1800119ad:	mov    %rax,%rcx
    1800119b0:	lea    0x53489(%rip),%rax        # 0x180064e40
    1800119b7:	mov    %rax,0x20(%rsp)
    1800119bc:	mov    $0x25d,%r9d
    1800119c2:	lea    0x532b7(%rip),%r8        # 0x180064c80
-   1800119c9:	lea    0x52e98(%rip),%rdx        # 0x180064868
+   1800119c9:	lea    0x52e90(%rip),%rdx        # 0x180064860
    1800119d0:	call   0x180015760
    1800119d5:	call   *0x52b7d(%rip)        # 0x180064558
    1800119db:	int3
    1800119dc:	mov    $0x2,%ecx
    1800119e1:	call   *0x52c29(%rip)        # 0x180064610
    1800119e7:	mov    %rax,%rcx
-   1800119ea:	lea    0x52ecf(%rip),%rax        # 0x1800648c0
+   1800119ea:	lea    0x52ec7(%rip),%rax        # 0x1800648b8
    1800119f1:	mov    %rax,0x20(%rsp)
    1800119f6:	mov    $0x65,%r9d
    1800119fc:	lea    0x52e0d(%rip),%r8        # 0x180064810
-   180011a03:	lea    0x52e5e(%rip),%rdx        # 0x180064868
+   180011a03:	lea    0x52e56(%rip),%rdx        # 0x180064860
    180011a0a:	call   0x180015760
    180011a0f:	call   *0x52b43(%rip)        # 0x180064558
    180011a15:	int3
    180011a16:	mov    $0x2,%ecx
    180011a1b:	call   *0x52bef(%rip)        # 0x180064610
    180011a21:	mov    %rax,%rcx
-   180011a24:	lea    0x52e85(%rip),%rax        # 0x1800648b0
+   180011a24:	lea    0x52e7d(%rip),%rax        # 0x1800648a8
    180011a2b:	mov    %rax,0x20(%rsp)
    180011a30:	mov    $0x5b,%r9d
    180011a36:	lea    0x52dd3(%rip),%r8        # 0x180064810
-   180011a3d:	lea    0x52e24(%rip),%rdx        # 0x180064868
+   180011a3d:	lea    0x52e1c(%rip),%rdx        # 0x180064860
    180011a44:	call   0x180015760
    180011a49:	call   *0x52b09(%rip)        # 0x180064558
    180011a4f:	int3
    180011a50:	mov    $0x2,%ecx
    180011a55:	call   *0x52bb5(%rip)        # 0x180064610
    180011a5b:	mov    %rax,%rcx
    180011a5e:	lea    0x5310f(%rip),%rax        # 0x180064b74
    180011a65:	mov    %rax,0x20(%rsp)
    180011a6a:	mov    $0x255,%r9d
    180011a70:	lea    0x53209(%rip),%r8        # 0x180064c80
-   180011a77:	lea    0x52dea(%rip),%rdx        # 0x180064868
+   180011a77:	lea    0x52de2(%rip),%rdx        # 0x180064860
    180011a7e:	call   0x180015760
    180011a83:	call   *0x52acf(%rip)        # 0x180064558
    180011a89:	nop
    180011a8a:	mov    -0x50(%rbp),%rsi
    180011a8e:	jmp    0x180011aa9
    180011a90:	mov    0x100(%rbp),%rdi
    180011a97:	mov    0x40(%rsp),%rsi
@@ -36208,19 +36208,19 @@
    180011eeb:	test   %rsi,%rsi
    180011eee:	js     0x180011f31
    180011ef0:	vcvtsi2ss %rsi,%xmm1,%xmm1
    180011ef5:	jmp    0x180011f49
    180011ef7:	mov    $0x2,%ecx
    180011efc:	call   *0x5270e(%rip)        # 0x180064610
    180011f02:	mov    %rax,%rcx
-   180011f05:	lea    0x52abc(%rip),%rax        # 0x1800649c8
+   180011f05:	lea    0x52ab4(%rip),%rax        # 0x1800649c0
    180011f0c:	mov    %rax,0x20(%rsp)
    180011f11:	mov    $0x10f,%r9d
    180011f17:	lea    0x528f2(%rip),%r8        # 0x180064810
-   180011f1e:	lea    0x52943(%rip),%rdx        # 0x180064868
+   180011f1e:	lea    0x5293b(%rip),%rdx        # 0x180064860
    180011f25:	call   0x180015760
    180011f2a:	call   *0x52628(%rip)        # 0x180064558
    180011f30:	int3
    180011f31:	mov    %rsi,%rcx
    180011f34:	shr    $1,%rcx
    180011f37:	mov    %rsi,%rax
    180011f3a:	and    $0x1,%eax
@@ -36288,30 +36288,30 @@
    180012018:	cmp    %r13,%rbx
    18001201b:	je     0x1800120a2
    180012021:	mov    0xb0(%rsp),%r8
    180012029:	jmp    0x180011ed0
    18001202e:	mov    $0x2,%ecx
    180012033:	call   *0x525d7(%rip)        # 0x180064610
    180012039:	mov    %rax,%rcx
-   18001203c:	lea    0x529a1(%rip),%rax        # 0x1800649e4
+   18001203c:	lea    0x52999(%rip),%rax        # 0x1800649dc
    180012043:	mov    %rax,0x20(%rsp)
    180012048:	mov    $0x114,%r9d
    18001204e:	lea    0x527bb(%rip),%r8        # 0x180064810
-   180012055:	lea    0x5280c(%rip),%rdx        # 0x180064868
+   180012055:	lea    0x52804(%rip),%rdx        # 0x180064860
    18001205c:	call   0x180015760
    180012061:	call   *0x524f1(%rip)        # 0x180064558
    180012067:	int3
    180012068:	mov    $0x2,%ecx
    18001206d:	call   *0x5259d(%rip)        # 0x180064610
    180012073:	mov    %rax,%rcx
    180012076:	lea    0x52fa3(%rip),%rax        # 0x180065020
    18001207d:	mov    %rax,0x20(%rsp)
    180012082:	mov    $0x2e1,%r9d
    180012088:	lea    0x52bf1(%rip),%r8        # 0x180064c80
-   18001208f:	lea    0x527d2(%rip),%rdx        # 0x180064868
+   18001208f:	lea    0x527ca(%rip),%rdx        # 0x180064860
    180012096:	call   0x180015760
    18001209b:	call   *0x524b7(%rip)        # 0x180064558
    1800120a1:	int3
    1800120a2:	mov    0xa8(%rsp),%rbx
    1800120aa:	add    $0x60,%rsp
    1800120ae:	pop    %r15
    1800120b0:	pop    %r14
@@ -36345,15 +36345,15 @@
    1800120f8:	mov    $0x2,%ecx
    1800120fd:	call   *0x5250d(%rip)        # 0x180064610
    180012103:	mov    %rax,%rcx
    180012106:	lea    0x52f23(%rip),%rax        # 0x180065030
    18001210d:	mov    %rax,0x20(%rsp)
    180012112:	mov    $0x2ee,%r9d
    180012118:	lea    0x52b61(%rip),%r8        # 0x180064c80
-   18001211f:	lea    0x52742(%rip),%rdx        # 0x180064868
+   18001211f:	lea    0x5273a(%rip),%rdx        # 0x180064860
    180012126:	call   0x180015760
    18001212b:	call   *0x52427(%rip)        # 0x180064558
    180012131:	int3
    180012132:	movabs $0x4924924924924925,%rax
    18001213c:	imul   %rcx
    18001213f:	sar    $0x4,%rdx
    180012143:	mov    %rdx,%rax
@@ -36391,19 +36391,19 @@
    1800121c6:	mov    (%rbx),%rcx
    1800121c9:	call   *0x52469(%rip)        # 0x180064638
    1800121cf:	test   %eax,%eax
    1800121d1:	je     0x18001220d
    1800121d3:	mov    $0x2,%ecx
    1800121d8:	call   *0x52432(%rip)        # 0x180064610
    1800121de:	mov    %rax,%rcx
-   1800121e1:	lea    0x526d8(%rip),%rax        # 0x1800648c0
+   1800121e1:	lea    0x526d0(%rip),%rax        # 0x1800648b8
    1800121e8:	mov    %rax,0x20(%rsp)
    1800121ed:	mov    $0x65,%r9d
    1800121f3:	lea    0x52616(%rip),%r8        # 0x180064810
-   1800121fa:	lea    0x52667(%rip),%rdx        # 0x180064868
+   1800121fa:	lea    0x5265f(%rip),%rdx        # 0x180064860
    180012201:	call   0x180015760
    180012206:	call   *0x5234c(%rip)        # 0x180064558
    18001220c:	int3
    18001220d:	mov    0x58(%r14),%r8
    180012211:	mov    0x68(%r14),%rdx
    180012215:	mov    %rbx,%rcx
    180012218:	call   0x180012ee0
@@ -36444,26 +36444,26 @@
    18001229d:	mov    $0x2,%ecx
    1800122a2:	call   *0x52368(%rip)        # 0x180064610
    1800122a8:	mov    %rax,%rcx
    1800122ab:	lea    0x52d96(%rip),%rax        # 0x180065048
    1800122b2:	mov    %rax,0x20(%rsp)
    1800122b7:	mov    $0x2fc,%r9d
    1800122bd:	lea    0x529bc(%rip),%r8        # 0x180064c80
-   1800122c4:	lea    0x5259d(%rip),%rdx        # 0x180064868
+   1800122c4:	lea    0x52595(%rip),%rdx        # 0x180064860
    1800122cb:	call   0x180015760
    1800122d0:	call   *0x52282(%rip)        # 0x180064558
    1800122d6:	int3
    1800122d7:	mov    $0x2,%ecx
    1800122dc:	call   *0x5232e(%rip)        # 0x180064610
    1800122e2:	mov    %rax,%rcx
-   1800122e5:	lea    0x525d4(%rip),%rax        # 0x1800648c0
+   1800122e5:	lea    0x525cc(%rip),%rax        # 0x1800648b8
    1800122ec:	mov    %rax,0x20(%rsp)
    1800122f1:	mov    $0x65,%r9d
    1800122f7:	lea    0x52512(%rip),%r8        # 0x180064810
-   1800122fe:	lea    0x52563(%rip),%rdx        # 0x180064868
+   1800122fe:	lea    0x5255b(%rip),%rdx        # 0x180064860
    180012305:	call   0x180015760
    18001230a:	call   *0x52248(%rip)        # 0x180064558
    180012310:	int3
    180012311:	cmp    $0x1,%eax
    180012314:	jne    0x1800126cc
    18001231a:	mov    0x8(%rdx),%rcx
    18001231e:	sub    (%rdx),%rcx
@@ -36653,26 +36653,26 @@
    1800125fa:	mov    $0x2,%ecx
    1800125ff:	call   *0x5200b(%rip)        # 0x180064610
    180012605:	mov    %rax,%rcx
    180012608:	lea    0x52a51(%rip),%rax        # 0x180065060
    18001260f:	mov    %rax,0x20(%rsp)
    180012614:	mov    $0x313,%r9d
    18001261a:	lea    0x5265f(%rip),%r8        # 0x180064c80
-   180012621:	lea    0x52240(%rip),%rdx        # 0x180064868
+   180012621:	lea    0x52238(%rip),%rdx        # 0x180064860
    180012628:	call   0x180015760
    18001262d:	call   *0x51f25(%rip)        # 0x180064558
    180012633:	int3
    180012634:	mov    $0x2,%ecx
    180012639:	call   *0x51fd1(%rip)        # 0x180064610
    18001263f:	mov    %rax,%rcx
-   180012642:	lea    0x52277(%rip),%rax        # 0x1800648c0
+   180012642:	lea    0x5226f(%rip),%rax        # 0x1800648b8
    180012649:	mov    %rax,0x20(%rsp)
    18001264e:	mov    $0x65,%r9d
    180012654:	lea    0x521b5(%rip),%r8        # 0x180064810
-   18001265b:	lea    0x52206(%rip),%rdx        # 0x180064868
+   18001265b:	lea    0x521fe(%rip),%rdx        # 0x180064860
    180012662:	call   0x180015760
    180012667:	call   *0x51eeb(%rip)        # 0x180064558
    18001266d:	nop
    18001266e:	test   %r12,%r12
    180012671:	je     0x1800126cc
    180012673:	mov    %r12,%rbx
    180012676:	cmp    %rsi,%r12
@@ -37331,30 +37331,30 @@
    180012f40:	xor    %rsp,%rcx
    180012f43:	call   0x180061bb0
    180012f48:	add    $0x60,%rsp
    180012f4c:	pop    %rdi
    180012f4d:	pop    %rsi
    180012f4e:	pop    %rbx
    180012f4f:	ret
-   180012f50:	lea    0x51989(%rip),%rdx        # 0x1800648e0
+   180012f50:	lea    0x51981(%rip),%rdx        # 0x1800648d8
    180012f57:	lea    0x38(%rsp),%rcx
    180012f5c:	call   0x180007010
    180012f61:	nop
    180012f62:	mov    %rax,%rdx
    180012f65:	lea    0x20(%rsp),%rcx
    180012f6a:	call   0x1800086c0
    180012f6f:	lea    0x5f7aa(%rip),%rdx        # 0x180072720
    180012f76:	lea    0x20(%rsp),%rcx
    180012f7b:	call   0x180062722
    180012f80:	nop
    180012f81:	call   *0x515b1(%rip)        # 0x180064538
    180012f87:	mov    (%rax),%ecx
    180012f89:	call   *0x515c1(%rip)        # 0x180064550
    180012f8f:	mov    %rax,%r8
-   180012f92:	lea    0x51937(%rip),%rdx        # 0x1800648d0
+   180012f92:	lea    0x5192f(%rip),%rdx        # 0x1800648c8
    180012f99:	lea    0x38(%rsp),%rcx
    180012f9e:	call   0x18000c010
    180012fa3:	nop
    180012fa4:	mov    %rax,%rdx
    180012fa7:	lea    0x20(%rsp),%rcx
    180012fac:	call   0x1800086c0
    180012fb1:	lea    0x5f768(%rip),%rdx        # 0x180072720
@@ -37962,69 +37962,69 @@
    180013902:	call   0x180061594
    180013907:	mov    -0x48(%rbp),%r12
    18001390b:	mov    (%r12),%rcx
    18001390f:	jmp    0x180013010
    180013914:	mov    $0x2,%ecx
    180013919:	call   *0x50cf1(%rip)        # 0x180064610
    18001391f:	mov    %rax,%rcx
-   180013922:	lea    0x50f97(%rip),%rax        # 0x1800648c0
+   180013922:	lea    0x50f8f(%rip),%rax        # 0x1800648b8
    180013929:	mov    %rax,0x20(%rsp)
    18001392e:	mov    $0x65,%r9d
    180013934:	lea    0x50ed5(%rip),%r8        # 0x180064810
-   18001393b:	lea    0x50f26(%rip),%rdx        # 0x180064868
+   18001393b:	lea    0x50f1e(%rip),%rdx        # 0x180064860
    180013942:	call   0x180015760
    180013947:	call   *0x50c0b(%rip)        # 0x180064558
    18001394d:	int3
    18001394e:	mov    $0x2,%ecx
    180013953:	call   *0x50cb7(%rip)        # 0x180064610
    180013959:	mov    %rax,%rcx
-   18001395c:	lea    0x50f4d(%rip),%rax        # 0x1800648b0
+   18001395c:	lea    0x50f45(%rip),%rax        # 0x1800648a8
    180013963:	mov    %rax,0x20(%rsp)
    180013968:	mov    $0x5b,%r9d
    18001396e:	lea    0x50e9b(%rip),%r8        # 0x180064810
-   180013975:	lea    0x50eec(%rip),%rdx        # 0x180064868
+   180013975:	lea    0x50ee4(%rip),%rdx        # 0x180064860
    18001397c:	call   0x180015760
    180013981:	call   *0x50bd1(%rip)        # 0x180064558
    180013987:	nop
    180013988:	call   *0x50c12(%rip)        # 0x1800645a0
    18001398e:	nop
    18001398f:	call   *0x50c0b(%rip)        # 0x1800645a0
    180013995:	nop
    180013996:	call   *0x50c04(%rip)        # 0x1800645a0
    18001399c:	nop
    18001399d:	mov    $0x2,%ecx
    1800139a2:	call   *0x50c68(%rip)        # 0x180064610
    1800139a8:	mov    %rax,%rcx
-   1800139ab:	lea    0x50f0e(%rip),%rax        # 0x1800648c0
+   1800139ab:	lea    0x50f06(%rip),%rax        # 0x1800648b8
    1800139b2:	mov    %rax,0x20(%rsp)
    1800139b7:	mov    $0x65,%r9d
    1800139bd:	lea    0x50e4c(%rip),%r8        # 0x180064810
-   1800139c4:	lea    0x50e9d(%rip),%rdx        # 0x180064868
+   1800139c4:	lea    0x50e95(%rip),%rdx        # 0x180064860
    1800139cb:	call   0x180015760
    1800139d0:	call   *0x50b82(%rip)        # 0x180064558
    1800139d6:	int3
    1800139d7:	mov    $0x2,%ecx
    1800139dc:	call   *0x50c2e(%rip)        # 0x180064610
    1800139e2:	mov    %rax,%rcx
-   1800139e5:	lea    0x50ec4(%rip),%rax        # 0x1800648b0
+   1800139e5:	lea    0x50ebc(%rip),%rax        # 0x1800648a8
    1800139ec:	mov    %rax,0x20(%rsp)
    1800139f1:	mov    $0x5b,%r9d
    1800139f7:	lea    0x50e12(%rip),%r8        # 0x180064810
-   1800139fe:	lea    0x50e63(%rip),%rdx        # 0x180064868
+   1800139fe:	lea    0x50e5b(%rip),%rdx        # 0x180064860
    180013a05:	call   0x180015760
    180013a0a:	call   *0x50b48(%rip)        # 0x180064558
    180013a10:	nop
    180013a11:	mov    $0x2,%ecx
    180013a16:	call   *0x50bf4(%rip)        # 0x180064610
    180013a1c:	mov    %rax,%rcx
-   180013a1f:	lea    0x50e8a(%rip),%rax        # 0x1800648b0
+   180013a1f:	lea    0x50e82(%rip),%rax        # 0x1800648a8
    180013a26:	mov    %rax,0x20(%rsp)
    180013a2b:	mov    $0x5b,%r9d
    180013a31:	lea    0x50dd8(%rip),%r8        # 0x180064810
-   180013a38:	lea    0x50e29(%rip),%rdx        # 0x180064868
+   180013a38:	lea    0x50e21(%rip),%rdx        # 0x180064860
    180013a3f:	call   0x180015760
    180013a44:	call   *0x50b0e(%rip)        # 0x180064558
    180013a4a:	int3
    180013a4b:	mov    0x30(%rbp),%rcx
    180013a4f:	xor    %rsp,%rcx
    180013a52:	call   0x180061bb0
    180013a57:	mov    0x198(%rsp),%rbx
@@ -38044,30 +38044,30 @@
    180013a81:	lea    0x512d8(%rip),%rdx        # 0x180064d60
    180013a88:	lea    -0x10(%rbp),%rcx
    180013a8c:	call   0x18000c010
    180013a91:	lea    0x5edb8(%rip),%rdx        # 0x180072850
    180013a98:	lea    -0x10(%rbp),%rcx
    180013a9c:	call   0x180062722
    180013aa1:	nop
-   180013aa2:	lea    0x50e37(%rip),%rdx        # 0x1800648e0
+   180013aa2:	lea    0x50e2f(%rip),%rdx        # 0x1800648d8
    180013aa9:	lea    0x10(%rbp),%rcx
    180013aad:	call   0x180007010
    180013ab2:	nop
    180013ab3:	mov    %rax,%rdx
    180013ab6:	lea    -0x10(%rbp),%rcx
    180013aba:	call   0x1800086c0
    180013abf:	lea    0x5ec5a(%rip),%rdx        # 0x180072720
    180013ac6:	lea    -0x10(%rbp),%rcx
    180013aca:	call   0x180062722
    180013acf:	nop
    180013ad0:	call   *0x50a62(%rip)        # 0x180064538
    180013ad6:	mov    (%rax),%ecx
    180013ad8:	call   *0x50a72(%rip)        # 0x180064550
    180013ade:	mov    %rax,%r8
-   180013ae1:	lea    0x50de8(%rip),%rdx        # 0x1800648d0
+   180013ae1:	lea    0x50de0(%rip),%rdx        # 0x1800648c8
    180013ae8:	lea    0x10(%rbp),%rcx
    180013aec:	call   0x18000c010
    180013af1:	nop
    180013af2:	mov    %rax,%rdx
    180013af5:	lea    -0x10(%rbp),%rcx
    180013af9:	call   0x1800086c0
    180013afe:	lea    0x5ec1b(%rip),%rdx        # 0x180072720
@@ -38355,26 +38355,26 @@
    180013ef6:	vzeroupper
    180013ef9:	call   *0x506a1(%rip)        # 0x1800645a0
    180013eff:	nop
    180013f00:	call   *0x50632(%rip)        # 0x180064538
    180013f06:	mov    (%rax),%ecx
    180013f08:	call   *0x50642(%rip)        # 0x180064550
    180013f0e:	mov    %rax,%r8
-   180013f11:	lea    0x509b8(%rip),%rdx        # 0x1800648d0
+   180013f11:	lea    0x509b0(%rip),%rdx        # 0x1800648c8
    180013f18:	lea    -0x1(%rbp),%rcx
    180013f1c:	call   0x18000c010
    180013f21:	nop
    180013f22:	mov    %rax,%rdx
    180013f25:	lea    -0x39(%rbp),%rcx
    180013f29:	call   0x1800086c0
    180013f2e:	lea    0x5e7eb(%rip),%rdx        # 0x180072720
    180013f35:	lea    -0x39(%rbp),%rcx
    180013f39:	call   0x180062722
    180013f3e:	nop
-   180013f3f:	lea    0x5099a(%rip),%rdx        # 0x1800648e0
+   180013f3f:	lea    0x50992(%rip),%rdx        # 0x1800648d8
    180013f46:	lea    -0x1(%rbp),%rcx
    180013f4a:	call   0x180007010
    180013f4f:	nop
    180013f50:	mov    %rax,%rdx
    180013f53:	lea    -0x39(%rbp),%rcx
    180013f57:	call   0x1800086c0
    180013f5c:	lea    0x5e7bd(%rip),%rdx        # 0x180072720
@@ -39853,15 +39853,15 @@
    18001530d:	pop    %rsi
    18001530e:	pop    %rbx
    18001530f:	ret
    180015310:	call   *0x4f222(%rip)        # 0x180064538
    180015316:	mov    (%rax),%ecx
    180015318:	call   *0x4f232(%rip)        # 0x180064550
    18001531e:	mov    %rax,%r8
-   180015321:	lea    0x4f5e0(%rip),%rdx        # 0x180064908
+   180015321:	lea    0x4f5d8(%rip),%rdx        # 0x180064900
    180015328:	lea    0x38(%rsp),%rcx
    18001532d:	call   0x18000c010
    180015332:	nop
    180015333:	mov    %rax,%rdx
    180015336:	lea    0x20(%rsp),%rcx
    18001533b:	call   0x1800086c0
    180015340:	lea    0x5d3d9(%rip),%rdx        # 0x180072720
@@ -39973,15 +39973,15 @@
    1800154c0:	pop    %r12
    1800154c2:	pop    %rdi
    1800154c3:	ret
    1800154c4:	call   *0x4f06e(%rip)        # 0x180064538
    1800154ca:	mov    (%rax),%ecx
    1800154cc:	call   *0x4f07e(%rip)        # 0x180064550
    1800154d2:	mov    %rax,%r8
-   1800154d5:	lea    0x4f42c(%rip),%rdx        # 0x180064908
+   1800154d5:	lea    0x4f424(%rip),%rdx        # 0x180064900
    1800154dc:	lea    0x40(%rsp),%rcx
    1800154e1:	call   0x18000c010
    1800154e6:	nop
    1800154e7:	mov    %rax,%rdx
    1800154ea:	lea    0x28(%rsp),%rcx
    1800154ef:	call   0x1800086c0
    1800154f4:	lea    0x5d225(%rip),%rdx        # 0x180072720
@@ -39990,15 +39990,15 @@
    180015505:	nop
    180015506:	call   0x18000b580
    18001550b:	int3
    18001550c:	call   *0x4f026(%rip)        # 0x180064538
    180015512:	mov    (%rax),%ecx
    180015514:	call   *0x4f036(%rip)        # 0x180064550
    18001551a:	mov    %rax,%r8
-   18001551d:	lea    0x4f3e4(%rip),%rdx        # 0x180064908
+   18001551d:	lea    0x4f3dc(%rip),%rdx        # 0x180064900
    180015524:	lea    0x40(%rsp),%rcx
    180015529:	call   0x18000c010
    18001552e:	nop
    18001552f:	mov    %rax,%rdx
    180015532:	lea    0x28(%rsp),%rcx
    180015537:	call   0x1800086c0
    18001553c:	lea    0x5d1dd(%rip),%rdx        # 0x180072720
@@ -40560,15 +40560,15 @@
    180015d80:	cmp    %rcx,%r15
    180015d83:	jbe    0x180015dbf
    180015d85:	mov    $0x2,%ecx
    180015d8a:	call   *0x4e880(%rip)        # 0x180064610
    180015d90:	mov    $0xac1,%r9d
    180015d96:	lea    0x4eee3(%rip),%r8        # 0x180064c80
    180015d9d:	mov    %rax,%rcx
-   180015da0:	lea    0x4eac1(%rip),%rdx        # 0x180064868
+   180015da0:	lea    0x4eab9(%rip),%rdx        # 0x180064860
    180015da7:	lea    0x4ff9a(%rip),%rax        # 0x180065d48
    180015dae:	mov    %rax,0x20(%rsp)
    180015db3:	call   0x180015760
    180015db8:	call   *0x4e79a(%rip)        # 0x180064558
    180015dbe:	int3
    180015dbf:	mov    %r15,%rax
    180015dc2:	mov    0x18ff0(%rbp),%rcx
@@ -41199,15 +41199,15 @@
    180016742:	sub    $0xb8,%rsp
    180016749:	mov    0x6dd38(%rip),%rax        # 0x180084488
    180016750:	xor    %rsp,%rax
    180016753:	mov    %rax,-0x1(%rbp)
    180016757:	mov    0x7f(%rbp),%r13
    18001675b:	mov    %r8,%r12
    18001675e:	mov    %rcx,%rdi
-   180016761:	lea    0x4e568(%rip),%r8        # 0x180064cd0
+   180016761:	lea    0x4e564(%rip),%r8        # 0x180064ccc
    180016768:	lea    -0x21(%rbp),%rcx
    18001676c:	mov    %r9,%r15
    18001676f:	call   0x180007920
    180016774:	call   *0x4ddbe(%rip)        # 0x180064538
    18001677a:	mov    -0x21(%rbp),%rbx
    18001677e:	lea    -0x6d(%rbp),%rcx
    180016782:	xor    %r14d,%r14d
@@ -41304,16 +41304,16 @@
    180016922:	cmp    $0xffffffffffffffff,%rax
    180016926:	jne    0x180016960
    180016928:	lea    0x3(%rax),%ecx
    18001692b:	call   *0x4dcdf(%rip)        # 0x180064610
    180016931:	mov    $0x5b,%r9d
    180016937:	lea    0x4ded2(%rip),%r8        # 0x180064810
    18001693e:	mov    %rax,%rcx
-   180016941:	lea    0x4df20(%rip),%rdx        # 0x180064868
-   180016948:	lea    0x4df61(%rip),%rax        # 0x1800648b0
+   180016941:	lea    0x4df18(%rip),%rdx        # 0x180064860
+   180016948:	lea    0x4df59(%rip),%rax        # 0x1800648a8
    18001694f:	mov    %rax,0x20(%rsp)
    180016954:	call   0x180015760
    180016959:	call   *0x4dbf9(%rip)        # 0x180064558
    18001695f:	int3
    180016960:	mov    -0x19(%rbp),%rsi
    180016964:	mov    0x1540(%rdi),%r14
    18001696b:	sub    %rax,%rsi
@@ -41392,77 +41392,77 @@
    180016a99:	pop    %r13
    180016a9b:	pop    %r12
    180016a9d:	pop    %rdi
    180016a9e:	pop    %rsi
    180016a9f:	pop    %rbx
    180016aa0:	pop    %rbp
    180016aa1:	ret
-   180016aa2:	lea    0x4de37(%rip),%rdx        # 0x1800648e0
+   180016aa2:	lea    0x4de2f(%rip),%rdx        # 0x1800648d8
    180016aa9:	lea    -0x21(%rbp),%rcx
    180016aad:	call   0x180007010
    180016ab2:	mov    %rax,%rdx
    180016ab5:	lea    -0x69(%rbp),%rcx
    180016ab9:	call   0x1800086c0
    180016abe:	lea    0x5bc5b(%rip),%rdx        # 0x180072720
    180016ac5:	lea    -0x69(%rbp),%rcx
    180016ac9:	call   0x180062722
    180016ace:	int3
    180016acf:	call   *0x4da63(%rip)        # 0x180064538
    180016ad5:	mov    (%rax),%ecx
    180016ad7:	call   *0x4da73(%rip)        # 0x180064550
    180016add:	mov    %rax,%r8
-   180016ae0:	lea    0x4dde9(%rip),%rdx        # 0x1800648d0
+   180016ae0:	lea    0x4dde1(%rip),%rdx        # 0x1800648c8
    180016ae7:	lea    -0x21(%rbp),%rcx
    180016aeb:	call   0x18000c010
    180016af0:	mov    %rax,%rdx
    180016af3:	lea    -0x69(%rbp),%rcx
    180016af7:	call   0x1800086c0
    180016afc:	lea    0x5bc1d(%rip),%rdx        # 0x180072720
    180016b03:	lea    -0x69(%rbp),%rcx
    180016b07:	call   0x180062722
    180016b0c:	int3
-   180016b0d:	lea    0x4ddcc(%rip),%rdx        # 0x1800648e0
+   180016b0d:	lea    0x4ddc4(%rip),%rdx        # 0x1800648d8
    180016b14:	lea    -0x21(%rbp),%rcx
    180016b18:	call   0x180007010
    180016b1d:	mov    %rax,%rdx
    180016b20:	lea    -0x69(%rbp),%rcx
    180016b24:	call   0x1800086c0
    180016b29:	lea    0x5bbf0(%rip),%rdx        # 0x180072720
    180016b30:	lea    -0x69(%rbp),%rcx
    180016b34:	call   0x180062722
    180016b39:	int3
    180016b3a:	call   *0x4d9f8(%rip)        # 0x180064538
    180016b40:	mov    (%rax),%ecx
    180016b42:	call   *0x4da08(%rip)        # 0x180064550
    180016b48:	mov    %rax,%r8
-   180016b4b:	lea    0x4dd7e(%rip),%rdx        # 0x1800648d0
+   180016b4b:	lea    0x4dd76(%rip),%rdx        # 0x1800648c8
    180016b52:	lea    -0x21(%rbp),%rcx
    180016b56:	call   0x18000c010
    180016b5b:	mov    %rax,%rdx
    180016b5e:	lea    -0x69(%rbp),%rcx
    180016b62:	call   0x1800086c0
    180016b67:	lea    0x5bbb2(%rip),%rdx        # 0x180072720
    180016b6e:	lea    -0x69(%rbp),%rcx
    180016b72:	call   0x180062722
    180016b77:	int3
-   180016b78:	lea    0x4dd61(%rip),%rdx        # 0x1800648e0
+   180016b78:	lea    0x4dd59(%rip),%rdx        # 0x1800648d8
    180016b7f:	lea    -0x21(%rbp),%rcx
    180016b83:	call   0x180007010
    180016b88:	mov    %rax,%rdx
    180016b8b:	lea    -0x69(%rbp),%rcx
    180016b8f:	call   0x1800086c0
    180016b94:	lea    0x5bb85(%rip),%rdx        # 0x180072720
    180016b9b:	lea    -0x69(%rbp),%rcx
    180016b9f:	call   0x180062722
    180016ba4:	int3
    180016ba5:	call   *0x4d98d(%rip)        # 0x180064538
    180016bab:	mov    (%rax),%ecx
    180016bad:	call   *0x4d99d(%rip)        # 0x180064550
    180016bb3:	mov    %rax,%r8
-   180016bb6:	lea    0x4dd13(%rip),%rdx        # 0x1800648d0
+   180016bb6:	lea    0x4dd0b(%rip),%rdx        # 0x1800648c8
    180016bbd:	lea    -0x21(%rbp),%rcx
    180016bc1:	call   0x18000c010
    180016bc6:	mov    %rax,%rdx
    180016bc9:	lea    -0x69(%rbp),%rcx
    180016bcd:	call   0x1800086c0
    180016bd2:	lea    0x5bb47(%rip),%rdx        # 0x180072720
    180016bd9:	lea    -0x69(%rbp),%rcx
@@ -43618,85 +43618,85 @@
    180018b9d:	ret
    180018b9e:	call   *0x4b9fc(%rip)        # 0x1800645a0
    180018ba4:	int3
    180018ba5:	call   *0x4b98d(%rip)        # 0x180064538
    180018bab:	mov    (%rax),%ecx
    180018bad:	call   *0x4b99d(%rip)        # 0x180064550
    180018bb3:	mov    %rax,%r8
-   180018bb6:	lea    0x4bd4b(%rip),%rdx        # 0x180064908
+   180018bb6:	lea    0x4bd43(%rip),%rdx        # 0x180064900
    180018bbd:	lea    -0x38(%rbp),%rcx
    180018bc1:	call   0x18000c010
    180018bc6:	mov    %rax,%rdx
    180018bc9:	lea    -0x50(%rbp),%rcx
    180018bcd:	call   0x1800086c0
    180018bd2:	lea    0x59b47(%rip),%rdx        # 0x180072720
    180018bd9:	lea    -0x50(%rbp),%rcx
    180018bdd:	call   0x180062722
    180018be2:	int3
    180018be3:	call   *0x4b94f(%rip)        # 0x180064538
    180018be9:	mov    (%rax),%ecx
    180018beb:	call   *0x4b95f(%rip)        # 0x180064550
    180018bf1:	mov    %rax,%r8
-   180018bf4:	lea    0x4bd0d(%rip),%rdx        # 0x180064908
+   180018bf4:	lea    0x4bd05(%rip),%rdx        # 0x180064900
    180018bfb:	lea    -0x38(%rbp),%rcx
    180018bff:	call   0x18000c010
    180018c04:	mov    %rax,%rdx
    180018c07:	lea    -0x50(%rbp),%rcx
    180018c0b:	call   0x1800086c0
    180018c10:	lea    0x59b09(%rip),%rdx        # 0x180072720
    180018c17:	lea    -0x50(%rbp),%rcx
    180018c1b:	call   0x180062722
    180018c20:	int3
    180018c21:	call   *0x4b911(%rip)        # 0x180064538
    180018c27:	mov    (%rax),%ecx
    180018c29:	call   *0x4b921(%rip)        # 0x180064550
    180018c2f:	mov    %rax,%r8
-   180018c32:	lea    0x4bccf(%rip),%rdx        # 0x180064908
+   180018c32:	lea    0x4bcc7(%rip),%rdx        # 0x180064900
    180018c39:	lea    -0x38(%rbp),%rcx
    180018c3d:	call   0x18000c010
    180018c42:	mov    %rax,%rdx
    180018c45:	lea    -0x50(%rbp),%rcx
    180018c49:	call   0x1800086c0
    180018c4e:	lea    0x59acb(%rip),%rdx        # 0x180072720
    180018c55:	lea    -0x50(%rbp),%rcx
    180018c59:	call   0x180062722
    180018c5e:	int3
    180018c5f:	call   *0x4b8d3(%rip)        # 0x180064538
    180018c65:	mov    (%rax),%ecx
    180018c67:	call   *0x4b8e3(%rip)        # 0x180064550
    180018c6d:	mov    %rax,%r8
-   180018c70:	lea    0x4bc91(%rip),%rdx        # 0x180064908
+   180018c70:	lea    0x4bc89(%rip),%rdx        # 0x180064900
    180018c77:	lea    -0x38(%rbp),%rcx
    180018c7b:	call   0x18000c010
    180018c80:	mov    %rax,%rdx
    180018c83:	lea    -0x50(%rbp),%rcx
    180018c87:	call   0x1800086c0
    180018c8c:	lea    0x59a8d(%rip),%rdx        # 0x180072720
    180018c93:	lea    -0x50(%rbp),%rcx
    180018c97:	call   0x180062722
    180018c9c:	int3
    180018c9d:	call   *0x4b895(%rip)        # 0x180064538
    180018ca3:	mov    (%rax),%ecx
    180018ca5:	call   *0x4b8a5(%rip)        # 0x180064550
    180018cab:	mov    %rax,%r8
-   180018cae:	lea    0x4bc53(%rip),%rdx        # 0x180064908
+   180018cae:	lea    0x4bc4b(%rip),%rdx        # 0x180064900
    180018cb5:	lea    -0x38(%rbp),%rcx
    180018cb9:	call   0x18000c010
    180018cbe:	mov    %rax,%rdx
    180018cc1:	lea    -0x50(%rbp),%rcx
    180018cc5:	call   0x1800086c0
    180018cca:	lea    0x59a4f(%rip),%rdx        # 0x180072720
    180018cd1:	lea    -0x50(%rbp),%rcx
    180018cd5:	call   0x180062722
    180018cda:	int3
    180018cdb:	call   *0x4b857(%rip)        # 0x180064538
    180018ce1:	mov    (%rax),%ecx
    180018ce3:	call   *0x4b867(%rip)        # 0x180064550
    180018ce9:	mov    %rax,%r8
-   180018cec:	lea    0x4bc15(%rip),%rdx        # 0x180064908
+   180018cec:	lea    0x4bc0d(%rip),%rdx        # 0x180064900
    180018cf3:	lea    -0x38(%rbp),%rcx
    180018cf7:	call   0x18000c010
    180018cfc:	mov    %rax,%rdx
    180018cff:	lea    -0x50(%rbp),%rcx
    180018d03:	call   0x1800086c0
    180018d08:	lea    0x59a11(%rip),%rdx        # 0x180072720
    180018d0f:	lea    -0x50(%rbp),%rcx
@@ -43922,15 +43922,15 @@
    180019091:	test   %al,%al
    180019093:	je     0x1800190cf
    180019095:	mov    $0x2,%ecx
    18001909a:	call   *0x4b570(%rip)        # 0x180064610
    1800190a0:	mov    $0xad6,%r9d
    1800190a6:	lea    0x4bbd3(%rip),%r8        # 0x180064c80
    1800190ad:	mov    %rax,%rcx
-   1800190b0:	lea    0x4b7b1(%rip),%rdx        # 0x180064868
+   1800190b0:	lea    0x4b7a9(%rip),%rdx        # 0x180064860
    1800190b7:	lea    0x4cca2(%rip),%rax        # 0x180065d60
    1800190be:	mov    %rax,0x20(%rsp)
    1800190c3:	call   0x180015760
    1800190c8:	call   *0x4b48a(%rip)        # 0x180064558
    1800190ce:	int3
    1800190cf:	mov    0x17ff0(%rbp),%rax
    1800190d6:	movslq 0x4(%rax),%rcx
@@ -43961,15 +43961,15 @@
    18001916e:	cmp    %rdi,%rax
    180019171:	je     0x1800191ad
    180019173:	mov    $0x2,%ecx
    180019178:	call   *0x4b492(%rip)        # 0x180064610
    18001917e:	mov    $0xae1,%r9d
    180019184:	lea    0x4baf5(%rip),%r8        # 0x180064c80
    18001918b:	mov    %rax,%rcx
-   18001918e:	lea    0x4b6d3(%rip),%rdx        # 0x180064868
+   18001918e:	lea    0x4b6cb(%rip),%rdx        # 0x180064860
    180019195:	lea    0x4cbdc(%rip),%rax        # 0x180065d78
    18001919c:	mov    %rax,0x20(%rsp)
    1800191a1:	call   0x180015760
    1800191a6:	call   *0x4b3ac(%rip)        # 0x180064558
    1800191ac:	int3
    1800191ad:	test   %rbx,%rbx
    1800191b0:	je     0x1800191d0
@@ -43990,15 +43990,15 @@
    1800191f1:	cmp    %rdi,%rax
    1800191f4:	je     0x180019230
    1800191f6:	mov    $0x2,%ecx
    1800191fb:	call   *0x4b40f(%rip)        # 0x180064610
    180019201:	mov    $0xaf1,%r9d
    180019207:	lea    0x4ba72(%rip),%r8        # 0x180064c80
    18001920e:	mov    %rax,%rcx
-   180019211:	lea    0x4b650(%rip),%rdx        # 0x180064868
+   180019211:	lea    0x4b648(%rip),%rdx        # 0x180064860
    180019218:	lea    0x4cb81(%rip),%rax        # 0x180065da0
    18001921f:	mov    %rax,0x20(%rsp)
    180019224:	call   0x180015760
    180019229:	call   *0x4b329(%rip)        # 0x180064558
    18001922f:	int3
    180019230:	test   %rdi,%rdi
    180019233:	je     0x18001924b
@@ -44021,15 +44021,15 @@
    180019280:	cmp    %rax,0x1448(%r15)
    180019287:	je     0x1800192c3
    180019289:	mov    $0x2,%ecx
    18001928e:	call   *0x4b37c(%rip)        # 0x180064610
    180019294:	mov    $0xb08,%r9d
    18001929a:	lea    0x4b9df(%rip),%r8        # 0x180064c80
    1800192a1:	mov    %rax,%rcx
-   1800192a4:	lea    0x4b5bd(%rip),%rdx        # 0x180064868
+   1800192a4:	lea    0x4b5b5(%rip),%rdx        # 0x180064860
    1800192ab:	lea    0x4cb1e(%rip),%rax        # 0x180065dd0
    1800192b2:	mov    %rax,0x20(%rsp)
    1800192b7:	call   0x180015760
    1800192bc:	call   *0x4b296(%rip)        # 0x180064558
    1800192c2:	int3
    1800192c3:	mov    0x1428(%r15),%rcx
    1800192ca:	call   0x18003b060
@@ -44143,15 +44143,15 @@
    1800194c4:	cmp    %rcx,%rbx
    1800194c7:	jbe    0x180019503
    1800194c9:	mov    $0x2,%ecx
    1800194ce:	call   *0x4b13c(%rip)        # 0x180064610
    1800194d4:	mov    $0xb2f,%r9d
    1800194da:	lea    0x4b79f(%rip),%r8        # 0x180064c80
    1800194e1:	mov    %rax,%rcx
-   1800194e4:	lea    0x4b37d(%rip),%rdx        # 0x180064868
+   1800194e4:	lea    0x4b375(%rip),%rdx        # 0x180064860
    1800194eb:	lea    0x4c8fe(%rip),%rax        # 0x180065df0
    1800194f2:	mov    %rax,0x20(%rsp)
    1800194f7:	call   0x180015760
    1800194fc:	call   *0x4b056(%rip)        # 0x180064558
    180019502:	int3
    180019503:	mov    %rbx,%rax
    180019506:	mov    0x18ff0(%rbp),%rcx
@@ -118082,171 +118082,168 @@
    180064819:	jae    0x180064848
    18006481b:	jb     0x180064892
    18006481d:	outsb  %ds:(%rsi),(%dx)
    18006481e:	outsb  %ds:(%rsi),(%dx)
    18006481f:	gs jb  0x18006487e
    180064822:	(bad)
    180064827:	sub    $0x6c697562,%eax
-   18006482c:	fs sub $0x5c77656e,%eax
-   180064832:	pop    %rdi
-   180064833:	ja     0x1800648a4
-   180064835:	jb     0x1800648a2
-   180064837:	pop    %rsp
-   180064838:	imul   $0x6c6c2d78,0x65(%rax),%esi
-   18006483f:	insl   (%dx),%es:(%rdi)
-   180064840:	pop    %rsp
-   180064841:	imul   $0x6c6c2d78,0x65(%rax),%esi
-   180064848:	insl   (%dx),%es:(%rdi)
-   180064849:	pop    %rsp
-   18006484a:	jae    0x1800648be
-   18006484c:	movsxd 0x6c(%rsp,%rbp,2),%ebx
-   180064850:	(bad)
-   180064851:	insl   (%dx),%es:(%rdi)
+   18006482c:	fs pop %rsp
+   18006482e:	pop    %rdi
+   18006482f:	ja     0x1800648a0
+   180064831:	jb     0x18006489e
+   180064833:	pop    %rsp
+   180064834:	imul   $0x6c6c2d78,0x65(%rax),%esi
+   18006483b:	insl   (%dx),%es:(%rdi)
+   18006483c:	pop    %rsp
+   18006483d:	imul   $0x6c6c2d78,0x65(%rax),%esi
+   180064844:	insl   (%dx),%es:(%rdi)
+   180064845:	pop    %rsp
+   180064846:	jae    0x1800648ba
+   180064848:	movsxd 0x6c(%rsp,%rbp,2),%ebx
+   18006484c:	(bad)
+   18006484d:	insl   (%dx),%es:(%rdi)
+   18006484e:	(bad)
+   18006484f:	pop    %rsp
+   180064850:	insb   (%dx),%es:(%rdi)
+   180064851:	insb   (%dx),%es:(%rdi)
    180064852:	(bad)
-   180064853:	pop    %rsp
-   180064854:	insb   (%dx),%es:(%rdi)
-   180064855:	insb   (%dx),%es:(%rdi)
-   180064856:	(bad)
-   180064857:	insl   (%dx),%es:(%rdi)
-   180064858:	(bad)
-   180064859:	sub    $0x6c697475,%eax
-   18006485e:	cs push $0x0
-   180064864:	add    %al,(%rax)
-   180064866:	add    %al,(%rax)
-   180064868:	rex.WR
-   180064869:	rex.WR
-   18006486a:	rex.B
-   18006486b:	rex.WRB
-   18006486c:	pop    %r15
-   18006486e:	push   %r11
-   180064870:	push   %rbx
-   180064871:	rex.RB push %r10
-   180064873:	push   %rsp
-   180064874:	cmp    (%rax),%ah
-   180064876:	and    $0x64253a73,%eax
-   18006487b:	cmp    (%rax),%ah
-   18006487d:	and    $0xa73,%eax
-   180064882:	add    %al,(%rax)
-   180064884:	add    %al,(%rax)
-   180064886:	add    %al,(%rax)
-   180064888:	jae    0x1800648f3
-   18006488a:	jp     0x1800648f1
-   18006488c:	xor    (%rax),%ah
-   18006488e:	cmp    $0x6973203d,%eax
-   180064893:	jp     0x1800648fa
-   180064895:	add    %al,(%rax)
-   180064897:	add    %ah,0x61(%rsi)
-   18006489a:	imul   $0x206f7420,0x64(%rbp,%riz,2),%ebp
-   1800648a2:	outsl  %ds:(%rsi),(%dx)
-   1800648a3:	jo     0x18006490a
-   1800648a5:	outsb  %ds:(%rsi),(%dx)
-   1800648a6:	and    %ah,0x25203a73(%rip)        # 0x1a526831f
-   1800648ac:	jae    0x1800648ae
-   1800648ae:	add    %al,(%rax)
-   1800648b0:	jb     0x180064917
-   1800648b2:	je     0x1800648d4
-   1800648b4:	and    %edi,0x312d20(%rip)        # 0x1803775da
-   1800648ba:	add    %al,(%rax)
-   1800648bc:	add    %al,(%rax)
-   1800648be:	add    %al,(%rax)
-   1800648c0:	jb     0x180064927
-   1800648c2:	je     0x1800648e4
-   1800648c4:	cmp    $0x30203d,%eax
-   1800648c9:	add    %al,(%rax)
-   1800648cb:	add    %al,(%rax)
-   1800648cd:	add    %al,(%rax)
-   1800648cf:	add    %dh,0x65(%rdx)
-   1800648d2:	(bad)
-   1800648d3:	and    %ah,%fs:0x72(%rbp)
-   1800648d7:	jb     0x180064948
-   1800648d9:	jb     0x180064915
-   1800648db:	and    %ah,0x75000073(%rip)        # 0x1f5064954
-   1800648e1:	outsb  %ds:(%rsi),(%dx)
-   1800648e2:	gs js  0x180064955
-   1800648e5:	movsxd %gs:0x64(%rbp,%riz,2),%esi
-   1800648ea:	insb   (%dx),%es:(%rdi)
-   1800648eb:	jns    0x18006490d
-   1800648ed:	jb     0x180064954
-   1800648ef:	(bad)
-   1800648f0:	movsxd 0x65(%rax),%ebp
-   1800648f3:	and    %ah,%fs:0x6e(%rbp)
-   1800648f7:	and    %ch,%fs:0x66(%rdi)
-   1800648fb:	and    %ah,0x69(%rsi)
-   1800648fe:	insb   (%dx),%es:(%rdi)
-   1800648ff:	add    %al,%gs:(%rax)
-   180064902:	add    %al,(%rax)
-   180064904:	add    %al,(%rax)
-   180064906:	add    %al,(%rax)
-   180064908:	ja     0x18006497c
-   18006490a:	imul   $0x6f727265,0x20(%rbp,%riz,2),%esi
-   180064912:	jb     0x18006494e
-   180064914:	and    %ah,0x6f460073(%rip)        # 0x1ef4c498d
-   18006491a:	jb     0x180064989
-   18006491c:	(bad)
-   18006491d:	je     0x18006496c
-   18006491f:	gs jae 0x180064995
-   180064922:	(bad)
-   180064923:	and    %spl,%gs:0x61(%r14d)
-   180064929:	imul   $0x43000000,0x64(%rbp,%riz,2),%ebp
-   180064931:	jb     0x180064998
-   180064933:	(bad)
-   180064934:	je     0x18006499b
-   180064936:	imul   $0x69707061,0x4d(%rbp,%r12,2),%r13d
-   18006493f:	outsb  %ds:(%rsi),(%dx)
-   180064940:	and    %spl,0x61(%r14d)
-   180064945:	imul   $0x7325203a,0x64(%rbp,%riz,2),%ebp
-   18006494d:	add    %al,(%rax)
-   18006494f:	add    %cl,0x61(%rbp)
-   180064952:	jo     0x1800649aa
-   180064954:	imul   $0x6946664f,0x77(%rbp),%esp
-   18006495b:	insb   (%dx),%es:(%rdi)
-   18006495c:	and    %ah,%gs:0x61(%rsi)
-   180064960:	imul   $0x7325203a,0x64(%rbp,%riz,2),%ebp
+   180064853:	insl   (%dx),%es:(%rdi)
+   180064854:	(bad)
+   180064855:	sub    $0x6c697475,%eax
+   18006485a:	cs push $0x0
+   180064860:	rex.WR
+   180064861:	rex.WR
+   180064862:	rex.B
+   180064863:	rex.WRB
+   180064864:	pop    %r15
+   180064866:	push   %r11
+   180064868:	push   %rbx
+   180064869:	rex.RB push %r10
+   18006486b:	push   %rsp
+   18006486c:	cmp    (%rax),%ah
+   18006486e:	and    $0x64253a73,%eax
+   180064873:	cmp    (%rax),%ah
+   180064875:	and    $0xa73,%eax
+   18006487a:	add    %al,(%rax)
+   18006487c:	add    %al,(%rax)
+   18006487e:	add    %al,(%rax)
+   180064880:	jae    0x1800648eb
+   180064882:	jp     0x1800648e9
+   180064884:	xor    (%rax),%ah
+   180064886:	cmp    $0x6973203d,%eax
+   18006488b:	jp     0x1800648f2
+   18006488d:	add    %al,(%rax)
+   18006488f:	add    %ah,0x61(%rsi)
+   180064892:	imul   $0x206f7420,0x64(%rbp,%riz,2),%ebp
+   18006489a:	outsl  %ds:(%rsi),(%dx)
+   18006489b:	jo     0x180064902
+   18006489d:	outsb  %ds:(%rsi),(%dx)
+   18006489e:	and    %ah,0x25203a73(%rip)        # 0x1a5268317
+   1800648a4:	jae    0x1800648a6
+   1800648a6:	add    %al,(%rax)
+   1800648a8:	jb     0x18006490f
+   1800648aa:	je     0x1800648cc
+   1800648ac:	and    %edi,0x312d20(%rip)        # 0x1803775d2
+   1800648b2:	add    %al,(%rax)
+   1800648b4:	add    %al,(%rax)
+   1800648b6:	add    %al,(%rax)
+   1800648b8:	jb     0x18006491f
+   1800648ba:	je     0x1800648dc
+   1800648bc:	cmp    $0x30203d,%eax
+   1800648c1:	add    %al,(%rax)
+   1800648c3:	add    %al,(%rax)
+   1800648c5:	add    %al,(%rax)
+   1800648c7:	add    %dh,0x65(%rdx)
+   1800648ca:	(bad)
+   1800648cb:	and    %ah,%fs:0x72(%rbp)
+   1800648cf:	jb     0x180064940
+   1800648d1:	jb     0x18006490d
+   1800648d3:	and    %ah,0x75000073(%rip)        # 0x1f506494c
+   1800648d9:	outsb  %ds:(%rsi),(%dx)
+   1800648da:	gs js  0x18006494d
+   1800648dd:	movsxd %gs:0x64(%rbp,%riz,2),%esi
+   1800648e2:	insb   (%dx),%es:(%rdi)
+   1800648e3:	jns    0x180064905
+   1800648e5:	jb     0x18006494c
+   1800648e7:	(bad)
+   1800648e8:	movsxd 0x65(%rax),%ebp
+   1800648eb:	and    %ah,%fs:0x6e(%rbp)
+   1800648ef:	and    %ch,%fs:0x66(%rdi)
+   1800648f3:	and    %ah,0x69(%rsi)
+   1800648f6:	insb   (%dx),%es:(%rdi)
+   1800648f7:	add    %al,%gs:(%rax)
+   1800648fa:	add    %al,(%rax)
+   1800648fc:	add    %al,(%rax)
+   1800648fe:	add    %al,(%rax)
+   180064900:	ja     0x180064974
+   180064902:	imul   $0x6f727265,0x20(%rbp,%riz,2),%esi
+   18006490a:	jb     0x180064946
+   18006490c:	and    %ah,0x6f460073(%rip)        # 0x1ef4c4985
+   180064912:	jb     0x180064981
+   180064914:	(bad)
+   180064915:	je     0x180064964
+   180064917:	gs jae 0x18006498d
+   18006491a:	(bad)
+   18006491b:	and    %spl,%gs:0x61(%r14d)
+   180064921:	imul   $0x43000000,0x64(%rbp,%riz,2),%ebp
+   180064929:	jb     0x180064990
+   18006492b:	(bad)
+   18006492c:	je     0x180064993
+   18006492e:	imul   $0x69707061,0x4d(%rbp,%r12,2),%r13d
+   180064937:	outsb  %ds:(%rsi),(%dx)
+   180064938:	and    %spl,0x61(%r14d)
+   18006493d:	imul   $0x7325203a,0x64(%rbp,%riz,2),%ebp
+   180064945:	add    %al,(%rax)
+   180064947:	add    %cl,0x61(%rbp)
+   18006494a:	jo     0x1800649a2
+   18006494c:	imul   $0x6946664f,0x77(%rbp),%esp
+   180064953:	insb   (%dx),%es:(%rdi)
+   180064954:	and    %ah,%gs:0x61(%rsi)
+   180064958:	imul   $0x7325203a,0x64(%rbp,%riz,2),%ebp
+	...
+   180064968:	ja     0x1800649cb
+   18006496a:	jb     0x1800649da
+   18006496c:	imul   $0x7250203a,0x67(%rsi),%ebp
+   180064973:	gs data16 gs je 0x1800649db
+   180064978:	push   $0x74726956
+   18006497d:	jne    0x1800649e0
+   18006497f:	insb   (%dx),%es:(%rdi)
+   180064980:	rex.WRB
+   180064981:	gs insl (%dx),%es:(%rdi)
+   180064983:	outsl  %ds:(%rsi),(%dx)
+   180064984:	jb     0x1800649ff
+   180064986:	and    %ah,0x61(%rsi)
+   180064989:	imul   $0x7325203a,0x64(%rbp,%riz,2),%ebp
+   180064991:	or     (%rax),%al
+   180064993:	add    %al,(%rax)
+   180064995:	add    %al,(%rax)
+   180064997:	add    %dh,0x61(%rdi)
+   18006499a:	jb     0x180064a0a
+   18006499c:	imul   $0x6e55203a,0x67(%rsi),%ebp
+   1800649a3:	insl   (%dx),%es:(%rdi)
+   1800649a4:	(bad)
+   1800649a5:	jo     0x1800649fd
+   1800649a7:	imul   $0x6946664f,0x77(%rbp),%esp
+   1800649ae:	insb   (%dx),%es:(%rdi)
+   1800649af:	and    %ah,%gs:0x61(%rsi)
+   1800649b3:	imul   $0x7325203a,0x64(%rbp,%riz,2),%ebp
+   1800649bb:	or     (%rax),%al
+   1800649bd:	add    %al,(%rax)
+   1800649bf:	add    %ah,0x64(%rcx)
+   1800649c2:	fs jb  0x1800649e5
+   1800649c5:	cmp    $0x554e203d,%eax
+   1800649ca:	rex.WR
+   1800649cb:	rex.WR and %r12b,(%rsi)
+   1800649ce:	es and %dh,0x69(%rbx)
+   1800649d2:	jp     0x180064a39
+   1800649d4:	and    %bh,0x30203d(%rip)        # 0x180366a17
+   1800649da:	add    %al,(%rax)
+   1800649dc:	(bad)
+   1800649dd:	fs fs jb 0x1800649e1
 	...
-   180064970:	ja     0x1800649d3
-   180064972:	jb     0x1800649e2
-   180064974:	imul   $0x7250203a,0x67(%rsi),%ebp
-   18006497b:	gs data16 gs je 0x1800649e3
-   180064980:	push   $0x74726956
-   180064985:	jne    0x1800649e8
-   180064987:	insb   (%dx),%es:(%rdi)
-   180064988:	rex.WRB
-   180064989:	gs insl (%dx),%es:(%rdi)
-   18006498b:	outsl  %ds:(%rsi),(%dx)
-   18006498c:	jb     0x180064a07
-   18006498e:	and    %ah,0x61(%rsi)
-   180064991:	imul   $0x7325203a,0x64(%rbp,%riz,2),%ebp
-   180064999:	or     (%rax),%al
-   18006499b:	add    %al,(%rax)
-   18006499d:	add    %al,(%rax)
-   18006499f:	add    %dh,0x61(%rdi)
-   1800649a2:	jb     0x180064a12
-   1800649a4:	imul   $0x6e55203a,0x67(%rsi),%ebp
-   1800649ab:	insl   (%dx),%es:(%rdi)
-   1800649ac:	(bad)
-   1800649ad:	jo     0x180064a05
-   1800649af:	imul   $0x6946664f,0x77(%rbp),%esp
-   1800649b6:	insb   (%dx),%es:(%rdi)
-   1800649b7:	and    %ah,%gs:0x61(%rsi)
-   1800649bb:	imul   $0x7325203a,0x64(%rbp,%riz,2),%ebp
-   1800649c3:	or     (%rax),%al
-   1800649c5:	add    %al,(%rax)
-   1800649c7:	add    %ah,0x64(%rcx)
-   1800649ca:	fs jb  0x1800649ed
-   1800649cd:	cmp    $0x554e203d,%eax
-   1800649d2:	rex.WR
-   1800649d3:	rex.WR and %r12b,(%rsi)
-   1800649d6:	es and %dh,0x69(%rbx)
-   1800649da:	jp     0x180064a41
-   1800649dc:	and    %bh,0x30203d(%rip)        # 0x180366a1f
-   1800649e2:	add    %al,(%rax)
-   1800649e4:	(bad)
-   1800649e5:	fs fs jb 0x1800649e9
-   1800649e9:	add    %al,(%rax)
-   1800649eb:	add    %al,(%rax)
    1800649ed:	add    %al,(%rax)
    1800649ef:	add    %dh,0x61(%rdi)
    1800649f2:	jb     0x180064a62
    1800649f4:	imul   $0x6166203a,0x67(%rsi),%ebp
    1800649fb:	imul   $0x206f7420,0x64(%rbp,%riz,2),%ebp
    180064a03:	push   %rsi
    180064a04:	imul   $0x4c6c6175,0x74(%rdx),%esi
@@ -118471,53 +118468,50 @@
    180064c89:	jae    0x180064cb8
    180064c8b:	jb     0x180064d02
    180064c8d:	outsb  %ds:(%rsi),(%dx)
    180064c8e:	outsb  %ds:(%rsi),(%dx)
    180064c8f:	gs jb  0x180064cee
    180064c92:	(bad)
    180064c97:	sub    $0x6c697562,%eax
-   180064c9c:	fs sub $0x5c77656e,%eax
-   180064ca2:	pop    %rdi
-   180064ca3:	ja     0x180064d14
-   180064ca5:	jb     0x180064d12
-   180064ca7:	pop    %rsp
-   180064ca8:	imul   $0x6c6c2d78,0x65(%rax),%esi
-   180064caf:	insl   (%dx),%es:(%rdi)
-   180064cb0:	pop    %rsp
-   180064cb1:	imul   $0x6c6c2d78,0x65(%rax),%esi
-   180064cb8:	insl   (%dx),%es:(%rdi)
-   180064cb9:	pop    %rsp
-   180064cba:	jae    0x180064d2e
-   180064cbc:	movsxd 0x6c(%rsp,%rbp,2),%ebx
-   180064cc0:	(bad)
-   180064cc1:	insl   (%dx),%es:(%rdi)
+   180064c9c:	fs pop %rsp
+   180064c9e:	pop    %rdi
+   180064c9f:	ja     0x180064d10
+   180064ca1:	jb     0x180064d0e
+   180064ca3:	pop    %rsp
+   180064ca4:	imul   $0x6c6c2d78,0x65(%rax),%esi
+   180064cab:	insl   (%dx),%es:(%rdi)
+   180064cac:	pop    %rsp
+   180064cad:	imul   $0x6c6c2d78,0x65(%rax),%esi
+   180064cb4:	insl   (%dx),%es:(%rdi)
+   180064cb5:	pop    %rsp
+   180064cb6:	jae    0x180064d2a
+   180064cb8:	movsxd 0x6c(%rsp,%rbp,2),%ebx
+   180064cbc:	(bad)
+   180064cbd:	insl   (%dx),%es:(%rdi)
+   180064cbe:	(bad)
+   180064cbf:	pop    %rsp
+   180064cc0:	insb   (%dx),%es:(%rdi)
+   180064cc1:	insb   (%dx),%es:(%rdi)
    180064cc2:	(bad)
-   180064cc3:	pop    %rsp
-   180064cc4:	insb   (%dx),%es:(%rdi)
-   180064cc5:	insb   (%dx),%es:(%rdi)
-   180064cc6:	(bad)
-   180064cc7:	insl   (%dx),%es:(%rdi)
-   180064cc8:	(bad)
-   180064cc9:	cs movsxd 0x70(%rax),%esi
-   180064ccd:	add    %al,(%rax)
-   180064ccf:	add    %dh,0x62(%rdx)
-   180064cd2:	add    %al,(%rax)
-   180064cd4:	add    %al,(%rax)
-   180064cd6:	add    %al,(%rax)
-   180064cd8:	(bad)
-   180064cdd:	sub    $0x3a6d6c6c,%eax
-   180064ce2:	and    %ch,0x61(%rdi,%rbp,2)
-   180064ce6:	imul   $0x646f6d20,%fs:0x67(%rsi),%ebp
-   180064cee:	gs insb (%dx),%es:(%rdi)
-   180064cf0:	and    %ah,0x72(%rsi)
-   180064cf3:	outsl  %ds:(%rsi),(%dx)
-   180064cf4:	insl   (%dx),%es:(%rdi)
-   180064cf5:	and    %ah,0xa73(%rip)        # 0x18006576e
-   180064cfb:	add    %al,(%rax)
-   180064cfd:	add    %al,(%rax)
+   180064cc3:	insl   (%dx),%es:(%rdi)
+   180064cc4:	(bad)
+   180064cc5:	cs movsxd 0x70(%rax),%esi
+   180064cc9:	add    %al,(%rax)
+   180064ccb:	add    %dh,0x62(%rdx)
+   180064cce:	add    %al,(%rax)
+   180064cd0:	(bad)
+   180064cd5:	sub    $0x3a6d6c6c,%eax
+   180064cda:	and    %ch,0x61(%rdi,%rbp,2)
+   180064cde:	imul   $0x646f6d20,%fs:0x67(%rsi),%ebp
+   180064ce6:	gs insb (%dx),%es:(%rdi)
+   180064ce8:	and    %ah,0x72(%rsi)
+   180064ceb:	outsl  %ds:(%rsi),(%dx)
+   180064cec:	insl   (%dx),%es:(%rdi)
+   180064ced:	and    %ah,0xa73(%rip)        # 0x180065766
+	...
    180064cff:	add    %dh,0x6e(%rbp)
    180064d02:	imul   $0x77,0x6f(%rsi),%ebp
    180064d06:	outsb  %ds:(%rsi),(%dx)
    180064d07:	and    %ch,(%rax)
    180064d09:	insl   (%dx),%es:(%rdi)
    180064d0a:	(bad)
    180064d0b:	imul   $0x72657620,0x2c(%ebx),%esp
@@ -124984,30 +124978,32 @@
    180069089:	jae    0x1800690b8
    18006908b:	jb     0x180069102
    18006908d:	outsb  %ds:(%rsi),(%dx)
    18006908e:	outsb  %ds:(%rsi),(%dx)
    18006908f:	gs jb  0x1800690ee
    180069092:	(bad)
    180069097:	sub    $0x6c697562,%eax
-   18006909c:	fs sub $0x5c77656e,%eax
-   1800690a2:	pop    %rdi
-   1800690a3:	ja     0x180069114
-   1800690a5:	jb     0x180069112
-   1800690a7:	pop    %rsp
-   1800690a8:	imul   $0x6c6c2d78,0x65(%rax),%esi
-   1800690af:	insl   (%dx),%es:(%rdi)
-   1800690b0:	pop    %rsp
-   1800690b1:	imul   $0x6c6c2d78,0x65(%rax),%esi
-   1800690b8:	insl   (%dx),%es:(%rdi)
-   1800690b9:	pop    %rsp
-   1800690ba:	jae    0x18006912e
-   1800690bc:	movsxd 0x67(%rdi,%riz,2),%ebx
-   1800690c0:	insl   (%dx),%es:(%rdi)
-   1800690c1:	insb   (%dx),%es:(%rdi)
-   1800690c2:	cs movsxd (%rax),%eax
+   18006909c:	fs pop %rsp
+   18006909e:	pop    %rdi
+   18006909f:	ja     0x180069110
+   1800690a1:	jb     0x18006910e
+   1800690a3:	pop    %rsp
+   1800690a4:	imul   $0x6c6c2d78,0x65(%rax),%esi
+   1800690ab:	insl   (%dx),%es:(%rdi)
+   1800690ac:	pop    %rsp
+   1800690ad:	imul   $0x6c6c2d78,0x65(%rax),%esi
+   1800690b4:	insl   (%dx),%es:(%rdi)
+   1800690b5:	pop    %rsp
+   1800690b6:	jae    0x18006912a
+   1800690b8:	movsxd 0x67(%rdi,%riz,2),%ebx
+   1800690bc:	insl   (%dx),%es:(%rdi)
+   1800690bd:	insb   (%dx),%es:(%rdi)
+   1800690be:	cs movsxd (%rax),%eax
+   1800690c1:	add    %al,(%rax)
+   1800690c3:	add    %al,(%rax)
    1800690c5:	add    %al,(%rax)
    1800690c7:	add    %al,0x47(%rdi)
    1800690ca:	rex.WRB
    1800690cb:	rex.WR pop %rdi
    1800690cd:	push   %r11
    1800690cf:	push   %rbx
    1800690d0:	rex.RB push %r10
@@ -128200,17 +128196,15 @@
    18006b114:	add    %eax,(%rax)
    18006b116:	add    %al,(%rax)
    18006b118:	rolb   $1,0x6(%rsi)
    18006b11b:	addb   $0x0,(%rcx)
    18006b11e:	add    %al,(%rax)
    18006b120:	add    %al,(%rax)
    18006b122:	add    %al,(%rax)
-   18006b124:	and    (%rax),%bh
-   18006b126:	pop    %rbx
-   18006b127:	data16 add %al,(%rax)
+   18006b124:	rorb   %cl,0x665c(%rcx)
    18006b12a:	add    %al,(%rax)
    18006b12c:	or     $0x50000000,%eax
    18006b131:	add    (%rax),%eax
    18006b133:	add    %al,-0x7ffff943(%rax)
    18006b139:	test   $0x6,%eax
 	...
    18006b17e:	add    %al,(%rax)
```

## ipex_llm/libs/libllama_vnni.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x000000018005c0a8
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Sat Jun  1 15:03:45 2024
+Time/Date		Sun Jun  2 15:02:55 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		000000000005c800
 SizeOfInitializedData	00000000000c6200
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000005c0a8
@@ -24695,52 +24695,52 @@
    18000795d:	mov    %rax,%rcx
    180007960:	call   *0x56cd2(%rip)        # 0x18005e638
    180007966:	test   %eax,%eax
    180007968:	je     0x1800079a4
    18000796a:	mov    $0x2,%ecx
    18000796f:	call   *0x56c9b(%rip)        # 0x18005e610
    180007975:	mov    %rax,%rcx
-   180007978:	lea    0x56f39(%rip),%rax        # 0x18005e8b8
+   180007978:	lea    0x56f41(%rip),%rax        # 0x18005e8c0
    18000797f:	mov    %rax,0x20(%rsp)
    180007984:	mov    $0x65,%r9d
    18000798a:	lea    0x56e7f(%rip),%r8        # 0x18005e810
-   180007991:	lea    0x56ec8(%rip),%rdx        # 0x18005e860
+   180007991:	lea    0x56ed0(%rip),%rdx        # 0x18005e868
    180007998:	call   0x1800157c0
    18000799d:	call   *0x56bb5(%rip)        # 0x18005e558
    1800079a3:	int3
    1800079a4:	mov    (%rbx),%rcx
    1800079a7:	call   *0x56c83(%rip)        # 0x18005e630
    1800079ad:	cmp    $0xffffffffffffffff,%rax
    1800079b1:	jne    0x1800079eb
    1800079b3:	lea    0x3(%rax),%ecx
    1800079b6:	call   *0x56c54(%rip)        # 0x18005e610
    1800079bc:	mov    %rax,%rcx
-   1800079bf:	lea    0x56ee2(%rip),%rax        # 0x18005e8a8
+   1800079bf:	lea    0x56eea(%rip),%rax        # 0x18005e8b0
    1800079c6:	mov    %rax,0x20(%rsp)
    1800079cb:	mov    $0x5b,%r9d
    1800079d1:	lea    0x56e38(%rip),%r8        # 0x18005e810
-   1800079d8:	lea    0x56e81(%rip),%rdx        # 0x18005e860
+   1800079d8:	lea    0x56e89(%rip),%rdx        # 0x18005e868
    1800079df:	call   0x1800157c0
    1800079e4:	call   *0x56b6e(%rip)        # 0x18005e558
    1800079ea:	int3
    1800079eb:	mov    %rax,0x8(%rbx)
    1800079ef:	xor    %r8d,%r8d
    1800079f2:	xor    %edx,%edx
    1800079f4:	mov    (%rbx),%rcx
    1800079f7:	call   *0x56c3b(%rip)        # 0x18005e638
    1800079fd:	test   %eax,%eax
    1800079ff:	je     0x180007a3b
    180007a01:	mov    $0x2,%ecx
    180007a06:	call   *0x56c04(%rip)        # 0x18005e610
    180007a0c:	mov    %rax,%rcx
-   180007a0f:	lea    0x56ea2(%rip),%rax        # 0x18005e8b8
+   180007a0f:	lea    0x56eaa(%rip),%rax        # 0x18005e8c0
    180007a16:	mov    %rax,0x20(%rsp)
    180007a1b:	mov    $0x65,%r9d
    180007a21:	lea    0x56de8(%rip),%r8        # 0x18005e810
-   180007a28:	lea    0x56e31(%rip),%rdx        # 0x18005e860
+   180007a28:	lea    0x56e39(%rip),%rdx        # 0x18005e868
    180007a2f:	call   0x1800157c0
    180007a34:	call   *0x56b1e(%rip)        # 0x18005e558
    180007a3a:	int3
    180007a3b:	mov    %rbx,%rax
    180007a3e:	mov    0x68(%rsp),%rcx
    180007a43:	xor    %rsp,%rcx
    180007a46:	call   0x18005baa0
@@ -24749,15 +24749,15 @@
    180007a57:	pop    %rdi
    180007a58:	ret
    180007a59:	call   *0x56ad9(%rip)        # 0x18005e538
    180007a5f:	mov    (%rax),%ecx
    180007a61:	call   *0x56ae9(%rip)        # 0x18005e550
    180007a67:	mov    %rax,%r9
    180007a6a:	mov    %rdi,%r8
-   180007a6d:	lea    0x56e1c(%rip),%rdx        # 0x18005e890
+   180007a6d:	lea    0x56e24(%rip),%rdx        # 0x18005e898
    180007a74:	lea    0x48(%rsp),%rcx
    180007a79:	call   0x18000c070
    180007a7e:	nop
    180007a7f:	mov    %rax,%rdx
    180007a82:	lea    0x30(%rsp),%rcx
    180007a87:	call   0x1800086c0
    180007a8c:	lea    0x648bd(%rip),%rdx        # 0x18006c350
@@ -24775,15 +24775,15 @@
    180007ab0:	xor    %rsp,%rax
    180007ab3:	mov    %rax,0x50(%rsp)
    180007ab8:	mov    %r9,%rbp
    180007abb:	mov    %r8,%rsi
    180007abe:	mov    %rdx,%rbx
    180007ac1:	mov    %rcx,%rdi
    180007ac4:	mov    %rcx,0x28(%rsp)
-   180007ac9:	lea    0x571fc(%rip),%r8        # 0x18005eccc
+   180007ac9:	lea    0x57200(%rip),%r8        # 0x18005ecd0
    180007ad0:	call   0x180007920
    180007ad5:	nop
    180007ad6:	movl   $0x7d00,0x14(%rdi)
    180007add:	movl   $0x200,0x18(%rdi)
    180007ae4:	movl   $0x1000,0x1c(%rdi)
    180007aeb:	movl   $0x100,0x20(%rdi)
    180007af2:	movl   $0x20,0x24(%rdi)
@@ -24794,15 +24794,15 @@
    180007b15:	lea    0x38(%rdi),%rcx
    180007b19:	call   0x1800085f0
    180007b1e:	nop
    180007b1f:	mov    $0x2,%ecx
    180007b24:	call   *0x56ae6(%rip)        # 0x18005e610
    180007b2a:	mov    %rax,%rcx
    180007b2d:	mov    %rbx,%r8
-   180007b30:	lea    0x57199(%rip),%rdx        # 0x18005ecd0
+   180007b30:	lea    0x571a1(%rip),%rdx        # 0x18005ecd8
    180007b37:	call   0x1800157c0
    180007b3c:	mov    $0x4,%r8d
    180007b42:	lea    0x20(%rsp),%rdx
    180007b47:	mov    %rdi,%rcx
    180007b4a:	call   0x180012f40
    180007b4f:	mov    0x20(%rsp),%ebx
    180007b53:	cmp    $0x67676d6c,%ebx
@@ -24976,15 +24976,15 @@
    180007df2:	cmpq   $0x10,0x18(%rax)
    180007df7:	jb     0x180007dfc
    180007df9:	mov    (%rax),%rbx
    180007dfc:	mov    $0x2,%ecx
    180007e01:	call   *0x56809(%rip)        # 0x18005e610
    180007e07:	mov    %rax,%rcx
    180007e0a:	mov    %rbx,%r8
-   180007e0d:	lea    0x56b54(%rip),%rdx        # 0x18005e968
+   180007e0d:	lea    0x56b5c(%rip),%rdx        # 0x18005e970
    180007e14:	call   0x1800157c0
    180007e19:	mov    0x60(%rsp),%rdx
    180007e1e:	cmp    $0x10,%rdx
    180007e22:	jb     0x180007e59
    180007e24:	inc    %rdx
    180007e27:	mov    0x48(%rsp),%rcx
    180007e2c:	mov    %rcx,%rax
@@ -25012,15 +25012,15 @@
    180007e7f:	mov    %ebp,%edx
    180007e81:	lea    0x68(%rsp),%rcx
    180007e86:	call   0x18000ef50
    180007e8b:	nop
    180007e8c:	mov    %rax,%rcx
    180007e8f:	call   0x18000b930
    180007e94:	mov    %rax,%r8
-   180007e97:	lea    0x56aaa(%rip),%rdx        # 0x18005e948
+   180007e97:	lea    0x56ab2(%rip),%rdx        # 0x18005e950
    180007e9e:	lea    0x48(%rsp),%rcx
    180007ea3:	call   0x18000c070
    180007ea8:	nop
    180007ea9:	mov    %rax,%rdx
    180007eac:	lea    0x30(%rsp),%rcx
    180007eb1:	call   0x1800086c0
    180007eb6:	lea    0x64493(%rip),%rdx        # 0x18006c350
@@ -25030,15 +25030,15 @@
    180007ec8:	mov    %eax,%edx
    180007eca:	lea    0x48(%rsp),%rcx
    180007ecf:	call   0x18000ef50
    180007ed4:	nop
    180007ed5:	mov    %rax,%rcx
    180007ed8:	call   0x18000b930
    180007edd:	mov    %rax,%r8
-   180007ee0:	lea    0x56a41(%rip),%rdx        # 0x18005e928
+   180007ee0:	lea    0x56a49(%rip),%rdx        # 0x18005e930
    180007ee7:	lea    0x68(%rsp),%rcx
    180007eec:	call   0x18000c070
    180007ef1:	nop
    180007ef2:	mov    %rax,%rdx
    180007ef5:	lea    0x30(%rsp),%rcx
    180007efa:	call   0x1800086c0
    180007eff:	lea    0x6444a(%rip),%rdx        # 0x18006c350
@@ -27227,15 +27227,15 @@
    180009ae7:	cmpq   $0x10,0x18(%rax)
    180009aec:	jb     0x180009af1
    180009aee:	mov    (%rax),%rbx
    180009af1:	mov    $0x2,%ecx
    180009af6:	call   *0x54b14(%rip)        # 0x18005e610
    180009afc:	mov    %rax,%rcx
    180009aff:	mov    %rbx,%r8
-   180009b02:	lea    0x54e8f(%rip),%rdx        # 0x18005e998
+   180009b02:	lea    0x54e97(%rip),%rdx        # 0x18005e9a0
    180009b09:	call   0x1800157c0
    180009b0e:	mov    0x38(%rsp),%rdx
    180009b13:	cmp    $0x10,%rdx
    180009b17:	jb     0x180009b4f
    180009b19:	inc    %rdx
    180009b1c:	mov    0x20(%rsp),%rcx
    180009b21:	mov    %rcx,%rax
@@ -29518,15 +29518,15 @@
    18000ba26:	mov    $0x2,%ecx
    18000ba2b:	call   *0x52bdf(%rip)        # 0x18005e610
    18000ba31:	mov    %rax,%rcx
    18000ba34:	lea    0x5321d(%rip),%rax        # 0x18005ec58
    18000ba3b:	mov    %rax,0x20(%rsp)
    18000ba40:	mov    $0x187,%r9d
    18000ba46:	lea    0x53233(%rip),%r8        # 0x18005ec80
-   18000ba4d:	lea    0x52e0c(%rip),%rdx        # 0x18005e860
+   18000ba4d:	lea    0x52e14(%rip),%rdx        # 0x18005e868
    18000ba54:	call   0x1800157c0
    18000ba59:	call   *0x52af9(%rip)        # 0x18005e558
    18000ba5f:	int3
    18000ba60:	mov    0x3c(%r14),%ecx
    18000ba64:	test   %ecx,%ecx
    18000ba66:	je     0x18000bac5
    18000ba68:	sub    $0x1,%ecx
@@ -30139,19 +30139,19 @@
    18000c184:	mov    %r14,%rcx
    18000c187:	call   0x1800199e0
    18000c18c:	cmp    %r15d,%eax
    18000c18f:	je     0x18000c1cb
    18000c191:	mov    $0x2,%ecx
    18000c196:	call   *0x52474(%rip)        # 0x18005e610
    18000c19c:	mov    %rax,%rcx
-   18000c19f:	lea    0x526da(%rip),%rax        # 0x18005e880
+   18000c19f:	lea    0x526e2(%rip),%rax        # 0x18005e888
    18000c1a6:	mov    %rax,0x20(%rsp)
    18000c1ab:	mov    $0x40,%r9d
    18000c1b1:	lea    0x52658(%rip),%r8        # 0x18005e810
-   18000c1b8:	lea    0x526a1(%rip),%rdx        # 0x18005e860
+   18000c1b8:	lea    0x526a9(%rip),%rdx        # 0x18005e868
    18000c1bf:	call   0x1800157c0
    18000c1c4:	call   *0x5238e(%rip)        # 0x18005e558
    18000c1ca:	int3
    18000c1cb:	vpxor  %xmm0,%xmm0,%xmm0
    18000c1cf:	vmovups %xmm0,0x0(%rbp)
    18000c1d4:	mov    %r12,0x10(%rbp)
    18000c1d8:	mov    %r12,0x18(%rbp)
@@ -30191,15 +30191,15 @@
    18000c23a:	mov    $0x2,%ecx
    18000c23f:	call   *0x523cb(%rip)        # 0x18005e610
    18000c245:	mov    %rax,%rcx
    18000c248:	lea    0x52599(%rip),%rax        # 0x18005e7e8
    18000c24f:	mov    %rax,0x20(%rsp)
    18000c254:	mov    $0x3d,%r9d
    18000c25a:	lea    0x525af(%rip),%r8        # 0x18005e810
-   18000c261:	lea    0x525f8(%rip),%rdx        # 0x18005e860
+   18000c261:	lea    0x52600(%rip),%rdx        # 0x18005e868
    18000c268:	call   0x1800157c0
    18000c26d:	call   *0x522e5(%rip)        # 0x18005e558
    18000c273:	int3
    18000c274:	call   0x18000b150
    18000c279:	int3
    18000c27a:	call   0x18000b5a0
    18000c27f:	int3
@@ -30289,15 +30289,15 @@
    18000c3c0:	mov    $0x2,%ecx
    18000c3c5:	call   *0x52245(%rip)        # 0x18005e610
    18000c3cb:	mov    %rax,%rcx
    18000c3ce:	lea    0x52be3(%rip),%rax        # 0x18005efb8
    18000c3d5:	mov    %rax,0x20(%rsp)
    18000c3da:	mov    $0x2b2,%r9d
    18000c3e0:	lea    0x52899(%rip),%r8        # 0x18005ec80
-   18000c3e7:	lea    0x52472(%rip),%rdx        # 0x18005e860
+   18000c3e7:	lea    0x5247a(%rip),%rdx        # 0x18005e868
    18000c3ee:	call   0x1800157c0
    18000c3f3:	call   *0x5215f(%rip)        # 0x18005e558
    18000c3f9:	int3
    18000c3fa:	mov    (%r14),%r8d
    18000c3fd:	mov    0x38(%rdi),%edx
    18000c400:	mov    0x80(%rbx),%rcx
    18000c407:	call   0x18003b4f0
@@ -30313,15 +30313,15 @@
    18000c42c:	mov    $0x2,%ecx
    18000c431:	call   *0x521d9(%rip)        # 0x18005e610
    18000c437:	mov    %rax,%rcx
    18000c43a:	lea    0x52b8f(%rip),%rax        # 0x18005efd0
    18000c441:	mov    %rax,0x20(%rsp)
    18000c446:	mov    $0x2b6,%r9d
    18000c44c:	lea    0x5282d(%rip),%r8        # 0x18005ec80
-   18000c453:	lea    0x52406(%rip),%rdx        # 0x18005e860
+   18000c453:	lea    0x5240e(%rip),%rdx        # 0x18005e868
    18000c45a:	call   0x1800157c0
    18000c45f:	call   *0x520f3(%rip)        # 0x18005e558
    18000c465:	int3
    18000c466:	mov    %r13d,0x4(%rsi)
    18000c46a:	mov    %rsi,0x60(%rdi)
    18000c46e:	incq   0x78(%rbx)
    18000c472:	mov    %rsi,%rax
@@ -30395,16 +30395,16 @@
    18000c561:	mov    %rcx,%rbx
    18000c564:	jne    0x18000c5a0
    18000c566:	mov    $0x2,%ecx
    18000c56b:	call   *0x5209f(%rip)        # 0x18005e610
    18000c571:	mov    $0x114,%r9d
    18000c577:	lea    0x52292(%rip),%r8        # 0x18005e810
    18000c57e:	mov    %rax,%rcx
-   18000c581:	lea    0x522d8(%rip),%rdx        # 0x18005e860
-   18000c588:	lea    0x5244d(%rip),%rax        # 0x18005e9dc
+   18000c581:	lea    0x522e0(%rip),%rdx        # 0x18005e868
+   18000c588:	lea    0x52455(%rip),%rax        # 0x18005e9e4
    18000c58f:	mov    %rax,0x20(%rsp)
    18000c594:	call   0x1800157c0
    18000c599:	call   *0x51fb9(%rip)        # 0x18005e558
    18000c59f:	int3
    18000c5a0:	cmpb   $0x0,0x10(%rcx)
    18000c5a4:	jne    0x18000c5f8
    18000c5a6:	lea    0x30(%rsp),%rcx
@@ -30620,16 +30620,16 @@
    18000c894:	add    $0x38,%rsp
    18000c898:	ret
    18000c899:	mov    $0x2,%ecx
    18000c89e:	call   *0x51d6c(%rip)        # 0x18005e610
    18000c8a4:	mov    $0x10f,%r9d
    18000c8aa:	lea    0x51f5f(%rip),%r8        # 0x18005e810
    18000c8b1:	mov    %rax,%rcx
-   18000c8b4:	lea    0x51fa5(%rip),%rdx        # 0x18005e860
-   18000c8bb:	lea    0x520fe(%rip),%rax        # 0x18005e9c0
+   18000c8b4:	lea    0x51fad(%rip),%rdx        # 0x18005e868
+   18000c8bb:	lea    0x52106(%rip),%rax        # 0x18005e9c8
    18000c8c2:	mov    %rax,0x20(%rsp)
    18000c8c7:	call   0x1800157c0
    18000c8cc:	call   *0x51c86(%rip)        # 0x18005e558
    18000c8d2:	int3
    18000c8d3:	int3
    18000c8d4:	int3
    18000c8d5:	int3
@@ -32130,15 +32130,15 @@
    18000e2e0:	mov    %rax,-0x30(%rbp)
    18000e2e4:	jne    0x18000e320
    18000e2e6:	mov    $0x2,%ecx
    18000e2eb:	call   *0x5031f(%rip)        # 0x18005e610
    18000e2f1:	mov    $0x4e8,%r9d
    18000e2f7:	lea    0x50982(%rip),%r8        # 0x18005ec80
    18000e2fe:	mov    %rax,%rcx
-   18000e301:	lea    0x50558(%rip),%rdx        # 0x18005e860
+   18000e301:	lea    0x50560(%rip),%rdx        # 0x18005e868
    18000e308:	lea    0x512f1(%rip),%rax        # 0x18005f600
    18000e30f:	mov    %rax,0x20(%rsp)
    18000e314:	call   0x1800157c0
    18000e319:	call   *0x50239(%rip)        # 0x18005e558
    18000e31f:	int3
    18000e320:	mov    0x13e0(%r14),%ecx
    18000e327:	mov    0x13e4(%r14),%eax
@@ -32886,19 +32886,19 @@
    18000efb1:	mov    %rdi,0x10(%rbx)
    18000efb5:	mov    %rbx,%rcx
    18000efb8:	movq   $0xf,0x18(%rbx)
    18000efc0:	call   0x18000b600
    18000efc5:	mov    %rax,(%rbx)
    18000efc8:	movq   $0x15,0x10(%rbx)
    18000efd0:	movq   $0x1f,0x18(%rbx)
-   18000efd8:	vmovups 0x4f930(%rip),%xmm0        # 0x18005e910
+   18000efd8:	vmovups 0x4f938(%rip),%xmm0        # 0x18005e918
    18000efe0:	vmovups %xmm0,(%rax)
-   18000efe4:	mov    0x4f936(%rip),%ecx        # 0x18005e920
+   18000efe4:	mov    0x4f93e(%rip),%ecx        # 0x18005e928
    18000efea:	mov    %ecx,0x10(%rax)
-   18000efed:	movzbl 0x4f930(%rip),%ecx        # 0x18005e924
+   18000efed:	movzbl 0x4f938(%rip),%ecx        # 0x18005e92c
    18000eff4:	mov    %cl,0x14(%rax)
    18000eff7:	mov    %dil,0x15(%rax)
    18000effb:	jmp    0x18000f031
    18000effd:	mov    0x40(%rsp),%rdx
    18000f002:	lea    0x50(%rsp),%rcx
    18000f007:	vpxor  %xmm1,%xmm1,%xmm1
    18000f00b:	vmovdqu %xmm1,0x60(%rsp)
@@ -34593,15 +34593,15 @@
    180010bfe:	mov    $0x2,%ecx
    180010c03:	call   *0x4da07(%rip)        # 0x18005e610
    180010c09:	mov    %rax,%rcx
    180010c0c:	lea    0x4df61(%rip),%rax        # 0x18005eb74
    180010c13:	mov    %rax,0x20(%rsp)
    180010c18:	mov    $0x39e,%r9d
    180010c1e:	lea    0x4e05b(%rip),%r8        # 0x18005ec80
-   180010c25:	lea    0x4dc34(%rip),%rdx        # 0x18005e860
+   180010c25:	lea    0x4dc3c(%rip),%rdx        # 0x18005e868
    180010c2c:	call   0x1800157c0
    180010c31:	call   *0x4d921(%rip)        # 0x18005e558
    180010c37:	int3
    180010c38:	lea    0x4f491(%rip),%rcx        # 0x1800600d0
    180010c3f:	call   0x18005b248
    180010c44:	int3
    180010c45:	lea    0x4e794(%rip),%rdx        # 0x18005f3e0
@@ -35470,48 +35470,48 @@
    180011a02:	mov    $0x2,%ecx
    180011a07:	call   *0x4cc03(%rip)        # 0x18005e610
    180011a0d:	mov    %rax,%rcx
    180011a10:	lea    0x4d429(%rip),%rax        # 0x18005ee40
    180011a17:	mov    %rax,0x20(%rsp)
    180011a1c:	mov    $0x25d,%r9d
    180011a22:	lea    0x4d257(%rip),%r8        # 0x18005ec80
-   180011a29:	lea    0x4ce30(%rip),%rdx        # 0x18005e860
+   180011a29:	lea    0x4ce38(%rip),%rdx        # 0x18005e868
    180011a30:	call   0x1800157c0
    180011a35:	call   *0x4cb1d(%rip)        # 0x18005e558
    180011a3b:	int3
    180011a3c:	mov    $0x2,%ecx
    180011a41:	call   *0x4cbc9(%rip)        # 0x18005e610
    180011a47:	mov    %rax,%rcx
-   180011a4a:	lea    0x4ce67(%rip),%rax        # 0x18005e8b8
+   180011a4a:	lea    0x4ce6f(%rip),%rax        # 0x18005e8c0
    180011a51:	mov    %rax,0x20(%rsp)
    180011a56:	mov    $0x65,%r9d
    180011a5c:	lea    0x4cdad(%rip),%r8        # 0x18005e810
-   180011a63:	lea    0x4cdf6(%rip),%rdx        # 0x18005e860
+   180011a63:	lea    0x4cdfe(%rip),%rdx        # 0x18005e868
    180011a6a:	call   0x1800157c0
    180011a6f:	call   *0x4cae3(%rip)        # 0x18005e558
    180011a75:	int3
    180011a76:	mov    $0x2,%ecx
    180011a7b:	call   *0x4cb8f(%rip)        # 0x18005e610
    180011a81:	mov    %rax,%rcx
-   180011a84:	lea    0x4ce1d(%rip),%rax        # 0x18005e8a8
+   180011a84:	lea    0x4ce25(%rip),%rax        # 0x18005e8b0
    180011a8b:	mov    %rax,0x20(%rsp)
    180011a90:	mov    $0x5b,%r9d
    180011a96:	lea    0x4cd73(%rip),%r8        # 0x18005e810
-   180011a9d:	lea    0x4cdbc(%rip),%rdx        # 0x18005e860
+   180011a9d:	lea    0x4cdc4(%rip),%rdx        # 0x18005e868
    180011aa4:	call   0x1800157c0
    180011aa9:	call   *0x4caa9(%rip)        # 0x18005e558
    180011aaf:	int3
    180011ab0:	mov    $0x2,%ecx
    180011ab5:	call   *0x4cb55(%rip)        # 0x18005e610
    180011abb:	mov    %rax,%rcx
    180011abe:	lea    0x4d0af(%rip),%rax        # 0x18005eb74
    180011ac5:	mov    %rax,0x20(%rsp)
    180011aca:	mov    $0x255,%r9d
    180011ad0:	lea    0x4d1a9(%rip),%r8        # 0x18005ec80
-   180011ad7:	lea    0x4cd82(%rip),%rdx        # 0x18005e860
+   180011ad7:	lea    0x4cd8a(%rip),%rdx        # 0x18005e868
    180011ade:	call   0x1800157c0
    180011ae3:	call   *0x4ca6f(%rip)        # 0x18005e558
    180011ae9:	nop
    180011aea:	mov    -0x50(%rbp),%rsi
    180011aee:	jmp    0x180011b09
    180011af0:	mov    0x100(%rbp),%rdi
    180011af7:	mov    0x40(%rsp),%rsi
@@ -35804,19 +35804,19 @@
    180011f4b:	test   %rsi,%rsi
    180011f4e:	js     0x180011f91
    180011f50:	vcvtsi2ss %rsi,%xmm1,%xmm1
    180011f55:	jmp    0x180011fa9
    180011f57:	mov    $0x2,%ecx
    180011f5c:	call   *0x4c6ae(%rip)        # 0x18005e610
    180011f62:	mov    %rax,%rcx
-   180011f65:	lea    0x4ca54(%rip),%rax        # 0x18005e9c0
+   180011f65:	lea    0x4ca5c(%rip),%rax        # 0x18005e9c8
    180011f6c:	mov    %rax,0x20(%rsp)
    180011f71:	mov    $0x10f,%r9d
    180011f77:	lea    0x4c892(%rip),%r8        # 0x18005e810
-   180011f7e:	lea    0x4c8db(%rip),%rdx        # 0x18005e860
+   180011f7e:	lea    0x4c8e3(%rip),%rdx        # 0x18005e868
    180011f85:	call   0x1800157c0
    180011f8a:	call   *0x4c5c8(%rip)        # 0x18005e558
    180011f90:	int3
    180011f91:	mov    %rsi,%rcx
    180011f94:	shr    $1,%rcx
    180011f97:	mov    %rsi,%rax
    180011f9a:	and    $0x1,%eax
@@ -35883,30 +35883,30 @@
    180012077:	cmp    %r13,%rbx
    18001207a:	je     0x180012101
    180012080:	mov    0xb0(%rsp),%r8
    180012088:	jmp    0x180011f30
    18001208d:	mov    $0x2,%ecx
    180012092:	call   *0x4c578(%rip)        # 0x18005e610
    180012098:	mov    %rax,%rcx
-   18001209b:	lea    0x4c93a(%rip),%rax        # 0x18005e9dc
+   18001209b:	lea    0x4c942(%rip),%rax        # 0x18005e9e4
    1800120a2:	mov    %rax,0x20(%rsp)
    1800120a7:	mov    $0x114,%r9d
    1800120ad:	lea    0x4c75c(%rip),%r8        # 0x18005e810
-   1800120b4:	lea    0x4c7a5(%rip),%rdx        # 0x18005e860
+   1800120b4:	lea    0x4c7ad(%rip),%rdx        # 0x18005e868
    1800120bb:	call   0x1800157c0
    1800120c0:	call   *0x4c492(%rip)        # 0x18005e558
    1800120c6:	int3
    1800120c7:	mov    $0x2,%ecx
    1800120cc:	call   *0x4c53e(%rip)        # 0x18005e610
    1800120d2:	mov    %rax,%rcx
    1800120d5:	lea    0x4cf44(%rip),%rax        # 0x18005f020
    1800120dc:	mov    %rax,0x20(%rsp)
    1800120e1:	mov    $0x2e1,%r9d
    1800120e7:	lea    0x4cb92(%rip),%r8        # 0x18005ec80
-   1800120ee:	lea    0x4c76b(%rip),%rdx        # 0x18005e860
+   1800120ee:	lea    0x4c773(%rip),%rdx        # 0x18005e868
    1800120f5:	call   0x1800157c0
    1800120fa:	call   *0x4c458(%rip)        # 0x18005e558
    180012100:	int3
    180012101:	mov    0xa8(%rsp),%rbx
    180012109:	add    $0x60,%rsp
    18001210d:	pop    %r15
    18001210f:	pop    %r14
@@ -35941,15 +35941,15 @@
    180012158:	mov    $0x2,%ecx
    18001215d:	call   *0x4c4ad(%rip)        # 0x18005e610
    180012163:	mov    %rax,%rcx
    180012166:	lea    0x4cec3(%rip),%rax        # 0x18005f030
    18001216d:	mov    %rax,0x20(%rsp)
    180012172:	mov    $0x2ee,%r9d
    180012178:	lea    0x4cb01(%rip),%r8        # 0x18005ec80
-   18001217f:	lea    0x4c6da(%rip),%rdx        # 0x18005e860
+   18001217f:	lea    0x4c6e2(%rip),%rdx        # 0x18005e868
    180012186:	call   0x1800157c0
    18001218b:	call   *0x4c3c7(%rip)        # 0x18005e558
    180012191:	int3
    180012192:	movabs $0x4924924924924925,%rax
    18001219c:	imul   %rcx
    18001219f:	sar    $0x4,%rdx
    1800121a3:	mov    %rdx,%rax
@@ -35987,19 +35987,19 @@
    180012226:	mov    (%rbx),%rcx
    180012229:	call   *0x4c409(%rip)        # 0x18005e638
    18001222f:	test   %eax,%eax
    180012231:	je     0x18001226d
    180012233:	mov    $0x2,%ecx
    180012238:	call   *0x4c3d2(%rip)        # 0x18005e610
    18001223e:	mov    %rax,%rcx
-   180012241:	lea    0x4c670(%rip),%rax        # 0x18005e8b8
+   180012241:	lea    0x4c678(%rip),%rax        # 0x18005e8c0
    180012248:	mov    %rax,0x20(%rsp)
    18001224d:	mov    $0x65,%r9d
    180012253:	lea    0x4c5b6(%rip),%r8        # 0x18005e810
-   18001225a:	lea    0x4c5ff(%rip),%rdx        # 0x18005e860
+   18001225a:	lea    0x4c607(%rip),%rdx        # 0x18005e868
    180012261:	call   0x1800157c0
    180012266:	call   *0x4c2ec(%rip)        # 0x18005e558
    18001226c:	int3
    18001226d:	mov    0x58(%r14),%r8
    180012271:	mov    0x68(%r14),%rdx
    180012275:	mov    %rbx,%rcx
    180012278:	call   0x180012f40
@@ -36040,26 +36040,26 @@
    1800122fd:	mov    $0x2,%ecx
    180012302:	call   *0x4c308(%rip)        # 0x18005e610
    180012308:	mov    %rax,%rcx
    18001230b:	lea    0x4cd36(%rip),%rax        # 0x18005f048
    180012312:	mov    %rax,0x20(%rsp)
    180012317:	mov    $0x2fc,%r9d
    18001231d:	lea    0x4c95c(%rip),%r8        # 0x18005ec80
-   180012324:	lea    0x4c535(%rip),%rdx        # 0x18005e860
+   180012324:	lea    0x4c53d(%rip),%rdx        # 0x18005e868
    18001232b:	call   0x1800157c0
    180012330:	call   *0x4c222(%rip)        # 0x18005e558
    180012336:	int3
    180012337:	mov    $0x2,%ecx
    18001233c:	call   *0x4c2ce(%rip)        # 0x18005e610
    180012342:	mov    %rax,%rcx
-   180012345:	lea    0x4c56c(%rip),%rax        # 0x18005e8b8
+   180012345:	lea    0x4c574(%rip),%rax        # 0x18005e8c0
    18001234c:	mov    %rax,0x20(%rsp)
    180012351:	mov    $0x65,%r9d
    180012357:	lea    0x4c4b2(%rip),%r8        # 0x18005e810
-   18001235e:	lea    0x4c4fb(%rip),%rdx        # 0x18005e860
+   18001235e:	lea    0x4c503(%rip),%rdx        # 0x18005e868
    180012365:	call   0x1800157c0
    18001236a:	call   *0x4c1e8(%rip)        # 0x18005e558
    180012370:	int3
    180012371:	cmp    $0x1,%eax
    180012374:	jne    0x18001272c
    18001237a:	mov    0x8(%rdx),%rcx
    18001237e:	sub    (%rdx),%rcx
@@ -36249,26 +36249,26 @@
    18001265a:	mov    $0x2,%ecx
    18001265f:	call   *0x4bfab(%rip)        # 0x18005e610
    180012665:	mov    %rax,%rcx
    180012668:	lea    0x4c9f1(%rip),%rax        # 0x18005f060
    18001266f:	mov    %rax,0x20(%rsp)
    180012674:	mov    $0x313,%r9d
    18001267a:	lea    0x4c5ff(%rip),%r8        # 0x18005ec80
-   180012681:	lea    0x4c1d8(%rip),%rdx        # 0x18005e860
+   180012681:	lea    0x4c1e0(%rip),%rdx        # 0x18005e868
    180012688:	call   0x1800157c0
    18001268d:	call   *0x4bec5(%rip)        # 0x18005e558
    180012693:	int3
    180012694:	mov    $0x2,%ecx
    180012699:	call   *0x4bf71(%rip)        # 0x18005e610
    18001269f:	mov    %rax,%rcx
-   1800126a2:	lea    0x4c20f(%rip),%rax        # 0x18005e8b8
+   1800126a2:	lea    0x4c217(%rip),%rax        # 0x18005e8c0
    1800126a9:	mov    %rax,0x20(%rsp)
    1800126ae:	mov    $0x65,%r9d
    1800126b4:	lea    0x4c155(%rip),%r8        # 0x18005e810
-   1800126bb:	lea    0x4c19e(%rip),%rdx        # 0x18005e860
+   1800126bb:	lea    0x4c1a6(%rip),%rdx        # 0x18005e868
    1800126c2:	call   0x1800157c0
    1800126c7:	call   *0x4be8b(%rip)        # 0x18005e558
    1800126cd:	nop
    1800126ce:	test   %r12,%r12
    1800126d1:	je     0x18001272c
    1800126d3:	mov    %r12,%rbx
    1800126d6:	cmp    %rsi,%r12
@@ -36927,30 +36927,30 @@
    180012fa0:	xor    %rsp,%rcx
    180012fa3:	call   0x18005baa0
    180012fa8:	add    $0x60,%rsp
    180012fac:	pop    %rdi
    180012fad:	pop    %rsi
    180012fae:	pop    %rbx
    180012faf:	ret
-   180012fb0:	lea    0x4b921(%rip),%rdx        # 0x18005e8d8
+   180012fb0:	lea    0x4b929(%rip),%rdx        # 0x18005e8e0
    180012fb7:	lea    0x38(%rsp),%rcx
    180012fbc:	call   0x180007010
    180012fc1:	nop
    180012fc2:	mov    %rax,%rdx
    180012fc5:	lea    0x20(%rsp),%rcx
    180012fca:	call   0x1800086c0
    180012fcf:	lea    0x5937a(%rip),%rdx        # 0x18006c350
    180012fd6:	lea    0x20(%rsp),%rcx
    180012fdb:	call   0x18005c612
    180012fe0:	nop
    180012fe1:	call   *0x4b551(%rip)        # 0x18005e538
    180012fe7:	mov    (%rax),%ecx
    180012fe9:	call   *0x4b561(%rip)        # 0x18005e550
    180012fef:	mov    %rax,%r8
-   180012ff2:	lea    0x4b8cf(%rip),%rdx        # 0x18005e8c8
+   180012ff2:	lea    0x4b8d7(%rip),%rdx        # 0x18005e8d0
    180012ff9:	lea    0x38(%rsp),%rcx
    180012ffe:	call   0x18000c070
    180013003:	nop
    180013004:	mov    %rax,%rdx
    180013007:	lea    0x20(%rsp),%rcx
    18001300c:	call   0x1800086c0
    180013011:	lea    0x59338(%rip),%rdx        # 0x18006c350
@@ -37558,69 +37558,69 @@
    180013962:	call   0x18005b484
    180013967:	mov    -0x48(%rbp),%r12
    18001396b:	mov    (%r12),%rcx
    18001396f:	jmp    0x180013070
    180013974:	mov    $0x2,%ecx
    180013979:	call   *0x4ac91(%rip)        # 0x18005e610
    18001397f:	mov    %rax,%rcx
-   180013982:	lea    0x4af2f(%rip),%rax        # 0x18005e8b8
+   180013982:	lea    0x4af37(%rip),%rax        # 0x18005e8c0
    180013989:	mov    %rax,0x20(%rsp)
    18001398e:	mov    $0x65,%r9d
    180013994:	lea    0x4ae75(%rip),%r8        # 0x18005e810
-   18001399b:	lea    0x4aebe(%rip),%rdx        # 0x18005e860
+   18001399b:	lea    0x4aec6(%rip),%rdx        # 0x18005e868
    1800139a2:	call   0x1800157c0
    1800139a7:	call   *0x4abab(%rip)        # 0x18005e558
    1800139ad:	int3
    1800139ae:	mov    $0x2,%ecx
    1800139b3:	call   *0x4ac57(%rip)        # 0x18005e610
    1800139b9:	mov    %rax,%rcx
-   1800139bc:	lea    0x4aee5(%rip),%rax        # 0x18005e8a8
+   1800139bc:	lea    0x4aeed(%rip),%rax        # 0x18005e8b0
    1800139c3:	mov    %rax,0x20(%rsp)
    1800139c8:	mov    $0x5b,%r9d
    1800139ce:	lea    0x4ae3b(%rip),%r8        # 0x18005e810
-   1800139d5:	lea    0x4ae84(%rip),%rdx        # 0x18005e860
+   1800139d5:	lea    0x4ae8c(%rip),%rdx        # 0x18005e868
    1800139dc:	call   0x1800157c0
    1800139e1:	call   *0x4ab71(%rip)        # 0x18005e558
    1800139e7:	nop
    1800139e8:	call   *0x4abb2(%rip)        # 0x18005e5a0
    1800139ee:	nop
    1800139ef:	call   *0x4abab(%rip)        # 0x18005e5a0
    1800139f5:	nop
    1800139f6:	call   *0x4aba4(%rip)        # 0x18005e5a0
    1800139fc:	nop
    1800139fd:	mov    $0x2,%ecx
    180013a02:	call   *0x4ac08(%rip)        # 0x18005e610
    180013a08:	mov    %rax,%rcx
-   180013a0b:	lea    0x4aea6(%rip),%rax        # 0x18005e8b8
+   180013a0b:	lea    0x4aeae(%rip),%rax        # 0x18005e8c0
    180013a12:	mov    %rax,0x20(%rsp)
    180013a17:	mov    $0x65,%r9d
    180013a1d:	lea    0x4adec(%rip),%r8        # 0x18005e810
-   180013a24:	lea    0x4ae35(%rip),%rdx        # 0x18005e860
+   180013a24:	lea    0x4ae3d(%rip),%rdx        # 0x18005e868
    180013a2b:	call   0x1800157c0
    180013a30:	call   *0x4ab22(%rip)        # 0x18005e558
    180013a36:	int3
    180013a37:	mov    $0x2,%ecx
    180013a3c:	call   *0x4abce(%rip)        # 0x18005e610
    180013a42:	mov    %rax,%rcx
-   180013a45:	lea    0x4ae5c(%rip),%rax        # 0x18005e8a8
+   180013a45:	lea    0x4ae64(%rip),%rax        # 0x18005e8b0
    180013a4c:	mov    %rax,0x20(%rsp)
    180013a51:	mov    $0x5b,%r9d
    180013a57:	lea    0x4adb2(%rip),%r8        # 0x18005e810
-   180013a5e:	lea    0x4adfb(%rip),%rdx        # 0x18005e860
+   180013a5e:	lea    0x4ae03(%rip),%rdx        # 0x18005e868
    180013a65:	call   0x1800157c0
    180013a6a:	call   *0x4aae8(%rip)        # 0x18005e558
    180013a70:	nop
    180013a71:	mov    $0x2,%ecx
    180013a76:	call   *0x4ab94(%rip)        # 0x18005e610
    180013a7c:	mov    %rax,%rcx
-   180013a7f:	lea    0x4ae22(%rip),%rax        # 0x18005e8a8
+   180013a7f:	lea    0x4ae2a(%rip),%rax        # 0x18005e8b0
    180013a86:	mov    %rax,0x20(%rsp)
    180013a8b:	mov    $0x5b,%r9d
    180013a91:	lea    0x4ad78(%rip),%r8        # 0x18005e810
-   180013a98:	lea    0x4adc1(%rip),%rdx        # 0x18005e860
+   180013a98:	lea    0x4adc9(%rip),%rdx        # 0x18005e868
    180013a9f:	call   0x1800157c0
    180013aa4:	call   *0x4aaae(%rip)        # 0x18005e558
    180013aaa:	int3
    180013aab:	mov    0x30(%rbp),%rcx
    180013aaf:	xor    %rsp,%rcx
    180013ab2:	call   0x18005baa0
    180013ab7:	mov    0x198(%rsp),%rbx
@@ -37640,30 +37640,30 @@
    180013ae1:	lea    0x4b278(%rip),%rdx        # 0x18005ed60
    180013ae8:	lea    -0x10(%rbp),%rcx
    180013aec:	call   0x18000c070
    180013af1:	lea    0x58988(%rip),%rdx        # 0x18006c480
    180013af8:	lea    -0x10(%rbp),%rcx
    180013afc:	call   0x18005c612
    180013b01:	nop
-   180013b02:	lea    0x4adcf(%rip),%rdx        # 0x18005e8d8
+   180013b02:	lea    0x4add7(%rip),%rdx        # 0x18005e8e0
    180013b09:	lea    0x10(%rbp),%rcx
    180013b0d:	call   0x180007010
    180013b12:	nop
    180013b13:	mov    %rax,%rdx
    180013b16:	lea    -0x10(%rbp),%rcx
    180013b1a:	call   0x1800086c0
    180013b1f:	lea    0x5882a(%rip),%rdx        # 0x18006c350
    180013b26:	lea    -0x10(%rbp),%rcx
    180013b2a:	call   0x18005c612
    180013b2f:	nop
    180013b30:	call   *0x4aa02(%rip)        # 0x18005e538
    180013b36:	mov    (%rax),%ecx
    180013b38:	call   *0x4aa12(%rip)        # 0x18005e550
    180013b3e:	mov    %rax,%r8
-   180013b41:	lea    0x4ad80(%rip),%rdx        # 0x18005e8c8
+   180013b41:	lea    0x4ad88(%rip),%rdx        # 0x18005e8d0
    180013b48:	lea    0x10(%rbp),%rcx
    180013b4c:	call   0x18000c070
    180013b51:	nop
    180013b52:	mov    %rax,%rdx
    180013b55:	lea    -0x10(%rbp),%rcx
    180013b59:	call   0x1800086c0
    180013b5e:	lea    0x587eb(%rip),%rdx        # 0x18006c350
@@ -37948,26 +37948,26 @@
    180013f56:	vzeroupper
    180013f59:	call   *0x4a641(%rip)        # 0x18005e5a0
    180013f5f:	nop
    180013f60:	call   *0x4a5d2(%rip)        # 0x18005e538
    180013f66:	mov    (%rax),%ecx
    180013f68:	call   *0x4a5e2(%rip)        # 0x18005e550
    180013f6e:	mov    %rax,%r8
-   180013f71:	lea    0x4a950(%rip),%rdx        # 0x18005e8c8
+   180013f71:	lea    0x4a958(%rip),%rdx        # 0x18005e8d0
    180013f78:	lea    -0x1(%rbp),%rcx
    180013f7c:	call   0x18000c070
    180013f81:	nop
    180013f82:	mov    %rax,%rdx
    180013f85:	lea    -0x39(%rbp),%rcx
    180013f89:	call   0x1800086c0
    180013f8e:	lea    0x583bb(%rip),%rdx        # 0x18006c350
    180013f95:	lea    -0x39(%rbp),%rcx
    180013f99:	call   0x18005c612
    180013f9e:	nop
-   180013f9f:	lea    0x4a932(%rip),%rdx        # 0x18005e8d8
+   180013f9f:	lea    0x4a93a(%rip),%rdx        # 0x18005e8e0
    180013fa6:	lea    -0x1(%rbp),%rcx
    180013faa:	call   0x180007010
    180013faf:	nop
    180013fb0:	mov    %rax,%rdx
    180013fb3:	lea    -0x39(%rbp),%rcx
    180013fb7:	call   0x1800086c0
    180013fbc:	lea    0x5838d(%rip),%rdx        # 0x18006c350
@@ -39446,15 +39446,15 @@
    18001536d:	pop    %rsi
    18001536e:	pop    %rbx
    18001536f:	ret
    180015370:	call   *0x491c2(%rip)        # 0x18005e538
    180015376:	mov    (%rax),%ecx
    180015378:	call   *0x491d2(%rip)        # 0x18005e550
    18001537e:	mov    %rax,%r8
-   180015381:	lea    0x49578(%rip),%rdx        # 0x18005e900
+   180015381:	lea    0x49580(%rip),%rdx        # 0x18005e908
    180015388:	lea    0x38(%rsp),%rcx
    18001538d:	call   0x18000c070
    180015392:	nop
    180015393:	mov    %rax,%rdx
    180015396:	lea    0x20(%rsp),%rcx
    18001539b:	call   0x1800086c0
    1800153a0:	lea    0x56fa9(%rip),%rdx        # 0x18006c350
@@ -39566,15 +39566,15 @@
    180015520:	pop    %r12
    180015522:	pop    %rdi
    180015523:	ret
    180015524:	call   *0x4900e(%rip)        # 0x18005e538
    18001552a:	mov    (%rax),%ecx
    18001552c:	call   *0x4901e(%rip)        # 0x18005e550
    180015532:	mov    %rax,%r8
-   180015535:	lea    0x493c4(%rip),%rdx        # 0x18005e900
+   180015535:	lea    0x493cc(%rip),%rdx        # 0x18005e908
    18001553c:	lea    0x40(%rsp),%rcx
    180015541:	call   0x18000c070
    180015546:	nop
    180015547:	mov    %rax,%rdx
    18001554a:	lea    0x28(%rsp),%rcx
    18001554f:	call   0x1800086c0
    180015554:	lea    0x56df5(%rip),%rdx        # 0x18006c350
@@ -39583,15 +39583,15 @@
    180015565:	nop
    180015566:	call   0x18000b5e0
    18001556b:	int3
    18001556c:	call   *0x48fc6(%rip)        # 0x18005e538
    180015572:	mov    (%rax),%ecx
    180015574:	call   *0x48fd6(%rip)        # 0x18005e550
    18001557a:	mov    %rax,%r8
-   18001557d:	lea    0x4937c(%rip),%rdx        # 0x18005e900
+   18001557d:	lea    0x49384(%rip),%rdx        # 0x18005e908
    180015584:	lea    0x40(%rsp),%rcx
    180015589:	call   0x18000c070
    18001558e:	nop
    18001558f:	mov    %rax,%rdx
    180015592:	lea    0x28(%rsp),%rcx
    180015597:	call   0x1800086c0
    18001559c:	lea    0x56dad(%rip),%rdx        # 0x18006c350
@@ -40153,15 +40153,15 @@
    180015de0:	cmp    %rcx,%r15
    180015de3:	jbe    0x180015e1f
    180015de5:	mov    $0x2,%ecx
    180015dea:	call   *0x48820(%rip)        # 0x18005e610
    180015df0:	mov    $0xac1,%r9d
    180015df6:	lea    0x48e83(%rip),%r8        # 0x18005ec80
    180015dfd:	mov    %rax,%rcx
-   180015e00:	lea    0x48a59(%rip),%rdx        # 0x18005e860
+   180015e00:	lea    0x48a61(%rip),%rdx        # 0x18005e868
    180015e07:	lea    0x49f3a(%rip),%rax        # 0x18005fd48
    180015e0e:	mov    %rax,0x20(%rsp)
    180015e13:	call   0x1800157c0
    180015e18:	call   *0x4873a(%rip)        # 0x18005e558
    180015e1e:	int3
    180015e1f:	mov    %r15,%rax
    180015e22:	mov    0x18ff0(%rbp),%rcx
@@ -40792,15 +40792,15 @@
    1800167a2:	sub    $0xb8,%rsp
    1800167a9:	mov    0x66cd8(%rip),%rax        # 0x18007d488
    1800167b0:	xor    %rsp,%rax
    1800167b3:	mov    %rax,-0x1(%rbp)
    1800167b7:	mov    0x7f(%rbp),%r13
    1800167bb:	mov    %r8,%r12
    1800167be:	mov    %rcx,%rdi
-   1800167c1:	lea    0x48504(%rip),%r8        # 0x18005eccc
+   1800167c1:	lea    0x48508(%rip),%r8        # 0x18005ecd0
    1800167c8:	lea    -0x21(%rbp),%rcx
    1800167cc:	mov    %r9,%r15
    1800167cf:	call   0x180007920
    1800167d4:	call   *0x47d5e(%rip)        # 0x18005e538
    1800167da:	mov    -0x21(%rbp),%rbx
    1800167de:	lea    -0x6d(%rbp),%rcx
    1800167e2:	xor    %r14d,%r14d
@@ -40897,16 +40897,16 @@
    180016982:	cmp    $0xffffffffffffffff,%rax
    180016986:	jne    0x1800169c0
    180016988:	lea    0x3(%rax),%ecx
    18001698b:	call   *0x47c7f(%rip)        # 0x18005e610
    180016991:	mov    $0x5b,%r9d
    180016997:	lea    0x47e72(%rip),%r8        # 0x18005e810
    18001699e:	mov    %rax,%rcx
-   1800169a1:	lea    0x47eb8(%rip),%rdx        # 0x18005e860
-   1800169a8:	lea    0x47ef9(%rip),%rax        # 0x18005e8a8
+   1800169a1:	lea    0x47ec0(%rip),%rdx        # 0x18005e868
+   1800169a8:	lea    0x47f01(%rip),%rax        # 0x18005e8b0
    1800169af:	mov    %rax,0x20(%rsp)
    1800169b4:	call   0x1800157c0
    1800169b9:	call   *0x47b99(%rip)        # 0x18005e558
    1800169bf:	int3
    1800169c0:	mov    -0x19(%rbp),%rsi
    1800169c4:	mov    0x1540(%rdi),%r14
    1800169cb:	sub    %rax,%rsi
@@ -40985,77 +40985,77 @@
    180016af9:	pop    %r13
    180016afb:	pop    %r12
    180016afd:	pop    %rdi
    180016afe:	pop    %rsi
    180016aff:	pop    %rbx
    180016b00:	pop    %rbp
    180016b01:	ret
-   180016b02:	lea    0x47dcf(%rip),%rdx        # 0x18005e8d8
+   180016b02:	lea    0x47dd7(%rip),%rdx        # 0x18005e8e0
    180016b09:	lea    -0x21(%rbp),%rcx
    180016b0d:	call   0x180007010
    180016b12:	mov    %rax,%rdx
    180016b15:	lea    -0x69(%rbp),%rcx
    180016b19:	call   0x1800086c0
    180016b1e:	lea    0x5582b(%rip),%rdx        # 0x18006c350
    180016b25:	lea    -0x69(%rbp),%rcx
    180016b29:	call   0x18005c612
    180016b2e:	int3
    180016b2f:	call   *0x47a03(%rip)        # 0x18005e538
    180016b35:	mov    (%rax),%ecx
    180016b37:	call   *0x47a13(%rip)        # 0x18005e550
    180016b3d:	mov    %rax,%r8
-   180016b40:	lea    0x47d81(%rip),%rdx        # 0x18005e8c8
+   180016b40:	lea    0x47d89(%rip),%rdx        # 0x18005e8d0
    180016b47:	lea    -0x21(%rbp),%rcx
    180016b4b:	call   0x18000c070
    180016b50:	mov    %rax,%rdx
    180016b53:	lea    -0x69(%rbp),%rcx
    180016b57:	call   0x1800086c0
    180016b5c:	lea    0x557ed(%rip),%rdx        # 0x18006c350
    180016b63:	lea    -0x69(%rbp),%rcx
    180016b67:	call   0x18005c612
    180016b6c:	int3
-   180016b6d:	lea    0x47d64(%rip),%rdx        # 0x18005e8d8
+   180016b6d:	lea    0x47d6c(%rip),%rdx        # 0x18005e8e0
    180016b74:	lea    -0x21(%rbp),%rcx
    180016b78:	call   0x180007010
    180016b7d:	mov    %rax,%rdx
    180016b80:	lea    -0x69(%rbp),%rcx
    180016b84:	call   0x1800086c0
    180016b89:	lea    0x557c0(%rip),%rdx        # 0x18006c350
    180016b90:	lea    -0x69(%rbp),%rcx
    180016b94:	call   0x18005c612
    180016b99:	int3
    180016b9a:	call   *0x47998(%rip)        # 0x18005e538
    180016ba0:	mov    (%rax),%ecx
    180016ba2:	call   *0x479a8(%rip)        # 0x18005e550
    180016ba8:	mov    %rax,%r8
-   180016bab:	lea    0x47d16(%rip),%rdx        # 0x18005e8c8
+   180016bab:	lea    0x47d1e(%rip),%rdx        # 0x18005e8d0
    180016bb2:	lea    -0x21(%rbp),%rcx
    180016bb6:	call   0x18000c070
    180016bbb:	mov    %rax,%rdx
    180016bbe:	lea    -0x69(%rbp),%rcx
    180016bc2:	call   0x1800086c0
    180016bc7:	lea    0x55782(%rip),%rdx        # 0x18006c350
    180016bce:	lea    -0x69(%rbp),%rcx
    180016bd2:	call   0x18005c612
    180016bd7:	int3
-   180016bd8:	lea    0x47cf9(%rip),%rdx        # 0x18005e8d8
+   180016bd8:	lea    0x47d01(%rip),%rdx        # 0x18005e8e0
    180016bdf:	lea    -0x21(%rbp),%rcx
    180016be3:	call   0x180007010
    180016be8:	mov    %rax,%rdx
    180016beb:	lea    -0x69(%rbp),%rcx
    180016bef:	call   0x1800086c0
    180016bf4:	lea    0x55755(%rip),%rdx        # 0x18006c350
    180016bfb:	lea    -0x69(%rbp),%rcx
    180016bff:	call   0x18005c612
    180016c04:	int3
    180016c05:	call   *0x4792d(%rip)        # 0x18005e538
    180016c0b:	mov    (%rax),%ecx
    180016c0d:	call   *0x4793d(%rip)        # 0x18005e550
    180016c13:	mov    %rax,%r8
-   180016c16:	lea    0x47cab(%rip),%rdx        # 0x18005e8c8
+   180016c16:	lea    0x47cb3(%rip),%rdx        # 0x18005e8d0
    180016c1d:	lea    -0x21(%rbp),%rcx
    180016c21:	call   0x18000c070
    180016c26:	mov    %rax,%rdx
    180016c29:	lea    -0x69(%rbp),%rcx
    180016c2d:	call   0x1800086c0
    180016c32:	lea    0x55717(%rip),%rdx        # 0x18006c350
    180016c39:	lea    -0x69(%rbp),%rcx
@@ -43225,85 +43225,85 @@
    180018c2d:	ret
    180018c2e:	call   *0x4596c(%rip)        # 0x18005e5a0
    180018c34:	int3
    180018c35:	call   *0x458fd(%rip)        # 0x18005e538
    180018c3b:	mov    (%rax),%ecx
    180018c3d:	call   *0x4590d(%rip)        # 0x18005e550
    180018c43:	mov    %rax,%r8
-   180018c46:	lea    0x45cb3(%rip),%rdx        # 0x18005e900
+   180018c46:	lea    0x45cbb(%rip),%rdx        # 0x18005e908
    180018c4d:	lea    -0x38(%rbp),%rcx
    180018c51:	call   0x18000c070
    180018c56:	mov    %rax,%rdx
    180018c59:	lea    -0x50(%rbp),%rcx
    180018c5d:	call   0x1800086c0
    180018c62:	lea    0x536e7(%rip),%rdx        # 0x18006c350
    180018c69:	lea    -0x50(%rbp),%rcx
    180018c6d:	call   0x18005c612
    180018c72:	int3
    180018c73:	call   *0x458bf(%rip)        # 0x18005e538
    180018c79:	mov    (%rax),%ecx
    180018c7b:	call   *0x458cf(%rip)        # 0x18005e550
    180018c81:	mov    %rax,%r8
-   180018c84:	lea    0x45c75(%rip),%rdx        # 0x18005e900
+   180018c84:	lea    0x45c7d(%rip),%rdx        # 0x18005e908
    180018c8b:	lea    -0x38(%rbp),%rcx
    180018c8f:	call   0x18000c070
    180018c94:	mov    %rax,%rdx
    180018c97:	lea    -0x50(%rbp),%rcx
    180018c9b:	call   0x1800086c0
    180018ca0:	lea    0x536a9(%rip),%rdx        # 0x18006c350
    180018ca7:	lea    -0x50(%rbp),%rcx
    180018cab:	call   0x18005c612
    180018cb0:	int3
    180018cb1:	call   *0x45881(%rip)        # 0x18005e538
    180018cb7:	mov    (%rax),%ecx
    180018cb9:	call   *0x45891(%rip)        # 0x18005e550
    180018cbf:	mov    %rax,%r8
-   180018cc2:	lea    0x45c37(%rip),%rdx        # 0x18005e900
+   180018cc2:	lea    0x45c3f(%rip),%rdx        # 0x18005e908
    180018cc9:	lea    -0x38(%rbp),%rcx
    180018ccd:	call   0x18000c070
    180018cd2:	mov    %rax,%rdx
    180018cd5:	lea    -0x50(%rbp),%rcx
    180018cd9:	call   0x1800086c0
    180018cde:	lea    0x5366b(%rip),%rdx        # 0x18006c350
    180018ce5:	lea    -0x50(%rbp),%rcx
    180018ce9:	call   0x18005c612
    180018cee:	int3
    180018cef:	call   *0x45843(%rip)        # 0x18005e538
    180018cf5:	mov    (%rax),%ecx
    180018cf7:	call   *0x45853(%rip)        # 0x18005e550
    180018cfd:	mov    %rax,%r8
-   180018d00:	lea    0x45bf9(%rip),%rdx        # 0x18005e900
+   180018d00:	lea    0x45c01(%rip),%rdx        # 0x18005e908
    180018d07:	lea    -0x38(%rbp),%rcx
    180018d0b:	call   0x18000c070
    180018d10:	mov    %rax,%rdx
    180018d13:	lea    -0x50(%rbp),%rcx
    180018d17:	call   0x1800086c0
    180018d1c:	lea    0x5362d(%rip),%rdx        # 0x18006c350
    180018d23:	lea    -0x50(%rbp),%rcx
    180018d27:	call   0x18005c612
    180018d2c:	int3
    180018d2d:	call   *0x45805(%rip)        # 0x18005e538
    180018d33:	mov    (%rax),%ecx
    180018d35:	call   *0x45815(%rip)        # 0x18005e550
    180018d3b:	mov    %rax,%r8
-   180018d3e:	lea    0x45bbb(%rip),%rdx        # 0x18005e900
+   180018d3e:	lea    0x45bc3(%rip),%rdx        # 0x18005e908
    180018d45:	lea    -0x38(%rbp),%rcx
    180018d49:	call   0x18000c070
    180018d4e:	mov    %rax,%rdx
    180018d51:	lea    -0x50(%rbp),%rcx
    180018d55:	call   0x1800086c0
    180018d5a:	lea    0x535ef(%rip),%rdx        # 0x18006c350
    180018d61:	lea    -0x50(%rbp),%rcx
    180018d65:	call   0x18005c612
    180018d6a:	int3
    180018d6b:	call   *0x457c7(%rip)        # 0x18005e538
    180018d71:	mov    (%rax),%ecx
    180018d73:	call   *0x457d7(%rip)        # 0x18005e550
    180018d79:	mov    %rax,%r8
-   180018d7c:	lea    0x45b7d(%rip),%rdx        # 0x18005e900
+   180018d7c:	lea    0x45b85(%rip),%rdx        # 0x18005e908
    180018d83:	lea    -0x38(%rbp),%rcx
    180018d87:	call   0x18000c070
    180018d8c:	mov    %rax,%rdx
    180018d8f:	lea    -0x50(%rbp),%rcx
    180018d93:	call   0x1800086c0
    180018d98:	lea    0x535b1(%rip),%rdx        # 0x18006c350
    180018d9f:	lea    -0x50(%rbp),%rcx
@@ -43529,15 +43529,15 @@
    180019121:	test   %al,%al
    180019123:	je     0x18001915f
    180019125:	mov    $0x2,%ecx
    18001912a:	call   *0x454e0(%rip)        # 0x18005e610
    180019130:	mov    $0xad6,%r9d
    180019136:	lea    0x45b43(%rip),%r8        # 0x18005ec80
    18001913d:	mov    %rax,%rcx
-   180019140:	lea    0x45719(%rip),%rdx        # 0x18005e860
+   180019140:	lea    0x45721(%rip),%rdx        # 0x18005e868
    180019147:	lea    0x46c12(%rip),%rax        # 0x18005fd60
    18001914e:	mov    %rax,0x20(%rsp)
    180019153:	call   0x1800157c0
    180019158:	call   *0x453fa(%rip)        # 0x18005e558
    18001915e:	int3
    18001915f:	mov    0x17ff0(%rbp),%rax
    180019166:	movslq 0x4(%rax),%rcx
@@ -43568,15 +43568,15 @@
    1800191fe:	cmp    %rdi,%rax
    180019201:	je     0x18001923d
    180019203:	mov    $0x2,%ecx
    180019208:	call   *0x45402(%rip)        # 0x18005e610
    18001920e:	mov    $0xae1,%r9d
    180019214:	lea    0x45a65(%rip),%r8        # 0x18005ec80
    18001921b:	mov    %rax,%rcx
-   18001921e:	lea    0x4563b(%rip),%rdx        # 0x18005e860
+   18001921e:	lea    0x45643(%rip),%rdx        # 0x18005e868
    180019225:	lea    0x46b4c(%rip),%rax        # 0x18005fd78
    18001922c:	mov    %rax,0x20(%rsp)
    180019231:	call   0x1800157c0
    180019236:	call   *0x4531c(%rip)        # 0x18005e558
    18001923c:	int3
    18001923d:	test   %rbx,%rbx
    180019240:	je     0x180019260
@@ -43597,15 +43597,15 @@
    180019281:	cmp    %rdi,%rax
    180019284:	je     0x1800192c0
    180019286:	mov    $0x2,%ecx
    18001928b:	call   *0x4537f(%rip)        # 0x18005e610
    180019291:	mov    $0xaf1,%r9d
    180019297:	lea    0x459e2(%rip),%r8        # 0x18005ec80
    18001929e:	mov    %rax,%rcx
-   1800192a1:	lea    0x455b8(%rip),%rdx        # 0x18005e860
+   1800192a1:	lea    0x455c0(%rip),%rdx        # 0x18005e868
    1800192a8:	lea    0x46af1(%rip),%rax        # 0x18005fda0
    1800192af:	mov    %rax,0x20(%rsp)
    1800192b4:	call   0x1800157c0
    1800192b9:	call   *0x45299(%rip)        # 0x18005e558
    1800192bf:	int3
    1800192c0:	test   %rdi,%rdi
    1800192c3:	je     0x1800192db
@@ -43628,15 +43628,15 @@
    180019310:	cmp    %rax,0x1448(%r15)
    180019317:	je     0x180019353
    180019319:	mov    $0x2,%ecx
    18001931e:	call   *0x452ec(%rip)        # 0x18005e610
    180019324:	mov    $0xb08,%r9d
    18001932a:	lea    0x4594f(%rip),%r8        # 0x18005ec80
    180019331:	mov    %rax,%rcx
-   180019334:	lea    0x45525(%rip),%rdx        # 0x18005e860
+   180019334:	lea    0x4552d(%rip),%rdx        # 0x18005e868
    18001933b:	lea    0x46a8e(%rip),%rax        # 0x18005fdd0
    180019342:	mov    %rax,0x20(%rsp)
    180019347:	call   0x1800157c0
    18001934c:	call   *0x45206(%rip)        # 0x18005e558
    180019352:	int3
    180019353:	mov    0x1428(%r15),%rcx
    18001935a:	call   0x180037970
@@ -43750,15 +43750,15 @@
    180019554:	cmp    %rcx,%rbx
    180019557:	jbe    0x180019593
    180019559:	mov    $0x2,%ecx
    18001955e:	call   *0x450ac(%rip)        # 0x18005e610
    180019564:	mov    $0xb2f,%r9d
    18001956a:	lea    0x4570f(%rip),%r8        # 0x18005ec80
    180019571:	mov    %rax,%rcx
-   180019574:	lea    0x452e5(%rip),%rdx        # 0x18005e860
+   180019574:	lea    0x452ed(%rip),%rdx        # 0x18005e868
    18001957b:	lea    0x4686e(%rip),%rax        # 0x18005fdf0
    180019582:	mov    %rax,0x20(%rsp)
    180019587:	call   0x1800157c0
    18001958c:	call   *0x44fc6(%rip)        # 0x18005e558
    180019592:	int3
    180019593:	mov    %rbx,%rax
    180019596:	mov    0x18ff0(%rbp),%rcx
@@ -112415,168 +112415,171 @@
    18005e819:	jae    0x18005e848
    18005e81b:	jb     0x18005e892
    18005e81d:	outsb  %ds:(%rsi),(%dx)
    18005e81e:	outsb  %ds:(%rsi),(%dx)
    18005e81f:	gs jb  0x18005e87e
    18005e822:	(bad)
    18005e827:	sub    $0x6c697562,%eax
-   18005e82c:	fs pop %rsp
-   18005e82e:	pop    %rdi
-   18005e82f:	ja     0x18005e8a0
-   18005e831:	jb     0x18005e89e
-   18005e833:	pop    %rsp
-   18005e834:	imul   $0x6c6c2d78,0x65(%rax),%esi
-   18005e83b:	insl   (%dx),%es:(%rdi)
-   18005e83c:	pop    %rsp
-   18005e83d:	imul   $0x6c6c2d78,0x65(%rax),%esi
-   18005e844:	insl   (%dx),%es:(%rdi)
-   18005e845:	pop    %rsp
-   18005e846:	jae    0x18005e8ba
-   18005e848:	movsxd 0x6c(%rsp,%rbp,2),%ebx
-   18005e84c:	(bad)
-   18005e84d:	insl   (%dx),%es:(%rdi)
-   18005e84e:	(bad)
-   18005e84f:	pop    %rsp
-   18005e850:	insb   (%dx),%es:(%rdi)
-   18005e851:	insb   (%dx),%es:(%rdi)
+   18005e82c:	fs sub $0x5c77656e,%eax
+   18005e832:	pop    %rdi
+   18005e833:	ja     0x18005e8a4
+   18005e835:	jb     0x18005e8a2
+   18005e837:	pop    %rsp
+   18005e838:	imul   $0x6c6c2d78,0x65(%rax),%esi
+   18005e83f:	insl   (%dx),%es:(%rdi)
+   18005e840:	pop    %rsp
+   18005e841:	imul   $0x6c6c2d78,0x65(%rax),%esi
+   18005e848:	insl   (%dx),%es:(%rdi)
+   18005e849:	pop    %rsp
+   18005e84a:	jae    0x18005e8be
+   18005e84c:	movsxd 0x6c(%rsp,%rbp,2),%ebx
+   18005e850:	(bad)
+   18005e851:	insl   (%dx),%es:(%rdi)
    18005e852:	(bad)
-   18005e853:	insl   (%dx),%es:(%rdi)
-   18005e854:	(bad)
-   18005e855:	sub    $0x6c697475,%eax
-   18005e85a:	cs push $0x0
-   18005e860:	rex.WR
-   18005e861:	rex.WR
-   18005e862:	rex.B
-   18005e863:	rex.WRB
-   18005e864:	pop    %r15
-   18005e866:	push   %r11
-   18005e868:	push   %rbx
-   18005e869:	rex.RB push %r10
-   18005e86b:	push   %rsp
-   18005e86c:	cmp    (%rax),%ah
-   18005e86e:	and    $0x64253a73,%eax
-   18005e873:	cmp    (%rax),%ah
-   18005e875:	and    $0xa73,%eax
-   18005e87a:	add    %al,(%rax)
-   18005e87c:	add    %al,(%rax)
-   18005e87e:	add    %al,(%rax)
-   18005e880:	jae    0x18005e8eb
-   18005e882:	jp     0x18005e8e9
-   18005e884:	xor    (%rax),%ah
-   18005e886:	cmp    $0x6973203d,%eax
-   18005e88b:	jp     0x18005e8f2
-   18005e88d:	add    %al,(%rax)
-   18005e88f:	add    %ah,0x61(%rsi)
-   18005e892:	imul   $0x206f7420,0x64(%rbp,%riz,2),%ebp
-   18005e89a:	outsl  %ds:(%rsi),(%dx)
-   18005e89b:	jo     0x18005e902
-   18005e89d:	outsb  %ds:(%rsi),(%dx)
-   18005e89e:	and    %ah,0x25203a73(%rip)        # 0x1a5262317
-   18005e8a4:	jae    0x18005e8a6
-   18005e8a6:	add    %al,(%rax)
-   18005e8a8:	jb     0x18005e90f
-   18005e8aa:	je     0x18005e8cc
-   18005e8ac:	and    %edi,0x312d20(%rip)        # 0x1803715d2
-   18005e8b2:	add    %al,(%rax)
-   18005e8b4:	add    %al,(%rax)
-   18005e8b6:	add    %al,(%rax)
-   18005e8b8:	jb     0x18005e91f
-   18005e8ba:	je     0x18005e8dc
-   18005e8bc:	cmp    $0x30203d,%eax
-   18005e8c1:	add    %al,(%rax)
-   18005e8c3:	add    %al,(%rax)
-   18005e8c5:	add    %al,(%rax)
-   18005e8c7:	add    %dh,0x65(%rdx)
-   18005e8ca:	(bad)
-   18005e8cb:	and    %ah,%fs:0x72(%rbp)
-   18005e8cf:	jb     0x18005e940
-   18005e8d1:	jb     0x18005e90d
-   18005e8d3:	and    %ah,0x75000073(%rip)        # 0x1f505e94c
-   18005e8d9:	outsb  %ds:(%rsi),(%dx)
-   18005e8da:	gs js  0x18005e94d
-   18005e8dd:	movsxd %gs:0x64(%rbp,%riz,2),%esi
-   18005e8e2:	insb   (%dx),%es:(%rdi)
-   18005e8e3:	jns    0x18005e905
-   18005e8e5:	jb     0x18005e94c
-   18005e8e7:	(bad)
-   18005e8e8:	movsxd 0x65(%rax),%ebp
-   18005e8eb:	and    %ah,%fs:0x6e(%rbp)
-   18005e8ef:	and    %ch,%fs:0x66(%rdi)
-   18005e8f3:	and    %ah,0x69(%rsi)
-   18005e8f6:	insb   (%dx),%es:(%rdi)
-   18005e8f7:	add    %al,%gs:(%rax)
-   18005e8fa:	add    %al,(%rax)
-   18005e8fc:	add    %al,(%rax)
-   18005e8fe:	add    %al,(%rax)
-   18005e900:	ja     0x18005e974
-   18005e902:	imul   $0x6f727265,0x20(%rbp,%riz,2),%esi
-   18005e90a:	jb     0x18005e946
-   18005e90c:	and    %ah,0x6f460073(%rip)        # 0x1ef4be985
-   18005e912:	jb     0x18005e981
-   18005e914:	(bad)
-   18005e915:	je     0x18005e964
-   18005e917:	gs jae 0x18005e98d
-   18005e91a:	(bad)
-   18005e91b:	and    %spl,%gs:0x61(%r14d)
-   18005e921:	imul   $0x43000000,0x64(%rbp,%riz,2),%ebp
-   18005e929:	jb     0x18005e990
-   18005e92b:	(bad)
-   18005e92c:	je     0x18005e993
-   18005e92e:	imul   $0x69707061,0x4d(%rbp,%r12,2),%r13d
-   18005e937:	outsb  %ds:(%rsi),(%dx)
-   18005e938:	and    %spl,0x61(%r14d)
-   18005e93d:	imul   $0x7325203a,0x64(%rbp,%riz,2),%ebp
-   18005e945:	add    %al,(%rax)
-   18005e947:	add    %cl,0x61(%rbp)
-   18005e94a:	jo     0x18005e9a2
-   18005e94c:	imul   $0x6946664f,0x77(%rbp),%esp
-   18005e953:	insb   (%dx),%es:(%rdi)
-   18005e954:	and    %ah,%gs:0x61(%rsi)
-   18005e958:	imul   $0x7325203a,0x64(%rbp,%riz,2),%ebp
-	...
-   18005e968:	ja     0x18005e9cb
-   18005e96a:	jb     0x18005e9da
-   18005e96c:	imul   $0x7250203a,0x67(%rsi),%ebp
-   18005e973:	gs data16 gs je 0x18005e9db
-   18005e978:	push   $0x74726956
-   18005e97d:	jne    0x18005e9e0
-   18005e97f:	insb   (%dx),%es:(%rdi)
-   18005e980:	rex.WRB
-   18005e981:	gs insl (%dx),%es:(%rdi)
-   18005e983:	outsl  %ds:(%rsi),(%dx)
-   18005e984:	jb     0x18005e9ff
-   18005e986:	and    %ah,0x61(%rsi)
-   18005e989:	imul   $0x7325203a,0x64(%rbp,%riz,2),%ebp
-   18005e991:	or     (%rax),%al
-   18005e993:	add    %al,(%rax)
-   18005e995:	add    %al,(%rax)
-   18005e997:	add    %dh,0x61(%rdi)
-   18005e99a:	jb     0x18005ea0a
-   18005e99c:	imul   $0x6e55203a,0x67(%rsi),%ebp
-   18005e9a3:	insl   (%dx),%es:(%rdi)
-   18005e9a4:	(bad)
-   18005e9a5:	jo     0x18005e9fd
-   18005e9a7:	imul   $0x6946664f,0x77(%rbp),%esp
-   18005e9ae:	insb   (%dx),%es:(%rdi)
-   18005e9af:	and    %ah,%gs:0x61(%rsi)
-   18005e9b3:	imul   $0x7325203a,0x64(%rbp,%riz,2),%ebp
-   18005e9bb:	or     (%rax),%al
-   18005e9bd:	add    %al,(%rax)
-   18005e9bf:	add    %ah,0x64(%rcx)
-   18005e9c2:	fs jb  0x18005e9e5
-   18005e9c5:	cmp    $0x554e203d,%eax
-   18005e9ca:	rex.WR
-   18005e9cb:	rex.WR and %r12b,(%rsi)
-   18005e9ce:	es and %dh,0x69(%rbx)
-   18005e9d2:	jp     0x18005ea39
-   18005e9d4:	and    %bh,0x30203d(%rip)        # 0x180360a17
-   18005e9da:	add    %al,(%rax)
-   18005e9dc:	(bad)
-   18005e9dd:	fs fs jb 0x18005e9e1
+   18005e853:	pop    %rsp
+   18005e854:	insb   (%dx),%es:(%rdi)
+   18005e855:	insb   (%dx),%es:(%rdi)
+   18005e856:	(bad)
+   18005e857:	insl   (%dx),%es:(%rdi)
+   18005e858:	(bad)
+   18005e859:	sub    $0x6c697475,%eax
+   18005e85e:	cs push $0x0
+   18005e864:	add    %al,(%rax)
+   18005e866:	add    %al,(%rax)
+   18005e868:	rex.WR
+   18005e869:	rex.WR
+   18005e86a:	rex.B
+   18005e86b:	rex.WRB
+   18005e86c:	pop    %r15
+   18005e86e:	push   %r11
+   18005e870:	push   %rbx
+   18005e871:	rex.RB push %r10
+   18005e873:	push   %rsp
+   18005e874:	cmp    (%rax),%ah
+   18005e876:	and    $0x64253a73,%eax
+   18005e87b:	cmp    (%rax),%ah
+   18005e87d:	and    $0xa73,%eax
+   18005e882:	add    %al,(%rax)
+   18005e884:	add    %al,(%rax)
+   18005e886:	add    %al,(%rax)
+   18005e888:	jae    0x18005e8f3
+   18005e88a:	jp     0x18005e8f1
+   18005e88c:	xor    (%rax),%ah
+   18005e88e:	cmp    $0x6973203d,%eax
+   18005e893:	jp     0x18005e8fa
+   18005e895:	add    %al,(%rax)
+   18005e897:	add    %ah,0x61(%rsi)
+   18005e89a:	imul   $0x206f7420,0x64(%rbp,%riz,2),%ebp
+   18005e8a2:	outsl  %ds:(%rsi),(%dx)
+   18005e8a3:	jo     0x18005e90a
+   18005e8a5:	outsb  %ds:(%rsi),(%dx)
+   18005e8a6:	and    %ah,0x25203a73(%rip)        # 0x1a526231f
+   18005e8ac:	jae    0x18005e8ae
+   18005e8ae:	add    %al,(%rax)
+   18005e8b0:	jb     0x18005e917
+   18005e8b2:	je     0x18005e8d4
+   18005e8b4:	and    %edi,0x312d20(%rip)        # 0x1803715da
+   18005e8ba:	add    %al,(%rax)
+   18005e8bc:	add    %al,(%rax)
+   18005e8be:	add    %al,(%rax)
+   18005e8c0:	jb     0x18005e927
+   18005e8c2:	je     0x18005e8e4
+   18005e8c4:	cmp    $0x30203d,%eax
+   18005e8c9:	add    %al,(%rax)
+   18005e8cb:	add    %al,(%rax)
+   18005e8cd:	add    %al,(%rax)
+   18005e8cf:	add    %dh,0x65(%rdx)
+   18005e8d2:	(bad)
+   18005e8d3:	and    %ah,%fs:0x72(%rbp)
+   18005e8d7:	jb     0x18005e948
+   18005e8d9:	jb     0x18005e915
+   18005e8db:	and    %ah,0x75000073(%rip)        # 0x1f505e954
+   18005e8e1:	outsb  %ds:(%rsi),(%dx)
+   18005e8e2:	gs js  0x18005e955
+   18005e8e5:	movsxd %gs:0x64(%rbp,%riz,2),%esi
+   18005e8ea:	insb   (%dx),%es:(%rdi)
+   18005e8eb:	jns    0x18005e90d
+   18005e8ed:	jb     0x18005e954
+   18005e8ef:	(bad)
+   18005e8f0:	movsxd 0x65(%rax),%ebp
+   18005e8f3:	and    %ah,%fs:0x6e(%rbp)
+   18005e8f7:	and    %ch,%fs:0x66(%rdi)
+   18005e8fb:	and    %ah,0x69(%rsi)
+   18005e8fe:	insb   (%dx),%es:(%rdi)
+   18005e8ff:	add    %al,%gs:(%rax)
+   18005e902:	add    %al,(%rax)
+   18005e904:	add    %al,(%rax)
+   18005e906:	add    %al,(%rax)
+   18005e908:	ja     0x18005e97c
+   18005e90a:	imul   $0x6f727265,0x20(%rbp,%riz,2),%esi
+   18005e912:	jb     0x18005e94e
+   18005e914:	and    %ah,0x6f460073(%rip)        # 0x1ef4be98d
+   18005e91a:	jb     0x18005e989
+   18005e91c:	(bad)
+   18005e91d:	je     0x18005e96c
+   18005e91f:	gs jae 0x18005e995
+   18005e922:	(bad)
+   18005e923:	and    %spl,%gs:0x61(%r14d)
+   18005e929:	imul   $0x43000000,0x64(%rbp,%riz,2),%ebp
+   18005e931:	jb     0x18005e998
+   18005e933:	(bad)
+   18005e934:	je     0x18005e99b
+   18005e936:	imul   $0x69707061,0x4d(%rbp,%r12,2),%r13d
+   18005e93f:	outsb  %ds:(%rsi),(%dx)
+   18005e940:	and    %spl,0x61(%r14d)
+   18005e945:	imul   $0x7325203a,0x64(%rbp,%riz,2),%ebp
+   18005e94d:	add    %al,(%rax)
+   18005e94f:	add    %cl,0x61(%rbp)
+   18005e952:	jo     0x18005e9aa
+   18005e954:	imul   $0x6946664f,0x77(%rbp),%esp
+   18005e95b:	insb   (%dx),%es:(%rdi)
+   18005e95c:	and    %ah,%gs:0x61(%rsi)
+   18005e960:	imul   $0x7325203a,0x64(%rbp,%riz,2),%ebp
 	...
+   18005e970:	ja     0x18005e9d3
+   18005e972:	jb     0x18005e9e2
+   18005e974:	imul   $0x7250203a,0x67(%rsi),%ebp
+   18005e97b:	gs data16 gs je 0x18005e9e3
+   18005e980:	push   $0x74726956
+   18005e985:	jne    0x18005e9e8
+   18005e987:	insb   (%dx),%es:(%rdi)
+   18005e988:	rex.WRB
+   18005e989:	gs insl (%dx),%es:(%rdi)
+   18005e98b:	outsl  %ds:(%rsi),(%dx)
+   18005e98c:	jb     0x18005ea07
+   18005e98e:	and    %ah,0x61(%rsi)
+   18005e991:	imul   $0x7325203a,0x64(%rbp,%riz,2),%ebp
+   18005e999:	or     (%rax),%al
+   18005e99b:	add    %al,(%rax)
+   18005e99d:	add    %al,(%rax)
+   18005e99f:	add    %dh,0x61(%rdi)
+   18005e9a2:	jb     0x18005ea12
+   18005e9a4:	imul   $0x6e55203a,0x67(%rsi),%ebp
+   18005e9ab:	insl   (%dx),%es:(%rdi)
+   18005e9ac:	(bad)
+   18005e9ad:	jo     0x18005ea05
+   18005e9af:	imul   $0x6946664f,0x77(%rbp),%esp
+   18005e9b6:	insb   (%dx),%es:(%rdi)
+   18005e9b7:	and    %ah,%gs:0x61(%rsi)
+   18005e9bb:	imul   $0x7325203a,0x64(%rbp,%riz,2),%ebp
+   18005e9c3:	or     (%rax),%al
+   18005e9c5:	add    %al,(%rax)
+   18005e9c7:	add    %ah,0x64(%rcx)
+   18005e9ca:	fs jb  0x18005e9ed
+   18005e9cd:	cmp    $0x554e203d,%eax
+   18005e9d2:	rex.WR
+   18005e9d3:	rex.WR and %r12b,(%rsi)
+   18005e9d6:	es and %dh,0x69(%rbx)
+   18005e9da:	jp     0x18005ea41
+   18005e9dc:	and    %bh,0x30203d(%rip)        # 0x180360a1f
+   18005e9e2:	add    %al,(%rax)
+   18005e9e4:	(bad)
+   18005e9e5:	fs fs jb 0x18005e9e9
+   18005e9e9:	add    %al,(%rax)
+   18005e9eb:	add    %al,(%rax)
    18005e9ed:	add    %al,(%rax)
    18005e9ef:	add    %dh,0x61(%rdi)
    18005e9f2:	jb     0x18005ea62
    18005e9f4:	imul   $0x6166203a,0x67(%rsi),%ebp
    18005e9fb:	imul   $0x206f7420,0x64(%rbp,%riz,2),%ebp
    18005ea03:	push   %rsi
    18005ea04:	imul   $0x4c6c6175,0x74(%rdx),%esi
@@ -112804,50 +112807,53 @@
    18005ec89:	jae    0x18005ecb8
    18005ec8b:	jb     0x18005ed02
    18005ec8d:	outsb  %ds:(%rsi),(%dx)
    18005ec8e:	outsb  %ds:(%rsi),(%dx)
    18005ec8f:	gs jb  0x18005ecee
    18005ec92:	(bad)
    18005ec97:	sub    $0x6c697562,%eax
-   18005ec9c:	fs pop %rsp
-   18005ec9e:	pop    %rdi
-   18005ec9f:	ja     0x18005ed10
-   18005eca1:	jb     0x18005ed0e
-   18005eca3:	pop    %rsp
-   18005eca4:	imul   $0x6c6c2d78,0x65(%rax),%esi
-   18005ecab:	insl   (%dx),%es:(%rdi)
-   18005ecac:	pop    %rsp
-   18005ecad:	imul   $0x6c6c2d78,0x65(%rax),%esi
-   18005ecb4:	insl   (%dx),%es:(%rdi)
-   18005ecb5:	pop    %rsp
-   18005ecb6:	jae    0x18005ed2a
-   18005ecb8:	movsxd 0x6c(%rsp,%rbp,2),%ebx
-   18005ecbc:	(bad)
-   18005ecbd:	insl   (%dx),%es:(%rdi)
-   18005ecbe:	(bad)
-   18005ecbf:	pop    %rsp
-   18005ecc0:	insb   (%dx),%es:(%rdi)
-   18005ecc1:	insb   (%dx),%es:(%rdi)
+   18005ec9c:	fs sub $0x5c77656e,%eax
+   18005eca2:	pop    %rdi
+   18005eca3:	ja     0x18005ed14
+   18005eca5:	jb     0x18005ed12
+   18005eca7:	pop    %rsp
+   18005eca8:	imul   $0x6c6c2d78,0x65(%rax),%esi
+   18005ecaf:	insl   (%dx),%es:(%rdi)
+   18005ecb0:	pop    %rsp
+   18005ecb1:	imul   $0x6c6c2d78,0x65(%rax),%esi
+   18005ecb8:	insl   (%dx),%es:(%rdi)
+   18005ecb9:	pop    %rsp
+   18005ecba:	jae    0x18005ed2e
+   18005ecbc:	movsxd 0x6c(%rsp,%rbp,2),%ebx
+   18005ecc0:	(bad)
+   18005ecc1:	insl   (%dx),%es:(%rdi)
    18005ecc2:	(bad)
-   18005ecc3:	insl   (%dx),%es:(%rdi)
-   18005ecc4:	(bad)
-   18005ecc5:	cs movsxd 0x70(%rax),%esi
-   18005ecc9:	add    %al,(%rax)
-   18005eccb:	add    %dh,0x62(%rdx)
-   18005ecce:	add    %al,(%rax)
-   18005ecd0:	(bad)
-   18005ecd5:	sub    $0x3a6d6c6c,%eax
-   18005ecda:	and    %ch,0x61(%rdi,%rbp,2)
-   18005ecde:	imul   $0x646f6d20,%fs:0x67(%rsi),%ebp
-   18005ece6:	gs insb (%dx),%es:(%rdi)
-   18005ece8:	and    %ah,0x72(%rsi)
-   18005eceb:	outsl  %ds:(%rsi),(%dx)
-   18005ecec:	insl   (%dx),%es:(%rdi)
-   18005eced:	and    %ah,0xa73(%rip)        # 0x18005f766
-	...
+   18005ecc3:	pop    %rsp
+   18005ecc4:	insb   (%dx),%es:(%rdi)
+   18005ecc5:	insb   (%dx),%es:(%rdi)
+   18005ecc6:	(bad)
+   18005ecc7:	insl   (%dx),%es:(%rdi)
+   18005ecc8:	(bad)
+   18005ecc9:	cs movsxd 0x70(%rax),%esi
+   18005eccd:	add    %al,(%rax)
+   18005eccf:	add    %dh,0x62(%rdx)
+   18005ecd2:	add    %al,(%rax)
+   18005ecd4:	add    %al,(%rax)
+   18005ecd6:	add    %al,(%rax)
+   18005ecd8:	(bad)
+   18005ecdd:	sub    $0x3a6d6c6c,%eax
+   18005ece2:	and    %ch,0x61(%rdi,%rbp,2)
+   18005ece6:	imul   $0x646f6d20,%fs:0x67(%rsi),%ebp
+   18005ecee:	gs insb (%dx),%es:(%rdi)
+   18005ecf0:	and    %ah,0x72(%rsi)
+   18005ecf3:	outsl  %ds:(%rsi),(%dx)
+   18005ecf4:	insl   (%dx),%es:(%rdi)
+   18005ecf5:	and    %ah,0xa73(%rip)        # 0x18005f76e
+   18005ecfb:	add    %al,(%rax)
+   18005ecfd:	add    %al,(%rax)
    18005ecff:	add    %dh,0x6e(%rbp)
    18005ed02:	imul   $0x77,0x6f(%rsi),%ebp
    18005ed06:	outsb  %ds:(%rsi),(%dx)
    18005ed07:	and    %ch,(%rax)
    18005ed09:	insl   (%dx),%es:(%rdi)
    18005ed0a:	(bad)
    18005ed0b:	imul   $0x72657620,0x2c(%ebx),%esp
@@ -119315,32 +119321,30 @@
    180063089:	jae    0x1800630b8
    18006308b:	jb     0x180063102
    18006308d:	outsb  %ds:(%rsi),(%dx)
    18006308e:	outsb  %ds:(%rsi),(%dx)
    18006308f:	gs jb  0x1800630ee
    180063092:	(bad)
    180063097:	sub    $0x6c697562,%eax
-   18006309c:	fs pop %rsp
-   18006309e:	pop    %rdi
-   18006309f:	ja     0x180063110
-   1800630a1:	jb     0x18006310e
-   1800630a3:	pop    %rsp
-   1800630a4:	imul   $0x6c6c2d78,0x65(%rax),%esi
-   1800630ab:	insl   (%dx),%es:(%rdi)
-   1800630ac:	pop    %rsp
-   1800630ad:	imul   $0x6c6c2d78,0x65(%rax),%esi
-   1800630b4:	insl   (%dx),%es:(%rdi)
-   1800630b5:	pop    %rsp
-   1800630b6:	jae    0x18006312a
-   1800630b8:	movsxd 0x67(%rdi,%riz,2),%ebx
-   1800630bc:	insl   (%dx),%es:(%rdi)
-   1800630bd:	insb   (%dx),%es:(%rdi)
-   1800630be:	cs movsxd (%rax),%eax
-   1800630c1:	add    %al,(%rax)
-   1800630c3:	add    %al,(%rax)
+   18006309c:	fs sub $0x5c77656e,%eax
+   1800630a2:	pop    %rdi
+   1800630a3:	ja     0x180063114
+   1800630a5:	jb     0x180063112
+   1800630a7:	pop    %rsp
+   1800630a8:	imul   $0x6c6c2d78,0x65(%rax),%esi
+   1800630af:	insl   (%dx),%es:(%rdi)
+   1800630b0:	pop    %rsp
+   1800630b1:	imul   $0x6c6c2d78,0x65(%rax),%esi
+   1800630b8:	insl   (%dx),%es:(%rdi)
+   1800630b9:	pop    %rsp
+   1800630ba:	jae    0x18006312e
+   1800630bc:	movsxd 0x67(%rdi,%riz,2),%ebx
+   1800630c0:	insl   (%dx),%es:(%rdi)
+   1800630c1:	insb   (%dx),%es:(%rdi)
+   1800630c2:	cs movsxd (%rax),%eax
    1800630c5:	add    %al,(%rax)
    1800630c7:	add    %al,0x47(%rdi)
    1800630ca:	rex.WRB
    1800630cb:	rex.WR pop %rdi
    1800630cd:	push   %r11
    1800630cf:	push   %rbx
    1800630d0:	rex.RB push %r10
@@ -122608,19 +122612,17 @@
    1800651c0:	enter  $0x5e6,$0x80
    1800651c4:	add    %eax,(%rax)
    1800651c6:	add    %al,(%rax)
    1800651c8:	shl    $1,%dh
    1800651ca:	add    $0x180,%eax
    1800651cf:	add    %al,(%rax)
    1800651d1:	add    %al,(%rax)
-   1800651d3:	add    %dl,0x38(%rcx)
-   1800651d6:	pop    %rbx
-   1800651d7:	data16 add %al,(%rax)
-   1800651da:	add    %al,(%rax)
-   1800651dc:	or     $0x50000000,%eax
+   1800651d3:	add    %bl,0x665c89(%rdi)
+   1800651d9:	add    %al,(%rax)
+   1800651db:	add    %cl,0x50000000(%rip)        # 0x1d00651e1
    1800651e1:	add    (%rax),%eax
    1800651e3:	add    %al,(%rax)
    1800651e5:	pop    %rsi
    1800651e6:	(bad)
    1800651e7:	add    %al,(%rax)
    1800651e9:	rex.WX (bad)
 	...
```

## ipex_llm/libs/libstarcoder_avx.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180069618
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Sat Jun  1 15:02:57 2024
+Time/Date		Sun Jun  2 15:03:45 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000069c00
 SizeOfInitializedData	00000000000c8600
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000069618
@@ -132676,30 +132676,32 @@
    18006ee19:	jae    0x18006ee48
    18006ee1b:	jb     0x18006ee92
    18006ee1d:	outsb  %ds:(%rsi),(%dx)
    18006ee1e:	outsb  %ds:(%rsi),(%dx)
    18006ee1f:	gs jb  0x18006ee7e
    18006ee22:	(bad)
    18006ee27:	sub    $0x6c697562,%eax
-   18006ee2c:	fs sub $0x5c77656e,%eax
-   18006ee32:	pop    %rdi
-   18006ee33:	ja     0x18006eea4
-   18006ee35:	jb     0x18006eea2
-   18006ee37:	pop    %rsp
-   18006ee38:	imul   $0x6c6c2d78,0x65(%rax),%esi
-   18006ee3f:	insl   (%dx),%es:(%rdi)
-   18006ee40:	pop    %rsp
-   18006ee41:	imul   $0x6c6c2d78,0x65(%rax),%esi
-   18006ee48:	insl   (%dx),%es:(%rdi)
-   18006ee49:	pop    %rsp
-   18006ee4a:	jae    0x18006eebe
-   18006ee4c:	movsxd 0x67(%rdi,%riz,2),%ebx
-   18006ee50:	insl   (%dx),%es:(%rdi)
-   18006ee51:	insb   (%dx),%es:(%rdi)
-   18006ee52:	cs movsxd (%rax),%eax
+   18006ee2c:	fs pop %rsp
+   18006ee2e:	pop    %rdi
+   18006ee2f:	ja     0x18006eea0
+   18006ee31:	jb     0x18006ee9e
+   18006ee33:	pop    %rsp
+   18006ee34:	imul   $0x6c6c2d78,0x65(%rax),%esi
+   18006ee3b:	insl   (%dx),%es:(%rdi)
+   18006ee3c:	pop    %rsp
+   18006ee3d:	imul   $0x6c6c2d78,0x65(%rax),%esi
+   18006ee44:	insl   (%dx),%es:(%rdi)
+   18006ee45:	pop    %rsp
+   18006ee46:	jae    0x18006eeba
+   18006ee48:	movsxd 0x67(%rdi,%riz,2),%ebx
+   18006ee4c:	insl   (%dx),%es:(%rdi)
+   18006ee4d:	insb   (%dx),%es:(%rdi)
+   18006ee4e:	cs movsxd (%rax),%eax
+   18006ee51:	add    %al,(%rax)
+   18006ee53:	add    %al,(%rax)
    18006ee55:	add    %al,(%rax)
    18006ee57:	add    %al,0x47(%rdi)
    18006ee5a:	rex.WRB
    18006ee5b:	rex.WR pop %rdi
    18006ee5d:	push   %r11
    18006ee5f:	push   %rbx
    18006ee60:	rex.RB push %r10
@@ -138722,17 +138724,15 @@
    180072c85:	add    %al,(%rax)
    180072c87:	add    %al,%al
    180072c89:	mov    $0x6,%dh
    180072c8b:	addb   $0x0,(%rcx)
    180072c8e:	add    %al,(%rax)
    180072c90:	add    %al,(%rax)
    180072c92:	add    %al,(%rax)
-   180072c94:	and    %edi,(%rax)
-   180072c96:	pop    %rbx
-   180072c97:	data16 add %al,(%rax)
+   180072c94:	rorl   $1,0x665c(%rcx)
    180072c9a:	add    %al,(%rax)
    180072c9c:	or     $0x50000000,%eax
    180072ca1:	add    (%rax),%eax
    180072ca3:	add    %dl,0x3e(%rax)
    180072ca6:	(bad)
    180072ca7:	add    %dl,0x2e(%rax)
    180072caa:	(bad)
```

## ipex_llm/libs/libstarcoder_vnni.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180063598
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Sat Jun  1 15:03:45 2024
+Time/Date		Sun Jun  2 15:02:55 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000063c00
 SizeOfInitializedData	00000000000c8000
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000063598
@@ -127106,32 +127106,30 @@
    180068e49:	jae    0x180068e78
    180068e4b:	jb     0x180068ec2
    180068e4d:	outsb  %ds:(%rsi),(%dx)
    180068e4e:	outsb  %ds:(%rsi),(%dx)
    180068e4f:	gs jb  0x180068eae
    180068e52:	(bad)
    180068e57:	sub    $0x6c697562,%eax
-   180068e5c:	fs pop %rsp
-   180068e5e:	pop    %rdi
-   180068e5f:	ja     0x180068ed0
-   180068e61:	jb     0x180068ece
-   180068e63:	pop    %rsp
-   180068e64:	imul   $0x6c6c2d78,0x65(%rax),%esi
-   180068e6b:	insl   (%dx),%es:(%rdi)
-   180068e6c:	pop    %rsp
-   180068e6d:	imul   $0x6c6c2d78,0x65(%rax),%esi
-   180068e74:	insl   (%dx),%es:(%rdi)
-   180068e75:	pop    %rsp
-   180068e76:	jae    0x180068eea
-   180068e78:	movsxd 0x67(%rdi,%riz,2),%ebx
-   180068e7c:	insl   (%dx),%es:(%rdi)
-   180068e7d:	insb   (%dx),%es:(%rdi)
-   180068e7e:	cs movsxd (%rax),%eax
-   180068e81:	add    %al,(%rax)
-   180068e83:	add    %al,(%rax)
+   180068e5c:	fs sub $0x5c77656e,%eax
+   180068e62:	pop    %rdi
+   180068e63:	ja     0x180068ed4
+   180068e65:	jb     0x180068ed2
+   180068e67:	pop    %rsp
+   180068e68:	imul   $0x6c6c2d78,0x65(%rax),%esi
+   180068e6f:	insl   (%dx),%es:(%rdi)
+   180068e70:	pop    %rsp
+   180068e71:	imul   $0x6c6c2d78,0x65(%rax),%esi
+   180068e78:	insl   (%dx),%es:(%rdi)
+   180068e79:	pop    %rsp
+   180068e7a:	jae    0x180068eee
+   180068e7c:	movsxd 0x67(%rdi,%riz,2),%ebx
+   180068e80:	insl   (%dx),%es:(%rdi)
+   180068e81:	insb   (%dx),%es:(%rdi)
+   180068e82:	cs movsxd (%rax),%eax
    180068e85:	add    %al,(%rax)
    180068e87:	add    %al,0x47(%rdi)
    180068e8a:	rex.WRB
    180068e8b:	rex.WR pop %rdi
    180068e8d:	push   %r11
    180068e8f:	push   %rbx
    180068e90:	rex.RB push %r10
@@ -133231,19 +133229,18 @@
    18006cd57:	add    %al,%al
    18006cd59:	push   %rsi
    18006cd5a:	(bad)
    18006cd5b:	addb   $0x0,(%rcx)
    18006cd5e:	add    %al,(%rax)
    18006cd60:	add    %al,(%rax)
    18006cd62:	add    %al,(%rax)
-   18006cd64:	push   %rcx
-   18006cd65:	cmp    %bl,0x66(%rbx)
-   18006cd68:	add    %al,(%rax)
-   18006cd6a:	add    %al,(%rax)
-   18006cd6c:	or     $0x50000000,%eax
+   18006cd64:	lahf
+   18006cd65:	mov    %ebx,0x0(%rsi,%riz,2)
+   18006cd69:	add    %al,(%rax)
+   18006cd6b:	add    %cl,0x50000000(%rip)        # 0x1d006cd71
    18006cd71:	add    (%rax),%eax
    18006cd73:	add    %dl,%al
    18006cd75:	fiadds (%rsi)
    18006cd77:	add    %dl,%al
    18006cd79:	(bad)
    18006cd7a:	(bad)
    18006cd7b:	add    %al,(%rax)
```

## ipex_llm/libs/llama-api.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180002dac
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Sat Jun  1 15:02:42 2024
+Time/Date		Sun Jun  2 15:02:41 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000002800
 SizeOfInitializedData	0000000000003e00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000002dac
@@ -5355,19 +5355,18 @@
    180004a20:	cmp    %al,0x0(%rdx)
    180004a23:	addb   $0x0,(%rcx)
    180004a26:	add    %al,(%rax)
    180004a28:	rex
    180004a29:	rex.X add %al,0x1(%rax)
    180004a30:	add    %al,(%rax)
    180004a32:	add    %al,(%rax)
-   180004a34:	adc    (%rax),%bh
-   180004a36:	pop    %rbx
-   180004a37:	data16 add %al,(%rax)
-   180004a3a:	add    %al,(%rax)
-   180004a3c:	or     $0xe0000000,%eax
+   180004a34:	xchg   %eax,%ecx
+   180004a35:	mov    %ebx,0x0(%rsi,%riz,2)
+   180004a39:	add    %al,(%rax)
+   180004a3b:	add    %cl,-0x20000000(%rip)        # 0x160004a41
    180004a41:	add    (%rax),%al
    180004a43:	add    %ah,%ah
    180004a45:	rex.WR add %r8b,(%rax)
    180004a48:	in     $0x38,%al
 	...
    180004a7e:	add    %al,(%rax)
    180004a80:	add    %eax,(%rax)
```

## ipex_llm/libs/llama.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x000000018005be98
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Sat Jun  1 15:02:42 2024
+Time/Date		Sun Jun  2 15:02:42 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		000000000005c600
 SizeOfInitializedData	00000000000c6400
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000005be98
@@ -122484,19 +122484,17 @@
    1800651e0:	enter  $0x5e6,$0x80
    1800651e4:	add    %eax,(%rax)
    1800651e6:	add    %al,(%rax)
    1800651e8:	shl    $1,%dh
    1800651ea:	add    $0x180,%eax
    1800651ef:	add    %al,(%rax)
    1800651f1:	add    %al,(%rax)
-   1800651f3:	add    %dl,(%rdx)
-   1800651f5:	cmp    %bl,0x66(%rbx)
-   1800651f8:	add    %al,(%rax)
-   1800651fa:	add    %al,(%rax)
-   1800651fc:	or     $0x50000000,%eax
+   1800651f3:	add    %dl,0x665c89(%rdx)
+   1800651f9:	add    %al,(%rax)
+   1800651fb:	add    %cl,0x50000000(%rip)        # 0x1d0065201
    180065201:	add    (%rax),%eax
    180065203:	add    %al,-0x7ffff9a2(%rax)
    180065209:	rex.W (bad)
 	...
    18006527f:	add    %dh,%al
    180065281:	(bad)
    180065282:	(bad)
```

## ipex_llm/libs/main-bloom.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x000000014001045c
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Sat Jun  1 15:02:42 2024
+Time/Date		Sun Jun  2 15:02:41 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000010800
 SizeOfInitializedData	0000000000008e00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000001045c
@@ -25509,19 +25509,18 @@
    140014ab0:	enter  $0x125,$0x40
    140014ab4:	add    %eax,(%rax)
    140014ab6:	add    %al,(%rax)
    140014ab8:	shlb   $1,0x14001(%rip)        # 0x140028abf
    140014abe:	add    %al,(%rax)
    140014ac0:	add    %al,(%rax)
    140014ac2:	add    %al,(%rax)
-   140014ac4:	adc    (%rax),%bh
-   140014ac6:	pop    %rbx
-   140014ac7:	data16 add %al,(%rax)
-   140014aca:	add    %al,(%rax)
-   140014acc:	or     $0x20000000,%eax
+   140014ac4:	xchg   %eax,%ecx
+   140014ac5:	mov    %ebx,0x0(%rsi,%riz,2)
+   140014ac9:	add    %al,(%rax)
+   140014acb:	add    %cl,0x20000000(%rip)        # 0x160014ad1
    140014ad1:	add    (%rax),%eax
    140014ad3:	add    %cl,%ah
    140014ad5:	push   %rsp
    140014ad6:	add    %eax,(%rax)
    140014ad8:	int3
    140014ad9:	rex add %eax,(%rax)
 	...
```

## ipex_llm/libs/main-gptneox.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x000000014000ef6c
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Sat Jun  1 15:02:42 2024
+Time/Date		Sun Jun  2 15:02:41 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		000000000000f200
 SizeOfInitializedData	0000000000009400
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000000ef6c
@@ -24136,19 +24136,18 @@
    140013edf:	add    %ch,%al
    140013ee1:	adc    $0x14001,%eax
    140013ee6:	add    %al,(%rax)
    140013ee8:	lock adc $0x14001,%eax
    140013eee:	add    %al,(%rax)
    140013ef0:	add    %al,(%rax)
    140013ef2:	add    %al,(%rax)
-   140013ef4:	adc    (%rax),%bh
-   140013ef6:	pop    %rbx
-   140013ef7:	data16 add %al,(%rax)
-   140013efa:	add    %al,(%rax)
-   140013efc:	or     $0x90000000,%eax
+   140013ef4:	xchg   %eax,%ecx
+   140013ef5:	mov    %ebx,0x0(%rsi,%riz,2)
+   140013ef9:	add    %al,(%rax)
+   140013efb:	add    %cl,-0x70000000(%rip)        # 0xd0013f01
    140013f01:	add    (%rax),%eax
    140013f03:	add    %ch,0x1(%rcx,%rcx,2)
    140013f07:	add    %ch,0x1(%rdi,%rbp,1)
 	...
    140013f7f:	add    %ah,(%rax)
    140013f81:	add    %r8,0x1(%r8)
    140013f85:	add    %al,(%rax)
```

## ipex_llm/libs/main-llama.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x000000014000f32c
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Sat Jun  1 15:02:42 2024
+Time/Date		Sun Jun  2 15:02:41 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		000000000000f600
 SizeOfInitializedData	0000000000009400
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000000f32c
@@ -24679,19 +24679,18 @@
    140013faf:	add    %ch,%al
    140013fb1:	adc    $0x14001,%eax
    140013fb6:	add    %al,(%rax)
    140013fb8:	lock adc $0x14001,%eax
    140013fbe:	add    %al,(%rax)
    140013fc0:	add    %al,(%rax)
    140013fc2:	add    %al,(%rax)
-   140013fc4:	adc    (%rax),%bh
-   140013fc6:	pop    %rbx
-   140013fc7:	data16 add %al,(%rax)
-   140013fca:	add    %al,(%rax)
-   140013fcc:	or     $0x90000000,%eax
+   140013fc4:	xchg   %eax,%ecx
+   140013fc5:	mov    %ebx,0x0(%rsi,%riz,2)
+   140013fc9:	add    %al,(%rax)
+   140013fcb:	add    %cl,-0x70000000(%rip)        # 0xd0013fd1
    140013fd1:	add    (%rax),%eax
    140013fd3:	add    %ch,%ah
    140013fd5:	add    %rax,(%r8)
    140013fd8:	in     (%dx),%al
    140013fd9:	xor    (%rcx),%eax
 	...
    140013fff:	add    %ah,0x140014d(%rax)
```

## ipex_llm/libs/main-starcoder.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x000000014001a85c
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Sat Jun  1 15:02:42 2024
+Time/Date		Sun Jun  2 15:02:41 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		000000000001b000
 SizeOfInitializedData	000000000000bc00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000001a85c
@@ -40341,19 +40341,17 @@
    14001f111:	movb   $0x40,(%rcx)
    14001f114:	add    %eax,(%rax)
    14001f116:	add    %al,(%rax)
    14001f118:	push   $0x14001c6
    14001f11d:	add    %al,(%rax)
    14001f11f:	add    %al,(%rax)
    14001f121:	add    %al,(%rax)
-   14001f123:	add    %dl,(%rdx)
-   14001f125:	cmp    %bl,0x66(%rbx)
-   14001f128:	add    %al,(%rax)
-   14001f12a:	add    %al,(%rax)
-   14001f12c:	or     $0x20000000,%eax
+   14001f123:	add    %dl,0x665c89(%rcx)
+   14001f129:	add    %al,(%rax)
+   14001f12b:	add    %cl,0x20000000(%rip)        # 0x16001f131
    14001f131:	add    (%rax),%eax
    14001f133:	add    %dl,(%rbx,%rax,1)
    14001f136:	add    (%rax),%al
    14001f138:	adc    $0xf7,%al
    14001f13a:	add    %eax,(%rax)
 	...
    14001f180:	add    %eax,(%rax)
```

## ipex_llm/libs/quantize-bloom.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x0000000140013918
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Sat Jun  1 15:02:42 2024
+Time/Date		Sun Jun  2 15:02:41 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000013a00
 SizeOfInitializedData	00000000000ace00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000013918
@@ -32236,19 +32236,17 @@
    140019225:	add    %al,(%rax)
    140019227:	add    %al,(%rax)
    140019229:	push   %rbp
    14001922a:	add    %eax,0x1(%rax)
    14001922d:	add    %al,(%rax)
    14001922f:	add    %al,(%rax)
    140019231:	add    %al,(%rax)
-   140019233:	add    %dl,(%rdx)
-   140019235:	cmp    %bl,0x66(%rbx)
-   140019238:	add    %al,(%rax)
-   14001923a:	add    %al,(%rax)
-   14001923c:	or     $0x20000000,%eax
+   140019233:	add    %dl,0x665c89(%rcx)
+   140019239:	add    %al,(%rax)
+   14001923b:	add    %cl,0x20000000(%rip)        # 0x160019241
    140019241:	add    (%rax),%eax
    140019243:	add    %dh,%al
    140019245:	movabs 0x18ff00001,%eax
 	...
    14001927e:	add    %al,(%rax)
    140019280:	add    %eax,(%rax)
 	...
```

## ipex_llm/libs/quantize-bloom_vnni.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x0000000140013b28
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Sat Jun  1 15:03:45 2024
+Time/Date		Sun Jun  2 15:02:54 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000013c00
 SizeOfInitializedData	00000000000ad000
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000013b28
@@ -32102,32 +32102,30 @@
    140018e89:	jae    0x140018eb8
    140018e8b:	jb     0x140018f02
    140018e8d:	outsb  %ds:(%rsi),(%dx)
    140018e8e:	outsb  %ds:(%rsi),(%dx)
    140018e8f:	gs jb  0x140018eee
    140018e92:	(bad)
    140018e97:	sub    $0x6c697562,%eax
-   140018e9c:	fs pop %rsp
-   140018e9e:	pop    %rdi
-   140018e9f:	ja     0x140018f10
-   140018ea1:	jb     0x140018f0e
-   140018ea3:	pop    %rsp
-   140018ea4:	imul   $0x6c6c2d78,0x65(%rax),%esi
-   140018eab:	insl   (%dx),%es:(%rdi)
-   140018eac:	pop    %rsp
-   140018ead:	imul   $0x6c6c2d78,0x65(%rax),%esi
-   140018eb4:	insl   (%dx),%es:(%rdi)
-   140018eb5:	pop    %rsp
-   140018eb6:	jae    0x140018f2a
-   140018eb8:	movsxd 0x67(%rdi,%riz,2),%ebx
-   140018ebc:	insl   (%dx),%es:(%rdi)
-   140018ebd:	insb   (%dx),%es:(%rdi)
-   140018ebe:	cs movsxd (%rax),%eax
-   140018ec1:	add    %al,(%rax)
-   140018ec3:	add    %al,(%rax)
+   140018e9c:	fs sub $0x5c77656e,%eax
+   140018ea2:	pop    %rdi
+   140018ea3:	ja     0x140018f14
+   140018ea5:	jb     0x140018f12
+   140018ea7:	pop    %rsp
+   140018ea8:	imul   $0x6c6c2d78,0x65(%rax),%esi
+   140018eaf:	insl   (%dx),%es:(%rdi)
+   140018eb0:	pop    %rsp
+   140018eb1:	imul   $0x6c6c2d78,0x65(%rax),%esi
+   140018eb8:	insl   (%dx),%es:(%rdi)
+   140018eb9:	pop    %rsp
+   140018eba:	jae    0x140018f2e
+   140018ebc:	movsxd 0x67(%rdi,%riz,2),%ebx
+   140018ec0:	insl   (%dx),%es:(%rdi)
+   140018ec1:	insb   (%dx),%es:(%rdi)
+   140018ec2:	cs movsxd (%rax),%eax
    140018ec5:	add    %al,(%rax)
    140018ec7:	add    %al,0x47(%rdi)
    140018eca:	rex.WRB
    140018ecb:	rex.WR pop %rdi
    140018ecd:	push   %r11
    140018ecf:	push   %rbx
    140018ed0:	rex.RB push %r10
@@ -32376,19 +32374,17 @@
    140019205:	add    %al,(%rax)
    140019207:	add    %al,(%rax)
    140019209:	push   %rbp
    14001920a:	add    %eax,0x1(%rax)
    14001920d:	add    %al,(%rax)
    14001920f:	add    %al,(%rax)
    140019211:	add    %al,(%rax)
-   140019213:	add    %dl,0x38(%rcx)
-   140019216:	pop    %rbx
-   140019217:	data16 add %al,(%rax)
-   14001921a:	add    %al,(%rax)
-   14001921c:	or     $0x20000000,%eax
+   140019213:	add    %bl,0x665c89(%rsi)
+   140019219:	add    %al,(%rax)
+   14001921b:	add    %cl,0x20000000(%rip)        # 0x160019221
    140019221:	add    (%rax),%eax
    140019223:	add    %dh,%al
    140019225:	movabs 0x191f00001,%eax
 	...
    14001927e:	add    %al,(%rax)
    140019280:	add    %eax,(%rax)
 	...
```

## ipex_llm/libs/quantize-gptneox.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x0000000140010988
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Sat Jun  1 15:02:41 2024
+Time/Date		Sun Jun  2 15:02:40 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000010a00
 SizeOfInitializedData	00000000000aa600
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000010988
@@ -27183,19 +27183,17 @@
    140016020:	push   $0x1400123
    140016025:	add    %al,(%rax)
    140016027:	add    %dh,0x23(%rax)
    14001602a:	add    %eax,0x1(%rax)
    14001602d:	add    %al,(%rax)
    14001602f:	add    %al,(%rax)
    140016031:	add    %al,(%rax)
-   140016033:	add    %dl,(%rcx)
-   140016035:	cmp    %bl,0x66(%rbx)
-   140016038:	add    %al,(%rax)
-   14001603a:	add    %al,(%rax)
-   14001603c:	or     $0x90000000,%eax
+   140016033:	add    %dl,0x665c89(%rax)
+   140016039:	add    %al,(%rax)
+   14001603b:	add    %cl,-0x70000000(%rip)        # 0xd0016041
    140016041:	add    (%rax),%eax
    140016043:	add    %ch,%al
    140016045:	add    %eax,%gs:(%rax)
    140016048:	call   0x1400161a0
 	...
    14001607d:	add    %al,(%rax)
    14001607f:	add    %bl,0x1400169(%rax)
```

## ipex_llm/libs/quantize-gptneox_vnni.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x0000000140010b98
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Sat Jun  1 15:03:44 2024
+Time/Date		Sun Jun  2 15:02:53 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000010c00
 SizeOfInitializedData	00000000000aa600
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000010b98
@@ -13439,15 +13439,15 @@
    14000acc0:	xor    %rsp,%rax
    14000acc3:	mov    %rax,0x50(%rsp)
    14000acc8:	mov    %r9,%rbp
    14000accb:	mov    %r8,%rsi
    14000acce:	mov    %rdx,%rbx
    14000acd1:	mov    %rcx,%rdi
    14000acd4:	mov    %rcx,0x28(%rsp)
-   14000acd9:	lea    0xace0(%rip),%r8        # 0x1400159c0
+   14000acd9:	lea    0xace4(%rip),%r8        # 0x1400159c4
    14000ace0:	call   0x14000ab40
    14000ace5:	nop
    14000ace6:	movl   $0xc470,0x14(%rdi)
    14000aced:	movl   $0x1000,0x18(%rdi)
    14000acf4:	movl   $0x1400,0x1c(%rdi)
    14000acfb:	movl   $0x28,0x20(%rdi)
    14000ad02:	movl   $0x24,0x24(%rdi)
@@ -26259,32 +26259,30 @@
    140015409:	jae    0x140015438
    14001540b:	jb     0x140015482
    14001540d:	outsb  %ds:(%rsi),(%dx)
    14001540e:	outsb  %ds:(%rsi),(%dx)
    14001540f:	gs jb  0x14001546e
    140015412:	(bad)
    140015417:	sub    $0x6c697562,%eax
-   14001541c:	fs pop %rsp
-   14001541e:	pop    %rdi
-   14001541f:	ja     0x140015490
-   140015421:	jb     0x14001548e
-   140015423:	pop    %rsp
-   140015424:	imul   $0x6c6c2d78,0x65(%rax),%esi
-   14001542b:	insl   (%dx),%es:(%rdi)
-   14001542c:	pop    %rsp
-   14001542d:	imul   $0x6c6c2d78,0x65(%rax),%esi
-   140015434:	insl   (%dx),%es:(%rdi)
-   140015435:	pop    %rsp
-   140015436:	jae    0x1400154aa
-   140015438:	movsxd 0x67(%rdi,%riz,2),%ebx
-   14001543c:	insl   (%dx),%es:(%rdi)
-   14001543d:	insb   (%dx),%es:(%rdi)
-   14001543e:	cs movsxd (%rax),%eax
-   140015441:	add    %al,(%rax)
-   140015443:	add    %al,(%rax)
+   14001541c:	fs sub $0x5c77656e,%eax
+   140015422:	pop    %rdi
+   140015423:	ja     0x140015494
+   140015425:	jb     0x140015492
+   140015427:	pop    %rsp
+   140015428:	imul   $0x6c6c2d78,0x65(%rax),%esi
+   14001542f:	insl   (%dx),%es:(%rdi)
+   140015430:	pop    %rsp
+   140015431:	imul   $0x6c6c2d78,0x65(%rax),%esi
+   140015438:	insl   (%dx),%es:(%rdi)
+   140015439:	pop    %rsp
+   14001543a:	jae    0x1400154ae
+   14001543c:	movsxd 0x67(%rdi,%riz,2),%ebx
+   140015440:	insl   (%dx),%es:(%rdi)
+   140015441:	insb   (%dx),%es:(%rdi)
+   140015442:	cs movsxd (%rax),%eax
    140015445:	add    %al,(%rax)
    140015447:	add    %al,0x47(%rdi)
    14001544a:	rex.WRB
    14001544b:	rex.WR pop %rdi
    14001544d:	push   %r11
    14001544f:	push   %rbx
    140015450:	rex.RB push %r10
@@ -26530,38 +26528,36 @@
    1400156b9:	jae    0x1400156e8
    1400156bb:	jb     0x140015732
    1400156bd:	outsb  %ds:(%rsi),(%dx)
    1400156be:	outsb  %ds:(%rsi),(%dx)
    1400156bf:	gs jb  0x14001571e
    1400156c2:	(bad)
    1400156c7:	sub    $0x6c697562,%eax
-   1400156cc:	fs pop %rsp
-   1400156ce:	pop    %rdi
-   1400156cf:	ja     0x140015740
-   1400156d1:	jb     0x14001573e
-   1400156d3:	pop    %rsp
-   1400156d4:	imul   $0x6c6c2d78,0x65(%rax),%esi
-   1400156db:	insl   (%dx),%es:(%rdi)
-   1400156dc:	pop    %rsp
-   1400156dd:	imul   $0x6c6c2d78,0x65(%rax),%esi
-   1400156e4:	insl   (%dx),%es:(%rdi)
-   1400156e5:	pop    %rsp
-   1400156e6:	jae    0x14001575a
-   1400156e8:	movsxd 0x70(%rdi,%riz,2),%ebx
-   1400156ec:	je     0x14001575c
-   1400156ee:	outsl  %gs:(%rsi),(%dx)
-   1400156f0:	js     0x14001574e
-   1400156f2:	addr32 jo 0x140015769
-   1400156f5:	outsb  %ds:(%rsi),(%dx)
-   1400156f6:	outsl  %gs:(%rsi),(%dx)
-   1400156f8:	js     0x140015727
-   1400156fa:	jne    0x140015770
-   1400156fc:	imul   $0x0,0x68(%rsi,%rbp,1),%ebp
-   140015704:	add    %al,(%rax)
-   140015706:	add    %al,(%rax)
+   1400156cc:	fs sub $0x5c77656e,%eax
+   1400156d2:	pop    %rdi
+   1400156d3:	ja     0x140015744
+   1400156d5:	jb     0x140015742
+   1400156d7:	pop    %rsp
+   1400156d8:	imul   $0x6c6c2d78,0x65(%rax),%esi
+   1400156df:	insl   (%dx),%es:(%rdi)
+   1400156e0:	pop    %rsp
+   1400156e1:	imul   $0x6c6c2d78,0x65(%rax),%esi
+   1400156e8:	insl   (%dx),%es:(%rdi)
+   1400156e9:	pop    %rsp
+   1400156ea:	jae    0x14001575e
+   1400156ec:	movsxd 0x70(%rdi,%riz,2),%ebx
+   1400156f0:	je     0x140015760
+   1400156f2:	outsl  %gs:(%rsi),(%dx)
+   1400156f4:	js     0x140015752
+   1400156f6:	addr32 jo 0x14001576d
+   1400156f9:	outsb  %ds:(%rsi),(%dx)
+   1400156fa:	outsl  %gs:(%rsi),(%dx)
+   1400156fc:	js     0x14001572b
+   1400156fe:	jne    0x140015774
+   140015700:	imul   $0x0,0x68(%rsi,%rbp,1),%ebp
    140015708:	rex.RXB push %r8
    14001570a:	push   %rsp
    14001570b:	rex.WRX
    14001570c:	rex.RB
    14001570d:	rex.WRXB pop %r8
    14001570f:	pop    %rdi
    140015710:	push   %r11
@@ -26790,39 +26786,37 @@
    140015979:	jae    0x1400159a8
    14001597b:	jb     0x1400159f2
    14001597d:	outsb  %ds:(%rsi),(%dx)
    14001597e:	outsb  %ds:(%rsi),(%dx)
    14001597f:	gs jb  0x1400159de
    140015982:	(bad)
    140015987:	sub    $0x6c697562,%eax
-   14001598c:	fs pop %rsp
-   14001598e:	pop    %rdi
-   14001598f:	ja     0x140015a00
-   140015991:	jb     0x1400159fe
-   140015993:	pop    %rsp
-   140015994:	imul   $0x6c6c2d78,0x65(%rax),%esi
-   14001599b:	insl   (%dx),%es:(%rdi)
-   14001599c:	pop    %rsp
-   14001599d:	imul   $0x6c6c2d78,0x65(%rax),%esi
-   1400159a4:	insl   (%dx),%es:(%rdi)
-   1400159a5:	pop    %rsp
-   1400159a6:	jae    0x140015a1a
-   1400159a8:	movsxd 0x70(%rdi,%riz,2),%ebx
-   1400159ac:	je     0x140015a1c
-   1400159ae:	outsl  %gs:(%rsi),(%dx)
-   1400159b0:	js     0x140015a0e
-   1400159b2:	addr32 jo 0x140015a29
-   1400159b5:	outsb  %ds:(%rsi),(%dx)
-   1400159b6:	outsl  %gs:(%rsi),(%dx)
-   1400159b8:	js     0x1400159e8
-   1400159ba:	movsxd 0x70(%rax),%esi
-   1400159bd:	add    %al,(%rax)
-   1400159bf:	add    %dh,0x62(%rdx)
-   1400159c2:	add    %al,(%rax)
-   1400159c4:	add    %al,(%rax)
+   14001598c:	fs sub $0x5c77656e,%eax
+   140015992:	pop    %rdi
+   140015993:	ja     0x140015a04
+   140015995:	jb     0x140015a02
+   140015997:	pop    %rsp
+   140015998:	imul   $0x6c6c2d78,0x65(%rax),%esi
+   14001599f:	insl   (%dx),%es:(%rdi)
+   1400159a0:	pop    %rsp
+   1400159a1:	imul   $0x6c6c2d78,0x65(%rax),%esi
+   1400159a8:	insl   (%dx),%es:(%rdi)
+   1400159a9:	pop    %rsp
+   1400159aa:	jae    0x140015a1e
+   1400159ac:	movsxd 0x70(%rdi,%riz,2),%ebx
+   1400159b0:	je     0x140015a20
+   1400159b2:	outsl  %gs:(%rsi),(%dx)
+   1400159b4:	js     0x140015a12
+   1400159b6:	addr32 jo 0x140015a2d
+   1400159b9:	outsb  %ds:(%rsi),(%dx)
+   1400159ba:	outsl  %gs:(%rsi),(%dx)
+   1400159bc:	js     0x1400159ec
+   1400159be:	movsxd 0x70(%rax),%esi
+   1400159c1:	add    %al,(%rax)
+   1400159c3:	add    %dh,0x62(%rdx)
    1400159c6:	add    %al,(%rax)
    1400159c8:	(bad)
    1400159cd:	sub    $0x3a6d6c6c,%eax
    1400159d2:	and    %ch,0x61(%rdi,%rbp,2)
    1400159d6:	imul   $0x646f6d20,%fs:0x67(%rsi),%ebp
    1400159de:	gs insb (%dx),%es:(%rdi)
    1400159e0:	and    %ah,0x72(%rsi)
@@ -27319,19 +27313,17 @@
    140016000:	push   $0x1400123
    140016005:	add    %al,(%rax)
    140016007:	add    %dh,0x23(%rax)
    14001600a:	add    %eax,0x1(%rax)
    14001600d:	add    %al,(%rax)
    14001600f:	add    %al,(%rax)
    140016011:	add    %al,(%rax)
-   140016013:	add    %dl,0x38(%rax)
-   140016016:	pop    %rbx
-   140016017:	data16 add %al,(%rax)
-   14001601a:	add    %al,(%rax)
-   14001601c:	or     $0x90000000,%eax
+   140016013:	add    %bl,0x665c89(%rbp)
+   140016019:	add    %al,(%rax)
+   14001601b:	add    %cl,-0x70000000(%rip)        # 0xd0016021
    140016021:	add    (%rax),%eax
    140016023:	add    %ch,%al
    140016025:	add    %eax,%gs:(%rax)
    140016028:	call   0x140016182
 	...
    14001607d:	add    %al,(%rax)
    14001607f:	add    %bl,0x1400169(%rax)
```

## ipex_llm/libs/quantize-llama.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x00000001400118e8
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Sat Jun  1 15:02:41 2024
+Time/Date		Sun Jun  2 15:02:40 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000011800
 SizeOfInitializedData	00000000000aac00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000000118e8
@@ -28462,19 +28462,17 @@
    1400170ed:	add    %al,(%rax)
    1400170ef:	add    %cl,0x1400133(%rax)
    1400170f5:	add    %al,(%rax)
    1400170f7:	add    %dl,0x1400133(%rax)
    1400170fd:	add    %al,(%rax)
    1400170ff:	add    %al,(%rax)
    140017101:	add    %al,(%rax)
-   140017103:	add    %dl,(%rcx)
-   140017105:	cmp    %bl,0x66(%rbx)
-   140017108:	add    %al,(%rax)
-   14001710a:	add    %al,(%rax)
-   14001710c:	or     $0x90000000,%eax
+   140017103:	add    %dl,0x665c89(%rax)
+   140017109:	add    %al,(%rax)
+   14001710b:	add    %cl,-0x70000000(%rip)        # 0xd0017111
    140017111:	add    (%rax),%eax
    140017113:	add    %ch,%ah
    140017115:	jbe    0x140017118
    140017117:	add    %ch,%ah
    140017119:	(bad)
 	...
    14001717e:	add    %al,(%rax)
```

## ipex_llm/libs/quantize-llama_vnni.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x0000000140011af8
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Sat Jun  1 15:03:44 2024
+Time/Date		Sun Jun  2 15:02:53 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000011c00
 SizeOfInitializedData	00000000000aac00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000011af8
@@ -2934,27 +2934,27 @@
 	reloc   26 offset  f90 [15f90] DIR64
 	reloc   27 offset  f98 [15f98] DIR64
 
 Virtual Address: 00016000 Chunk size 52 (0x34) Number of fixups 22
 	reloc    0 offset  768 [16768] DIR64
 	reloc    1 offset  770 [16770] DIR64
 	reloc    2 offset  778 [16778] DIR64
-	reloc    3 offset  8e0 [168e0] DIR64
-	reloc    4 offset  8e8 [168e8] DIR64
-	reloc    5 offset  8f0 [168f0] DIR64
-	reloc    6 offset  8f8 [168f8] DIR64
-	reloc    7 offset  900 [16900] DIR64
-	reloc    8 offset  908 [16908] DIR64
-	reloc    9 offset  910 [16910] DIR64
-	reloc   10 offset  918 [16918] DIR64
-	reloc   11 offset  920 [16920] DIR64
-	reloc   12 offset  928 [16928] DIR64
-	reloc   13 offset  930 [16930] DIR64
-	reloc   14 offset  938 [16938] DIR64
-	reloc   15 offset  940 [16940] DIR64
+	reloc    3 offset  8e8 [168e8] DIR64
+	reloc    4 offset  8f0 [168f0] DIR64
+	reloc    5 offset  8f8 [168f8] DIR64
+	reloc    6 offset  900 [16900] DIR64
+	reloc    7 offset  908 [16908] DIR64
+	reloc    8 offset  910 [16910] DIR64
+	reloc    9 offset  918 [16918] DIR64
+	reloc   10 offset  920 [16920] DIR64
+	reloc   11 offset  928 [16928] DIR64
+	reloc   12 offset  930 [16930] DIR64
+	reloc   13 offset  938 [16938] DIR64
+	reloc   14 offset  940 [16940] DIR64
+	reloc   15 offset  948 [16948] DIR64
 	reloc   16 offset  f70 [16f70] DIR64
 	reloc   17 offset  f78 [16f78] DIR64
 	reloc   18 offset  f80 [16f80] DIR64
 	reloc   19 offset  f88 [16f88] DIR64
 	reloc   20 offset  ff8 [16ff8] DIR64
 	reloc   21 offset    0 [16000] ABSOLUTE
 
@@ -14236,15 +14236,15 @@
    14000b804:	mov    %rax,(%rcx)
    14000b807:	lea    0x8(%rcx),%rdx
    14000b80b:	mov    %rcx,%rdi
    14000b80e:	vpxor  %xmm0,%xmm0,%xmm0
    14000b812:	lea    0x8(%rbx),%rcx
    14000b816:	vmovups %xmm0,(%rdx)
    14000b81a:	call   0x1400120c0
-   14000b81f:	lea    0xb0c2(%rip),%rax        # 0x1400168e8
+   14000b81f:	lea    0xb0ca(%rip),%rax        # 0x1400168f0
    14000b826:	mov    %rax,(%rdi)
    14000b829:	mov    %rdi,%rax
    14000b82c:	vmovups 0x18(%rbx),%xmm0
    14000b831:	mov    0x30(%rsp),%rbx
    14000b836:	vmovups %xmm0,0x18(%rdi)
    14000b83b:	add    $0x20,%rsp
    14000b83f:	pop    %rdi
@@ -14283,52 +14283,52 @@
    14000b88d:	mov    %rax,%rcx
    14000b890:	call   *0x7aa2(%rip)        # 0x140013338
    14000b896:	test   %eax,%eax
    14000b898:	je     0x14000b8d4
    14000b89a:	mov    $0x2,%ecx
    14000b89f:	call   *0x7a8b(%rip)        # 0x140013330
    14000b8a5:	mov    %rax,%rcx
-   14000b8a8:	lea    0xaf99(%rip),%rax        # 0x140016848
+   14000b8a8:	lea    0xafa1(%rip),%rax        # 0x140016850
    14000b8af:	mov    %rax,0x20(%rsp)
    14000b8b4:	mov    $0x65,%r9d
    14000b8ba:	lea    0xaedf(%rip),%r8        # 0x1400167a0
-   14000b8c1:	lea    0xaf28(%rip),%rdx        # 0x1400167f0
+   14000b8c1:	lea    0xaf30(%rip),%rdx        # 0x1400167f8
    14000b8c8:	call   0x140002470
    14000b8cd:	call   *0x79e5(%rip)        # 0x1400132b8
    14000b8d3:	int3
    14000b8d4:	mov    (%rbx),%rcx
    14000b8d7:	call   *0x7a4b(%rip)        # 0x140013328
    14000b8dd:	cmp    $0xffffffffffffffff,%rax
    14000b8e1:	jne    0x14000b91b
    14000b8e3:	lea    0x3(%rax),%ecx
    14000b8e6:	call   *0x7a44(%rip)        # 0x140013330
    14000b8ec:	mov    %rax,%rcx
-   14000b8ef:	lea    0xaf42(%rip),%rax        # 0x140016838
+   14000b8ef:	lea    0xaf4a(%rip),%rax        # 0x140016840
    14000b8f6:	mov    %rax,0x20(%rsp)
    14000b8fb:	mov    $0x5b,%r9d
    14000b901:	lea    0xae98(%rip),%r8        # 0x1400167a0
-   14000b908:	lea    0xaee1(%rip),%rdx        # 0x1400167f0
+   14000b908:	lea    0xaee9(%rip),%rdx        # 0x1400167f8
    14000b90f:	call   0x140002470
    14000b914:	call   *0x799e(%rip)        # 0x1400132b8
    14000b91a:	int3
    14000b91b:	mov    %rax,0x8(%rbx)
    14000b91f:	xor    %r8d,%r8d
    14000b922:	xor    %edx,%edx
    14000b924:	mov    (%rbx),%rcx
    14000b927:	call   *0x7a0b(%rip)        # 0x140013338
    14000b92d:	test   %eax,%eax
    14000b92f:	je     0x14000b96b
    14000b931:	mov    $0x2,%ecx
    14000b936:	call   *0x79f4(%rip)        # 0x140013330
    14000b93c:	mov    %rax,%rcx
-   14000b93f:	lea    0xaf02(%rip),%rax        # 0x140016848
+   14000b93f:	lea    0xaf0a(%rip),%rax        # 0x140016850
    14000b946:	mov    %rax,0x20(%rsp)
    14000b94b:	mov    $0x65,%r9d
    14000b951:	lea    0xae48(%rip),%r8        # 0x1400167a0
-   14000b958:	lea    0xae91(%rip),%rdx        # 0x1400167f0
+   14000b958:	lea    0xae99(%rip),%rdx        # 0x1400167f8
    14000b95f:	call   0x140002470
    14000b964:	call   *0x794e(%rip)        # 0x1400132b8
    14000b96a:	int3
    14000b96b:	mov    %rbx,%rax
    14000b96e:	mov    0x68(%rsp),%rcx
    14000b973:	xor    %rsp,%rcx
    14000b976:	call   0x1400115e0
@@ -14337,15 +14337,15 @@
    14000b987:	pop    %rdi
    14000b988:	ret
    14000b989:	call   *0x78b1(%rip)        # 0x140013240
    14000b98f:	mov    (%rax),%ecx
    14000b991:	call   *0x78f1(%rip)        # 0x140013288
    14000b997:	mov    %rax,%r9
    14000b99a:	mov    %rdi,%r8
-   14000b99d:	lea    0xae7c(%rip),%rdx        # 0x140016820
+   14000b99d:	lea    0xae84(%rip),%rdx        # 0x140016828
    14000b9a4:	lea    0x48(%rsp),%rcx
    14000b9a9:	call   0x14000de20
    14000b9ae:	nop
    14000b9af:	mov    %rax,%rdx
    14000b9b2:	lea    0x30(%rsp),%rcx
    14000b9b7:	call   0x14000c3d0
    14000b9bc:	lea    0xd8fd(%rip),%rdx        # 0x1400192c0
@@ -14363,15 +14363,15 @@
    14000b9e0:	xor    %rsp,%rax
    14000b9e3:	mov    %rax,0x50(%rsp)
    14000b9e8:	mov    %r9,%rbp
    14000b9eb:	mov    %r8,%rsi
    14000b9ee:	mov    %rdx,%rbx
    14000b9f1:	mov    %rcx,%rdi
    14000b9f4:	mov    %rcx,0x28(%rsp)
-   14000b9f9:	lea    0xb08c(%rip),%r8        # 0x140016a8c
+   14000b9f9:	lea    0xb090(%rip),%r8        # 0x140016a90
    14000ba00:	call   0x14000b850
    14000ba05:	nop
    14000ba06:	movl   $0x7d00,0x14(%rdi)
    14000ba0d:	movl   $0x200,0x18(%rdi)
    14000ba14:	movl   $0x1000,0x1c(%rdi)
    14000ba1b:	movl   $0x100,0x20(%rdi)
    14000ba22:	movl   $0x20,0x24(%rdi)
@@ -14382,15 +14382,15 @@
    14000ba45:	lea    0x38(%rdi),%rcx
    14000ba49:	call   0x14000c300
    14000ba4e:	nop
    14000ba4f:	mov    $0x2,%ecx
    14000ba54:	call   *0x78d6(%rip)        # 0x140013330
    14000ba5a:	mov    %rax,%rcx
    14000ba5d:	mov    %rbx,%r8
-   14000ba60:	lea    0xb029(%rip),%rdx        # 0x140016a90
+   14000ba60:	lea    0xb031(%rip),%rdx        # 0x140016a98
    14000ba67:	call   0x140002470
    14000ba6c:	mov    $0x4,%r8d
    14000ba72:	lea    0x20(%rsp),%rdx
    14000ba77:	mov    %rdi,%rcx
    14000ba7a:	call   0x14000fc30
    14000ba7f:	mov    0x20(%rsp),%ebx
    14000ba83:	cmp    $0x67676d6c,%ebx
@@ -14875,27 +14875,27 @@
    14000c1d0:	sub    (%r10),%rax
    14000c1d3:	sar    $0x2,%rax
    14000c1d7:	cmp    $0x1,%rax
    14000c1db:	je     0x14000c23c
    14000c1dd:	cmp    $0x1,%rdx
    14000c1e1:	je     0x14000c23c
    14000c1e3:	xor    %r8d,%r8d
-   14000c1e6:	lea    0xa79b(%rip),%rdx        # 0x140016988
+   14000c1e6:	lea    0xa7a3(%rip),%rdx        # 0x140016990
    14000c1ed:	mov    %rbx,%rcx
    14000c1f0:	call   0x14000dd20
    14000c1f5:	test   %rax,%rax
    14000c1f8:	je     0x14000c233
    14000c1fa:	xor    %r8d,%r8d
-   14000c1fd:	lea    0xa794(%rip),%rdx        # 0x140016998
+   14000c1fd:	lea    0xa79c(%rip),%rdx        # 0x1400169a0
    14000c204:	mov    %rbx,%rcx
    14000c207:	call   0x14000dd20
    14000c20c:	cmp    $0xffffffffffffffff,%rax
    14000c210:	jne    0x14000c233
    14000c212:	xor    %r8d,%r8d
-   14000c215:	lea    0xa794(%rip),%rdx        # 0x1400169b0
+   14000c215:	lea    0xa79c(%rip),%rdx        # 0x1400169b8
    14000c21c:	mov    %rbx,%rcx
    14000c21f:	call   0x14000dd20
    14000c224:	cmp    $0xffffffffffffffff,%rax
    14000c228:	jne    0x14000c233
    14000c22a:	movl   $0x2,0x24(%rbx)
    14000c231:	jmp    0x14000c243
    14000c233:	movl   $0x1,0x24(%rbx)
@@ -14924,15 +14924,15 @@
    14000c292:	pop    %rdi
    14000c293:	pop    %rsi
    14000c294:	pop    %rbp
    14000c295:	ret
    14000c296:	lea    0x18(%rdi),%rcx
    14000c29a:	call   0x14000d8a0
    14000c29f:	mov    %rax,%r8
-   14000c2a2:	lea    0xa6b7(%rip),%rdx        # 0x140016960
+   14000c2a2:	lea    0xa6bf(%rip),%rdx        # 0x140016968
    14000c2a9:	lea    -0x21(%rbp),%rcx
    14000c2ad:	call   0x14000de20
    14000c2b2:	lea    0xd0d7(%rip),%rdx        # 0x140019390
    14000c2b9:	lea    -0x21(%rbp),%rcx
    14000c2bd:	call   0x1400120cc
    14000c2c2:	int3
    14000c2c3:	call   0x14000d7a0
@@ -15064,17 +15064,17 @@
    14000c444:	mov    %rax,(%rcx)
    14000c447:	lea    0x8(%rcx),%rdx
    14000c44b:	mov    %rcx,%rdi
    14000c44e:	vpxor  %xmm0,%xmm0,%xmm0
    14000c452:	lea    0x8(%rbx),%rcx
    14000c456:	vmovups %xmm0,(%rdx)
    14000c45a:	call   0x1400120c0
-   14000c45f:	lea    0xa482(%rip),%rax        # 0x1400168e8
+   14000c45f:	lea    0xa48a(%rip),%rax        # 0x1400168f0
    14000c466:	mov    %rax,(%rdi)
-   14000c469:	lea    0xa490(%rip),%rax        # 0x140016900
+   14000c469:	lea    0xa498(%rip),%rax        # 0x140016908
    14000c470:	vmovups 0x18(%rbx),%xmm0
    14000c475:	mov    0x30(%rsp),%rbx
    14000c47a:	mov    %rax,(%rdi)
    14000c47d:	mov    %rdi,%rax
    14000c480:	vmovups %xmm0,0x18(%rdi)
    14000c485:	add    $0x20,%rsp
    14000c489:	pop    %rdi
@@ -15126,15 +15126,15 @@
    14000c535:	add    $0xfffffffffffffff8,%rax
    14000c539:	cmp    $0x1f,%rax
    14000c53d:	jbe    0x14000c546
    14000c53f:	call   *0x6cf3(%rip)        # 0x140013238
    14000c545:	int3
    14000c546:	call   0x1400112f4
    14000c54b:	vmovups (%rdi),%xmm0
-   14000c54f:	lea    0xa3aa(%rip),%rax        # 0x140016900
+   14000c54f:	lea    0xa3b2(%rip),%rax        # 0x140016908
    14000c556:	mov    %rax,(%rbx)
    14000c559:	mov    %rbx,%rax
    14000c55c:	vmovups %xmm0,0x18(%rbx)
    14000c561:	mov    0x50(%rsp),%rcx
    14000c566:	xor    %rsp,%rcx
    14000c569:	call   0x1400115e0
    14000c56e:	mov    0x80(%rsp),%rbx
@@ -16027,15 +16027,15 @@
    14000cfd7:	cmpq   $0x10,0x18(%rax)
    14000cfdc:	jb     0x14000cfe1
    14000cfde:	mov    (%rax),%rbx
    14000cfe1:	mov    $0x2,%ecx
    14000cfe6:	call   *0x6344(%rip)        # 0x140013330
    14000cfec:	mov    %rax,%rcx
    14000cfef:	mov    %rbx,%r8
-   14000cff2:	lea    0x98bf(%rip),%rdx        # 0x1400168b8
+   14000cff2:	lea    0x98c7(%rip),%rdx        # 0x1400168c0
    14000cff9:	call   0x140002470
    14000cffe:	mov    0x38(%rsp),%rdx
    14000d003:	cmp    $0x10,%rdx
    14000d007:	jb     0x14000d03f
    14000d009:	inc    %rdx
    14000d00c:	mov    0x20(%rsp),%rcx
    14000d011:	mov    %rcx,%rax
@@ -16775,15 +16775,15 @@
    14000d996:	mov    $0x2,%ecx
    14000d99b:	call   *0x598f(%rip)        # 0x140013330
    14000d9a1:	mov    %rax,%rcx
    14000d9a4:	lea    0x906d(%rip),%rax        # 0x140016a18
    14000d9ab:	mov    %rax,0x20(%rsp)
    14000d9b0:	mov    $0x187,%r9d
    14000d9b6:	lea    0x9083(%rip),%r8        # 0x140016a40
-   14000d9bd:	lea    0x8e2c(%rip),%rdx        # 0x1400167f0
+   14000d9bd:	lea    0x8e34(%rip),%rdx        # 0x1400167f8
    14000d9c4:	call   0x140002470
    14000d9c9:	call   *0x58e9(%rip)        # 0x1400132b8
    14000d9cf:	int3
    14000d9d0:	mov    0x3c(%r14),%ecx
    14000d9d4:	test   %ecx,%ecx
    14000d9d6:	je     0x14000da35
    14000d9d8:	sub    $0x1,%ecx
@@ -17238,19 +17238,19 @@
    14000df34:	mov    %r14,%rcx
    14000df37:	call   0x140011130
    14000df3c:	cmp    %r15d,%eax
    14000df3f:	je     0x14000df7b
    14000df41:	mov    $0x2,%ecx
    14000df46:	call   *0x53e4(%rip)        # 0x140013330
    14000df4c:	mov    %rax,%rcx
-   14000df4f:	lea    0x88ba(%rip),%rax        # 0x140016810
+   14000df4f:	lea    0x88c2(%rip),%rax        # 0x140016818
    14000df56:	mov    %rax,0x20(%rsp)
    14000df5b:	mov    $0x40,%r9d
    14000df61:	lea    0x8838(%rip),%r8        # 0x1400167a0
-   14000df68:	lea    0x8881(%rip),%rdx        # 0x1400167f0
+   14000df68:	lea    0x8889(%rip),%rdx        # 0x1400167f8
    14000df6f:	call   0x140002470
    14000df74:	call   *0x533e(%rip)        # 0x1400132b8
    14000df7a:	int3
    14000df7b:	vpxor  %xmm0,%xmm0,%xmm0
    14000df7f:	vmovups %xmm0,0x0(%rbp)
    14000df84:	mov    %r12,0x10(%rbp)
    14000df88:	mov    %r12,0x18(%rbp)
@@ -17290,15 +17290,15 @@
    14000dfea:	mov    $0x2,%ecx
    14000dfef:	call   *0x533b(%rip)        # 0x140013330
    14000dff5:	mov    %rax,%rcx
    14000dff8:	lea    0x8781(%rip),%rax        # 0x140016780
    14000dfff:	mov    %rax,0x20(%rsp)
    14000e004:	mov    $0x3d,%r9d
    14000e00a:	lea    0x878f(%rip),%r8        # 0x1400167a0
-   14000e011:	lea    0x87d8(%rip),%rdx        # 0x1400167f0
+   14000e011:	lea    0x87e0(%rip),%rdx        # 0x1400167f8
    14000e018:	call   0x140002470
    14000e01d:	call   *0x5295(%rip)        # 0x1400132b8
    14000e023:	int3
    14000e024:	call   0x140001f20
    14000e029:	int3
    14000e02a:	call   0x14000d780
    14000e02f:	int3
@@ -17513,15 +17513,15 @@
    14000e33c:	mov    %rcx,%rsi
    14000e33f:	sub    %r9,%rax
    14000e342:	mov    %rcx,0x28(%rsp)
    14000e347:	sar    $0x2,%rax
    14000e34b:	test   %rax,%rax
    14000e34e:	je     0x14000e450
    14000e354:	mov    (%r9),%r9d
-   14000e357:	lea    0x85f2(%rip),%r8        # 0x140016950
+   14000e357:	lea    0x85fa(%rip),%r8        # 0x140016958
    14000e35e:	mov    $0x100,%edx
    14000e363:	lea    0x30(%rsp),%rcx
    14000e368:	call   0x140009bc0
    14000e36d:	mov    0x8(%r14),%rcx
    14000e371:	mov    $0x1,%edi
    14000e376:	mov    (%r14),%r8
    14000e379:	mov    %rcx,%rax
@@ -17540,15 +17540,15 @@
    14000e3a8:	nopl   0x0(%rax,%rax,1)
    14000e3b0:	inc    %rax
    14000e3b3:	cmpb   $0x0,(%rcx,%rax,1)
    14000e3b7:	jne    0x14000e3b0
    14000e3b9:	mov    (%r8,%rdi,4),%r9d
    14000e3bd:	lea    0x30(%rsp),%rcx
    14000e3c2:	mov    $0x100,%edx
-   14000e3c7:	lea    0x8586(%rip),%r8        # 0x140016954
+   14000e3c7:	lea    0x858e(%rip),%r8        # 0x14001695c
    14000e3ce:	sub    %rax,%rdx
    14000e3d1:	add    %rax,%rcx
    14000e3d4:	call   0x140009bc0
    14000e3d9:	mov    0x8(%r14),%rcx
    14000e3dd:	inc    %rdi
    14000e3e0:	mov    (%r14),%r8
    14000e3e3:	mov    %rcx,%rax
@@ -17618,19 +17618,19 @@
    14000e4c1:	mov    %rdi,0x10(%rbx)
    14000e4c5:	mov    %rbx,%rcx
    14000e4c8:	movq   $0xf,0x18(%rbx)
    14000e4d0:	call   0x140001f80
    14000e4d5:	mov    %rax,(%rbx)
    14000e4d8:	movq   $0x15,0x10(%rbx)
    14000e4e0:	movq   $0x1f,0x18(%rbx)
-   14000e4e8:	vmovups 0x83b0(%rip),%xmm0        # 0x1400168a0
+   14000e4e8:	vmovups 0x83b8(%rip),%xmm0        # 0x1400168a8
    14000e4f0:	vmovups %xmm0,(%rax)
-   14000e4f4:	mov    0x83b6(%rip),%ecx        # 0x1400168b0
+   14000e4f4:	mov    0x83be(%rip),%ecx        # 0x1400168b8
    14000e4fa:	mov    %ecx,0x10(%rax)
-   14000e4fd:	movzbl 0x83b0(%rip),%ecx        # 0x1400168b4
+   14000e4fd:	movzbl 0x83b8(%rip),%ecx        # 0x1400168bc
    14000e504:	mov    %cl,0x14(%rax)
    14000e507:	mov    %dil,0x15(%rax)
    14000e50b:	jmp    0x14000e541
    14000e50d:	mov    0x40(%rsp),%rdx
    14000e512:	lea    0x50(%rsp),%rcx
    14000e517:	vpxor  %xmm1,%xmm1,%xmm1
    14000e51b:	vmovdqu %xmm1,0x60(%rsp)
@@ -18411,48 +18411,48 @@
    14000f142:	mov    $0x2,%ecx
    14000f147:	call   *0x41e3(%rip)        # 0x140013330
    14000f14d:	mov    %rax,%rcx
    14000f150:	lea    0x7a99(%rip),%rax        # 0x140016bf0
    14000f157:	mov    %rax,0x20(%rsp)
    14000f15c:	mov    $0x25d,%r9d
    14000f162:	lea    0x78d7(%rip),%r8        # 0x140016a40
-   14000f169:	lea    0x7680(%rip),%rdx        # 0x1400167f0
+   14000f169:	lea    0x7688(%rip),%rdx        # 0x1400167f8
    14000f170:	call   0x140002470
    14000f175:	call   *0x413d(%rip)        # 0x1400132b8
    14000f17b:	int3
    14000f17c:	mov    $0x2,%ecx
    14000f181:	call   *0x41a9(%rip)        # 0x140013330
    14000f187:	mov    %rax,%rcx
-   14000f18a:	lea    0x76b7(%rip),%rax        # 0x140016848
+   14000f18a:	lea    0x76bf(%rip),%rax        # 0x140016850
    14000f191:	mov    %rax,0x20(%rsp)
    14000f196:	mov    $0x65,%r9d
    14000f19c:	lea    0x75fd(%rip),%r8        # 0x1400167a0
-   14000f1a3:	lea    0x7646(%rip),%rdx        # 0x1400167f0
+   14000f1a3:	lea    0x764e(%rip),%rdx        # 0x1400167f8
    14000f1aa:	call   0x140002470
    14000f1af:	call   *0x4103(%rip)        # 0x1400132b8
    14000f1b5:	int3
    14000f1b6:	mov    $0x2,%ecx
    14000f1bb:	call   *0x416f(%rip)        # 0x140013330
    14000f1c1:	mov    %rax,%rcx
-   14000f1c4:	lea    0x766d(%rip),%rax        # 0x140016838
+   14000f1c4:	lea    0x7675(%rip),%rax        # 0x140016840
    14000f1cb:	mov    %rax,0x20(%rsp)
    14000f1d0:	mov    $0x5b,%r9d
    14000f1d6:	lea    0x75c3(%rip),%r8        # 0x1400167a0
-   14000f1dd:	lea    0x760c(%rip),%rdx        # 0x1400167f0
+   14000f1dd:	lea    0x7614(%rip),%rdx        # 0x1400167f8
    14000f1e4:	call   0x140002470
    14000f1e9:	call   *0x40c9(%rip)        # 0x1400132b8
    14000f1ef:	int3
    14000f1f0:	mov    $0x2,%ecx
    14000f1f5:	call   *0x4135(%rip)        # 0x140013330
    14000f1fb:	mov    %rax,%rcx
    14000f1fe:	lea    0x7387(%rip),%rax        # 0x14001658c
    14000f205:	mov    %rax,0x20(%rsp)
    14000f20a:	mov    $0x255,%r9d
    14000f210:	lea    0x7829(%rip),%r8        # 0x140016a40
-   14000f217:	lea    0x75d2(%rip),%rdx        # 0x1400167f0
+   14000f217:	lea    0x75da(%rip),%rdx        # 0x1400167f8
    14000f21e:	call   0x140002470
    14000f223:	call   *0x408f(%rip)        # 0x1400132b8
    14000f229:	nop
    14000f22a:	mov    -0x50(%rbp),%rsi
    14000f22e:	jmp    0x14000f249
    14000f230:	mov    0x100(%rbp),%rdi
    14000f237:	mov    0x40(%rsp),%rsi
@@ -18700,15 +18700,15 @@
    14000f588:	mov    $0x2,%ecx
    14000f58d:	call   *0x3d9d(%rip)        # 0x140013330
    14000f593:	mov    %rax,%rcx
    14000f596:	lea    0x775b(%rip),%rax        # 0x140016cf8
    14000f59d:	mov    %rax,0x20(%rsp)
    14000f5a2:	mov    $0x2ee,%r9d
    14000f5a8:	lea    0x7491(%rip),%r8        # 0x140016a40
-   14000f5af:	lea    0x723a(%rip),%rdx        # 0x1400167f0
+   14000f5af:	lea    0x7242(%rip),%rdx        # 0x1400167f8
    14000f5b6:	call   0x140002470
    14000f5bb:	call   *0x3cf7(%rip)        # 0x1400132b8
    14000f5c1:	int3
    14000f5c2:	movabs $0x4924924924924925,%rax
    14000f5cc:	imul   %rcx
    14000f5cf:	sar    $0x4,%rdx
    14000f5d3:	mov    %rdx,%rax
@@ -18746,19 +18746,19 @@
    14000f656:	mov    (%rbx),%rcx
    14000f659:	call   *0x3cd9(%rip)        # 0x140013338
    14000f65f:	test   %eax,%eax
    14000f661:	je     0x14000f69d
    14000f663:	mov    $0x2,%ecx
    14000f668:	call   *0x3cc2(%rip)        # 0x140013330
    14000f66e:	mov    %rax,%rcx
-   14000f671:	lea    0x71d0(%rip),%rax        # 0x140016848
+   14000f671:	lea    0x71d8(%rip),%rax        # 0x140016850
    14000f678:	mov    %rax,0x20(%rsp)
    14000f67d:	mov    $0x65,%r9d
    14000f683:	lea    0x7116(%rip),%r8        # 0x1400167a0
-   14000f68a:	lea    0x715f(%rip),%rdx        # 0x1400167f0
+   14000f68a:	lea    0x7167(%rip),%rdx        # 0x1400167f8
    14000f691:	call   0x140002470
    14000f696:	call   *0x3c1c(%rip)        # 0x1400132b8
    14000f69c:	int3
    14000f69d:	mov    0x58(%r14),%r8
    14000f6a1:	mov    0x68(%r14),%rdx
    14000f6a5:	mov    %rbx,%rcx
    14000f6a8:	call   0x14000fc30
@@ -18799,26 +18799,26 @@
    14000f72d:	mov    $0x2,%ecx
    14000f732:	call   *0x3bf8(%rip)        # 0x140013330
    14000f738:	mov    %rax,%rcx
    14000f73b:	lea    0x75ce(%rip),%rax        # 0x140016d10
    14000f742:	mov    %rax,0x20(%rsp)
    14000f747:	mov    $0x2fc,%r9d
    14000f74d:	lea    0x72ec(%rip),%r8        # 0x140016a40
-   14000f754:	lea    0x7095(%rip),%rdx        # 0x1400167f0
+   14000f754:	lea    0x709d(%rip),%rdx        # 0x1400167f8
    14000f75b:	call   0x140002470
    14000f760:	call   *0x3b52(%rip)        # 0x1400132b8
    14000f766:	int3
    14000f767:	mov    $0x2,%ecx
    14000f76c:	call   *0x3bbe(%rip)        # 0x140013330
    14000f772:	mov    %rax,%rcx
-   14000f775:	lea    0x70cc(%rip),%rax        # 0x140016848
+   14000f775:	lea    0x70d4(%rip),%rax        # 0x140016850
    14000f77c:	mov    %rax,0x20(%rsp)
    14000f781:	mov    $0x65,%r9d
    14000f787:	lea    0x7012(%rip),%r8        # 0x1400167a0
-   14000f78e:	lea    0x705b(%rip),%rdx        # 0x1400167f0
+   14000f78e:	lea    0x7063(%rip),%rdx        # 0x1400167f8
    14000f795:	call   0x140002470
    14000f79a:	call   *0x3b18(%rip)        # 0x1400132b8
    14000f7a0:	int3
    14000f7a1:	cmp    $0x1,%eax
    14000f7a4:	jne    0x14000fb5c
    14000f7aa:	mov    0x8(%rdx),%rcx
    14000f7ae:	sub    (%rdx),%rcx
@@ -19008,26 +19008,26 @@
    14000fa8a:	mov    $0x2,%ecx
    14000fa8f:	call   *0x389b(%rip)        # 0x140013330
    14000fa95:	mov    %rax,%rcx
    14000fa98:	lea    0x7289(%rip),%rax        # 0x140016d28
    14000fa9f:	mov    %rax,0x20(%rsp)
    14000faa4:	mov    $0x313,%r9d
    14000faaa:	lea    0x6f8f(%rip),%r8        # 0x140016a40
-   14000fab1:	lea    0x6d38(%rip),%rdx        # 0x1400167f0
+   14000fab1:	lea    0x6d40(%rip),%rdx        # 0x1400167f8
    14000fab8:	call   0x140002470
    14000fabd:	call   *0x37f5(%rip)        # 0x1400132b8
    14000fac3:	int3
    14000fac4:	mov    $0x2,%ecx
    14000fac9:	call   *0x3861(%rip)        # 0x140013330
    14000facf:	mov    %rax,%rcx
-   14000fad2:	lea    0x6d6f(%rip),%rax        # 0x140016848
+   14000fad2:	lea    0x6d77(%rip),%rax        # 0x140016850
    14000fad9:	mov    %rax,0x20(%rsp)
    14000fade:	mov    $0x65,%r9d
    14000fae4:	lea    0x6cb5(%rip),%r8        # 0x1400167a0
-   14000faeb:	lea    0x6cfe(%rip),%rdx        # 0x1400167f0
+   14000faeb:	lea    0x6d06(%rip),%rdx        # 0x1400167f8
    14000faf2:	call   0x140002470
    14000faf7:	call   *0x37bb(%rip)        # 0x1400132b8
    14000fafd:	nop
    14000fafe:	test   %r12,%r12
    14000fb01:	je     0x14000fb5c
    14000fb03:	mov    %r12,%rbx
    14000fb06:	cmp    %rsi,%r12
@@ -19130,15 +19130,15 @@
    14000fc10:	call   0x140001420
    14000fc15:	mov    %rbx,%rax
    14000fc18:	add    $0x30,%rsp
    14000fc1c:	pop    %rbx
    14000fc1d:	ret
    14000fc1e:	int3
    14000fc1f:	int3
-   14000fc20:	lea    0x6d21(%rip),%rax        # 0x140016948
+   14000fc20:	lea    0x6d29(%rip),%rax        # 0x140016950
    14000fc27:	ret
    14000fc28:	int3
    14000fc29:	int3
    14000fc2a:	int3
    14000fc2b:	int3
    14000fc2c:	int3
    14000fc2d:	int3
@@ -19174,30 +19174,30 @@
    14000fc90:	xor    %rsp,%rcx
    14000fc93:	call   0x1400115e0
    14000fc98:	add    $0x60,%rsp
    14000fc9c:	pop    %rdi
    14000fc9d:	pop    %rsi
    14000fc9e:	pop    %rbx
    14000fc9f:	ret
-   14000fca0:	lea    0x6bc1(%rip),%rdx        # 0x140016868
+   14000fca0:	lea    0x6bc9(%rip),%rdx        # 0x140016870
    14000fca7:	lea    0x38(%rsp),%rcx
    14000fcac:	call   0x14000b600
    14000fcb1:	nop
    14000fcb2:	mov    %rax,%rdx
    14000fcb5:	lea    0x20(%rsp),%rcx
    14000fcba:	call   0x14000c3d0
    14000fcbf:	lea    0x95fa(%rip),%rdx        # 0x1400192c0
    14000fcc6:	lea    0x20(%rsp),%rcx
    14000fccb:	call   0x1400120cc
    14000fcd0:	nop
    14000fcd1:	call   *0x3569(%rip)        # 0x140013240
    14000fcd7:	mov    (%rax),%ecx
    14000fcd9:	call   *0x35a9(%rip)        # 0x140013288
    14000fcdf:	mov    %rax,%r8
-   14000fce2:	lea    0x6b6f(%rip),%rdx        # 0x140016858
+   14000fce2:	lea    0x6b77(%rip),%rdx        # 0x140016860
    14000fce9:	lea    0x38(%rsp),%rcx
    14000fcee:	call   0x14000de20
    14000fcf3:	nop
    14000fcf4:	mov    %rax,%rdx
    14000fcf7:	lea    0x20(%rsp),%rcx
    14000fcfc:	call   0x14000c3d0
    14000fd01:	lea    0x95b8(%rip),%rdx        # 0x1400192c0
@@ -19805,69 +19805,69 @@
    140010652:	call   0x1400112f4
    140010657:	mov    -0x48(%rbp),%r12
    14001065b:	mov    (%r12),%rcx
    14001065f:	jmp    0x14000fd60
    140010664:	mov    $0x2,%ecx
    140010669:	call   *0x2cc1(%rip)        # 0x140013330
    14001066f:	mov    %rax,%rcx
-   140010672:	lea    0x61cf(%rip),%rax        # 0x140016848
+   140010672:	lea    0x61d7(%rip),%rax        # 0x140016850
    140010679:	mov    %rax,0x20(%rsp)
    14001067e:	mov    $0x65,%r9d
    140010684:	lea    0x6115(%rip),%r8        # 0x1400167a0
-   14001068b:	lea    0x615e(%rip),%rdx        # 0x1400167f0
+   14001068b:	lea    0x6166(%rip),%rdx        # 0x1400167f8
    140010692:	call   0x140002470
    140010697:	call   *0x2c1b(%rip)        # 0x1400132b8
    14001069d:	int3
    14001069e:	mov    $0x2,%ecx
    1400106a3:	call   *0x2c87(%rip)        # 0x140013330
    1400106a9:	mov    %rax,%rcx
-   1400106ac:	lea    0x6185(%rip),%rax        # 0x140016838
+   1400106ac:	lea    0x618d(%rip),%rax        # 0x140016840
    1400106b3:	mov    %rax,0x20(%rsp)
    1400106b8:	mov    $0x5b,%r9d
    1400106be:	lea    0x60db(%rip),%r8        # 0x1400167a0
-   1400106c5:	lea    0x6124(%rip),%rdx        # 0x1400167f0
+   1400106c5:	lea    0x612c(%rip),%rdx        # 0x1400167f8
    1400106cc:	call   0x140002470
    1400106d1:	call   *0x2be1(%rip)        # 0x1400132b8
    1400106d7:	nop
    1400106d8:	call   *0x2b5a(%rip)        # 0x140013238
    1400106de:	nop
    1400106df:	call   *0x2b53(%rip)        # 0x140013238
    1400106e5:	nop
    1400106e6:	call   *0x2b4c(%rip)        # 0x140013238
    1400106ec:	nop
    1400106ed:	mov    $0x2,%ecx
    1400106f2:	call   *0x2c38(%rip)        # 0x140013330
    1400106f8:	mov    %rax,%rcx
-   1400106fb:	lea    0x6146(%rip),%rax        # 0x140016848
+   1400106fb:	lea    0x614e(%rip),%rax        # 0x140016850
    140010702:	mov    %rax,0x20(%rsp)
    140010707:	mov    $0x65,%r9d
    14001070d:	lea    0x608c(%rip),%r8        # 0x1400167a0
-   140010714:	lea    0x60d5(%rip),%rdx        # 0x1400167f0
+   140010714:	lea    0x60dd(%rip),%rdx        # 0x1400167f8
    14001071b:	call   0x140002470
    140010720:	call   *0x2b92(%rip)        # 0x1400132b8
    140010726:	int3
    140010727:	mov    $0x2,%ecx
    14001072c:	call   *0x2bfe(%rip)        # 0x140013330
    140010732:	mov    %rax,%rcx
-   140010735:	lea    0x60fc(%rip),%rax        # 0x140016838
+   140010735:	lea    0x6104(%rip),%rax        # 0x140016840
    14001073c:	mov    %rax,0x20(%rsp)
    140010741:	mov    $0x5b,%r9d
    140010747:	lea    0x6052(%rip),%r8        # 0x1400167a0
-   14001074e:	lea    0x609b(%rip),%rdx        # 0x1400167f0
+   14001074e:	lea    0x60a3(%rip),%rdx        # 0x1400167f8
    140010755:	call   0x140002470
    14001075a:	call   *0x2b58(%rip)        # 0x1400132b8
    140010760:	nop
    140010761:	mov    $0x2,%ecx
    140010766:	call   *0x2bc4(%rip)        # 0x140013330
    14001076c:	mov    %rax,%rcx
-   14001076f:	lea    0x60c2(%rip),%rax        # 0x140016838
+   14001076f:	lea    0x60ca(%rip),%rax        # 0x140016840
    140010776:	mov    %rax,0x20(%rsp)
    14001077b:	mov    $0x5b,%r9d
    140010781:	lea    0x6018(%rip),%r8        # 0x1400167a0
-   140010788:	lea    0x6061(%rip),%rdx        # 0x1400167f0
+   140010788:	lea    0x6069(%rip),%rdx        # 0x1400167f8
    14001078f:	call   0x140002470
    140010794:	call   *0x2b1e(%rip)        # 0x1400132b8
    14001079a:	int3
    14001079b:	mov    0x30(%rbp),%rcx
    14001079f:	xor    %rsp,%rcx
    1400107a2:	call   0x1400115e0
    1400107a7:	mov    0x198(%rsp),%rbx
@@ -19887,30 +19887,30 @@
    1400107d1:	lea    0x6338(%rip),%rdx        # 0x140016b10
    1400107d8:	lea    -0x10(%rbp),%rcx
    1400107dc:	call   0x14000de20
    1400107e1:	lea    0x8ba8(%rip),%rdx        # 0x140019390
    1400107e8:	lea    -0x10(%rbp),%rcx
    1400107ec:	call   0x1400120cc
    1400107f1:	nop
-   1400107f2:	lea    0x606f(%rip),%rdx        # 0x140016868
+   1400107f2:	lea    0x6077(%rip),%rdx        # 0x140016870
    1400107f9:	lea    0x10(%rbp),%rcx
    1400107fd:	call   0x14000b600
    140010802:	nop
    140010803:	mov    %rax,%rdx
    140010806:	lea    -0x10(%rbp),%rcx
    14001080a:	call   0x14000c3d0
    14001080f:	lea    0x8aaa(%rip),%rdx        # 0x1400192c0
    140010816:	lea    -0x10(%rbp),%rcx
    14001081a:	call   0x1400120cc
    14001081f:	nop
    140010820:	call   *0x2a1a(%rip)        # 0x140013240
    140010826:	mov    (%rax),%ecx
    140010828:	call   *0x2a5a(%rip)        # 0x140013288
    14001082e:	mov    %rax,%r8
-   140010831:	lea    0x6020(%rip),%rdx        # 0x140016858
+   140010831:	lea    0x6028(%rip),%rdx        # 0x140016860
    140010838:	lea    0x10(%rbp),%rcx
    14001083c:	call   0x14000de20
    140010841:	nop
    140010842:	mov    %rax,%rdx
    140010845:	lea    -0x10(%rbp),%rcx
    140010849:	call   0x14000c3d0
    14001084e:	lea    0x8a6b(%rip),%rdx        # 0x1400192c0
@@ -20197,26 +20197,26 @@
    140010c46:	vzeroupper
    140010c49:	call   *0x25e9(%rip)        # 0x140013238
    140010c4f:	nop
    140010c50:	call   *0x25ea(%rip)        # 0x140013240
    140010c56:	mov    (%rax),%ecx
    140010c58:	call   *0x262a(%rip)        # 0x140013288
    140010c5e:	mov    %rax,%r8
-   140010c61:	lea    0x5bf0(%rip),%rdx        # 0x140016858
+   140010c61:	lea    0x5bf8(%rip),%rdx        # 0x140016860
    140010c68:	lea    -0x1(%rbp),%rcx
    140010c6c:	call   0x14000de20
    140010c71:	nop
    140010c72:	mov    %rax,%rdx
    140010c75:	lea    -0x39(%rbp),%rcx
    140010c79:	call   0x14000c3d0
    140010c7e:	lea    0x863b(%rip),%rdx        # 0x1400192c0
    140010c85:	lea    -0x39(%rbp),%rcx
    140010c89:	call   0x1400120cc
    140010c8e:	nop
-   140010c8f:	lea    0x5bd2(%rip),%rdx        # 0x140016868
+   140010c8f:	lea    0x5bda(%rip),%rdx        # 0x140016870
    140010c96:	lea    -0x1(%rbp),%rcx
    140010c9a:	call   0x14000b600
    140010c9f:	nop
    140010ca0:	mov    %rax,%rdx
    140010ca3:	lea    -0x39(%rbp),%rcx
    140010ca7:	call   0x14000c3d0
    140010cac:	lea    0x860d(%rip),%rdx        # 0x1400192c0
@@ -20267,15 +20267,15 @@
    140010d2d:	pop    %rsi
    140010d2e:	pop    %rbx
    140010d2f:	ret
    140010d30:	call   *0x250a(%rip)        # 0x140013240
    140010d36:	mov    (%rax),%ecx
    140010d38:	call   *0x254a(%rip)        # 0x140013288
    140010d3e:	mov    %rax,%r8
-   140010d41:	lea    0x5b48(%rip),%rdx        # 0x140016890
+   140010d41:	lea    0x5b50(%rip),%rdx        # 0x140016898
    140010d48:	lea    0x38(%rsp),%rcx
    140010d4d:	call   0x14000de20
    140010d52:	nop
    140010d53:	mov    %rax,%rdx
    140010d56:	lea    0x20(%rsp),%rcx
    140010d5b:	call   0x14000c3d0
    140010d60:	lea    0x8559(%rip),%rdx        # 0x1400192c0
@@ -20387,15 +20387,15 @@
    140010ee0:	pop    %r12
    140010ee2:	pop    %rdi
    140010ee3:	ret
    140010ee4:	call   *0x2356(%rip)        # 0x140013240
    140010eea:	mov    (%rax),%ecx
    140010eec:	call   *0x2396(%rip)        # 0x140013288
    140010ef2:	mov    %rax,%r8
-   140010ef5:	lea    0x5994(%rip),%rdx        # 0x140016890
+   140010ef5:	lea    0x599c(%rip),%rdx        # 0x140016898
    140010efc:	lea    0x40(%rsp),%rcx
    140010f01:	call   0x14000de20
    140010f06:	nop
    140010f07:	mov    %rax,%rdx
    140010f0a:	lea    0x28(%rsp),%rcx
    140010f0f:	call   0x14000c3d0
    140010f14:	lea    0x83a5(%rip),%rdx        # 0x1400192c0
@@ -20404,15 +20404,15 @@
    140010f25:	nop
    140010f26:	call   0x14000d7a0
    140010f2b:	int3
    140010f2c:	call   *0x230e(%rip)        # 0x140013240
    140010f32:	mov    (%rax),%ecx
    140010f34:	call   *0x234e(%rip)        # 0x140013288
    140010f3a:	mov    %rax,%r8
-   140010f3d:	lea    0x594c(%rip),%rdx        # 0x140016890
+   140010f3d:	lea    0x5954(%rip),%rdx        # 0x140016898
    140010f44:	lea    0x40(%rsp),%rcx
    140010f49:	call   0x14000de20
    140010f4e:	nop
    140010f4f:	mov    %rax,%rdx
    140010f52:	lea    0x28(%rsp),%rcx
    140010f57:	call   0x14000c3d0
    140010f5c:	lea    0x835d(%rip),%rdx        # 0x1400192c0
@@ -27515,32 +27515,30 @@
    1400164e9:	jae    0x140016518
    1400164eb:	jb     0x140016562
    1400164ed:	outsb  %ds:(%rsi),(%dx)
    1400164ee:	outsb  %ds:(%rsi),(%dx)
    1400164ef:	gs jb  0x14001654e
    1400164f2:	(bad)
    1400164f7:	sub    $0x6c697562,%eax
-   1400164fc:	fs pop %rsp
-   1400164fe:	pop    %rdi
-   1400164ff:	ja     0x140016570
-   140016501:	jb     0x14001656e
-   140016503:	pop    %rsp
-   140016504:	imul   $0x6c6c2d78,0x65(%rax),%esi
-   14001650b:	insl   (%dx),%es:(%rdi)
-   14001650c:	pop    %rsp
-   14001650d:	imul   $0x6c6c2d78,0x65(%rax),%esi
-   140016514:	insl   (%dx),%es:(%rdi)
-   140016515:	pop    %rsp
-   140016516:	jae    0x14001658a
-   140016518:	movsxd 0x67(%rdi,%riz,2),%ebx
-   14001651c:	insl   (%dx),%es:(%rdi)
-   14001651d:	insb   (%dx),%es:(%rdi)
-   14001651e:	cs movsxd (%rax),%eax
-   140016521:	add    %al,(%rax)
-   140016523:	add    %al,(%rax)
+   1400164fc:	fs sub $0x5c77656e,%eax
+   140016502:	pop    %rdi
+   140016503:	ja     0x140016574
+   140016505:	jb     0x140016572
+   140016507:	pop    %rsp
+   140016508:	imul   $0x6c6c2d78,0x65(%rax),%esi
+   14001650f:	insl   (%dx),%es:(%rdi)
+   140016510:	pop    %rsp
+   140016511:	imul   $0x6c6c2d78,0x65(%rax),%esi
+   140016518:	insl   (%dx),%es:(%rdi)
+   140016519:	pop    %rsp
+   14001651a:	jae    0x14001658e
+   14001651c:	movsxd 0x67(%rdi,%riz,2),%ebx
+   140016520:	insl   (%dx),%es:(%rdi)
+   140016521:	insb   (%dx),%es:(%rdi)
+   140016522:	cs movsxd (%rax),%eax
    140016525:	add    %al,(%rax)
    140016527:	add    %al,0x47(%rdi)
    14001652a:	rex.WRB
    14001652b:	rex.WR pop %rdi
    14001652d:	push   %r11
    14001652f:	push   %rbx
    140016530:	rex.RB push %r10
@@ -27802,216 +27800,216 @@
    1400167a9:	jae    0x1400167d8
    1400167ab:	jb     0x140016822
    1400167ad:	outsb  %ds:(%rsi),(%dx)
    1400167ae:	outsb  %ds:(%rsi),(%dx)
    1400167af:	gs jb  0x14001680e
    1400167b2:	(bad)
    1400167b7:	sub    $0x6c697562,%eax
-   1400167bc:	fs pop %rsp
-   1400167be:	pop    %rdi
-   1400167bf:	ja     0x140016830
-   1400167c1:	jb     0x14001682e
-   1400167c3:	pop    %rsp
-   1400167c4:	imul   $0x6c6c2d78,0x65(%rax),%esi
-   1400167cb:	insl   (%dx),%es:(%rdi)
-   1400167cc:	pop    %rsp
-   1400167cd:	imul   $0x6c6c2d78,0x65(%rax),%esi
-   1400167d4:	insl   (%dx),%es:(%rdi)
-   1400167d5:	pop    %rsp
-   1400167d6:	jae    0x14001684a
-   1400167d8:	movsxd 0x6c(%rsp,%rbp,2),%ebx
-   1400167dc:	(bad)
-   1400167dd:	insl   (%dx),%es:(%rdi)
-   1400167de:	(bad)
-   1400167df:	pop    %rsp
-   1400167e0:	insb   (%dx),%es:(%rdi)
-   1400167e1:	insb   (%dx),%es:(%rdi)
+   1400167bc:	fs sub $0x5c77656e,%eax
+   1400167c2:	pop    %rdi
+   1400167c3:	ja     0x140016834
+   1400167c5:	jb     0x140016832
+   1400167c7:	pop    %rsp
+   1400167c8:	imul   $0x6c6c2d78,0x65(%rax),%esi
+   1400167cf:	insl   (%dx),%es:(%rdi)
+   1400167d0:	pop    %rsp
+   1400167d1:	imul   $0x6c6c2d78,0x65(%rax),%esi
+   1400167d8:	insl   (%dx),%es:(%rdi)
+   1400167d9:	pop    %rsp
+   1400167da:	jae    0x14001684e
+   1400167dc:	movsxd 0x6c(%rsp,%rbp,2),%ebx
+   1400167e0:	(bad)
+   1400167e1:	insl   (%dx),%es:(%rdi)
    1400167e2:	(bad)
-   1400167e3:	insl   (%dx),%es:(%rdi)
-   1400167e4:	(bad)
-   1400167e5:	sub    $0x6c697475,%eax
-   1400167ea:	cs push $0x0
-   1400167f0:	rex.WR
-   1400167f1:	rex.WR
-   1400167f2:	rex.B
-   1400167f3:	rex.WRB
-   1400167f4:	pop    %r15
-   1400167f6:	push   %r11
-   1400167f8:	push   %rbx
-   1400167f9:	rex.RB push %r10
-   1400167fb:	push   %rsp
-   1400167fc:	cmp    (%rax),%ah
-   1400167fe:	and    $0x64253a73,%eax
-   140016803:	cmp    (%rax),%ah
-   140016805:	and    $0xa73,%eax
-   14001680a:	add    %al,(%rax)
-   14001680c:	add    %al,(%rax)
-   14001680e:	add    %al,(%rax)
-   140016810:	jae    0x14001687b
-   140016812:	jp     0x140016879
-   140016814:	xor    (%rax),%ah
-   140016816:	cmp    $0x6973203d,%eax
-   14001681b:	jp     0x140016882
-   14001681d:	add    %al,(%rax)
-   14001681f:	add    %ah,0x61(%rsi)
-   140016822:	imul   $0x206f7420,0x64(%rbp,%riz,2),%ebp
-   14001682a:	outsl  %ds:(%rsi),(%dx)
-   14001682b:	jo     0x140016892
-   14001682d:	outsb  %ds:(%rsi),(%dx)
-   14001682e:	and    %ah,0x25203a73(%rip)        # 0x16521a2a7
-   140016834:	jae    0x140016836
-   140016836:	add    %al,(%rax)
-   140016838:	jb     0x14001689f
-   14001683a:	je     0x14001685c
-   14001683c:	and    %edi,0x312d20(%rip)        # 0x140329562
-   140016842:	add    %al,(%rax)
-   140016844:	add    %al,(%rax)
-   140016846:	add    %al,(%rax)
-   140016848:	jb     0x1400168af
-   14001684a:	je     0x14001686c
-   14001684c:	cmp    $0x30203d,%eax
-   140016851:	add    %al,(%rax)
-   140016853:	add    %al,(%rax)
-   140016855:	add    %al,(%rax)
-   140016857:	add    %dh,0x65(%rdx)
-   14001685a:	(bad)
-   14001685b:	and    %ah,%fs:0x72(%rbp)
-   14001685f:	jb     0x1400168d0
-   140016861:	jb     0x14001689d
-   140016863:	and    %ah,0x75000073(%rip)        # 0x1b50168dc
-   140016869:	outsb  %ds:(%rsi),(%dx)
-   14001686a:	gs js  0x1400168dd
-   14001686d:	movsxd %gs:0x64(%rbp,%riz,2),%esi
-   140016872:	insb   (%dx),%es:(%rdi)
-   140016873:	jns    0x140016895
-   140016875:	jb     0x1400168dc
-   140016877:	(bad)
-   140016878:	movsxd 0x65(%rax),%ebp
-   14001687b:	and    %ah,%fs:0x6e(%rbp)
-   14001687f:	and    %ch,%fs:0x66(%rdi)
-   140016883:	and    %ah,0x69(%rsi)
-   140016886:	insb   (%dx),%es:(%rdi)
-   140016887:	add    %al,%gs:(%rax)
-   14001688a:	add    %al,(%rax)
-   14001688c:	add    %al,(%rax)
-   14001688e:	add    %al,(%rax)
-   140016890:	ja     0x140016904
-   140016892:	imul   $0x6f727265,0x20(%rbp,%riz,2),%esi
-   14001689a:	jb     0x1400168d6
-   14001689c:	and    %ah,0x6f460073(%rip)        # 0x1af476915
-   1400168a2:	jb     0x140016911
-   1400168a4:	(bad)
-   1400168a5:	je     0x1400168f4
-   1400168a7:	gs jae 0x14001691d
-   1400168aa:	(bad)
-   1400168ab:	and    %spl,%gs:0x61(%r14d)
-   1400168b1:	imul   $0x77000000,0x64(%rbp,%riz,2),%ebp
-   1400168b9:	(bad)
-   1400168ba:	jb     0x14001692a
-   1400168bc:	imul   $0x6e55203a,0x67(%rsi),%ebp
-   1400168c3:	insl   (%dx),%es:(%rdi)
-   1400168c4:	(bad)
-   1400168c5:	jo     0x14001691d
-   1400168c7:	imul   $0x6946664f,0x77(%rbp),%esp
-   1400168ce:	insb   (%dx),%es:(%rdi)
-   1400168cf:	and    %ah,%gs:0x61(%rsi)
-   1400168d3:	imul   $0x7325203a,0x64(%rbp,%riz,2),%ebp
-   1400168db:	or     (%rax),%al
-   1400168dd:	add    %al,(%rax)
-   1400168df:	add    %al,0x1400173(%rax)
+   1400167e3:	pop    %rsp
+   1400167e4:	insb   (%dx),%es:(%rdi)
+   1400167e5:	insb   (%dx),%es:(%rdi)
+   1400167e6:	(bad)
+   1400167e7:	insl   (%dx),%es:(%rdi)
+   1400167e8:	(bad)
+   1400167e9:	sub    $0x6c697475,%eax
+   1400167ee:	cs push $0x0
+   1400167f4:	add    %al,(%rax)
+   1400167f6:	add    %al,(%rax)
+   1400167f8:	rex.WR
+   1400167f9:	rex.WR
+   1400167fa:	rex.B
+   1400167fb:	rex.WRB
+   1400167fc:	pop    %r15
+   1400167fe:	push   %r11
+   140016800:	push   %rbx
+   140016801:	rex.RB push %r10
+   140016803:	push   %rsp
+   140016804:	cmp    (%rax),%ah
+   140016806:	and    $0x64253a73,%eax
+   14001680b:	cmp    (%rax),%ah
+   14001680d:	and    $0xa73,%eax
+   140016812:	add    %al,(%rax)
+   140016814:	add    %al,(%rax)
+   140016816:	add    %al,(%rax)
+   140016818:	jae    0x140016883
+   14001681a:	jp     0x140016881
+   14001681c:	xor    (%rax),%ah
+   14001681e:	cmp    $0x6973203d,%eax
+   140016823:	jp     0x14001688a
+   140016825:	add    %al,(%rax)
+   140016827:	add    %ah,0x61(%rsi)
+   14001682a:	imul   $0x206f7420,0x64(%rbp,%riz,2),%ebp
+   140016832:	outsl  %ds:(%rsi),(%dx)
+   140016833:	jo     0x14001689a
+   140016835:	outsb  %ds:(%rsi),(%dx)
+   140016836:	and    %ah,0x25203a73(%rip)        # 0x16521a2af
+   14001683c:	jae    0x14001683e
+   14001683e:	add    %al,(%rax)
+   140016840:	jb     0x1400168a7
+   140016842:	je     0x140016864
+   140016844:	and    %edi,0x312d20(%rip)        # 0x14032956a
+   14001684a:	add    %al,(%rax)
+   14001684c:	add    %al,(%rax)
+   14001684e:	add    %al,(%rax)
+   140016850:	jb     0x1400168b7
+   140016852:	je     0x140016874
+   140016854:	cmp    $0x30203d,%eax
+   140016859:	add    %al,(%rax)
+   14001685b:	add    %al,(%rax)
+   14001685d:	add    %al,(%rax)
+   14001685f:	add    %dh,0x65(%rdx)
+   140016862:	(bad)
+   140016863:	and    %ah,%fs:0x72(%rbp)
+   140016867:	jb     0x1400168d8
+   140016869:	jb     0x1400168a5
+   14001686b:	and    %ah,0x75000073(%rip)        # 0x1b50168e4
+   140016871:	outsb  %ds:(%rsi),(%dx)
+   140016872:	gs js  0x1400168e5
+   140016875:	movsxd %gs:0x64(%rbp,%riz,2),%esi
+   14001687a:	insb   (%dx),%es:(%rdi)
+   14001687b:	jns    0x14001689d
+   14001687d:	jb     0x1400168e4
+   14001687f:	(bad)
+   140016880:	movsxd 0x65(%rax),%ebp
+   140016883:	and    %ah,%fs:0x6e(%rbp)
+   140016887:	and    %ch,%fs:0x66(%rdi)
+   14001688b:	and    %ah,0x69(%rsi)
+   14001688e:	insb   (%dx),%es:(%rdi)
+   14001688f:	add    %al,%gs:(%rax)
+   140016892:	add    %al,(%rax)
+   140016894:	add    %al,(%rax)
+   140016896:	add    %al,(%rax)
+   140016898:	ja     0x14001690c
+   14001689a:	imul   $0x6f727265,0x20(%rbp,%riz,2),%esi
+   1400168a2:	jb     0x1400168de
+   1400168a4:	and    %ah,0x6f460073(%rip)        # 0x1af47691d
+   1400168aa:	jb     0x140016919
+   1400168ac:	(bad)
+   1400168ad:	je     0x1400168fc
+   1400168af:	gs jae 0x140016925
+   1400168b2:	(bad)
+   1400168b3:	and    %spl,%gs:0x61(%r14d)
+   1400168b9:	imul   $0x77000000,0x64(%rbp,%riz,2),%ebp
+   1400168c1:	(bad)
+   1400168c2:	jb     0x140016932
+   1400168c4:	imul   $0x6e55203a,0x67(%rsi),%ebp
+   1400168cb:	insl   (%dx),%es:(%rdi)
+   1400168cc:	(bad)
+   1400168cd:	jo     0x140016925
+   1400168cf:	imul   $0x6946664f,0x77(%rbp),%esp
+   1400168d6:	insb   (%dx),%es:(%rdi)
+   1400168d7:	and    %ah,%gs:0x61(%rsi)
+   1400168db:	imul   $0x7325203a,0x64(%rbp,%riz,2),%ebp
+   1400168e3:	or     (%rax),%al
    1400168e5:	add    %al,(%rax)
-   1400168e7:	add    %ah,0x14000d0(%rax)
+   1400168e7:	add    %al,0x1400173(%rax)
    1400168ed:	add    %al,(%rax)
-   1400168ef:	add    %al,0x24(%rax)
-   1400168f2:	add    %al,0x1(%rax)
+   1400168ef:	add    %ah,0x14000d0(%rax)
    1400168f5:	add    %al,(%rax)
-   1400168f7:	add    %cl,(%rax)
-   1400168f9:	je     0x1400168fc
-   1400168fb:	rex add %eax,(%rax)
-   1400168fe:	add    %al,(%rax)
-   140016900:	movabs 0x40000000014000d0,%al
-   140016909:	and    $0x0,%al
-   14001690b:	rex add %eax,(%rax)
-   14001690e:	add    %al,(%rax)
-   140016910:	cwtl
-   140016911:	je     0x140016914
+   1400168f7:	add    %al,0x24(%rax)
+   1400168fa:	add    %al,0x1(%rax)
+   1400168fd:	add    %al,(%rax)
+   1400168ff:	add    %cl,(%rax)
+   140016901:	je     0x140016904
+   140016903:	rex add %eax,(%rax)
+   140016906:	add    %al,(%rax)
+   140016908:	movabs 0x40000000014000d0,%al
+   140016911:	and    $0x0,%al
    140016913:	rex add %eax,(%rax)
    140016916:	add    %al,(%rax)
-   140016918:	jo     0x1400168ea
-   14001691a:	add    %al,0x1(%rax)
-   14001691d:	add    %al,(%rax)
-   14001691f:	add    %ah,(%rax)
-   140016921:	cld
+   140016918:	cwtl
+   140016919:	je     0x14001691c
+   14001691b:	rex add %eax,(%rax)
+   14001691e:	add    %al,(%rax)
+   140016920:	jo     0x1400168f2
    140016922:	add    %al,0x1(%rax)
    140016925:	add    %al,(%rax)
-   140016927:	add    %dl,%al
-   140016929:	sti
+   140016927:	add    %ah,(%rax)
+   140016929:	cld
    14001692a:	add    %al,0x1(%rax)
    14001692d:	add    %al,(%rax)
-   14001692f:	add    %dh,0x14000dc(%rax)
+   14001692f:	add    %dl,%al
+   140016931:	sti
+   140016932:	add    %al,0x1(%rax)
    140016935:	add    %al,(%rax)
-   140016937:	add    %al,%al
-   140016939:	faddl  (%rax)
-   14001693b:	rex add %eax,(%rax)
-   14001693e:	add    %al,(%rax)
-   140016940:	loopne 0x14001691e
-   140016942:	add    %al,0x1(%rax)
-   140016945:	add    %al,(%rax)
-   140016947:	add    %ah,0x65(%rdi)
-   14001694a:	outsb  %ds:(%rsi),(%dx)
-   14001694b:	gs jb  0x1400169b7
-   14001694e:	movsxd (%rax),%eax
-   140016950:	and    $0x20007535,%eax
-   140016955:	js     0x140016977
-   140016957:	and    $0x7535,%eax
-   14001695c:	add    %al,(%rax)
-   14001695e:	add    %al,(%rax)
-   140016960:	imul   $0x69736e6f,0x63(%rsi),%ebp
-   140016967:	jae    0x1400169dd
-   140016969:	outsb  %gs:(%rsi),(%dx)
-   14001696b:	je     0x14001698d
-   14001696d:	je     0x1400169d4
-   14001696f:	outsb  %ds:(%rsi),(%dx)
-   140016970:	jae    0x1400169e1
-   140016972:	jb     0x140016994
-   140016974:	jae    0x1400169de
-   140016976:	(bad)
-   140016977:	jb     0x1400169dd
-   140016979:	and    %dh,0x70(%rcx,%rdi,2)
-   14001697d:	and    %ch,%gs:0x6e(%rcx)
-   140016981:	and    %ah,(%rdi)
-   140016983:	and    $0x2773,%eax
-   140016988:	je     0x1400169f9
-   14001698a:	imul   $0x6d,0x65(%rdi),%ebx
-   14001698e:	(bad)
-   140016993:	outsb  %ds:(%rsi),(%dx)
-   140016994:	addr32 jae 0x1400169c5
-   140016997:	add    %ch,(%rsi)
-   140016999:	(bad)
-   14001699a:	je     0x140016a10
-   14001699c:	outsb  %gs:(%rsi),(%dx)
-   14001699e:	je     0x140016a09
-   1400169a0:	outsl  %ds:(%rsi),(%dx)
-   1400169a1:	outsb  %ds:(%rsi),(%dx)
-   1400169a2:	ja,pn  0x140016a14
-   1400169a5:	ja,pn  0x140016a0d
-   1400169a8:	imul   $0x74,0x68(%rdi),%esp
-   1400169af:	add    %ch,(%rsi)
-   1400169b1:	gs gs fs pop %di
-   1400169b6:	outsw  %ds:(%rsi),(%dx)
-   1400169b8:	jb     0x140016a31
-   1400169ba:	(bad)
-   1400169bb:	jb     0x140016a21
-   1400169bd:	ja,pn  0x1400169f2
-   1400169c0:	ja,pn  0x140016a28
-   1400169c3:	imul   $0x74,0x68(%rdi),%esp
-   1400169ca:	add    %al,(%rax)
-   1400169cc:	add    %al,(%rax)
-   1400169ce:	add    %al,(%rax)
-   1400169d0:	imul   $0x69736e6f,0x63(%rsi),%ebp
+   140016937:	add    %dh,0x14000dc(%rax)
+   14001693d:	add    %al,(%rax)
+   14001693f:	add    %al,%al
+   140016941:	faddl  (%rax)
+   140016943:	rex add %eax,(%rax)
+   140016946:	add    %al,(%rax)
+   140016948:	loopne 0x140016926
+   14001694a:	add    %al,0x1(%rax)
+   14001694d:	add    %al,(%rax)
+   14001694f:	add    %ah,0x65(%rdi)
+   140016952:	outsb  %ds:(%rsi),(%dx)
+   140016953:	gs jb  0x1400169bf
+   140016956:	movsxd (%rax),%eax
+   140016958:	and    $0x20007535,%eax
+   14001695d:	js     0x14001697f
+   14001695f:	and    $0x7535,%eax
+   140016964:	add    %al,(%rax)
+   140016966:	add    %al,(%rax)
+   140016968:	imul   $0x69736e6f,0x63(%rsi),%ebp
+   14001696f:	jae    0x1400169e5
+   140016971:	outsb  %gs:(%rsi),(%dx)
+   140016973:	je     0x140016995
+   140016975:	je     0x1400169dc
+   140016977:	outsb  %ds:(%rsi),(%dx)
+   140016978:	jae    0x1400169e9
+   14001697a:	jb     0x14001699c
+   14001697c:	jae    0x1400169e6
+   14001697e:	(bad)
+   14001697f:	jb     0x1400169e5
+   140016981:	and    %dh,0x70(%rcx,%rdi,2)
+   140016985:	and    %ch,%gs:0x6e(%rcx)
+   140016989:	and    %ah,(%rdi)
+   14001698b:	and    $0x2773,%eax
+   140016990:	je     0x140016a01
+   140016992:	imul   $0x6d,0x65(%rdi),%ebx
+   140016996:	(bad)
+   14001699b:	outsb  %ds:(%rsi),(%dx)
+   14001699c:	addr32 jae 0x1400169cd
+   14001699f:	add    %ch,(%rsi)
+   1400169a1:	(bad)
+   1400169a2:	je     0x140016a18
+   1400169a4:	outsb  %gs:(%rsi),(%dx)
+   1400169a6:	je     0x140016a11
+   1400169a8:	outsl  %ds:(%rsi),(%dx)
+   1400169a9:	outsb  %ds:(%rsi),(%dx)
+   1400169aa:	ja,pn  0x140016a1c
+   1400169ad:	ja,pn  0x140016a15
+   1400169b0:	imul   $0x74,0x68(%rdi),%esp
+   1400169b7:	add    %ch,(%rsi)
+   1400169b9:	gs gs fs pop %di
+   1400169be:	outsw  %ds:(%rsi),(%dx)
+   1400169c0:	jb     0x140016a39
+   1400169c2:	(bad)
+   1400169c3:	jb     0x140016a29
+   1400169c5:	ja,pn  0x1400169fa
+   1400169c8:	ja,pn  0x140016a30
+   1400169cb:	imul   $0x6e690074,0x68(%rdi),%esp
+   1400169d2:	movsxd 0x6e(%rdi),%ebp
+   1400169d5:	jae    0x140016a40
    1400169d7:	jae    0x140016a4d
    1400169d9:	outsb  %gs:(%rsi),(%dx)
    1400169db:	je     0x1400169fd
    1400169dd:	je     0x140016a44
    1400169df:	outsb  %ds:(%rsi),(%dx)
    1400169e0:	jae    0x140016a51
    1400169e2:	jb     0x140016a04
@@ -28055,50 +28053,53 @@
    140016a49:	jae    0x140016a78
    140016a4b:	jb     0x140016ac2
    140016a4d:	outsb  %ds:(%rsi),(%dx)
    140016a4e:	outsb  %ds:(%rsi),(%dx)
    140016a4f:	gs jb  0x140016aae
    140016a52:	(bad)
    140016a57:	sub    $0x6c697562,%eax
-   140016a5c:	fs pop %rsp
-   140016a5e:	pop    %rdi
-   140016a5f:	ja     0x140016ad0
-   140016a61:	jb     0x140016ace
-   140016a63:	pop    %rsp
-   140016a64:	imul   $0x6c6c2d78,0x65(%rax),%esi
-   140016a6b:	insl   (%dx),%es:(%rdi)
-   140016a6c:	pop    %rsp
-   140016a6d:	imul   $0x6c6c2d78,0x65(%rax),%esi
-   140016a74:	insl   (%dx),%es:(%rdi)
-   140016a75:	pop    %rsp
-   140016a76:	jae    0x140016aea
-   140016a78:	movsxd 0x6c(%rsp,%rbp,2),%ebx
-   140016a7c:	(bad)
-   140016a7d:	insl   (%dx),%es:(%rdi)
-   140016a7e:	(bad)
-   140016a7f:	pop    %rsp
-   140016a80:	insb   (%dx),%es:(%rdi)
-   140016a81:	insb   (%dx),%es:(%rdi)
+   140016a5c:	fs sub $0x5c77656e,%eax
+   140016a62:	pop    %rdi
+   140016a63:	ja     0x140016ad4
+   140016a65:	jb     0x140016ad2
+   140016a67:	pop    %rsp
+   140016a68:	imul   $0x6c6c2d78,0x65(%rax),%esi
+   140016a6f:	insl   (%dx),%es:(%rdi)
+   140016a70:	pop    %rsp
+   140016a71:	imul   $0x6c6c2d78,0x65(%rax),%esi
+   140016a78:	insl   (%dx),%es:(%rdi)
+   140016a79:	pop    %rsp
+   140016a7a:	jae    0x140016aee
+   140016a7c:	movsxd 0x6c(%rsp,%rbp,2),%ebx
+   140016a80:	(bad)
+   140016a81:	insl   (%dx),%es:(%rdi)
    140016a82:	(bad)
-   140016a83:	insl   (%dx),%es:(%rdi)
-   140016a84:	(bad)
-   140016a85:	cs movsxd 0x70(%rax),%esi
-   140016a89:	add    %al,(%rax)
-   140016a8b:	add    %dh,0x62(%rdx)
-   140016a8e:	add    %al,(%rax)
-   140016a90:	(bad)
-   140016a95:	sub    $0x3a6d6c6c,%eax
-   140016a9a:	and    %ch,0x61(%rdi,%rbp,2)
-   140016a9e:	imul   $0x646f6d20,%fs:0x67(%rsi),%ebp
-   140016aa6:	gs insb (%dx),%es:(%rdi)
-   140016aa8:	and    %ah,0x72(%rsi)
-   140016aab:	outsl  %ds:(%rsi),(%dx)
-   140016aac:	insl   (%dx),%es:(%rdi)
-   140016aad:	and    %ah,0xa73(%rip)        # 0x140017526
-	...
+   140016a83:	pop    %rsp
+   140016a84:	insb   (%dx),%es:(%rdi)
+   140016a85:	insb   (%dx),%es:(%rdi)
+   140016a86:	(bad)
+   140016a87:	insl   (%dx),%es:(%rdi)
+   140016a88:	(bad)
+   140016a89:	cs movsxd 0x70(%rax),%esi
+   140016a8d:	add    %al,(%rax)
+   140016a8f:	add    %dh,0x62(%rdx)
+   140016a92:	add    %al,(%rax)
+   140016a94:	add    %al,(%rax)
+   140016a96:	add    %al,(%rax)
+   140016a98:	(bad)
+   140016a9d:	sub    $0x3a6d6c6c,%eax
+   140016aa2:	and    %ch,0x61(%rdi,%rbp,2)
+   140016aa6:	imul   $0x646f6d20,%fs:0x67(%rsi),%ebp
+   140016aae:	gs insb (%dx),%es:(%rdi)
+   140016ab0:	and    %ah,0x72(%rsi)
+   140016ab3:	outsl  %ds:(%rsi),(%dx)
+   140016ab4:	insl   (%dx),%es:(%rdi)
+   140016ab5:	and    %ah,0xa73(%rip)        # 0x14001752e
+   140016abb:	add    %al,(%rax)
+   140016abd:	add    %al,(%rax)
    140016abf:	add    %dh,0x6e(%rbp)
    140016ac2:	imul   $0x77,0x6f(%rsi),%ebp
    140016ac6:	outsb  %ds:(%rsi),(%dx)
    140016ac7:	and    %ch,(%rax)
    140016ac9:	insl   (%dx),%es:(%rdi)
    140016aca:	(bad)
    140016acb:	imul   $0x72657620,0x2c(%ebx),%esp
@@ -28610,19 +28611,17 @@
    1400170cd:	add    %al,(%rax)
    1400170cf:	add    %cl,0x1400133(%rax)
    1400170d5:	add    %al,(%rax)
    1400170d7:	add    %dl,0x1400133(%rax)
    1400170dd:	add    %al,(%rax)
    1400170df:	add    %al,(%rax)
    1400170e1:	add    %al,(%rax)
-   1400170e3:	add    %dl,0x38(%rax)
-   1400170e6:	pop    %rbx
-   1400170e7:	data16 add %al,(%rax)
-   1400170ea:	add    %al,(%rax)
-   1400170ec:	or     $0x90000000,%eax
+   1400170e3:	add    %bl,0x665c89(%rbp)
+   1400170e9:	add    %al,(%rax)
+   1400170eb:	add    %cl,-0x70000000(%rip)        # 0xd00170f1
    1400170f1:	add    (%rax),%eax
    1400170f3:	add    %ch,0x1(%rsi,%rsi,2)
    1400170f7:	add    %ch,0x1(%rsi,%riz,2)
    1400170fb:	add    %al,(%rax)
    1400170fd:	add    %al,(%rax)
    1400170ff:	add    %ah,(%rax)
    140017101:	jp     0x140017104
@@ -33768,15 +33767,15 @@
    14001b439:	cmp    (%rcx),%eax
    14001b43b:	rex add %eax,(%rax)
    14001b43e:	add    %al,(%rax)
    14001b440:	pop    %rsp
    14001b441:	cmp    (%rcx),%eax
    14001b443:	rex add %eax,(%rax)
    14001b446:	add    %al,(%rax)
-   14001b448:	sbb    %ch,0x1(%rcx)
+   14001b448:	and    %ch,0x1(%rcx)
    14001b44b:	rex add %eax,(%rax)
    14001b44e:	add    %al,(%rax)
    14001b450:	add    (%rax),%eax
    14001b452:	add    %al,(%rax)
    14001b454:	add    %al,(%rax)
    14001b456:	add    %al,(%rax)
    14001b458:	(bad)
@@ -35693,22 +35692,20 @@
    1400c006e:	cwtl
    1400c006f:	scas   %es:(%rdi),%eax
    1400c0070:	add    %ah,0x1(%rax)
    1400c0073:	add    %dh,(%rax,%rax,1)
    1400c0076:	add    %al,(%rax)
    1400c0078:	push   $0x78a770a7
    1400c007d:	cmpsl  %es:(%rdi),%ds:(%rsi)
-   1400c007e:	loopne 0x1400c0028
-   1400c0080:	call   0x138b4f12d
-   1400c0085:	test   $0x0,%al
-   1400c0087:	test   $0xa910a908,%eax
-   1400c008c:	sbb    %ch,-0x56d756e0(%rcx)
-   1400c0092:	xor    %ch,-0x56bf56c8(%rcx)
-   1400c0098:	jo     0x1400c0049
-   1400c009a:	js     0x1400c004b
+   1400c007e:	call   0x138b4f12b
+   1400c0083:	test   $0x0,%al
+   1400c0085:	test   $0xa910a908,%eax
+   1400c008a:	sbb    %ch,-0x56d756e0(%rcx)
+   1400c0090:	xor    %ch,-0x56bf56c8(%rcx)
+   1400c0096:	test   $0xffffffffaf78af70,%rax
    1400c009c:	subb   $0x0,-0x50075078(%rdi)
    1400c00a3:	add    %al,(%rax)
    1400c00a5:	jo     0x1400c00a8
    1400c00a7:	add    %ah,(%rax)
    1400c00a9:	add    %al,(%rax)
    1400c00ab:	add    %dl,(%rax)
    1400c00ad:	movabs 0xa0c0a0b8a0a0a018,%al
```

## ipex_llm/libs/quantize-starcoder.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x0000000140013c70
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Sat Jun  1 15:02:42 2024
+Time/Date		Sun Jun  2 15:02:41 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000013c00
 SizeOfInitializedData	00000000000ace00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000013c70
@@ -32581,19 +32581,17 @@
    140019325:	add    %al,(%rax)
    140019327:	add    %al,(%rax)
    140019329:	push   %rbp
    14001932a:	add    %eax,0x1(%rax)
    14001932d:	add    %al,(%rax)
    14001932f:	add    %al,(%rax)
    140019331:	add    %al,(%rax)
-   140019333:	add    %dl,(%rdx)
-   140019335:	cmp    %bl,0x66(%rbx)
-   140019338:	add    %al,(%rax)
-   14001933a:	add    %al,(%rax)
-   14001933c:	or     $0x20000000,%eax
+   140019333:	add    %dl,0x665c89(%rcx)
+   140019339:	add    %al,(%rax)
+   14001933b:	add    %cl,0x20000000(%rip)        # 0x160019341
    140019341:	add    (%rax),%eax
    140019343:	add    %bh,%ah
    140019345:	movabs %al,0x192fc0001
 	...
    14001937e:	add    %al,(%rax)
    140019380:	add    %eax,(%rax)
 	...
```

## ipex_llm/libs/quantize-starcoder_vnni.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x0000000140013e80
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Sat Jun  1 15:03:45 2024
+Time/Date		Sun Jun  2 15:02:54 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000013e00
 SizeOfInitializedData	00000000000ad200
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000013e80
@@ -32434,32 +32434,30 @@
    140018f99:	jae    0x140018fc8
    140018f9b:	jb     0x140019012
    140018f9d:	outsb  %ds:(%rsi),(%dx)
    140018f9e:	outsb  %ds:(%rsi),(%dx)
    140018f9f:	gs jb  0x140018ffe
    140018fa2:	(bad)
    140018fa7:	sub    $0x6c697562,%eax
-   140018fac:	fs pop %rsp
-   140018fae:	pop    %rdi
-   140018faf:	ja     0x140019020
-   140018fb1:	jb     0x14001901e
-   140018fb3:	pop    %rsp
-   140018fb4:	imul   $0x6c6c2d78,0x65(%rax),%esi
-   140018fbb:	insl   (%dx),%es:(%rdi)
-   140018fbc:	pop    %rsp
-   140018fbd:	imul   $0x6c6c2d78,0x65(%rax),%esi
-   140018fc4:	insl   (%dx),%es:(%rdi)
-   140018fc5:	pop    %rsp
-   140018fc6:	jae    0x14001903a
-   140018fc8:	movsxd 0x67(%rdi,%riz,2),%ebx
-   140018fcc:	insl   (%dx),%es:(%rdi)
-   140018fcd:	insb   (%dx),%es:(%rdi)
-   140018fce:	cs movsxd (%rax),%eax
-   140018fd1:	add    %al,(%rax)
-   140018fd3:	add    %al,(%rax)
+   140018fac:	fs sub $0x5c77656e,%eax
+   140018fb2:	pop    %rdi
+   140018fb3:	ja     0x140019024
+   140018fb5:	jb     0x140019022
+   140018fb7:	pop    %rsp
+   140018fb8:	imul   $0x6c6c2d78,0x65(%rax),%esi
+   140018fbf:	insl   (%dx),%es:(%rdi)
+   140018fc0:	pop    %rsp
+   140018fc1:	imul   $0x6c6c2d78,0x65(%rax),%esi
+   140018fc8:	insl   (%dx),%es:(%rdi)
+   140018fc9:	pop    %rsp
+   140018fca:	jae    0x14001903e
+   140018fcc:	movsxd 0x67(%rdi,%riz,2),%ebx
+   140018fd0:	insl   (%dx),%es:(%rdi)
+   140018fd1:	insb   (%dx),%es:(%rdi)
+   140018fd2:	cs movsxd (%rax),%eax
    140018fd5:	add    %al,(%rax)
    140018fd7:	add    %al,0x47(%rdi)
    140018fda:	rex.WRB
    140018fdb:	rex.WR pop %rdi
    140018fdd:	push   %r11
    140018fdf:	push   %rbx
    140018fe0:	rex.RB push %r10
@@ -32706,19 +32704,17 @@
    140019305:	add    %al,(%rax)
    140019307:	add    %al,(%rax)
    140019309:	push   %rbp
    14001930a:	add    %eax,0x1(%rax)
    14001930d:	add    %al,(%rax)
    14001930f:	add    %al,(%rax)
    140019311:	add    %al,(%rax)
-   140019313:	add    %dl,0x38(%rcx)
-   140019316:	pop    %rbx
-   140019317:	data16 add %al,(%rax)
-   14001931a:	add    %al,(%rax)
-   14001931c:	or     $0x20000000,%eax
+   140019313:	add    %bl,0x665c89(%rsi)
+   140019319:	add    %al,(%rax)
+   14001931b:	add    %cl,0x20000000(%rip)        # 0x160019321
    140019321:	add    (%rax),%eax
    140019323:	add    %bh,%ah
    140019325:	movabs %al,0x194fc0001
 	...
    14001937e:	add    %al,(%rax)
    140019380:	add    %eax,(%rax)
 	...
```

## ipex_llm/libs/starcoder-api.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x000000018000277c
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Sat Jun  1 15:02:42 2024
+Time/Date		Sun Jun  2 15:02:41 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000002200
 SizeOfInitializedData	0000000000003400
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000000277c
@@ -4028,19 +4028,18 @@
    1800045f0:	cmp    %al,0x0(%rdx)
    1800045f3:	addb   $0x0,(%rcx)
    1800045f6:	add    %al,(%rax)
    1800045f8:	rex
    1800045f9:	rex.X add %al,0x1(%rax)
    180004600:	add    %al,(%rax)
    180004602:	add    %al,(%rax)
-   180004604:	adc    (%rax),%bh
-   180004606:	pop    %rbx
-   180004607:	data16 add %al,(%rax)
-   18000460a:	add    %al,(%rax)
-   18000460c:	or     $0xe0000000,%eax
+   180004604:	xchg   %eax,%ecx
+   180004605:	mov    %ebx,0x0(%rsi,%riz,2)
+   180004609:	add    %al,(%rax)
+   18000460b:	add    %cl,-0x20000000(%rip)        # 0x160004611
    180004611:	add    (%rax),%al
    180004613:	add    %ah,%ah
    180004615:	rex.W add %al,(%rax)
    180004618:	in     $0x2e,%al
 	...
    18000467e:	add    %al,(%rax)
    180004680:	add    %eax,(%rax)
```

## ipex_llm/libs/starcoder.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180063388
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Sat Jun  1 15:02:42 2024
+Time/Date		Sun Jun  2 15:02:41 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000063a00
 SizeOfInitializedData	00000000000c8000
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000063388
@@ -133106,19 +133106,18 @@
    18006cd77:	add    %al,%al
    18006cd79:	push   %rsi
    18006cd7a:	(bad)
    18006cd7b:	addb   $0x0,(%rcx)
    18006cd7e:	add    %al,(%rax)
    18006cd80:	add    %al,(%rax)
    18006cd82:	add    %al,(%rax)
-   18006cd84:	adc    (%rax),%bh
-   18006cd86:	pop    %rbx
-   18006cd87:	data16 add %al,(%rax)
-   18006cd8a:	add    %al,(%rax)
-   18006cd8c:	or     $0x50000000,%eax
+   18006cd84:	xchg   %eax,%ecx
+   18006cd85:	mov    %ebx,0x0(%rsi,%riz,2)
+   18006cd89:	add    %al,(%rax)
+   18006cd8b:	add    %cl,0x50000000(%rip)        # 0x1d006cd91
    18006cd91:	add    (%rax),%eax
    18006cd93:	add    %dl,-0x21(%rax)
    18006cd96:	(bad)
    18006cd97:	add    %dl,-0x33(%rax)
    18006cd9a:	(bad)
 	...
    18006cdff:	add    %al,%al
```

## Comparing `ipex_llm-2.1.0b20240601.data/scripts/ipex-llm-init.bat` & `ipex_llm-2.1.0b20240602.data/scripts/ipex-llm-init.bat`

 * *Files identical despite different names*

## Comparing `ipex_llm-2.1.0b20240601.data/scripts/llm-chat.ps1` & `ipex_llm-2.1.0b20240602.data/scripts/llm-chat.ps1`

 * *Files identical despite different names*

## Comparing `ipex_llm-2.1.0b20240601.data/scripts/llm-cli.ps1` & `ipex_llm-2.1.0b20240602.data/scripts/llm-cli.ps1`

 * *Files identical despite different names*

## Comparing `ipex_llm-2.1.0b20240601.dist-info/METADATA` & `ipex_llm-2.1.0b20240602.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipex-llm
-Version: 2.1.0b20240601
+Version: 2.1.0b20240602
 Summary: Large Language Model Develop Toolkit
 Home-page: https://github.com/intel-analytics/ipex-llm
 Author: BigDL Authors
 Author-email: bigdl-user-group@googlegroups.com
 License: Apache License, Version 2.0
 Platform: windows
 Classifier: License :: OSI Approved :: Apache Software License
@@ -22,15 +22,15 @@
 Requires-Dist: tokenizers (==0.15.2) ; extra == 'all'
 Requires-Dist: accelerate (==0.21.0) ; extra == 'all'
 Requires-Dist: tabulate ; extra == 'all'
 Requires-Dist: intel-openmp ; (platform_machine == "x86_64" or platform_machine == "AMD64") and extra == 'all'
 Requires-Dist: torch (==2.1.2+cpu) ; (platform_system == "Linux") and extra == 'all'
 Requires-Dist: torch (==2.1.2) ; (platform_system == "Windows") and extra == 'all'
 Provides-Extra: cpp
-Requires-Dist: bigdl-core-cpp (==2.5.0b20240601) ; extra == 'cpp'
+Requires-Dist: bigdl-core-cpp (==2.5.0b20240602) ; extra == 'cpp'
 Requires-Dist: dpcpp-cpp-rt (==2024.0.2) ; (platform_system == "Windows") and extra == 'cpp'
 Requires-Dist: mkl-dpcpp (==2024.0.0) ; (platform_system == "Windows") and extra == 'cpp'
 Requires-Dist: onednn (==2024.0.0) ; (platform_system == "Windows") and extra == 'cpp'
 Provides-Extra: llama-index
 Requires-Dist: py-cpuinfo ; extra == 'llama-index'
 Requires-Dist: protobuf ; extra == 'llama-index'
 Requires-Dist: mpmath (==1.3.0) ; extra == 'llama-index'
@@ -58,34 +58,34 @@
 Requires-Dist: tokenizers (==0.15.2) ; extra == 'xpu'
 Requires-Dist: accelerate (==0.21.0) ; extra == 'xpu'
 Requires-Dist: tabulate ; extra == 'xpu'
 Requires-Dist: setuptools (<70.0.0) ; extra == 'xpu'
 Requires-Dist: torch (==2.1.0a0) ; extra == 'xpu'
 Requires-Dist: torchvision (==0.16.0a0) ; extra == 'xpu'
 Requires-Dist: intel-extension-for-pytorch (==2.1.10+xpu) ; extra == 'xpu'
-Requires-Dist: bigdl-core-xe-21 (==2.5.0b20240601) ; extra == 'xpu'
-Requires-Dist: bigdl-core-xe-batch-21 (==2.5.0b20240601) ; extra == 'xpu'
-Requires-Dist: bigdl-core-xe-addons-21 (==2.5.0b20240601) ; extra == 'xpu'
+Requires-Dist: bigdl-core-xe-21 (==2.5.0b20240602) ; extra == 'xpu'
+Requires-Dist: bigdl-core-xe-batch-21 (==2.5.0b20240602) ; extra == 'xpu'
+Requires-Dist: bigdl-core-xe-addons-21 (==2.5.0b20240602) ; extra == 'xpu'
 Provides-Extra: xpu-2-1
 Requires-Dist: py-cpuinfo ; extra == 'xpu-2-1'
 Requires-Dist: protobuf ; extra == 'xpu-2-1'
 Requires-Dist: mpmath (==1.3.0) ; extra == 'xpu-2-1'
 Requires-Dist: numpy (==1.26.4) ; extra == 'xpu-2-1'
 Requires-Dist: transformers (==4.36.2) ; extra == 'xpu-2-1'
 Requires-Dist: sentencepiece ; extra == 'xpu-2-1'
 Requires-Dist: tokenizers (==0.15.2) ; extra == 'xpu-2-1'
 Requires-Dist: accelerate (==0.21.0) ; extra == 'xpu-2-1'
 Requires-Dist: tabulate ; extra == 'xpu-2-1'
 Requires-Dist: setuptools (<70.0.0) ; extra == 'xpu-2-1'
 Requires-Dist: torch (==2.1.0a0) ; extra == 'xpu-2-1'
 Requires-Dist: torchvision (==0.16.0a0) ; extra == 'xpu-2-1'
 Requires-Dist: intel-extension-for-pytorch (==2.1.10+xpu) ; extra == 'xpu-2-1'
-Requires-Dist: bigdl-core-xe-21 (==2.5.0b20240601) ; extra == 'xpu-2-1'
-Requires-Dist: bigdl-core-xe-batch-21 (==2.5.0b20240601) ; extra == 'xpu-2-1'
-Requires-Dist: bigdl-core-xe-addons-21 (==2.5.0b20240601) ; extra == 'xpu-2-1'
+Requires-Dist: bigdl-core-xe-21 (==2.5.0b20240602) ; extra == 'xpu-2-1'
+Requires-Dist: bigdl-core-xe-batch-21 (==2.5.0b20240602) ; extra == 'xpu-2-1'
+Requires-Dist: bigdl-core-xe-addons-21 (==2.5.0b20240602) ; extra == 'xpu-2-1'
 Requires-Dist: intel-openmp ; (platform_machine == "x86_64" or platform_machine == "AMD64") and extra == 'xpu-2-1'
 Requires-Dist: dpcpp-cpp-rt (==2024.0.2) ; (platform_system == "Windows") and extra == 'xpu-2-1'
 Requires-Dist: mkl-dpcpp (==2024.0.0) ; (platform_system == "Windows") and extra == 'xpu-2-1'
 Requires-Dist: onednn (==2024.0.0) ; (platform_system == "Windows") and extra == 'xpu-2-1'
 Requires-Dist: intel-openmp ; (platform_machine == "x86_64" or platform_machine == "AMD64") and extra == 'xpu'
 Requires-Dist: dpcpp-cpp-rt (==2024.0.2) ; (platform_system == "Windows") and extra == 'xpu'
 Requires-Dist: mkl-dpcpp (==2024.0.0) ; (platform_system == "Windows") and extra == 'xpu'
```

## Comparing `ipex_llm-2.1.0b20240601.dist-info/RECORD` & `ipex_llm-2.1.0b20240602.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -37,42 +37,42 @@
 ipex_llm/langchain/llms/__init__.py,sha256=aR443l0B4djP7nnc0ZS8c83wu52yg55R6jNHOJpBUfM,1588
 ipex_llm/langchain/llms/bigdlllm.py,sha256=T_9-cd_pTYzQgx-XG_Quv_nSDptBdupbngvsfI_e_S4,24235
 ipex_llm/langchain/llms/transformersllm.py,sha256=7eaIkJi1CbTCSgNxBCoZTe-o_5FYjD1GTYPWpn0Ccr4,10576
 ipex_llm/langchain/llms/transformerspipelinellm.py,sha256=vm522YPPwWxxAPVvQBtxRfBinC4hIbXdKW6VjHDaFXY,7379
 ipex_llm/langchain/vllm/__init__.py,sha256=T-EbRT6GJ_8RCu-iLmSzcftOimXSPQf2d5X72AUAy2Y,874
 ipex_llm/langchain/vllm/vllm.py,sha256=6dxc-ZISZQrJilEa_HA827l75Dv9rcHpY_G6FdJ8BVs,7793
 ipex_llm/libs/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-ipex_llm/libs/bloom-api.dll,sha256=4qY_O0IbjlNmvmmVZYQG9pRytctehGWQ-N-lA2Lk-3w,36352
-ipex_llm/libs/bloom.dll,sha256=g6prmY4Gz4MbS63iRCSHQNKTugvwd4cd0HBzJXmePYU,473088
-ipex_llm/libs/gptneox-api.dll,sha256=NgBGApS4hfol4hEyqvvF5Lme-z8wpZzKZb4PD5i8nN0,24576
-ipex_llm/libs/gptneox.dll,sha256=yPU_9AQcnM5Q51cCiH1S1K_k_6wJuXg14PQv9CA-XbY,532992
-ipex_llm/libs/libbloom_avx.dll,sha256=uw5lwfmfu0c3z0pY55e4N4W2tqY3aGxhjAohRycFZn8,499712
-ipex_llm/libs/libbloom_vnni.dll,sha256=IRg8Gz1gpW36HKn-bvLBn9Jht_gzn4Uxc_Rj9nVO3GA,473600
-ipex_llm/libs/libgptneox_avx.dll,sha256=FLXLzCj4YJtlo_tn5jzRlF-bTrI7Pw7tJ-KnV9hDpck,559616
-ipex_llm/libs/libgptneox_vnni.dll,sha256=OM1v1TX8JPW0owKtf57-X7oOPgaVXX3E3P_eewdSp_I,533504
-ipex_llm/libs/libllama_avx.dll,sha256=pVuEXSuPaQ3Sfj7LdIUM5aiSAHMH_pP7ezcYyg2j-QM,553472
-ipex_llm/libs/libllama_vnni.dll,sha256=Hgunt00_8wRSlGb09_zBvNMyDtoBsygwSi2x_adNKNk,527360
-ipex_llm/libs/libstarcoder_avx.dll,sha256=FcK0OkOQlgQf6WEL4B8H8jlE2bYXvu1a7zPLjSICA6s,590848
-ipex_llm/libs/libstarcoder_vnni.dll,sha256=CspTTFuXhQvbDBN2NfxRj-arQwaBNzkv2bncE9_kuhg,564736
-ipex_llm/libs/llama-api.dll,sha256=idrPi-be8ZYXKjeg9QFzmmGAm-bGPW2-wFzOjrj3kGc,25088
-ipex_llm/libs/llama.dll,sha256=GQClnoVMXtsz8X76XvEUElj3mzo7rUFJFuUYE0rU-NE,527360
-ipex_llm/libs/main-bloom.exe,sha256=FvLEWyXzrInt18Lyw-K0lgQnN8jqS2NIrnD-2abZbJs,103424
-ipex_llm/libs/main-gptneox.exe,sha256=IxC3lNHSpIrHHi6RwJA72nClaeZNFUuoG7MYVezpths,98816
-ipex_llm/libs/main-llama.exe,sha256=gS39H0TViJLhfy-W2_N26wtMqCBNUKRpzw4ZESUM5xI,99840
-ipex_llm/libs/main-starcoder.exe,sha256=1yt-wKBiA07v0fAxaPKNI2thQ7yCb8e5DohEU3rokdk,157696
-ipex_llm/libs/quantize-bloom.exe,sha256=04SJJWU28btUMWcT0Ft8GY2THLmdCwvoIRD3_kFRbiM,126464
-ipex_llm/libs/quantize-bloom_vnni.exe,sha256=aRPEiC8taJarNvQTho9HTP1_eZLBVUPiPs70sm0UxNw,127488
-ipex_llm/libs/quantize-gptneox.exe,sha256=pQAcTwxwr9Zkse4Yhv-w-KWhhvR7D0vHfRhwBq7JYB0,103936
-ipex_llm/libs/quantize-gptneox_vnni.exe,sha256=VgWEBK-mBX8Kwd_r8qJ33ycTTtiiRYsqU_gK90yHWRQ,104448
-ipex_llm/libs/quantize-llama.exe,sha256=8Jdz0FDExxQDgUKsMnK5LXYXZIz6QYA-LeOsAylc7x0,109056
-ipex_llm/libs/quantize-llama_vnni.exe,sha256=wxMvH7Hg0qCvFjyx39yRZavOGUPVdNCOq8nj7Rs6tao,110080
-ipex_llm/libs/quantize-starcoder.exe,sha256=Nf7f3GoifUsJ8FAxIOgi_laYcfaoaah9Tu7xlMsGIMI,126976
-ipex_llm/libs/quantize-starcoder_vnni.exe,sha256=nPEDS0cK-2c9JNZVZXzHxt-nfi1aL6W90OYpi1KjkYk,128512
-ipex_llm/libs/starcoder-api.dll,sha256=5wYx9dNa_SkBeA1j4YE9h3GyrgMg7Z_fIjeHkIkmnYA,21504
-ipex_llm/libs/starcoder.dll,sha256=Ud_lKvBwrUQHaNdBngsZ_et_JhF5oBiHSPbfr0AS6NM,564224
+ipex_llm/libs/bloom-api.dll,sha256=tdiWcIscsIbHFApm_cTOFUxGdsM_EQ1jVH8CdSvyPmU,36352
+ipex_llm/libs/bloom.dll,sha256=GJCaolfTsdXNb65cQJGHZwskfQeIhQzkNOTWfYgat6s,473088
+ipex_llm/libs/gptneox-api.dll,sha256=9v6_4orA0CZi3qF6iTokrvyiDAxRHnm0yrJLIAnqou0,24576
+ipex_llm/libs/gptneox.dll,sha256=7-zSsEnTfvecFqQKSfLBTpBr43nxfg5s-tjsScbOz-o,532992
+ipex_llm/libs/libbloom_avx.dll,sha256=NdrUeX2tK7pUeNCWfynavlPsWz_qfFjGnQgVji1a2PU,499712
+ipex_llm/libs/libbloom_vnni.dll,sha256=MhZymV2Rnb3R2ZrjgCKGmtFotLkKXpMV8_JRhQEHSqo,473600
+ipex_llm/libs/libgptneox_avx.dll,sha256=eronnu6_fbbcX0mXdGQaF9-NxWGOWXYZKT0b2cyuhMI,559616
+ipex_llm/libs/libgptneox_vnni.dll,sha256=pIYc6Yxgcqe2oXedY8srOu-NO1XfeRHPW4B7zyU61rU,533504
+ipex_llm/libs/libllama_avx.dll,sha256=wZ0hH7rnqCcAKfuGDUizg3qXZS9ngQ5MSuBX69kwmvI,553472
+ipex_llm/libs/libllama_vnni.dll,sha256=oIV_lRDD-LxBUe3m2gGRlJ1yBFH-4nnv_WFxcS-LYqA,527360
+ipex_llm/libs/libstarcoder_avx.dll,sha256=Ecyb1QnAFuadxPHt0Kz7-QusEzoAkqdnu72IokXQzBI,590848
+ipex_llm/libs/libstarcoder_vnni.dll,sha256=v5gFy9H73vBemGhWV90ElO5wtkZhDd6XKk6FYsPEAIc,564736
+ipex_llm/libs/llama-api.dll,sha256=wqpQV6TU-W7hre8wSoNRWfQu7sHG4SBg-iRO_jCEPrc,25088
+ipex_llm/libs/llama.dll,sha256=WbBcrUr0j-GSmmT9QKC31Z3wsbj6eJRbOO0rYjTkjK4,527360
+ipex_llm/libs/main-bloom.exe,sha256=1F8Ry-VH4OBE3Cl-CXzDuNEwrlfoqsAbfsSQKlhwhkU,103424
+ipex_llm/libs/main-gptneox.exe,sha256=kn7hGldsoQDFu7OmRn8NG2xI8q-sHVWSxvNp54TgoEI,98816
+ipex_llm/libs/main-llama.exe,sha256=_UR8hoQc2Z6MHQ_BI5r5V_Spaum1oWkD-Fc7ki3Thvg,99840
+ipex_llm/libs/main-starcoder.exe,sha256=beegg6KbWF1m5dLMlyrPHpNbFCrYXkQK_w5o1pPezw4,157696
+ipex_llm/libs/quantize-bloom.exe,sha256=c2blnxZ8vHpXRJxVPs1a9PS-nn2qqcIZYkC8X9KjqRU,126464
+ipex_llm/libs/quantize-bloom_vnni.exe,sha256=Jv-mgqlz8v5D06kVWilZZ7GaZ_qZg0m6RExzB0P-o6g,127488
+ipex_llm/libs/quantize-gptneox.exe,sha256=QCfUKhNV_55gAHRgl-uRWcBxGteL2D4TYTysRSXqwJA,103936
+ipex_llm/libs/quantize-gptneox_vnni.exe,sha256=eHcwLPoKuJiKWYjhxoDZ6IhLkfaZry23Rj9oxzuIxHE,104448
+ipex_llm/libs/quantize-llama.exe,sha256=hxWRi6ELsoIh_Nm4YR_oL4cn5qg4cXEkvAiCGKwM-Jo,109056
+ipex_llm/libs/quantize-llama_vnni.exe,sha256=wLK9epUBzXoN-_Uu6LR6Q5wdO1DrCowNnEDAgJnQcu8,110080
+ipex_llm/libs/quantize-starcoder.exe,sha256=CR55KQWeCBM0M7uVci6MIYV5lzLnWtM03mppF2dvHKs,126976
+ipex_llm/libs/quantize-starcoder_vnni.exe,sha256=TwwZPllt_-X9JYkxxL5sW2SKieD9gmWKWesW5a4SFdo,128512
+ipex_llm/libs/starcoder-api.dll,sha256=XPKheTwWW_Cs2wkDrTjgLg-ACIXkAf1dSKKLps35a0k,21504
+ipex_llm/libs/starcoder.dll,sha256=41Bo5B08nOkVupzoW0cmanOo88j5vlP95qhOHTskt-E,564224
 ipex_llm/llamaindex/__init__.py,sha256=T-EbRT6GJ_8RCu-iLmSzcftOimXSPQf2d5X72AUAy2Y,874
 ipex_llm/llamaindex/llms/__init__.py,sha256=KP1lEdGqDuxPoxL1ZSH25Pm2kKMPJBWUTLR0ckSLMIU,1139
 ipex_llm/llamaindex/llms/bigdlllm.py,sha256=FQBzq1KOjfc6uofTXAha3O7TqpJkNfOFepXQmOVlbnI,26314
 ipex_llm/serving/__init__.py,sha256=b2IXvVqQ5cItki021h8s3ymW12RPu8QNPprq4Mn3bDM,586
 ipex_llm/serving/fastchat/__init__.py,sha256=b2IXvVqQ5cItki021h8s3ymW12RPu8QNPprq4Mn3bDM,586
 ipex_llm/serving/fastchat/bigdl_llm_model.py,sha256=NXEN_3EPmcP3dDnvug4MokEXXE2zVUnENgBYxfubqic,10084
 ipex_llm/serving/fastchat/ipex_llm_worker.py,sha256=-nDeJIrGneosxjidzcQBMMkByLsRAM8kV70F5v8Kl10,19605
@@ -181,15 +181,15 @@
 ipex_llm/vllm/cpu/entrypoints/openai/api_server.py,sha256=NIeHHB8IcqmyA83sZEdKPhVM3vpJBupFuTFOuW2nj-Q,6944
 ipex_llm/vllm/xpu/__init__.py,sha256=zBSG6nzrVF5QnpR6_f7kPhBFeowTE9gaZ7D5m98E7_w,585
 ipex_llm/vllm/xpu/ipex_llm_gpu_executor.py,sha256=3lfClSuMWg6tfDmi_kCAI9zmc9_N5DINL-ZS6UHs0N0,18506
 ipex_llm/vllm/xpu/model_convert.py,sha256=lriPO5Ife5lMU6q5US4N6l9Y-iQmZa1fNGFPLXoVTuM,7172
 ipex_llm/vllm/xpu/engine/__init__.py,sha256=mzPVAyZdbvfzBQi-wxZh1sbme_NElPMmtrJ9C2zh8Us,747
 ipex_llm/vllm/xpu/engine/engine.py,sha256=6cRzT1UUoqbcaeLh-PigsRv881QavHIWUvHlB5miy3A,5953
 ipex_llm/vllm/xpu/entrypoints/openai/api_server.py,sha256=uIujXmuoKAcOcx5dz8DhnXpqpIlCgPz-4k-SfYKSvS0,10568
-ipex_llm-2.1.0b20240601.data/scripts/ipex-llm-init.bat,sha256=HPtCYuDYwEatq7dAwOvdfVcHYCpAVdbj75K1qh0vQek,2578
-ipex_llm-2.1.0b20240601.data/scripts/llm-chat.ps1,sha256=6qrs-hGVAV8IKh7Jx8nq_XrnZcjd7qGU5wndArM7Yag,2769
-ipex_llm-2.1.0b20240601.data/scripts/llm-cli.ps1,sha256=3qBtTLs_EjYDnM8YyCpJhzLnGCKTEGssu9UNqfkjVXs,3009
-ipex_llm-2.1.0b20240601.dist-info/METADATA,sha256=qCI2dKv6CZRTQxHkipxcGU5yDsQTojlx9RSpjx2s3IQ,5495
-ipex_llm-2.1.0b20240601.dist-info/WHEEL,sha256=bC8mYJUOJCh5KnyEeT6W_BCQYi3v39D3z64Vy_sFvVg,98
-ipex_llm-2.1.0b20240601.dist-info/entry_points.txt,sha256=TiUyBB2MRmfF3ko-pyAEzqeBCRnyhu27bNOAsWPp3e8,61
-ipex_llm-2.1.0b20240601.dist-info/top_level.txt,sha256=CGCMHM-SyqUabU4h8RqJ2KTYckQUO3LvIWwmUQ6Qbzw,9
-ipex_llm-2.1.0b20240601.dist-info/RECORD,,
+ipex_llm-2.1.0b20240602.data/scripts/ipex-llm-init.bat,sha256=HPtCYuDYwEatq7dAwOvdfVcHYCpAVdbj75K1qh0vQek,2578
+ipex_llm-2.1.0b20240602.data/scripts/llm-chat.ps1,sha256=6qrs-hGVAV8IKh7Jx8nq_XrnZcjd7qGU5wndArM7Yag,2769
+ipex_llm-2.1.0b20240602.data/scripts/llm-cli.ps1,sha256=3qBtTLs_EjYDnM8YyCpJhzLnGCKTEGssu9UNqfkjVXs,3009
+ipex_llm-2.1.0b20240602.dist-info/METADATA,sha256=-nMJ3ps7WTwNHFdZWS3sh3f536C-f-nUsYkST1d35Oo,5495
+ipex_llm-2.1.0b20240602.dist-info/WHEEL,sha256=bC8mYJUOJCh5KnyEeT6W_BCQYi3v39D3z64Vy_sFvVg,98
+ipex_llm-2.1.0b20240602.dist-info/entry_points.txt,sha256=TiUyBB2MRmfF3ko-pyAEzqeBCRnyhu27bNOAsWPp3e8,61
+ipex_llm-2.1.0b20240602.dist-info/top_level.txt,sha256=CGCMHM-SyqUabU4h8RqJ2KTYckQUO3LvIWwmUQ6Qbzw,9
+ipex_llm-2.1.0b20240602.dist-info/RECORD,,
```

