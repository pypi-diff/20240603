# Comparing `tmp/hezar-0.38.2.tar.gz` & `tmp/hezar-0.38.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hezar-0.38.2.tar", max compression
+gzip compressed data, was "hezar-0.38.3.tar", max compression
```

## Comparing `hezar-0.38.2.tar` & `hezar-0.38.3.tar`

### file list

```diff
@@ -1,137 +1,137 @@
--rw-r--r--   0        0        0    11337 2024-06-02 17:24:09.995188 hezar-0.38.2/LICENSE
--rw-r--r--   0        0        0    14442 2024-06-02 17:24:09.995188 hezar-0.38.2/README.md
--rw-r--r--   0        0        0      623 2024-06-02 17:24:09.999188 hezar-0.38.2/hezar/__init__.py
--rw-r--r--   0        0        0     5651 2024-06-02 17:24:09.999188 hezar-0.38.2/hezar/builders.py
--rw-r--r--   0        0        0    18631 2024-06-02 17:24:09.999188 hezar-0.38.2/hezar/configs.py
--rw-r--r--   0        0        0     4752 2024-06-02 17:24:09.999188 hezar-0.38.2/hezar/constants.py
--rw-r--r--   0        0        0       83 2024-06-02 17:24:09.999188 hezar-0.38.2/hezar/data/__init__.py
--rw-r--r--   0        0        0    13756 2024-06-02 17:24:09.999188 hezar-0.38.2/hezar/data/data_collators.py
--rw-r--r--   0        0        0     2057 2024-06-02 17:24:09.999188 hezar-0.38.2/hezar/data/data_samplers.py
--rw-r--r--   0        0        0      634 2024-06-02 17:24:09.999188 hezar-0.38.2/hezar/data/datasets/__init__.py
--rw-r--r--   0        0        0     3760 2024-06-02 17:24:09.999188 hezar-0.38.2/hezar/data/datasets/dataset.py
--rw-r--r--   0        0        0     3727 2024-06-02 17:24:09.999188 hezar-0.38.2/hezar/data/datasets/image_captioning_dataset.py
--rw-r--r--   0        0        0     7384 2024-06-02 17:24:09.999188 hezar-0.38.2/hezar/data/datasets/ocr_dataset.py
--rw-r--r--   0        0        0     5923 2024-06-02 17:24:09.999188 hezar-0.38.2/hezar/data/datasets/sequence_labeling_dataset.py
--rw-r--r--   0        0        0     3079 2024-06-02 17:24:09.999188 hezar-0.38.2/hezar/data/datasets/speech_recognition_dataset.py
--rw-r--r--   0        0        0     4498 2024-06-02 17:24:09.999188 hezar-0.38.2/hezar/data/datasets/text_classification_dataset.py
--rw-r--r--   0        0        0     4820 2024-06-02 17:24:09.999188 hezar-0.38.2/hezar/data/datasets/text_summarization_dataset.py
--rw-r--r--   0        0        0      202 2024-06-02 17:24:09.999188 hezar-0.38.2/hezar/embeddings/__init__.py
--rw-r--r--   0        0        0    11544 2024-06-02 17:24:09.999188 hezar-0.38.2/hezar/embeddings/embedding.py
--rw-r--r--   0        0        0     7171 2024-06-02 17:24:09.999188 hezar-0.38.2/hezar/embeddings/fasttext.py
--rw-r--r--   0        0        0     7668 2024-06-02 17:24:09.999188 hezar-0.38.2/hezar/embeddings/word2vec.py
--rw-r--r--   0        0        0      444 2024-06-02 17:24:09.999188 hezar-0.38.2/hezar/metrics/__init__.py
--rw-r--r--   0        0        0     2285 2024-06-02 17:24:09.999188 hezar-0.38.2/hezar/metrics/accuracy.py
--rw-r--r--   0        0        0     2484 2024-06-02 17:24:09.999188 hezar-0.38.2/hezar/metrics/bleu.py
--rw-r--r--   0        0        0     3711 2024-06-02 17:24:09.999188 hezar-0.38.2/hezar/metrics/cer.py
--rw-r--r--   0        0        0     3209 2024-06-02 17:24:09.999188 hezar-0.38.2/hezar/metrics/f1.py
--rw-r--r--   0        0        0     1302 2024-06-02 17:24:09.999188 hezar-0.38.2/hezar/metrics/metric.py
--rw-r--r--   0        0        0     3566 2024-06-02 17:24:09.999188 hezar-0.38.2/hezar/metrics/precision.py
--rw-r--r--   0        0        0     3509 2024-06-02 17:24:09.999188 hezar-0.38.2/hezar/metrics/recall.py
--rw-r--r--   0        0        0     3155 2024-06-02 17:24:09.999188 hezar-0.38.2/hezar/metrics/rouge.py
--rw-r--r--   0        0        0     4029 2024-06-02 17:24:09.999188 hezar-0.38.2/hezar/metrics/seqeval.py
--rw-r--r--   0        0        0     2950 2024-06-02 17:24:09.999188 hezar-0.38.2/hezar/metrics/wer.py
--rw-r--r--   0        0        0      362 2024-06-02 17:24:09.999188 hezar-0.38.2/hezar/models/__init__.py
--rw-r--r--   0        0        0       88 2024-06-02 17:24:09.999188 hezar-0.38.2/hezar/models/backbone/__init__.py
--rw-r--r--   0        0        0       35 2024-06-02 17:24:09.999188 hezar-0.38.2/hezar/models/backbone/bert/__init__.py
--rw-r--r--   0        0        0     2787 2024-06-02 17:24:09.999188 hezar-0.38.2/hezar/models/backbone/bert/bert.py
--rw-r--r--   0        0        0      743 2024-06-02 17:24:09.999188 hezar-0.38.2/hezar/models/backbone/bert/bert_config.py
--rw-r--r--   0        0        0       53 2024-06-02 17:24:09.999188 hezar-0.38.2/hezar/models/backbone/distilbert/__init__.py
--rw-r--r--   0        0        0     2288 2024-06-02 17:24:09.999188 hezar-0.38.2/hezar/models/backbone/distilbert/distilbert.py
--rw-r--r--   0        0        0      618 2024-06-02 17:24:10.003188 hezar-0.38.2/hezar/models/backbone/distilbert/distilbert_config.py
--rw-r--r--   0        0        0       44 2024-06-02 17:24:10.003188 hezar-0.38.2/hezar/models/backbone/roberta/__init__.py
--rw-r--r--   0        0        0     2788 2024-06-02 17:24:10.003188 hezar-0.38.2/hezar/models/backbone/roberta/roberta.py
--rw-r--r--   0        0        0      812 2024-06-02 17:24:10.003188 hezar-0.38.2/hezar/models/backbone/roberta/roberta_config.py
--rw-r--r--   0        0        0       55 2024-06-02 17:24:10.003188 hezar-0.38.2/hezar/models/backbone/vit/__init__.py
--rw-r--r--   0        0        0     2172 2024-06-02 17:24:10.003188 hezar-0.38.2/hezar/models/backbone/vit/vit.py
--rw-r--r--   0        0        0      572 2024-06-02 17:24:10.003188 hezar-0.38.2/hezar/models/backbone/vit/vit_config.py
--rw-r--r--   0        0        0      120 2024-06-02 17:24:10.003188 hezar-0.38.2/hezar/models/image2text/__init__.py
--rw-r--r--   0        0        0      131 2024-06-02 17:24:10.003188 hezar-0.38.2/hezar/models/image2text/beit_roberta/__init__.py
--rw-r--r--   0        0        0     3493 2024-06-02 17:24:10.003188 hezar-0.38.2/hezar/models/image2text/beit_roberta/beit_roberta_image2text.py
--rw-r--r--   0        0        0     2376 2024-06-02 17:24:10.003188 hezar-0.38.2/hezar/models/image2text/beit_roberta/beit_roberta_image2text_config.py
--rw-r--r--   0        0        0      101 2024-06-02 17:24:10.003188 hezar-0.38.2/hezar/models/image2text/crnn/__init__.py
--rw-r--r--   0        0        0     1106 2024-06-02 17:24:10.003188 hezar-0.38.2/hezar/models/image2text/crnn/crnn_decode_utils.py
--rw-r--r--   0        0        0     4649 2024-06-02 17:24:10.003188 hezar-0.38.2/hezar/models/image2text/crnn/crnn_image2text.py
--rw-r--r--   0        0        0      478 2024-06-02 17:24:10.003188 hezar-0.38.2/hezar/models/image2text/crnn/crnn_image2text_config.py
--rw-r--r--   0        0        0      105 2024-06-02 17:24:10.003188 hezar-0.38.2/hezar/models/image2text/trocr/__init__.py
--rw-r--r--   0        0        0     3430 2024-06-02 17:24:10.003188 hezar-0.38.2/hezar/models/image2text/trocr/trocr_image2text.py
--rw-r--r--   0        0        0     1899 2024-06-02 17:24:10.003188 hezar-0.38.2/hezar/models/image2text/trocr/trocr_image2text_config.py
--rw-r--r--   0        0        0      115 2024-06-02 17:24:10.003188 hezar-0.38.2/hezar/models/image2text/vit_gpt2/__init__.py
--rw-r--r--   0        0        0     3463 2024-06-02 17:24:10.003188 hezar-0.38.2/hezar/models/image2text/vit_gpt2/vit_gpt2_image2text.py
--rw-r--r--   0        0        0     1872 2024-06-02 17:24:10.003188 hezar-0.38.2/hezar/models/image2text/vit_gpt2/vit_gpt2_image2text_config.py
--rw-r--r--   0        0        0      127 2024-06-02 17:24:10.003188 hezar-0.38.2/hezar/models/image2text/vit_roberta/__init__.py
--rw-r--r--   0        0        0     3864 2024-06-02 17:24:10.003188 hezar-0.38.2/hezar/models/image2text/vit_roberta/vit_roberta_image2text.py
--rw-r--r--   0        0        0     1952 2024-06-02 17:24:10.003188 hezar-0.38.2/hezar/models/image2text/vit_roberta/vit_roberta_image2text_config.py
--rw-r--r--   0        0        0       69 2024-06-02 17:24:10.003188 hezar-0.38.2/hezar/models/mask_filling/__init__.py
--rw-r--r--   0        0        0      107 2024-06-02 17:24:10.003188 hezar-0.38.2/hezar/models/mask_filling/bert/__init__.py
--rw-r--r--   0        0        0     4320 2024-06-02 17:24:10.003188 hezar-0.38.2/hezar/models/mask_filling/bert/bert_mask_filling.py
--rw-r--r--   0        0        0      771 2024-06-02 17:24:10.003188 hezar-0.38.2/hezar/models/mask_filling/bert/bert_mask_filling_config.py
--rw-r--r--   0        0        0      131 2024-06-02 17:24:10.003188 hezar-0.38.2/hezar/models/mask_filling/distilbert/__init__.py
--rw-r--r--   0        0        0     3921 2024-06-02 17:24:10.003188 hezar-0.38.2/hezar/models/mask_filling/distilbert/distilbert_mask_filling.py
--rw-r--r--   0        0        0      637 2024-06-02 17:24:10.003188 hezar-0.38.2/hezar/models/mask_filling/distilbert/distilbert_mask_filling_config.py
--rw-r--r--   0        0        0      119 2024-06-02 17:24:10.003188 hezar-0.38.2/hezar/models/mask_filling/roberta/__init__.py
--rw-r--r--   0        0        0     4384 2024-06-02 17:24:10.003188 hezar-0.38.2/hezar/models/mask_filling/roberta/roberta_mask_filling.py
--rw-r--r--   0        0        0      831 2024-06-02 17:24:10.003188 hezar-0.38.2/hezar/models/mask_filling/roberta/roberta_mask_filling_config.py
--rw-r--r--   0        0        0    20471 2024-06-02 17:24:10.003188 hezar-0.38.2/hezar/models/model.py
--rw-r--r--   0        0        0     2346 2024-06-02 17:24:10.003188 hezar-0.38.2/hezar/models/model_outputs.py
--rw-r--r--   0        0        0       69 2024-06-02 17:24:10.003188 hezar-0.38.2/hezar/models/sequence_labeling/__init__.py
--rw-r--r--   0        0        0      127 2024-06-02 17:24:10.003188 hezar-0.38.2/hezar/models/sequence_labeling/bert/__init__.py
--rw-r--r--   0        0        0     5118 2024-06-02 17:24:10.003188 hezar-0.38.2/hezar/models/sequence_labeling/bert/bert_sequence_labeling.py
--rw-r--r--   0        0        0      931 2024-06-02 17:24:10.003188 hezar-0.38.2/hezar/models/sequence_labeling/bert/bert_sequence_labeling_config.py
--rw-r--r--   0        0        0      151 2024-06-02 17:24:10.003188 hezar-0.38.2/hezar/models/sequence_labeling/distilbert/__init__.py
--rw-r--r--   0        0        0     5172 2024-06-02 17:24:10.003188 hezar-0.38.2/hezar/models/sequence_labeling/distilbert/distilbert_sequence_labeling.py
--rw-r--r--   0        0        0      872 2024-06-02 17:24:10.003188 hezar-0.38.2/hezar/models/sequence_labeling/distilbert/distilbert_sequence_labeling_config.py
--rw-r--r--   0        0        0      139 2024-06-02 17:24:10.003188 hezar-0.38.2/hezar/models/sequence_labeling/roberta/__init__.py
--rw-r--r--   0        0        0     5821 2024-06-02 17:24:10.003188 hezar-0.38.2/hezar/models/sequence_labeling/roberta/roberta_sequence_labeling.py
--rw-r--r--   0        0        0     1025 2024-06-02 17:24:10.003188 hezar-0.38.2/hezar/models/sequence_labeling/roberta/roberta_sequence_labeling_config.py
--rw-r--r--   0        0        0       23 2024-06-02 17:24:10.003188 hezar-0.38.2/hezar/models/speech_recognition/__init__.py
--rw-r--r--   0        0        0      306 2024-06-02 17:24:10.003188 hezar-0.38.2/hezar/models/speech_recognition/whisper/__init__.py
--rw-r--r--   0        0        0     7713 2024-06-02 17:24:10.003188 hezar-0.38.2/hezar/models/speech_recognition/whisper/whisper_feature_extractor.py
--rw-r--r--   0        0        0     7067 2024-06-02 17:24:10.003188 hezar-0.38.2/hezar/models/speech_recognition/whisper/whisper_speech_recognition.py
--rw-r--r--   0        0        0     2821 2024-06-02 17:24:10.003188 hezar-0.38.2/hezar/models/speech_recognition/whisper/whisper_speech_recognition_config.py
--rw-r--r--   0        0        0    27594 2024-06-02 17:24:10.003188 hezar-0.38.2/hezar/models/speech_recognition/whisper/whisper_tokenizer.py
--rw-r--r--   0        0        0       69 2024-06-02 17:24:10.003188 hezar-0.38.2/hezar/models/text_classification/__init__.py
--rw-r--r--   0        0        0      135 2024-06-02 17:24:10.003188 hezar-0.38.2/hezar/models/text_classification/bert/__init__.py
--rw-r--r--   0        0        0     4796 2024-06-02 17:24:10.003188 hezar-0.38.2/hezar/models/text_classification/bert/bert_text_classification.py
--rw-r--r--   0        0        0      845 2024-06-02 17:24:10.003188 hezar-0.38.2/hezar/models/text_classification/bert/bert_text_classification_config.py
--rw-r--r--   0        0        0      159 2024-06-02 17:24:10.003188 hezar-0.38.2/hezar/models/text_classification/distilbert/__init__.py
--rw-r--r--   0        0        0     4357 2024-06-02 17:24:10.003188 hezar-0.38.2/hezar/models/text_classification/distilbert/distilbert_text_classification.py
--rw-r--r--   0        0        0      748 2024-06-02 17:24:10.003188 hezar-0.38.2/hezar/models/text_classification/distilbert/distilbert_text_classification_config.py
--rw-r--r--   0        0        0      147 2024-06-02 17:24:10.003188 hezar-0.38.2/hezar/models/text_classification/roberta/__init__.py
--rw-r--r--   0        0        0     4963 2024-06-02 17:24:10.003188 hezar-0.38.2/hezar/models/text_classification/roberta/roberta_text_classification.py
--rw-r--r--   0        0        0      942 2024-06-02 17:24:10.003188 hezar-0.38.2/hezar/models/text_classification/roberta/roberta_text_classification_config.py
--rw-r--r--   0        0        0        0 2024-06-02 17:24:10.003188 hezar-0.38.2/hezar/models/text_embedding/__init__.py
--rw-r--r--   0        0        0       38 2024-06-02 17:24:10.003188 hezar-0.38.2/hezar/models/text_generation/__init__.py
--rw-r--r--   0        0        0      119 2024-06-02 17:24:10.003188 hezar-0.38.2/hezar/models/text_generation/gpt2/__init__.py
--rw-r--r--   0        0        0     3324 2024-06-02 17:24:10.003188 hezar-0.38.2/hezar/models/text_generation/gpt2/gpt2_text_generation.py
--rw-r--r--   0        0        0     1148 2024-06-02 17:24:10.003188 hezar-0.38.2/hezar/models/text_generation/gpt2/gpt2_text_generation_config.py
--rw-r--r--   0        0        0      111 2024-06-02 17:24:10.003188 hezar-0.38.2/hezar/models/text_generation/t5/__init__.py
--rw-r--r--   0        0        0     4053 2024-06-02 17:24:10.003188 hezar-0.38.2/hezar/models/text_generation/t5/t5_text_generation.py
--rw-r--r--   0        0        0      837 2024-06-02 17:24:10.003188 hezar-0.38.2/hezar/models/text_generation/t5/t5_text_generation_config.py
--rw-r--r--   0        0        0      390 2024-06-02 17:24:10.003188 hezar-0.38.2/hezar/preprocessors/__init__.py
--rw-r--r--   0        0        0    13303 2024-06-02 17:24:10.003188 hezar-0.38.2/hezar/preprocessors/audio_feature_extractor.py
--rw-r--r--   0        0        0     8292 2024-06-02 17:24:10.003188 hezar-0.38.2/hezar/preprocessors/image_processor.py
--rw-r--r--   0        0        0     5043 2024-06-02 17:24:10.003188 hezar-0.38.2/hezar/preprocessors/preprocessor.py
--rw-r--r--   0        0        0     4635 2024-06-02 17:24:10.003188 hezar-0.38.2/hezar/preprocessors/text_normalizer.py
--rw-r--r--   0        0        0      337 2024-06-02 17:24:10.003188 hezar-0.38.2/hezar/preprocessors/tokenizers/__init__.py
--rw-r--r--   0        0        0     3973 2024-06-02 17:24:10.003188 hezar-0.38.2/hezar/preprocessors/tokenizers/bpe.py
--rw-r--r--   0        0        0     4181 2024-06-02 17:24:10.003188 hezar-0.38.2/hezar/preprocessors/tokenizers/sentencepiece_bpe.py
--rw-r--r--   0        0        0     4102 2024-06-02 17:24:10.007188 hezar-0.38.2/hezar/preprocessors/tokenizers/sentencepiece_unigram.py
--rw-r--r--   0        0        0    27637 2024-06-02 17:24:10.007188 hezar-0.38.2/hezar/preprocessors/tokenizers/tokenizer.py
--rw-r--r--   0        0        0     3537 2024-06-02 17:24:10.007188 hezar-0.38.2/hezar/preprocessors/tokenizers/wordpiece.py
--rw-r--r--   0        0        0     6584 2024-06-02 17:24:10.007188 hezar-0.38.2/hezar/registry.py
--rw-r--r--   0        0        0      113 2024-06-02 17:24:10.007188 hezar-0.38.2/hezar/trainer/__init__.py
--rw-r--r--   0        0        0     7345 2024-06-02 17:24:10.007188 hezar-0.38.2/hezar/trainer/metrics_handlers.py
--rw-r--r--   0        0        0    33116 2024-06-02 17:24:10.007188 hezar-0.38.2/hezar/trainer/trainer.py
--rw-r--r--   0        0        0     5624 2024-06-02 17:24:10.007188 hezar-0.38.2/hezar/trainer/trainer_utils.py
--rw-r--r--   0        0        0      245 2024-06-02 17:24:10.007188 hezar-0.38.2/hezar/utils/__init__.py
--rw-r--r--   0        0        0    23979 2024-06-02 17:24:10.007188 hezar-0.38.2/hezar/utils/audio_utils.py
--rw-r--r--   0        0        0     3955 2024-06-02 17:24:10.007188 hezar-0.38.2/hezar/utils/common_utils.py
--rw-r--r--   0        0        0     8240 2024-06-02 17:24:10.007188 hezar-0.38.2/hezar/utils/data_utils.py
--rw-r--r--   0        0        0      976 2024-06-02 17:24:10.007188 hezar-0.38.2/hezar/utils/file_utils.py
--rw-r--r--   0        0        0     4145 2024-06-02 17:24:10.007188 hezar-0.38.2/hezar/utils/hub_utils.py
--rw-r--r--   0        0        0     7352 2024-06-02 17:24:10.007188 hezar-0.38.2/hezar/utils/image_utils.py
--rw-r--r--   0        0        0     1376 2024-06-02 17:24:10.007188 hezar-0.38.2/hezar/utils/integration_utils.py
--rw-r--r--   0        0        0      622 2024-06-02 17:24:10.007188 hezar-0.38.2/hezar/utils/logging.py
--rw-r--r--   0        0        0     4498 2024-06-02 17:24:10.007188 hezar-0.38.2/hezar/utils/registry_utils.py
--rw-r--r--   0        0        0     2602 2024-06-02 17:24:10.007188 hezar-0.38.2/pyproject.toml
--rw-r--r--   0        0        0    17052 1970-01-01 00:00:00.000000 hezar-0.38.2/PKG-INFO
+-rw-r--r--   0        0        0    11337 2024-06-03 07:29:57.459390 hezar-0.38.3/LICENSE
+-rw-r--r--   0        0        0    14442 2024-06-03 07:29:57.459390 hezar-0.38.3/README.md
+-rw-r--r--   0        0        0      623 2024-06-03 07:29:57.463390 hezar-0.38.3/hezar/__init__.py
+-rw-r--r--   0        0        0     5651 2024-06-03 07:29:57.463390 hezar-0.38.3/hezar/builders.py
+-rw-r--r--   0        0        0    18631 2024-06-03 07:29:57.463390 hezar-0.38.3/hezar/configs.py
+-rw-r--r--   0        0        0     4752 2024-06-03 07:29:57.463390 hezar-0.38.3/hezar/constants.py
+-rw-r--r--   0        0        0       83 2024-06-03 07:29:57.463390 hezar-0.38.3/hezar/data/__init__.py
+-rw-r--r--   0        0        0    13756 2024-06-03 07:29:57.463390 hezar-0.38.3/hezar/data/data_collators.py
+-rw-r--r--   0        0        0     2057 2024-06-03 07:29:57.463390 hezar-0.38.3/hezar/data/data_samplers.py
+-rw-r--r--   0        0        0      634 2024-06-03 07:29:57.463390 hezar-0.38.3/hezar/data/datasets/__init__.py
+-rw-r--r--   0        0        0     3760 2024-06-03 07:29:57.463390 hezar-0.38.3/hezar/data/datasets/dataset.py
+-rw-r--r--   0        0        0     3727 2024-06-03 07:29:57.463390 hezar-0.38.3/hezar/data/datasets/image_captioning_dataset.py
+-rw-r--r--   0        0        0     7384 2024-06-03 07:29:57.463390 hezar-0.38.3/hezar/data/datasets/ocr_dataset.py
+-rw-r--r--   0        0        0     5923 2024-06-03 07:29:57.463390 hezar-0.38.3/hezar/data/datasets/sequence_labeling_dataset.py
+-rw-r--r--   0        0        0     3079 2024-06-03 07:29:57.463390 hezar-0.38.3/hezar/data/datasets/speech_recognition_dataset.py
+-rw-r--r--   0        0        0     4498 2024-06-03 07:29:57.463390 hezar-0.38.3/hezar/data/datasets/text_classification_dataset.py
+-rw-r--r--   0        0        0     4820 2024-06-03 07:29:57.463390 hezar-0.38.3/hezar/data/datasets/text_summarization_dataset.py
+-rw-r--r--   0        0        0      202 2024-06-03 07:29:57.463390 hezar-0.38.3/hezar/embeddings/__init__.py
+-rw-r--r--   0        0        0    11544 2024-06-03 07:29:57.463390 hezar-0.38.3/hezar/embeddings/embedding.py
+-rw-r--r--   0        0        0     7171 2024-06-03 07:29:57.463390 hezar-0.38.3/hezar/embeddings/fasttext.py
+-rw-r--r--   0        0        0     7668 2024-06-03 07:29:57.463390 hezar-0.38.3/hezar/embeddings/word2vec.py
+-rw-r--r--   0        0        0      444 2024-06-03 07:29:57.463390 hezar-0.38.3/hezar/metrics/__init__.py
+-rw-r--r--   0        0        0     2285 2024-06-03 07:29:57.467390 hezar-0.38.3/hezar/metrics/accuracy.py
+-rw-r--r--   0        0        0     2484 2024-06-03 07:29:57.467390 hezar-0.38.3/hezar/metrics/bleu.py
+-rw-r--r--   0        0        0     3711 2024-06-03 07:29:57.467390 hezar-0.38.3/hezar/metrics/cer.py
+-rw-r--r--   0        0        0     3209 2024-06-03 07:29:57.467390 hezar-0.38.3/hezar/metrics/f1.py
+-rw-r--r--   0        0        0     1302 2024-06-03 07:29:57.467390 hezar-0.38.3/hezar/metrics/metric.py
+-rw-r--r--   0        0        0     3566 2024-06-03 07:29:57.467390 hezar-0.38.3/hezar/metrics/precision.py
+-rw-r--r--   0        0        0     3509 2024-06-03 07:29:57.467390 hezar-0.38.3/hezar/metrics/recall.py
+-rw-r--r--   0        0        0     3155 2024-06-03 07:29:57.467390 hezar-0.38.3/hezar/metrics/rouge.py
+-rw-r--r--   0        0        0     4029 2024-06-03 07:29:57.467390 hezar-0.38.3/hezar/metrics/seqeval.py
+-rw-r--r--   0        0        0     2950 2024-06-03 07:29:57.467390 hezar-0.38.3/hezar/metrics/wer.py
+-rw-r--r--   0        0        0      362 2024-06-03 07:29:57.467390 hezar-0.38.3/hezar/models/__init__.py
+-rw-r--r--   0        0        0       88 2024-06-03 07:29:57.467390 hezar-0.38.3/hezar/models/backbone/__init__.py
+-rw-r--r--   0        0        0       35 2024-06-03 07:29:57.467390 hezar-0.38.3/hezar/models/backbone/bert/__init__.py
+-rw-r--r--   0        0        0     2787 2024-06-03 07:29:57.467390 hezar-0.38.3/hezar/models/backbone/bert/bert.py
+-rw-r--r--   0        0        0      743 2024-06-03 07:29:57.467390 hezar-0.38.3/hezar/models/backbone/bert/bert_config.py
+-rw-r--r--   0        0        0       53 2024-06-03 07:29:57.467390 hezar-0.38.3/hezar/models/backbone/distilbert/__init__.py
+-rw-r--r--   0        0        0     2288 2024-06-03 07:29:57.467390 hezar-0.38.3/hezar/models/backbone/distilbert/distilbert.py
+-rw-r--r--   0        0        0      618 2024-06-03 07:29:57.467390 hezar-0.38.3/hezar/models/backbone/distilbert/distilbert_config.py
+-rw-r--r--   0        0        0       44 2024-06-03 07:29:57.467390 hezar-0.38.3/hezar/models/backbone/roberta/__init__.py
+-rw-r--r--   0        0        0     2788 2024-06-03 07:29:57.467390 hezar-0.38.3/hezar/models/backbone/roberta/roberta.py
+-rw-r--r--   0        0        0      812 2024-06-03 07:29:57.467390 hezar-0.38.3/hezar/models/backbone/roberta/roberta_config.py
+-rw-r--r--   0        0        0       55 2024-06-03 07:29:57.467390 hezar-0.38.3/hezar/models/backbone/vit/__init__.py
+-rw-r--r--   0        0        0     2172 2024-06-03 07:29:57.467390 hezar-0.38.3/hezar/models/backbone/vit/vit.py
+-rw-r--r--   0        0        0      572 2024-06-03 07:29:57.467390 hezar-0.38.3/hezar/models/backbone/vit/vit_config.py
+-rw-r--r--   0        0        0      120 2024-06-03 07:29:57.467390 hezar-0.38.3/hezar/models/image2text/__init__.py
+-rw-r--r--   0        0        0      131 2024-06-03 07:29:57.467390 hezar-0.38.3/hezar/models/image2text/beit_roberta/__init__.py
+-rw-r--r--   0        0        0     3493 2024-06-03 07:29:57.467390 hezar-0.38.3/hezar/models/image2text/beit_roberta/beit_roberta_image2text.py
+-rw-r--r--   0        0        0     2376 2024-06-03 07:29:57.467390 hezar-0.38.3/hezar/models/image2text/beit_roberta/beit_roberta_image2text_config.py
+-rw-r--r--   0        0        0      101 2024-06-03 07:29:57.467390 hezar-0.38.3/hezar/models/image2text/crnn/__init__.py
+-rw-r--r--   0        0        0     1106 2024-06-03 07:29:57.467390 hezar-0.38.3/hezar/models/image2text/crnn/crnn_decode_utils.py
+-rw-r--r--   0        0        0     4649 2024-06-03 07:29:57.467390 hezar-0.38.3/hezar/models/image2text/crnn/crnn_image2text.py
+-rw-r--r--   0        0        0      478 2024-06-03 07:29:57.467390 hezar-0.38.3/hezar/models/image2text/crnn/crnn_image2text_config.py
+-rw-r--r--   0        0        0      105 2024-06-03 07:29:57.467390 hezar-0.38.3/hezar/models/image2text/trocr/__init__.py
+-rw-r--r--   0        0        0     3430 2024-06-03 07:29:57.467390 hezar-0.38.3/hezar/models/image2text/trocr/trocr_image2text.py
+-rw-r--r--   0        0        0     1899 2024-06-03 07:29:57.467390 hezar-0.38.3/hezar/models/image2text/trocr/trocr_image2text_config.py
+-rw-r--r--   0        0        0      115 2024-06-03 07:29:57.467390 hezar-0.38.3/hezar/models/image2text/vit_gpt2/__init__.py
+-rw-r--r--   0        0        0     3463 2024-06-03 07:29:57.467390 hezar-0.38.3/hezar/models/image2text/vit_gpt2/vit_gpt2_image2text.py
+-rw-r--r--   0        0        0     1872 2024-06-03 07:29:57.467390 hezar-0.38.3/hezar/models/image2text/vit_gpt2/vit_gpt2_image2text_config.py
+-rw-r--r--   0        0        0      127 2024-06-03 07:29:57.467390 hezar-0.38.3/hezar/models/image2text/vit_roberta/__init__.py
+-rw-r--r--   0        0        0     3864 2024-06-03 07:29:57.467390 hezar-0.38.3/hezar/models/image2text/vit_roberta/vit_roberta_image2text.py
+-rw-r--r--   0        0        0     1952 2024-06-03 07:29:57.467390 hezar-0.38.3/hezar/models/image2text/vit_roberta/vit_roberta_image2text_config.py
+-rw-r--r--   0        0        0       69 2024-06-03 07:29:57.467390 hezar-0.38.3/hezar/models/mask_filling/__init__.py
+-rw-r--r--   0        0        0      107 2024-06-03 07:29:57.467390 hezar-0.38.3/hezar/models/mask_filling/bert/__init__.py
+-rw-r--r--   0        0        0     4320 2024-06-03 07:29:57.467390 hezar-0.38.3/hezar/models/mask_filling/bert/bert_mask_filling.py
+-rw-r--r--   0        0        0      771 2024-06-03 07:29:57.467390 hezar-0.38.3/hezar/models/mask_filling/bert/bert_mask_filling_config.py
+-rw-r--r--   0        0        0      131 2024-06-03 07:29:57.467390 hezar-0.38.3/hezar/models/mask_filling/distilbert/__init__.py
+-rw-r--r--   0        0        0     3921 2024-06-03 07:29:57.467390 hezar-0.38.3/hezar/models/mask_filling/distilbert/distilbert_mask_filling.py
+-rw-r--r--   0        0        0      637 2024-06-03 07:29:57.467390 hezar-0.38.3/hezar/models/mask_filling/distilbert/distilbert_mask_filling_config.py
+-rw-r--r--   0        0        0      119 2024-06-03 07:29:57.467390 hezar-0.38.3/hezar/models/mask_filling/roberta/__init__.py
+-rw-r--r--   0        0        0     4384 2024-06-03 07:29:57.467390 hezar-0.38.3/hezar/models/mask_filling/roberta/roberta_mask_filling.py
+-rw-r--r--   0        0        0      831 2024-06-03 07:29:57.467390 hezar-0.38.3/hezar/models/mask_filling/roberta/roberta_mask_filling_config.py
+-rw-r--r--   0        0        0    20471 2024-06-03 07:29:57.467390 hezar-0.38.3/hezar/models/model.py
+-rw-r--r--   0        0        0     2346 2024-06-03 07:29:57.467390 hezar-0.38.3/hezar/models/model_outputs.py
+-rw-r--r--   0        0        0       69 2024-06-03 07:29:57.467390 hezar-0.38.3/hezar/models/sequence_labeling/__init__.py
+-rw-r--r--   0        0        0      127 2024-06-03 07:29:57.467390 hezar-0.38.3/hezar/models/sequence_labeling/bert/__init__.py
+-rw-r--r--   0        0        0     5118 2024-06-03 07:29:57.467390 hezar-0.38.3/hezar/models/sequence_labeling/bert/bert_sequence_labeling.py
+-rw-r--r--   0        0        0      931 2024-06-03 07:29:57.467390 hezar-0.38.3/hezar/models/sequence_labeling/bert/bert_sequence_labeling_config.py
+-rw-r--r--   0        0        0      151 2024-06-03 07:29:57.467390 hezar-0.38.3/hezar/models/sequence_labeling/distilbert/__init__.py
+-rw-r--r--   0        0        0     5172 2024-06-03 07:29:57.467390 hezar-0.38.3/hezar/models/sequence_labeling/distilbert/distilbert_sequence_labeling.py
+-rw-r--r--   0        0        0      872 2024-06-03 07:29:57.467390 hezar-0.38.3/hezar/models/sequence_labeling/distilbert/distilbert_sequence_labeling_config.py
+-rw-r--r--   0        0        0      139 2024-06-03 07:29:57.467390 hezar-0.38.3/hezar/models/sequence_labeling/roberta/__init__.py
+-rw-r--r--   0        0        0     5821 2024-06-03 07:29:57.467390 hezar-0.38.3/hezar/models/sequence_labeling/roberta/roberta_sequence_labeling.py
+-rw-r--r--   0        0        0     1025 2024-06-03 07:29:57.467390 hezar-0.38.3/hezar/models/sequence_labeling/roberta/roberta_sequence_labeling_config.py
+-rw-r--r--   0        0        0       23 2024-06-03 07:29:57.467390 hezar-0.38.3/hezar/models/speech_recognition/__init__.py
+-rw-r--r--   0        0        0      306 2024-06-03 07:29:57.467390 hezar-0.38.3/hezar/models/speech_recognition/whisper/__init__.py
+-rw-r--r--   0        0        0     7713 2024-06-03 07:29:57.467390 hezar-0.38.3/hezar/models/speech_recognition/whisper/whisper_feature_extractor.py
+-rw-r--r--   0        0        0     7067 2024-06-03 07:29:57.467390 hezar-0.38.3/hezar/models/speech_recognition/whisper/whisper_speech_recognition.py
+-rw-r--r--   0        0        0     2821 2024-06-03 07:29:57.467390 hezar-0.38.3/hezar/models/speech_recognition/whisper/whisper_speech_recognition_config.py
+-rw-r--r--   0        0        0    27594 2024-06-03 07:29:57.467390 hezar-0.38.3/hezar/models/speech_recognition/whisper/whisper_tokenizer.py
+-rw-r--r--   0        0        0       69 2024-06-03 07:29:57.467390 hezar-0.38.3/hezar/models/text_classification/__init__.py
+-rw-r--r--   0        0        0      135 2024-06-03 07:29:57.467390 hezar-0.38.3/hezar/models/text_classification/bert/__init__.py
+-rw-r--r--   0        0        0     4796 2024-06-03 07:29:57.467390 hezar-0.38.3/hezar/models/text_classification/bert/bert_text_classification.py
+-rw-r--r--   0        0        0      845 2024-06-03 07:29:57.467390 hezar-0.38.3/hezar/models/text_classification/bert/bert_text_classification_config.py
+-rw-r--r--   0        0        0      159 2024-06-03 07:29:57.467390 hezar-0.38.3/hezar/models/text_classification/distilbert/__init__.py
+-rw-r--r--   0        0        0     4357 2024-06-03 07:29:57.467390 hezar-0.38.3/hezar/models/text_classification/distilbert/distilbert_text_classification.py
+-rw-r--r--   0        0        0      748 2024-06-03 07:29:57.467390 hezar-0.38.3/hezar/models/text_classification/distilbert/distilbert_text_classification_config.py
+-rw-r--r--   0        0        0      147 2024-06-03 07:29:57.467390 hezar-0.38.3/hezar/models/text_classification/roberta/__init__.py
+-rw-r--r--   0        0        0     4963 2024-06-03 07:29:57.467390 hezar-0.38.3/hezar/models/text_classification/roberta/roberta_text_classification.py
+-rw-r--r--   0        0        0      942 2024-06-03 07:29:57.471390 hezar-0.38.3/hezar/models/text_classification/roberta/roberta_text_classification_config.py
+-rw-r--r--   0        0        0        0 2024-06-03 07:29:57.471390 hezar-0.38.3/hezar/models/text_embedding/__init__.py
+-rw-r--r--   0        0        0       38 2024-06-03 07:29:57.471390 hezar-0.38.3/hezar/models/text_generation/__init__.py
+-rw-r--r--   0        0        0      119 2024-06-03 07:29:57.471390 hezar-0.38.3/hezar/models/text_generation/gpt2/__init__.py
+-rw-r--r--   0        0        0     3324 2024-06-03 07:29:57.471390 hezar-0.38.3/hezar/models/text_generation/gpt2/gpt2_text_generation.py
+-rw-r--r--   0        0        0     1148 2024-06-03 07:29:57.471390 hezar-0.38.3/hezar/models/text_generation/gpt2/gpt2_text_generation_config.py
+-rw-r--r--   0        0        0      111 2024-06-03 07:29:57.471390 hezar-0.38.3/hezar/models/text_generation/t5/__init__.py
+-rw-r--r--   0        0        0     4053 2024-06-03 07:29:57.471390 hezar-0.38.3/hezar/models/text_generation/t5/t5_text_generation.py
+-rw-r--r--   0        0        0      837 2024-06-03 07:29:57.471390 hezar-0.38.3/hezar/models/text_generation/t5/t5_text_generation_config.py
+-rw-r--r--   0        0        0      390 2024-06-03 07:29:57.471390 hezar-0.38.3/hezar/preprocessors/__init__.py
+-rw-r--r--   0        0        0    13303 2024-06-03 07:29:57.471390 hezar-0.38.3/hezar/preprocessors/audio_feature_extractor.py
+-rw-r--r--   0        0        0     8292 2024-06-03 07:29:57.471390 hezar-0.38.3/hezar/preprocessors/image_processor.py
+-rw-r--r--   0        0        0     5043 2024-06-03 07:29:57.471390 hezar-0.38.3/hezar/preprocessors/preprocessor.py
+-rw-r--r--   0        0        0     4635 2024-06-03 07:29:57.471390 hezar-0.38.3/hezar/preprocessors/text_normalizer.py
+-rw-r--r--   0        0        0      337 2024-06-03 07:29:57.471390 hezar-0.38.3/hezar/preprocessors/tokenizers/__init__.py
+-rw-r--r--   0        0        0     3973 2024-06-03 07:29:57.471390 hezar-0.38.3/hezar/preprocessors/tokenizers/bpe.py
+-rw-r--r--   0        0        0     4181 2024-06-03 07:29:57.471390 hezar-0.38.3/hezar/preprocessors/tokenizers/sentencepiece_bpe.py
+-rw-r--r--   0        0        0     4102 2024-06-03 07:29:57.471390 hezar-0.38.3/hezar/preprocessors/tokenizers/sentencepiece_unigram.py
+-rw-r--r--   0        0        0    27637 2024-06-03 07:29:57.471390 hezar-0.38.3/hezar/preprocessors/tokenizers/tokenizer.py
+-rw-r--r--   0        0        0     3537 2024-06-03 07:29:57.471390 hezar-0.38.3/hezar/preprocessors/tokenizers/wordpiece.py
+-rw-r--r--   0        0        0     6584 2024-06-03 07:29:57.471390 hezar-0.38.3/hezar/registry.py
+-rw-r--r--   0        0        0      113 2024-06-03 07:29:57.471390 hezar-0.38.3/hezar/trainer/__init__.py
+-rw-r--r--   0        0        0     7345 2024-06-03 07:29:57.471390 hezar-0.38.3/hezar/trainer/metrics_handlers.py
+-rw-r--r--   0        0        0    33116 2024-06-03 07:29:57.471390 hezar-0.38.3/hezar/trainer/trainer.py
+-rw-r--r--   0        0        0     5624 2024-06-03 07:29:57.471390 hezar-0.38.3/hezar/trainer/trainer_utils.py
+-rw-r--r--   0        0        0      245 2024-06-03 07:29:57.471390 hezar-0.38.3/hezar/utils/__init__.py
+-rw-r--r--   0        0        0    23979 2024-06-03 07:29:57.471390 hezar-0.38.3/hezar/utils/audio_utils.py
+-rw-r--r--   0        0        0     3955 2024-06-03 07:29:57.471390 hezar-0.38.3/hezar/utils/common_utils.py
+-rw-r--r--   0        0        0     8239 2024-06-03 07:29:57.471390 hezar-0.38.3/hezar/utils/data_utils.py
+-rw-r--r--   0        0        0      976 2024-06-03 07:29:57.471390 hezar-0.38.3/hezar/utils/file_utils.py
+-rw-r--r--   0        0        0     4145 2024-06-03 07:29:57.471390 hezar-0.38.3/hezar/utils/hub_utils.py
+-rw-r--r--   0        0        0     7352 2024-06-03 07:29:57.471390 hezar-0.38.3/hezar/utils/image_utils.py
+-rw-r--r--   0        0        0     1376 2024-06-03 07:29:57.471390 hezar-0.38.3/hezar/utils/integration_utils.py
+-rw-r--r--   0        0        0      622 2024-06-03 07:29:57.471390 hezar-0.38.3/hezar/utils/logging.py
+-rw-r--r--   0        0        0     4498 2024-06-03 07:29:57.471390 hezar-0.38.3/hezar/utils/registry_utils.py
+-rw-r--r--   0        0        0     2602 2024-06-03 07:29:57.471390 hezar-0.38.3/pyproject.toml
+-rw-r--r--   0        0        0    17052 1970-01-01 00:00:00.000000 hezar-0.38.3/PKG-INFO
```

### Comparing `hezar-0.38.2/LICENSE` & `hezar-0.38.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hezar-0.38.2/README.md` & `hezar-0.38.3/README.md`

 * *Files identical despite different names*

### Comparing `hezar-0.38.2/hezar/__init__.py` & `hezar-0.38.3/hezar/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.38.2"
+__version__ = "0.38.3"
```

### Comparing `hezar-0.38.2/hezar/builders.py` & `hezar-0.38.3/hezar/builders.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.2/hezar/configs.py` & `hezar-0.38.3/hezar/configs.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.2/hezar/constants.py` & `hezar-0.38.3/hezar/constants.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.2/hezar/data/data_collators.py` & `hezar-0.38.3/hezar/data/data_collators.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.2/hezar/data/data_samplers.py` & `hezar-0.38.3/hezar/data/data_samplers.py`

 * *Ordering differences only*

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from typing import Sized
 import random
+from typing import Sized
 
 from torch.utils.data import Sampler
 
 from ..utils import set_seed
 
 
 __all__ = [
```

### Comparing `hezar-0.38.2/hezar/data/datasets/__init__.py` & `hezar-0.38.3/hezar/data/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.2/hezar/data/datasets/dataset.py` & `hezar-0.38.3/hezar/data/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.2/hezar/data/datasets/image_captioning_dataset.py` & `hezar-0.38.3/hezar/data/datasets/image_captioning_dataset.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.2/hezar/data/datasets/ocr_dataset.py` & `hezar-0.38.3/hezar/data/datasets/ocr_dataset.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.2/hezar/data/datasets/sequence_labeling_dataset.py` & `hezar-0.38.3/hezar/data/datasets/sequence_labeling_dataset.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.2/hezar/data/datasets/speech_recognition_dataset.py` & `hezar-0.38.3/hezar/data/datasets/speech_recognition_dataset.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.2/hezar/data/datasets/text_classification_dataset.py` & `hezar-0.38.3/hezar/data/datasets/text_classification_dataset.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.2/hezar/data/datasets/text_summarization_dataset.py` & `hezar-0.38.3/hezar/data/datasets/text_summarization_dataset.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.2/hezar/embeddings/embedding.py` & `hezar-0.38.3/hezar/embeddings/embedding.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.2/hezar/embeddings/fasttext.py` & `hezar-0.38.3/hezar/embeddings/fasttext.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.2/hezar/embeddings/word2vec.py` & `hezar-0.38.3/hezar/embeddings/word2vec.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.2/hezar/metrics/accuracy.py` & `hezar-0.38.3/hezar/metrics/accuracy.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.2/hezar/metrics/bleu.py` & `hezar-0.38.3/hezar/metrics/bleu.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.2/hezar/metrics/cer.py` & `hezar-0.38.3/hezar/metrics/cer.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.2/hezar/metrics/f1.py` & `hezar-0.38.3/hezar/metrics/f1.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.2/hezar/metrics/metric.py` & `hezar-0.38.3/hezar/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.2/hezar/metrics/precision.py` & `hezar-0.38.3/hezar/metrics/precision.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.2/hezar/metrics/recall.py` & `hezar-0.38.3/hezar/metrics/recall.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.2/hezar/metrics/rouge.py` & `hezar-0.38.3/hezar/metrics/rouge.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.2/hezar/metrics/seqeval.py` & `hezar-0.38.3/hezar/metrics/seqeval.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.2/hezar/metrics/wer.py` & `hezar-0.38.3/hezar/metrics/wer.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.2/hezar/models/backbone/bert/bert.py` & `hezar-0.38.3/hezar/models/backbone/bert/bert.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.2/hezar/models/backbone/bert/bert_config.py` & `hezar-0.38.3/hezar/models/backbone/bert/bert_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.2/hezar/models/backbone/distilbert/distilbert.py` & `hezar-0.38.3/hezar/models/backbone/distilbert/distilbert.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.2/hezar/models/backbone/distilbert/distilbert_config.py` & `hezar-0.38.3/hezar/models/backbone/distilbert/distilbert_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.2/hezar/models/backbone/roberta/roberta.py` & `hezar-0.38.3/hezar/models/backbone/roberta/roberta.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.2/hezar/models/backbone/roberta/roberta_config.py` & `hezar-0.38.3/hezar/models/backbone/roberta/roberta_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.2/hezar/models/backbone/vit/vit.py` & `hezar-0.38.3/hezar/models/backbone/vit/vit.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.2/hezar/models/backbone/vit/vit_config.py` & `hezar-0.38.3/hezar/models/backbone/vit/vit_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.2/hezar/models/image2text/beit_roberta/beit_roberta_image2text.py` & `hezar-0.38.3/hezar/models/image2text/beit_roberta/beit_roberta_image2text.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.2/hezar/models/image2text/beit_roberta/beit_roberta_image2text_config.py` & `hezar-0.38.3/hezar/models/image2text/beit_roberta/beit_roberta_image2text_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.2/hezar/models/image2text/crnn/crnn_decode_utils.py` & `hezar-0.38.3/hezar/models/image2text/crnn/crnn_decode_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.2/hezar/models/image2text/crnn/crnn_image2text.py` & `hezar-0.38.3/hezar/models/image2text/crnn/crnn_image2text.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.2/hezar/models/image2text/trocr/trocr_image2text.py` & `hezar-0.38.3/hezar/models/image2text/trocr/trocr_image2text.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.2/hezar/models/image2text/trocr/trocr_image2text_config.py` & `hezar-0.38.3/hezar/models/image2text/trocr/trocr_image2text_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.2/hezar/models/image2text/vit_gpt2/vit_gpt2_image2text.py` & `hezar-0.38.3/hezar/models/image2text/vit_gpt2/vit_gpt2_image2text.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.2/hezar/models/image2text/vit_gpt2/vit_gpt2_image2text_config.py` & `hezar-0.38.3/hezar/models/image2text/vit_gpt2/vit_gpt2_image2text_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.2/hezar/models/image2text/vit_roberta/vit_roberta_image2text.py` & `hezar-0.38.3/hezar/models/image2text/vit_roberta/vit_roberta_image2text.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.2/hezar/models/image2text/vit_roberta/vit_roberta_image2text_config.py` & `hezar-0.38.3/hezar/models/image2text/vit_roberta/vit_roberta_image2text_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.2/hezar/models/mask_filling/bert/bert_mask_filling.py` & `hezar-0.38.3/hezar/models/mask_filling/bert/bert_mask_filling.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.2/hezar/models/mask_filling/bert/bert_mask_filling_config.py` & `hezar-0.38.3/hezar/models/mask_filling/bert/bert_mask_filling_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.2/hezar/models/mask_filling/distilbert/distilbert_mask_filling.py` & `hezar-0.38.3/hezar/models/mask_filling/distilbert/distilbert_mask_filling.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.2/hezar/models/mask_filling/distilbert/distilbert_mask_filling_config.py` & `hezar-0.38.3/hezar/models/mask_filling/distilbert/distilbert_mask_filling_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.2/hezar/models/mask_filling/roberta/roberta_mask_filling.py` & `hezar-0.38.3/hezar/models/mask_filling/roberta/roberta_mask_filling.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.2/hezar/models/mask_filling/roberta/roberta_mask_filling_config.py` & `hezar-0.38.3/hezar/models/mask_filling/roberta/roberta_mask_filling_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.2/hezar/models/model.py` & `hezar-0.38.3/hezar/models/model.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.2/hezar/models/model_outputs.py` & `hezar-0.38.3/hezar/models/model_outputs.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.2/hezar/models/sequence_labeling/bert/bert_sequence_labeling.py` & `hezar-0.38.3/hezar/models/sequence_labeling/bert/bert_sequence_labeling.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.2/hezar/models/sequence_labeling/bert/bert_sequence_labeling_config.py` & `hezar-0.38.3/hezar/models/sequence_labeling/bert/bert_sequence_labeling_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.2/hezar/models/sequence_labeling/distilbert/distilbert_sequence_labeling.py` & `hezar-0.38.3/hezar/models/sequence_labeling/distilbert/distilbert_sequence_labeling.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.2/hezar/models/sequence_labeling/distilbert/distilbert_sequence_labeling_config.py` & `hezar-0.38.3/hezar/models/sequence_labeling/distilbert/distilbert_sequence_labeling_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.2/hezar/models/sequence_labeling/roberta/roberta_sequence_labeling.py` & `hezar-0.38.3/hezar/models/sequence_labeling/roberta/roberta_sequence_labeling.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.2/hezar/models/sequence_labeling/roberta/roberta_sequence_labeling_config.py` & `hezar-0.38.3/hezar/models/sequence_labeling/roberta/roberta_sequence_labeling_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.2/hezar/models/speech_recognition/whisper/whisper_feature_extractor.py` & `hezar-0.38.3/hezar/models/speech_recognition/whisper/whisper_feature_extractor.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.2/hezar/models/speech_recognition/whisper/whisper_speech_recognition.py` & `hezar-0.38.3/hezar/models/speech_recognition/whisper/whisper_speech_recognition.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.2/hezar/models/speech_recognition/whisper/whisper_speech_recognition_config.py` & `hezar-0.38.3/hezar/models/speech_recognition/whisper/whisper_speech_recognition_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.2/hezar/models/speech_recognition/whisper/whisper_tokenizer.py` & `hezar-0.38.3/hezar/models/speech_recognition/whisper/whisper_tokenizer.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.2/hezar/models/text_classification/bert/bert_text_classification.py` & `hezar-0.38.3/hezar/models/text_classification/bert/bert_text_classification.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.2/hezar/models/text_classification/bert/bert_text_classification_config.py` & `hezar-0.38.3/hezar/models/text_classification/bert/bert_text_classification_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.2/hezar/models/text_classification/distilbert/distilbert_text_classification.py` & `hezar-0.38.3/hezar/models/text_classification/distilbert/distilbert_text_classification.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.2/hezar/models/text_classification/distilbert/distilbert_text_classification_config.py` & `hezar-0.38.3/hezar/models/text_classification/distilbert/distilbert_text_classification_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.2/hezar/models/text_classification/roberta/roberta_text_classification.py` & `hezar-0.38.3/hezar/models/text_classification/roberta/roberta_text_classification.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.2/hezar/models/text_classification/roberta/roberta_text_classification_config.py` & `hezar-0.38.3/hezar/models/text_classification/roberta/roberta_text_classification_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.2/hezar/models/text_generation/gpt2/gpt2_text_generation.py` & `hezar-0.38.3/hezar/models/text_generation/gpt2/gpt2_text_generation.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.2/hezar/models/text_generation/gpt2/gpt2_text_generation_config.py` & `hezar-0.38.3/hezar/models/text_generation/gpt2/gpt2_text_generation_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.2/hezar/models/text_generation/t5/t5_text_generation.py` & `hezar-0.38.3/hezar/models/text_generation/t5/t5_text_generation.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.2/hezar/models/text_generation/t5/t5_text_generation_config.py` & `hezar-0.38.3/hezar/models/text_generation/t5/t5_text_generation_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.2/hezar/preprocessors/audio_feature_extractor.py` & `hezar-0.38.3/hezar/preprocessors/audio_feature_extractor.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.2/hezar/preprocessors/image_processor.py` & `hezar-0.38.3/hezar/preprocessors/image_processor.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.2/hezar/preprocessors/preprocessor.py` & `hezar-0.38.3/hezar/preprocessors/preprocessor.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.2/hezar/preprocessors/text_normalizer.py` & `hezar-0.38.3/hezar/preprocessors/text_normalizer.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.2/hezar/preprocessors/tokenizers/bpe.py` & `hezar-0.38.3/hezar/preprocessors/tokenizers/bpe.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.2/hezar/preprocessors/tokenizers/sentencepiece_bpe.py` & `hezar-0.38.3/hezar/preprocessors/tokenizers/sentencepiece_bpe.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.2/hezar/preprocessors/tokenizers/sentencepiece_unigram.py` & `hezar-0.38.3/hezar/preprocessors/tokenizers/sentencepiece_unigram.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.2/hezar/preprocessors/tokenizers/tokenizer.py` & `hezar-0.38.3/hezar/preprocessors/tokenizers/tokenizer.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.2/hezar/preprocessors/tokenizers/wordpiece.py` & `hezar-0.38.3/hezar/preprocessors/tokenizers/wordpiece.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.2/hezar/registry.py` & `hezar-0.38.3/hezar/registry.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.2/hezar/trainer/metrics_handlers.py` & `hezar-0.38.3/hezar/trainer/metrics_handlers.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.2/hezar/trainer/trainer.py` & `hezar-0.38.3/hezar/trainer/trainer.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -29,19 +29,19 @@
 )
 from ..data import Dataset, RangedSampler
 from ..models import Model
 from ..preprocessors import Preprocessor, PreprocessorsContainer
 from ..utils import (
     Logger,
     colorize_text,
+    dataloader_worker_init_fn,
     is_backend_available,
     sanitize_function_parameters,
     set_seed,
     verify_dependencies,
-    dataloader_worker_init_fn,
 )
 from .metrics_handlers import (
     Image2TextMetricHandler,
     MetricsHandler,
     SequenceLabelingMetricsHandler,
     SpeechRecognitionMetricsHandler,
     TextClassificationMetricsHandler,
```

### Comparing `hezar-0.38.2/hezar/trainer/trainer_utils.py` & `hezar-0.38.3/hezar/trainer/trainer_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.2/hezar/utils/audio_utils.py` & `hezar-0.38.3/hezar/utils/audio_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.2/hezar/utils/common_utils.py` & `hezar-0.38.3/hezar/utils/common_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.2/hezar/utils/data_utils.py` & `hezar-0.38.3/hezar/utils/data_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, Dict, List, Literal, Optional
 from functools import partial
+from typing import TYPE_CHECKING, Any, Dict, List, Literal, Optional
 
 from omegaconf import DictConfig
 
 from ..constants import PaddingType
 from .logging import Logger
 
 
@@ -250,16 +250,18 @@
 
     torch.manual_seed(seed)
     if torch.cuda.is_available():
         torch.cuda.manual_seed(seed)
         torch.cuda.manual_seed_all(seed)
     np.random.seed(seed)
     random.seed(seed)
-    
+
+
 def dataloader_worker_init_fn(seed):
     """
     A dataloader worker init function that handles reproducibility by hard-setting the seed for all workers.
     """
+
     def worker_init_fn(worker_id, seed):
-        seet_seed(seed+worker_id)
+        set_seed(seed + worker_id)
 
     return partial(worker_init_fn, seed=seed)
```

### Comparing `hezar-0.38.2/hezar/utils/file_utils.py` & `hezar-0.38.3/hezar/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.2/hezar/utils/hub_utils.py` & `hezar-0.38.3/hezar/utils/hub_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.2/hezar/utils/image_utils.py` & `hezar-0.38.3/hezar/utils/image_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.2/hezar/utils/integration_utils.py` & `hezar-0.38.3/hezar/utils/integration_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.2/hezar/utils/logging.py` & `hezar-0.38.3/hezar/utils/logging.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.2/hezar/utils/registry_utils.py` & `hezar-0.38.3/hezar/utils/registry_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.2/pyproject.toml` & `hezar-0.38.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "hezar"
-version = "0.38.2"
+version = "0.38.3"
 packages = [{ include = "hezar" }]
 description = "Hezar: The all-in-one AI library for Persian, supporting a wide variety of tasks and modalities!"
 license = "Apache-2.0"
 authors = ["Aryan Shekarlaban <arxyzan@gmail.com>"]
 maintainers = ["Aryan Shekarlaban <arxyzan@gmail.com>"]
 repository = "https://github.com/hezarai/hezar"
 homepage = "https://github.com/hezarai"
```

### Comparing `hezar-0.38.2/PKG-INFO` & `hezar-0.38.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hezar
-Version: 0.38.2
+Version: 0.38.3
 Summary: Hezar: The all-in-one AI library for Persian, supporting a wide variety of tasks and modalities!
 Home-page: https://github.com/hezarai
 License: Apache-2.0
 Keywords: packaging,poetry
 Author: Aryan Shekarlaban
 Author-email: arxyzan@gmail.com
 Maintainer: Aryan Shekarlaban
```

