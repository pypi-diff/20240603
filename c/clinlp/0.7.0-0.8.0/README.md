# Comparing `tmp/clinlp-0.7.0.tar.gz` & `tmp/clinlp-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clinlp-0.7.0.tar", max compression
+gzip compressed data, was "clinlp-0.8.0.tar", max compression
```

## Comparing `clinlp-0.7.0.tar` & `clinlp-0.8.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
--rw-r--r--   0        0        0    35149 2024-05-16 11:48:14.545758 clinlp-0.7.0/LICENSE
--rw-r--r--   0        0        0    25871 2024-05-16 11:48:14.545758 clinlp-0.7.0/README.md
--rw-r--r--   0        0        0     1084 2024-05-16 11:48:14.549758 clinlp-0.7.0/pyproject.toml
--rw-r--r--   0        0        0      525 2024-05-16 11:48:14.549758 clinlp-0.7.0/src/clinlp/__init__.py
--rw-r--r--   0        0        0       48 2024-05-16 11:48:14.549758 clinlp-0.7.0/src/clinlp/exceptions.py
--rw-r--r--   0        0        0      121 2024-05-16 11:48:14.549758 clinlp-0.7.0/src/clinlp/ie/__init__.py
--rw-r--r--   0        0        0     7962 2024-05-16 11:48:14.549758 clinlp-0.7.0/src/clinlp/ie/entity.py
--rw-r--r--   0        0        0      740 2024-05-16 11:48:14.549758 clinlp-0.7.0/src/clinlp/ie/qualifier/__init__.py
--rw-r--r--   0        0        0    13855 2024-05-16 11:48:14.549758 clinlp-0.7.0/src/clinlp/ie/qualifier/context_algorithm.py
--rw-r--r--   0        0        0     4141 2024-05-16 11:48:14.549758 clinlp-0.7.0/src/clinlp/ie/qualifier/qualifier.py
--rw-r--r--   0        0        0     7576 2024-05-16 11:48:14.549758 clinlp-0.7.0/src/clinlp/ie/qualifier/transformer.py
--rw-r--r--   0        0        0     9053 2024-05-16 11:48:14.549758 clinlp-0.7.0/src/clinlp/language.py
--rw-r--r--   0        0        0      123 2024-05-16 11:48:14.549758 clinlp-0.7.0/src/clinlp/metrics/__init__.py
--rw-r--r--   0        0        0    22664 2024-05-16 11:48:14.549758 clinlp-0.7.0/src/clinlp/metrics/ie.py
--rw-r--r--   0        0        0     1656 2024-05-16 11:48:14.549758 clinlp-0.7.0/src/clinlp/normalizer.py
--rw-r--r--   0        0        0        0 2024-05-16 11:48:14.549758 clinlp-0.7.0/src/clinlp/resources/__init__.py
--rw-r--r--   0        0        0    38312 2024-05-16 11:48:14.549758 clinlp-0.7.0/src/clinlp/resources/context_rules.json
--rw-r--r--   0        0        0     2412 2024-05-16 11:48:14.549758 clinlp-0.7.0/src/clinlp/sentencizer.py
--rw-r--r--   0        0        0     2173 2024-05-16 11:48:14.549758 clinlp-0.7.0/src/clinlp/util.py
--rw-r--r--   0        0        0    26854 1970-01-01 00:00:00.000000 clinlp-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-06-03 12:03:01.795096 clinlp-0.8.0/LICENSE
+-rw-r--r--   0        0        0    26480 2024-06-03 12:03:01.795096 clinlp-0.8.0/README.md
+-rw-r--r--   0        0        0     1239 2024-06-03 12:03:01.799096 clinlp-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0      543 2024-06-03 12:03:01.799096 clinlp-0.8.0/src/clinlp/__init__.py
+-rw-r--r--   0        0        0       48 2024-06-03 12:03:01.799096 clinlp-0.8.0/src/clinlp/exceptions.py
+-rw-r--r--   0        0        0      180 2024-06-03 12:03:01.799096 clinlp-0.8.0/src/clinlp/ie/__init__.py
+-rw-r--r--   0        0        0     7125 2024-06-03 12:03:01.799096 clinlp-0.8.0/src/clinlp/ie/entity.py
+-rw-r--r--   0        0        0      740 2024-06-03 12:03:01.803096 clinlp-0.8.0/src/clinlp/ie/qualifier/__init__.py
+-rw-r--r--   0        0        0    14253 2024-06-03 12:03:01.803096 clinlp-0.8.0/src/clinlp/ie/qualifier/context_algorithm.py
+-rw-r--r--   0        0        0     4544 2024-06-03 12:03:01.803096 clinlp-0.8.0/src/clinlp/ie/qualifier/qualifier.py
+-rw-r--r--   0        0        0     7857 2024-06-03 12:03:01.803096 clinlp-0.8.0/src/clinlp/ie/qualifier/transformer.py
+-rw-r--r--   0        0        0     1576 2024-06-03 12:03:01.803096 clinlp-0.8.0/src/clinlp/ie/term.py
+-rw-r--r--   0        0        0     9347 2024-06-03 12:03:01.803096 clinlp-0.8.0/src/clinlp/language.py
+-rw-r--r--   0        0        0      123 2024-06-03 12:03:01.803096 clinlp-0.8.0/src/clinlp/metrics/__init__.py
+-rw-r--r--   0        0        0    22883 2024-06-03 12:03:01.803096 clinlp-0.8.0/src/clinlp/metrics/ie.py
+-rw-r--r--   0        0        0     1759 2024-06-03 12:03:01.803096 clinlp-0.8.0/src/clinlp/normalizer.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:03:01.803096 clinlp-0.8.0/src/clinlp/resources/__init__.py
+-rw-r--r--   0        0        0    38312 2024-06-03 12:03:01.803096 clinlp-0.8.0/src/clinlp/resources/context_rules.json
+-rw-r--r--   0        0        0     2271 2024-06-03 12:03:01.803096 clinlp-0.8.0/src/clinlp/sentencizer.py
+-rw-r--r--   0        0        0     2615 2024-06-03 12:03:01.803096 clinlp-0.8.0/src/clinlp/util.py
+-rw-r--r--   0        0        0    27463 1970-01-01 00:00:00.000000 clinlp-0.8.0/PKG-INFO
```

### Comparing `clinlp-0.7.0/LICENSE` & `clinlp-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `clinlp-0.7.0/README.md` & `clinlp-0.8.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         "hypotensie", Term("bd verlaagd", proximity=1)
     ],
     "veneus_infarct": [
         "veneus infarct", Term("VI", attr="TEXT")
     ]
 }
 
-entity_matcher = nlp.add_pipe("clinlp_entity_matcher", config={"attr": "NORM", "fuzzy": 1})
+entity_matcher = nlp.add_pipe("clinlp_rule_based_entity_matcher", config={"attr": "NORM", "fuzzy": 1})
 entity_matcher.load_concepts(concepts)
 
 # Qualifiers
 nlp.add_pipe("clinlp_context_algorithm", config={"phrase_matcher_attr": "NORM"})
 
 text = (
     "Preterme neonaat (<p3), bd enigszins verlaagd, familieanamnese vermeldt eveneens hypotensie "
@@ -74,15 +74,15 @@
 ```
 
 ![example_doc_render.png](media/example_doc_render.png)
 
 With relevant qualifiers (defaults omitted for readability):
 
 ```python
-for ent in doc.ents:
+for ent in doc.spans["ents"]:
   print(ent, ent._.qualifiers_str)
 ```
 
 * `Preterme` `set()`
 * `<p3` `set()`
 * `bd enigszins verlaagd` `set()`
 * `hypotensie` `{'Experiencer.Family'}`
@@ -144,15 +144,15 @@
 nlp.add_pipe("clinlp_sentencizer")
 ```
 
 It is designed to detect sentence boundaries in clinical text, whenever a character that demarks a sentence ending is matched (e.g. newline, period, question mark). It also correctly detects items in an enumerations (e.g. starting with `-` or `*`). 
 
 ### Entity matcher
 
-`clinlp` includes a `clinlp_entity_matcher` component that can be used for matching entities in text, based on a dictionary of known concepts and their terms/synonyms. It includes options for matching on different token attributes, proximity matching, fuzzy matching and matching pseudo/negative terms. 
+`clinlp` includes a `clinlp_rule_based_entity_matcher` component that can be used for matching entities in text, based on a dictionary of known concepts and their terms/synonyms. It includes options for matching on different token attributes, proximity matching, fuzzy matching and matching pseudo/negative terms. 
 
 The most basic example would be the following, with further options described below:
 
 ```python
 concepts = {
     "sepsis": [
         "sepsis",
@@ -162,50 +162,56 @@
     ],
     "veneus_infarct": [
         "veneus infarct",
         "VI",
     ]
 }
 
-entity_matcher = nlp.add_pipe("clinlp_entity_matcher")
+entity_matcher = nlp.add_pipe("clinlp_rule_based_entity_matcher")
 entity_matcher.load_concepts(concepts)
-
 ```
-> :bulb: The `clinlp_entity_matcher` component wraps the spaCy `Matcher` and `PhraseMatcher` components, adding some convenience and configurability. However, the `Matcher`, `PhraseMatcher` or `EntityRuler` can also be used directly with `clinlp` for those who prefer it.
+
+> :bulb: `clinlp` stores entities in `doc.spans`, specifically in `doc.spans["ents"]`. The reason for this is that spans can overlap, while the entities in `doc.ents` cannot. If you use other/custom components, make sure they read/write entities from/to the same span key if interoperability is needed.
+
+> :bulb: The `clinlp_rule_based_entity_matcher` component wraps the spaCy `Matcher` and `PhraseMatcher` components, adding some convenience and configurability. However, the `Matcher`, `PhraseMatcher` or `SpanRuler` can also be used directly with `clinlp` for those who prefer it. You can configure the `SpanRuler` to write to the same `SpanGroup` as follows: 
+> ```python
+> from clinlp.ie import SPAN_KEY
+> ruler = nlp.add_pipe('span_ruler', config={'span_key': SPAN_KEY})
+> ```
 
 #### Attribute
 
 Specify the token attribute the entity matcher should use as follows (by default `TEXT`):
 
 ```python
-entity_matcher = nlp.add_pipe("clinlp_entity_matcher", config={"attr": "NORM"})
+entity_matcher = nlp.add_pipe("clinlp_rule_based_entity_matcher", config={"attr": "NORM"})
 ```
 
 Any [Token attribute](https://spacy.io/api/token#attributes) can be used, but in the above example the `clinlp_normalizer` should be added before the entity matcher, or the `NORM` attribute is simply the literal text. `clinlp` does not include Part of Speech tags and dependency trees, at least not until a reliable model for Dutch clinical text is created, though it's always possible to add a relevant component from a trained (general) Dutch model if needed.
 
 #### Proximity matching
 
 The proxmity setting defines how many tokens can optionally be skipped between the tokens of a pattern. With `proxmity` set to `1`, the pattern `slaapt slecht` will also match `slaapt vaak slecht`, but not `slaapt al weken slecht`. 
 
 ```python
-entity_matcher = nlp.add_pipe("clinlp_entity_matcher", config={"proximity": 1})
+entity_matcher = nlp.add_pipe("clinlp_rule_based_entity_matcher", config={"proximity": 1})
 ```
 
 #### Fuzzy matching
 
 Fuzzy matching enables finding misspelled variants of terms. For instance, with `fuzzy` set to `1`, the pattern `diabetes` will also match `diabets`, `ddiabetes`, or `diabetis`, but not `diabetse` or `ddiabetess`. The threshold is based on Levenshtein distance with insertions, deletions and replacements (but not swaps).  
 
 ```python
-entity_matcher = nlp.add_pipe("clinlp_entity_matcher", config={"fuzzy": 1})
+entity_matcher = nlp.add_pipe("clinlp_rule_based_entity_matcher", config={"fuzzy": 1})
 ```
 
 Additionally, the `fuzzy_min_len` argument can be used to specify the minimum length of a phrase for fuzzy matching. This also works for multi-token phrases. For example, with `fuzzy` set to `1` and `fuzzy_min_len` set to `5`, the pattern `bloeding graad ii` would also match `bloedin graad ii`, but not `bloeding graad iii`. 
 
 ```python
-entity_matcher = nlp.add_pipe("clinlp_entity_matcher", config={"fuzzy": 1, "fuzzy_min_len": 5})
+entity_matcher = nlp.add_pipe("clinlp_rule_based_entity_matcher", config={"fuzzy": 1, "fuzzy_min_len": 5})
 ```
 
 #### Terms
 The settings above are described at the matcher level, but can all be overridden at the term level by adding a `Term` to a concept, rather than a literal phrase:
 
 ```python
 from clinlp.ie import Term
@@ -217,15 +223,15 @@
         Term("early onset", proximity=1),
         Term("late onset", proximity=1),
         Term("EOS", attr="TEXT", fuzzy=0),
         Term("LOS", attr="TEXT", fuzzy=0)
     ]
 }
 
-entity_matcher = nlp.add_pipe("clinlp_entity_matcher", config={"attr": "NORM", "fuzzy": 1})
+entity_matcher = nlp.add_pipe("clinlp_rule_based_entity_matcher", config={"attr": "NORM", "fuzzy": 1})
 entity_matcher.load_concepts(concepts)
 ```
 
 In the above example, by default the `NORM` attribute is used, and `fuzzy` is set to `1`. In addition, for the terms `early onset` and `late onset` proximity matching is set to `1`, in addition to matcher-level config of matching the `NORM` attribute and fuzzy matching. For the `EOS` and `LOS` abbreviations the `TEXT` attribute is used (so the matching is case sensitive), and fuzzy matching is disabled. 
 
 #### Pseudo/negative phrases
```

### Comparing `clinlp-0.7.0/src/clinlp/__init__.py` & `clinlp-0.8.0/src/clinlp/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import importlib.util
 
 # components
-from .ie.entity import EntityMatcher
+from .ie.entity import RuleBasedEntityMatcher
 from .ie.qualifier import ContextAlgorithm
 
 if importlib.util.find_spec("transformers") is not None:
     from .ie.qualifier import ExperiencerTransformer, NegationTransformer
 
 # base
 from .language import Clinlp
 from .normalizer import Normalizer
 from .sentencizer import Sentencizer
 
 __all__ = [
-    "EntityMatcher",
+    "RuleBasedEntityMatcher",
     "ContextAlgorithm",
     "ExperiencerTransformer",
     "NegationTransformer",
     "Clinlp",
     "Normalizer",
     "Sentencizer",
 ]
```

### Comparing `clinlp-0.7.0/src/clinlp/ie/qualifier/__init__.py` & `clinlp-0.8.0/src/clinlp/ie/qualifier/__init__.py`

 * *Files identical despite different names*

### Comparing `clinlp-0.7.0/src/clinlp/ie/qualifier/context_algorithm.py` & `clinlp-0.8.0/src/clinlp/ie/qualifier/context_algorithm.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,28 +2,32 @@
 import itertools
 import json
 import re
 import warnings
 from collections import defaultdict
 from dataclasses import dataclass
 from enum import Enum
-from typing import Iterator, Optional, Union
+from pathlib import Path
+from typing import Optional, Union
 
 import intervaltree as ivt
 from spacy.language import Language
 from spacy.matcher import Matcher, PhraseMatcher
 from spacy.tokens import Doc, Span
 
 from clinlp.ie.qualifier.qualifier import (
     ATTR_QUALIFIERS,
     Qualifier,
     QualifierClass,
     QualifierDetector,
 )
-from clinlp.util import clinlp_autocomponent, interval_dist
+from clinlp.util import clinlp_component, interval_dist
+
+_RESOURCES_DIR = importlib.resources.files("clinlp.resources")
+_DEFAULT_CONTEXT_RULES_FILE = "context_rules.json"
 
 
 class ContextRuleDirection(Enum):
     """
     Direction of a Context rule, as in the original Context Algorithm.
     """
 
@@ -73,15 +77,16 @@
         the window determined in the `max_scope` of the rule, or the sentence
         boundaries if no `max_scope` is set.
         """
 
         max_scope = self.rule.max_scope or len(sentence)
 
         if max_scope < 1:
-            raise ValueError(f"max_scope must be at least 1, but got {max_scope}")
+            msg = f"max_scope must be at least 1, but got {max_scope}"
+            raise ValueError(msg)
 
         scoped_start = max(self.start - max_scope, sentence.start)
         scoped_end = min(self.end + max_scope, sentence.end)
 
         if self.rule.direction == ContextRuleDirection.PRECEDING:
             self.scope = (self.start, scoped_end)
 
@@ -91,27 +96,24 @@
         elif self.rule.direction == ContextRuleDirection.BIDIRECTIONAL:
             self.scope = (scoped_start, scoped_end)
 
 
 _defaults_context_algorithm = {
     "phrase_matcher_attr": "TEXT",
     "load_rules": True,
-    "rules": str(
-        importlib.resources.files("clinlp.resources").joinpath("context_rules.json")
-    ),
+    "rules": str(_RESOURCES_DIR.joinpath(_DEFAULT_CONTEXT_RULES_FILE)),
 }
 
 
-@Language.factory(
+@clinlp_component(
     name="clinlp_context_algorithm",
-    requires=["doc.sents", "doc.ents"],
+    requires=["doc.sents", "doc.spans"],
     assigns=[f"span._.{ATTR_QUALIFIERS}"],
     default_config=_defaults_context_algorithm,
 )
-@clinlp_autocomponent
 class ContextAlgorithm(QualifierDetector):
     """
     Implements the Context algorithm (https://doi.org/10.1016%2Fj.jbi.2009.05.002) as
     a spaCy pipeline component.
 
     Args:
         nlp: The Spacy language object to use
@@ -123,65 +125,43 @@
         (see clinlp.resources dir for example).
     """
 
     def __init__(
         self,
         nlp: Language,
         phrase_matcher_attr: str = _defaults_context_algorithm["phrase_matcher_attr"],
-        load_rules=_defaults_context_algorithm["load_rules"],
+        load_rules: bool = _defaults_context_algorithm["load_rules"],  # noqa FBT001
         rules: Optional[Union[str | dict]] = _defaults_context_algorithm["rules"],
+        **kwargs,
     ) -> None:
         self._nlp = nlp
 
         self._matcher = Matcher(self._nlp.vocab)
         self._phrase_matcher = PhraseMatcher(self._nlp.vocab, attr=phrase_matcher_attr)
 
         self.rules = {}
         self._qualifier_classes = {}
 
         if load_rules:
             if rules is None:
-                raise ValueError(
+                msg = (
                     "Did not provide rules. Set `load_rules` to False if you "
                     "want to add `ContextRule` manually."
                 )
+                raise ValueError(msg)
+
+            parsed_rules = self._parse_rules(rules)
+            self.add_rules(parsed_rules)
 
-            rules = self._parse_rules(rules)
-            self.add_rules(rules)
+        super().__init__(**kwargs)
 
     @property
     def qualifier_classes(self) -> dict[str, QualifierClass]:
         return self._qualifier_classes
 
-    def add_rule(self, rule: ContextRule) -> None:
-        """
-        Add a rule.
-        """
-        rule_key = f"rule_{len(self.rules)}"
-        self.rules[rule_key] = rule
-
-        if isinstance(rule.pattern, str):
-            self._phrase_matcher.add(key=rule_key, docs=[self._nlp(rule.pattern)])
-
-        elif isinstance(rule.pattern, list):
-            self._matcher.add(key=rule_key, patterns=[rule.pattern])
-
-        else:
-            raise ValueError(
-                f"Don't know how to process ContextRule with pattern of "
-                f"type {type(rule.pattern)}"
-            )
-
-    def add_rules(self, rules: list[ContextRule]) -> None:
-        """
-        Add multiple rules.
-        """
-        for rule in rules:
-            self.add_rule(rule)
-
     @staticmethod
     def _parse_qualifier(
         qualifier: str, qualifier_classes: dict[str, QualifierClass]
     ) -> Qualifier:
         """
         Parse a Qualifier from string.
 
@@ -190,18 +170,19 @@
 
         Returns: A qualifier, as specified.
         """
 
         match_regexp = r"\w+\.\w+"
 
         if not re.match(match_regexp, qualifier):
-            raise ValueError(
+            msg = (
                 f"Cannot parse qualifier {qualifier}, please adhere to format "
                 f"{match_regexp} (e.g. NegationQualifier.NEGATED)"
             )
+            raise ValueError(msg)
 
         qualifier_class, qualifier = qualifier.split(".")
 
         return qualifier_classes[qualifier_class].create(value=qualifier)
 
     @staticmethod
     def _parse_direction(direction: str) -> ContextRuleDirection:
@@ -213,15 +194,15 @@
 
         Returns: THe ContextRuleDirection.
         """
         return ContextRuleDirection[direction.upper()]
 
     def _parse_rules(self, rules: Union[str | dict]) -> list[ContextRule]:
         if isinstance(rules, str):
-            with open(rules, "rb") as file:
+            with Path(rules).open(mode="rb") as file:
                 rules = json.load(file)
 
         for qualifier in rules["qualifiers"]:
             self._qualifier_classes[qualifier["name"]] = QualifierClass(**qualifier)
 
         qualifier_rules = []
 
@@ -233,20 +214,52 @@
             qualifier_rules += [
                 ContextRule(pattern, qualifier, direction, max_scope)
                 for pattern in rule["patterns"]
             ]
 
         return qualifier_rules
 
-    @staticmethod
-    def _get_sentences_having_entity(doc: Doc) -> Iterator[Span]:
+    def add_rule(self, rule: ContextRule) -> None:
+        """
+        Add a rule.
+        """
+        rule_key = f"rule_{len(self.rules)}"
+        self.rules[rule_key] = rule
+
+        if isinstance(rule.pattern, str):
+            self._phrase_matcher.add(key=rule_key, docs=[self._nlp(rule.pattern)])
+
+        elif isinstance(rule.pattern, list):
+            self._matcher.add(key=rule_key, patterns=[rule.pattern])
+
+        else:
+            msg = (
+                f"Don't know how to process ContextRule with pattern of "
+                f"type {type(rule.pattern)}"
+            )
+            raise TypeError(msg)
+
+    def add_rules(self, rules: list[ContextRule]) -> None:
+        """
+        Add multiple rules.
         """
-        Return sentences in a doc that have at least one entity.
+        for rule in rules:
+            self.add_rule(rule)
+
+    def _get_sentences_with_entities(self, doc: Doc) -> dict[Span, list[Span]]:
+        """
+        Return sentences in a doc that have at least one entity, mapped to the entities.
         """
-        return (sent for sent in doc.sents if len(sent.ents) > 0)
+
+        sents = defaultdict(list)
+
+        for ent in doc.spans[self.spans_key]:
+            sents[ent.sent].append(ent)
+
+        return sents
 
     def _get_rule_from_match_id(self, match_id: int) -> ContextRule:
         """
         Get the rule that was matched, from the match_id (first element of match tuple
         returned by matcher).
         """
         return self.rules[self._nlp.vocab.strings[match_id]]
@@ -360,23 +373,24 @@
                             -mp.rule.qualifier.priority,
                         ),
                     )
                 )
 
         return result_patterns
 
-    def _detect_qualifiers(self, doc: Doc):
+    def _detect_qualifiers(self, doc: Doc) -> None:
         """
         Apply the Context Algorithm to a doc.
         """
 
         if len(self.rules) == 0:
-            raise RuntimeError("Cannot match qualifiers without any ContextRule.")
+            msg = "Cannot match qualifiers without any ContextRule."
+            raise RuntimeError(msg)
 
-        for sentence in self._get_sentences_having_entity(doc):
+        for sentence, ents in self._get_sentences_with_entities(doc).items():
             with warnings.catch_warnings():
                 # a UserWarning will trigger when one of the matchers is empty
                 warnings.simplefilter("ignore", UserWarning)
 
                 matches = itertools.chain(
                     self._matcher(sentence), self._phrase_matcher(sentence)
                 )
@@ -398,15 +412,15 @@
                 )
 
                 matched_pattern.initialize_scope(sentence)
                 matched_patterns.append(matched_pattern)
 
             match_scopes = self._compute_match_scopes(matched_patterns)
 
-            for ent in sentence.ents:
+            for ent in ents:
                 matched_patterns = []
 
                 for match_interval in match_scopes.overlap(ent.start, ent.end):
                     if (ent.start + 1 > match_interval.data.end) or (
                         ent.end < match_interval.data.start + 1
                     ):
                         matched_patterns.append(match_interval.data)
```

### Comparing `clinlp-0.7.0/src/clinlp/ie/qualifier/qualifier.py` & `clinlp-0.8.0/src/clinlp/ie/qualifier/qualifier.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,16 @@
-from abc import ABC, abstractmethod
+from abc import abstractmethod
 from dataclasses import dataclass, field
 from typing import Optional
 
+from spacy.pipeline import Pipe
 from spacy.tokens import Doc, Span
 
+from clinlp.ie import SPANS_KEY
+
 ATTR_QUALIFIERS = "qualifiers"
 ATTR_QUALIFIERS_STR = f"{ATTR_QUALIFIERS}_str"
 ATTR_QUALIFIERS_DICT = f"{ATTR_QUALIFIERS}_dict"
 
 
 def qualifiers_to_str(ent: Span) -> Optional[set[str]]:
     qualifiers = getattr(ent._, ATTR_QUALIFIERS)
@@ -63,84 +66,96 @@
 class QualifierClass:
     def __init__(
         self,
         name: str,
         values: list[str],
         default: Optional[str] = None,
         priorities: Optional[dict] = None,
-    ):
+    ) -> None:
         self.name = name
         self.values = values
         self.default = default or values[0]
         self.priorities = priorities or {value: n for n, value in enumerate(values)}
 
         if len(set(values)) != len(values):
-            raise ValueError(f"Please do not provide any duplicate values ({values})")
+            msg = f"Please do not provide any duplicate values ({values})"
+            raise ValueError(msg)
 
         if self.default not in values:
-            raise ValueError(f"Default {default} not in provided value {values}")
+            msg = f"Default {default} not in provided value {values}"
+            raise ValueError(msg)
 
     def create(self, value: Optional[str] = None, **kwargs) -> Qualifier:
         if value is None:
             value = self.default
 
         if value not in self.values:
-            raise ValueError(
+            msg = (
                 f"The qualifier {self.name} cannot take value '{value}'. "
                 f"Please choose one of {self.values}."
             )
+            raise ValueError(msg)
 
         is_default = value == self.default
         priority = self.priorities[value]
 
         return Qualifier(
             name=self.name,
             value=value,
             is_default=is_default,
             priority=priority,
             **kwargs,
         )
 
 
-class QualifierDetector(ABC):
+_defaults_qualifier_detector = {
+    "spans_key": SPANS_KEY,
+}
+
+
+class QualifierDetector(Pipe):
     """For usage as a spaCy pipeline component"""
 
+    def __init__(
+        self, spans_key: str = _defaults_qualifier_detector["spans_key"]
+    ) -> None:
+        self.spans_key = spans_key
+
     @property
     @abstractmethod
     def qualifier_classes(self) -> dict[str, QualifierClass]:
         pass
 
     @staticmethod
     def add_qualifier_to_ent(entity: Span, new_qualifier: Qualifier) -> None:
         qualifiers = get_qualifiers(entity)
 
         if qualifiers is None:
-            raise RuntimeError(
-                "Cannot add qualifier to entity with non-initialized qualifiers."
-            )
+            msg = "Cannot add qualifier to entity with non-initialized qualifiers."
+            raise RuntimeError(msg)
 
         qualifiers = {q for q in qualifiers if q.name != new_qualifier.name}
         qualifiers.add(new_qualifier)
 
         set_qualifiers(entity, qualifiers)
 
     def _initialize_ent_qualifiers(self, entity: Span) -> None:
         if get_qualifiers(entity) is None:
             set_qualifiers(entity, set())
 
-        for _, qualifier_class in self.qualifier_classes.items():
+        for qualifier_class in self.qualifier_classes.values():
             self.add_qualifier_to_ent(entity, qualifier_class.create())
 
     @abstractmethod
     def _detect_qualifiers(self, doc: Doc) -> None:
         pass
 
     def __call__(self, doc: Doc) -> Doc:
-        if len(doc.ents) == 0:
+        if self.spans_key not in doc.spans or len(doc.spans[self.spans_key]) == 0:
             return doc
 
-        for ent in doc.ents:
+        for ent in doc.spans[self.spans_key]:
             self._initialize_ent_qualifiers(ent)
 
         self._detect_qualifiers(doc)
 
         return doc
```

### Comparing `clinlp-0.7.0/src/clinlp/ie/qualifier/transformer.py` & `clinlp-0.8.0/src/clinlp/ie/qualifier/transformer.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import statistics
-from typing import Callable, Optional, Tuple
+from abc import abstractmethod
+from typing import Callable, Tuple
 
 import torch
 from spacy import Language
 from spacy.tokens import Doc, Span
 from transformers import AutoTokenizer, RobertaForTokenClassification
 
 from clinlp.ie.qualifier.qualifier import (
     ATTR_QUALIFIERS,
     QualifierClass,
     QualifierDetector,
 )
-from clinlp.util import clinlp_autocomponent
+from clinlp.util import clinlp_component
 
 HF_FROM_PRETRAINED_NEGATION = {
     "pretrained_model_name_or_path": "UMCU/MedRoBERTa.nl_NegationDetection",
     "revision": "83068ba132b6ce38e9f668c1e3ab636f79b774d3",
 }
 
 HF_FROM_PRETRAINED_EXPERIENCER = {
@@ -32,31 +33,44 @@
 
 _defaults_negation_transformer = {
     "absence_threshold": 0.1,
     "presence_threshold": 0.9,
 }
 _defaults_experiencer_transformer = {
     "token_window": 64,
-    "other_threshold": 0.5,
+    "family_threshold": 0.5,
 }
 
 
 class QualifierTransformer(QualifierDetector):
     def __init__(
         self,
         token_window: int = _defaults_qualifier_transformer["token_window"],
-        strip_entities: bool = _defaults_qualifier_transformer["strip_entities"],
-        placeholder: Optional[str] = _defaults_qualifier_transformer["placeholder"],
-        prob_aggregator: int = _defaults_qualifier_transformer["prob_aggregator"],
-    ):
+        strip_entities: bool = _defaults_qualifier_transformer["strip_entities"],  # noqa: FBT001
+        placeholder: str = _defaults_qualifier_transformer["placeholder"],
+        prob_aggregator: Callable = _defaults_qualifier_transformer["prob_aggregator"],
+        **kwargs,
+    ) -> None:
         self.token_window = token_window
         self.strip_entities = strip_entities
         self.placeholder = placeholder
         self.prob_aggregator = prob_aggregator
 
+        super().__init__(**kwargs)
+
+    @property
+    @abstractmethod
+    def tokenizer(self) -> AutoTokenizer:
+        raise NotImplementedError
+
+    @property
+    @abstractmethod
+    def model(self) -> RobertaForTokenClassification:
+        raise NotImplementedError
+
     @staticmethod
     def _get_ent_window(ent: Span, token_window: int) -> Tuple[str, int, int]:
         start_token_i = max(0, ent.start - token_window)
         end_token_i = min(len(ent.doc), ent.end + token_window)
 
         text_span = ent.doc[start_token_i:end_token_i]
 
@@ -118,52 +132,49 @@
         end_token = inputs.char_to_token(ent_end_char - 1)
 
         return prob_aggregator(
             sum(pos[prob_indices]) for pos in probs[start_token : end_token + 1]
         )
 
 
-@Language.factory(
+@clinlp_component(
     name="clinlp_negation_transformer",
-    requires=["doc.ents"],
+    requires=["doc.spans"],
     assigns=[f"span._.{ATTR_QUALIFIERS}"],
     default_config=_defaults_negation_transformer,
 )
-@clinlp_autocomponent
 class NegationTransformer(QualifierTransformer):
+    tokenizer = AutoTokenizer.from_pretrained(**HF_FROM_PRETRAINED_NEGATION)
+    model = RobertaForTokenClassification.from_pretrained(**HF_FROM_PRETRAINED_NEGATION)
+
     def __init__(
         self,
         nlp: Language,
         absence_threshold: float = _defaults_negation_transformer["absence_threshold"],
         presence_threshold: float = _defaults_negation_transformer[
             "presence_threshold"
         ],
         **kwargs,
     ) -> None:
         self.nlp = nlp
         self.absence_threshold = absence_threshold
         self.presence_threshold = presence_threshold
 
-        self.tokenizer = AutoTokenizer.from_pretrained(**HF_FROM_PRETRAINED_NEGATION)
-        self.model = RobertaForTokenClassification.from_pretrained(
-            **HF_FROM_PRETRAINED_NEGATION
-        )
-
         super().__init__(**kwargs)
 
     @property
     def qualifier_classes(self) -> dict[str, QualifierClass]:
         return {
             "Presence": QualifierClass(
                 "Presence", ["Absent", "Uncertain", "Present"], default="Present"
             )
         }
 
-    def _detect_qualifiers(self, doc: Doc):
-        for ent in doc.ents:
+    def _detect_qualifiers(self, doc: Doc) -> None:
+        for ent in doc.spans[self.spans_key]:
             text, ent_start_char, ent_end_char = self._prepare_ent(ent)
 
             prob = 1 - self._predict(
                 text,
                 ent_start_char,
                 ent_end_char,
                 prob_indices=[0, 2],
@@ -179,56 +190,55 @@
 
             self.add_qualifier_to_ent(
                 ent,
                 self.qualifier_classes["Presence"].create(qualifier_value, prob=prob),
             )
 
 
-@Language.factory(
+@clinlp_component(
     name="clinlp_experiencer_transformer",
-    requires=["doc.ents"],
+    requires=["doc.spans"],
     assigns=[f"span._.{ATTR_QUALIFIERS}"],
     default_config=_defaults_experiencer_transformer,
 )
-@clinlp_autocomponent
 class ExperiencerTransformer(QualifierTransformer):
+    tokenizer = AutoTokenizer.from_pretrained(**HF_FROM_PRETRAINED_EXPERIENCER)
+    model = RobertaForTokenClassification.from_pretrained(
+        **HF_FROM_PRETRAINED_EXPERIENCER
+    )
+
     def __init__(
         self,
         nlp: Language,
-        other_threshold: float = _defaults_experiencer_transformer["other_threshold"],
+        family_threshold: float = _defaults_experiencer_transformer["family_threshold"],
         **kwargs,
     ) -> None:
         self.nlp = nlp
-        self.other_threshold = other_threshold
-
-        self.tokenizer = AutoTokenizer.from_pretrained(**HF_FROM_PRETRAINED_EXPERIENCER)
-        self.model = RobertaForTokenClassification.from_pretrained(
-            **HF_FROM_PRETRAINED_EXPERIENCER
-        )
+        self.family_threshold = family_threshold
 
         super().__init__(**kwargs)
 
     @property
     def qualifier_classes(self) -> dict[str, QualifierClass]:
         return {
             "Experiencer": QualifierClass(
-                "Experiencer", ["Patient", "Family"], default="Patient"
+                "Experiencer", ["Patient", "Family", "Other"], default="Patient"
             )
         }
 
-    def _detect_qualifiers(self, doc: Doc):
-        for ent in doc.ents:
+    def _detect_qualifiers(self, doc: Doc) -> None:
+        for ent in doc.spans[self.spans_key]:
             text, ent_start_char, ent_end_char = self._prepare_ent(ent)
 
             prob = self._predict(
                 text,
                 ent_start_char,
                 ent_end_char,
                 prob_indices=[1, 3],
                 prob_aggregator=self.prob_aggregator,
             )
 
-            if prob > self.other_threshold:
+            if prob > self.family_threshold:
                 self.add_qualifier_to_ent(
                     ent,
                     self.qualifier_classes["Experiencer"].create("Family", prob=prob),
                 )
```

### Comparing `clinlp-0.7.0/src/clinlp/language.py` & `clinlp-0.8.0/src/clinlp/language.py`

 * *Files 10% similar despite different names*

```diff
@@ -234,29 +234,31 @@
 ]
 
 ALPHA_LOWER = "a-z"
 ALPHA_UPPER = "A-Z"
 ALPHA = "a-zA-Z"
 
 
-def _get_abbreviations():
+def _get_abbreviations() -> list[str]:
     base = set(spacy.lang.nl.tokenizer_exceptions.abbrevs.copy())
 
     for abbrev in CLINLP_REMOVE_ABBREVIATIONS:
         base.remove(abbrev)
 
     return list(base) + CLINLP_ABBREVIATIONS
 
 
 def _get_tokenizer_exceptions(
     abbreviations: list[str],
-    abbrev_transforms: list[Callable[[str], str]] = None,
+    *,
+    abbrev_transforms: Optional[list[Callable[[str], str]]] = None,
     keep_emoticons: bool = False,
-):
+) -> dict[str, list[dict]]:
     tokenizer_exceptions = spacy.lang.tokenizer_exceptions.BASE_EXCEPTIONS.copy()
+    abbrev_transforms = abbrev_transforms or []
 
     if not keep_emoticons:
         for emoticon in spacy.lang.tokenizer_exceptions.emoticons:
             del tokenizer_exceptions[emoticon]
 
     for abbrev_transform in abbrev_transforms:
         abbr_update = {
@@ -265,15 +267,15 @@
         tokenizer_exceptions = update_exc(tokenizer_exceptions, abbr_update)
 
     return update_exc(tokenizer_exceptions, CLINLP_TOKENIZER_EXCEPTIONS)
 
 
 def _get_list(
     base: list[str], add: Optional[list[str]] = None, remove: Optional[list[str]] = None
-):
+) -> list[str]:
     """
     Create a list, based on a base list, with some additions and removals.
     """
     _lst = base.copy()
 
     if add is not None:
         for item in add:
@@ -282,46 +284,46 @@
     if remove is not None:
         for item in remove:
             _lst.remove(item)
 
     return _lst
 
 
-def _get_ellipses():
+def _get_ellipses() -> list[str]:
     return spacy.lang.punctuation.LIST_ELLIPSES.copy()
 
 
-def _get_currencies():
+def _get_currencies() -> list[str]:
     return spacy.lang.punctuation.LIST_CURRENCY.copy()
 
 
-def _get_units():
+def _get_units() -> list[str]:
     return CLINLP_UNITS.copy()
 
 
-def _get_tokenizer_prefix_rules():
+def _get_tokenizer_prefix_rules() -> list[str]:
     return [
         r"\[(?![A-Z]{3,}-)",
         r"\S+(?=\[[A-Z]{3,}-)",
         r"x(?=[0-9]+)",
         r"`(?=[0-9])",
         r"([0-9]{,5}(\.|,))?[0-9]{,4}" + f"(?=({'|'.join(_get_units())}))",
     ]
 
 
-def _get_tokenizer_prefixes():
+def _get_tokenizer_prefixes() -> list[str]:
     punct = _get_list(
         base=spacy.lang.punctuation.LIST_PUNCT,
         add=[
             ",,",
             "§",
             "%",
             "=",
             "—",
-            "–",
+            "–",  # noqa RUF001
             r"\+(?![0-9])",
             "/",
             "-",
             r"\+",
             "~",
             ",",
             r"\s",
@@ -336,67 +338,65 @@
         + _get_ellipses()
         + quotes
         + _get_currencies()
         + _get_tokenizer_prefix_rules()
     )
 
 
-def _get_tokenizer_infix_rules(quotes: list[str]):
+def _get_tokenizer_infix_rules(quotes: list[str]) -> list[str]:
     return [
-        r"(?<=[{al}])\.(?=[{au}])".format(al=ALPHA_LOWER, au=ALPHA_UPPER),
-        r"(?<=[{a}])[,!?](?=[{a}])".format(a=ALPHA),
-        r'(?<=[{a}"])[:<>=](?=[{a}])'.format(a=ALPHA),
-        r"(?<=[{a}]),(?=[{a}])".format(a=ALPHA),
+        rf"(?<=[{ALPHA_LOWER}])\.(?=[{ALPHA_UPPER}])",
+        rf"(?<=[{ALPHA}])[,!?](?=[{ALPHA}])",
+        rf'(?<=[{ALPHA}"])[:<>=](?=[{ALPHA}])',
+        rf"(?<=[{ALPHA}]),(?=[{ALPHA}])",
         r"(?<=[{a}])([{q}\)\]\(\[])(?=[{a}])".format(a=ALPHA, q="".join(quotes)),
-        r"(?<=[{a}])--(?=[{a}])".format(a=ALPHA),
+        rf"(?<=[{ALPHA}])--(?=[{ALPHA}])",
         r"-(?![0-9]{1,2}\])",
         r"(?<=[0-9])x(?=[0-9])",
         r"(?<=10)E(?=\d)",
         r"(?<=[0-9])(x?d?d)(?=[0-9])",
     ]
 
 
-def _get_tokenizer_infixes():
+def _get_tokenizer_infixes() -> list[str]:
     punct = _get_list(
         base=[],
         add=["/", r"\+", "=", ":", "&", ";", r"\*", "<", r"\(", r"\)", r"\s", r"\^"],
     )
 
     quotes = _get_list(base=spacy.lang.punctuation.LIST_QUOTES, remove=["`", r"\'"])
 
-    infixes = punct + _get_ellipses() + _get_tokenizer_infix_rules(quotes)
-
-    return infixes
+    return punct + _get_ellipses() + _get_tokenizer_infix_rules(quotes)
 
 
 def _get_tokenizer_suffix_rules(
     currencies: list[str], units: list[str], punct: list[str], quotes: list[str]
-):
+) -> list[str]:
     return [
         r"(?<=[0-9])\+",
         r"(?<=°[FfCcKk])\.",
         r"(?<=[0-9])(?:{c})".format(c="|".join(currencies)),
         r"(?<=[0-9{al}{e}{p}(?:{q})])\.".format(
             al=ALPHA_LOWER, e=r"%²\-\+", q="".join(quotes), p="|".join(punct)
         ),
-        r"(?<=[{au}][{au}])\.".format(au=ALPHA_UPPER),
+        rf"(?<=[{ALPHA_UPPER}][{ALPHA_UPPER}])\.",
         r"(?<=[0-9]\])\S+",
         r"(?<!([A-Z]-\d|-\d\d))\]",  # tricky one
         r"(?<=[0-9])x",
         r"(?<=[0-9])" + f"({'|'.join(units)})",
         r"\s",
         r"(?<=[0-9])d?d",
         r"(?<=[0-9])(e|de|ste)",
     ]
 
 
-def _get_tokenizer_suffixes():
+def _get_tokenizer_suffixes() -> list[str]:
     punct = _get_list(
         base=spacy.lang.punctuation.LIST_PUNCT,
-        add=["/", "-", "=", "%", r"\+", "~", "''", "—", "–"],
+        add=["/", "-", "=", "%", r"\+", "~", "''", "—", "–"],  # noqa RUF001
         remove=[r"\]"],
     )
 
     quotes = _get_list(base=spacy.lang.punctuation.LIST_QUOTES)
 
     return (
         punct
@@ -413,29 +413,33 @@
         abbreviations=_get_abbreviations(), abbrev_transforms=CLINLP_ABBREV_TRANSFORMS
     )
 
     prefixes = _get_tokenizer_prefixes()
     infixes = _get_tokenizer_infixes()
     suffixes = _get_tokenizer_suffixes()
 
-    lex_attr_getters = {}
-    syntax_iterators = {}
-    stop_words = []
+    lex_attr_getters = {}  # noqa: RUF012
+    syntax_iterators = {}  # noqa: RUF012
+    stop_words = set()  # noqa: RUF012
     url_match = None
     token_match = None
 
-    writing_system = {"direction": "ltr", "has_case": True, "has_letters": True}
+    writing_system = {  # noqa: RUF012
+        "direction": "ltr",
+        "has_case": True,
+        "has_letters": True,
+    }
 
 
 @spacy.registry.languages("clinlp")
 class Clinlp(Language):
     lang = "clinlp"
     Defaults = ClinlpDefaults
 
-    def __init__(self, *args, **kwargs):
+    def __init__(self, *args, **kwargs) -> None:
         meta = dict(kwargs.pop("meta", {}))
         clinlp_version = importlib.metadata.version(__package__ or __name__)
 
         if "clinlp_version" in meta:
             if meta["clinlp_version"] != clinlp_version:
                 warnings.warn(
                     f"This spaCy model was built with clinlp version "
```

### Comparing `clinlp-0.7.0/src/clinlp/metrics/ie.py` & `clinlp-0.8.0/src/clinlp/metrics/ie.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import inspect
 import itertools
 import warnings
 from collections import Counter, defaultdict
 from dataclasses import dataclass, field
-from typing import Callable, Iterable, Optional
+from typing import Callable, ClassVar, Iterable, Optional
 
 import nervaluate
 import spacy
 from sklearn.metrics import f1_score, precision_score, recall_score
 
+from clinlp.ie import SPANS_KEY
+
 
 @dataclass
 class Annotation:
     """
     An annotation of a single entity in a piece of text.
     """
 
@@ -24,34 +26,34 @@
 
     end: int
     """ The end char"""
 
     label: str
     """ The label/tag"""
 
-    qualifiers: list[dict] = field(default_factory=lambda: list())
+    qualifiers: list[dict] = field(default_factory=list)
     """ Optionally, a list of qualifiers"""
 
-    def lstrip(self, chars=" ,"):
+    def lstrip(self, chars: str = " ,") -> None:
         """
         Strips punctuation and whitespaces from the beginning of the annotation.
         """
 
         self.start += len(self.text) - len(self.text.lstrip(chars))
         self.text = self.text.lstrip(chars)
 
-    def rstrip(self, chars=" ,"):
+    def rstrip(self, chars: str = " ,") -> None:
         """
         Strips punctuation and whitespaces from the end of the annotation.
         """
 
         self.end -= len(self.text) - len(self.text.rstrip(chars))
         self.text = self.text.rstrip(chars)
 
-    def strip(self, chars=" ,"):
+    def strip(self, chars: str = " ,") -> None:
         """
         Strips punctuation and whitespaces from the beginning and end of the annotation.
         """
 
         self.lstrip(chars=chars)
         self.rstrip(chars=chars)
 
@@ -95,15 +97,16 @@
         The entire qualifier, e.g. {"name": "Negation", "value": "Affirmed", ...}
 
         """
         for qualifier in self.qualifiers:
             if qualifier["name"] == qualifier_name:
                 return qualifier
 
-        raise KeyError(f"No qualifier with name {qualifier_name}.")
+        msg = f"No qualifier with name {qualifier_name}."
+        raise KeyError(msg)
 
 
 @dataclass
 class Document:
     """Any length of annotated text."""
 
     identifier: str
@@ -127,15 +130,15 @@
         if they should be included, False otherwise.
 
         Returns
         -------
         A list of dictionaries corresponding to annotations.
         """
 
-        ann_filter = ann_filter or (lambda ann: True)
+        ann_filter = ann_filter or (lambda _: True)
 
         return [ann.to_nervaluate() for ann in self.annotations if ann_filter(ann)]
 
     def labels(
         self, ann_filter: Optional[Callable[[Annotation], bool]] = None
     ) -> set[str]:
         """
@@ -146,15 +149,15 @@
         ann_filter: A filter to apply to annotations, should map to annotations to True
         if they should be included, False otherwise.
 
         Returns
         -------
         A set containing all annotation labels for this document.
         """
-        ann_filter = ann_filter or (lambda ann: True)
+        ann_filter = ann_filter or (lambda _: True)
 
         return {
             annotation.label
             for annotation in self.annotations
             if ann_filter(annotation)
         }
 
@@ -183,18 +186,18 @@
 @dataclass
 class InfoExtractionDataset:
     """Any number of Documents."""
 
     docs: list[Document]
     """ The annotated documents. """
 
-    default_qualifiers: dict[str, str] = None
+    default_qualifiers: Optional[dict[str, str]] = None
     """ Mapping of qualifiers to their default value, e.g. {"Negation": "Affirmed"}"""
 
-    def __post_init__(self):
+    def __post_init__(self) -> None:
         """
         Responsible for setting the default qualifiers by checking the default
         qualifiers set on Annotations, if set, or inferring them from the majority
         class otherwise.
         """
 
         self.default_qualifiers = {}
@@ -206,23 +209,55 @@
                         if qualifier["is_default"]:
                             self.default_qualifiers[qualifier["name"]] = qualifier[
                                 "value"
                             ]
         except KeyError:
             self.default_qualifiers = self.infer_default_qualifiers()
 
-    _ALL_STATS = [
+    _ALL_STATS: ClassVar[list] = [
         "num_docs",
         "num_annotations",
         "span_counts",
         "label_counts",
         "qualifier_counts",
     ]
     """ All methods to call when computing full dataset stats """
 
+    def infer_default_qualifiers(self) -> dict:
+        """
+        Infer the default values for qualifiers, based on the majority class, and
+        set this value on all annotations.
+
+        Returns
+        A dictionary with defaults, e.g. {"Negation": "Negated", "Experiencer":
+        "Patient"}.
+        -------
+        """
+
+        default_qualifiers = {
+            name: max(counts, key=lambda item: counts[item])
+            for name, counts in self.qualifier_counts().items()
+        }
+
+        warnings.warn(
+            f"Inferred the following qualifier defaults from the majority "
+            f"classes: {default_qualifiers}. ",
+            UserWarning,
+            stacklevel=2,
+        )
+
+        for doc in self.docs:
+            for annotation in doc.annotations:
+                for qualifier in annotation.qualifiers:
+                    qualifier["is_default"] = (
+                        default_qualifiers[qualifier["name"]] == qualifier["value"]
+                    )
+
+        return default_qualifiers
+
     @staticmethod
     def from_clinlp_docs(
         nlp_docs: Iterable[spacy.language.Doc], ids: Optional[Iterable[str]] = None
     ) -> "InfoExtractionDataset":
         """
         Creates a new dataset from clinlp output, by converting the spaCy Docs.
 
@@ -240,25 +275,23 @@
         ids = ids or itertools.count()
 
         docs = []
 
         for doc, identifier in zip(nlp_docs, ids):
             annotations = []
 
-            for ent in doc.ents:
-                qualifiers = []
-
-                for qualifier in ent._.qualifiers_dict:
-                    qualifiers.append(
-                        {
-                            "name": qualifier["name"].title(),
-                            "value": qualifier["value"].title(),
-                            "is_default": qualifier["is_default"],
-                        }
-                    )
+            for ent in doc.spans[SPANS_KEY]:
+                qualifiers = [
+                    {
+                        "name": qualifier.name.title(),
+                        "value": qualifier.value.title(),
+                        "is_default": qualifier.is_default,
+                    }
+                    for qualifier in ent._.qualifiers
+                ]
 
                 annotations.append(
                     Annotation(
                         text=str(ent),
                         start=ent.start_char,
                         end=ent.end_char,
                         label=ent.label_,
@@ -270,49 +303,18 @@
                 Document(
                     identifier=str(identifier), text=doc.text, annotations=annotations
                 )
             )
 
         return InfoExtractionDataset(docs=docs)
 
-    def infer_default_qualifiers(self) -> dict:
-        """
-        Infer the default values for qualifiers, based on the majority class, and
-        set this value on all annotations.
-
-        Returns
-        A dictionary with defaults, e.g. {"Negation": "Negated", "Experiencer":
-        "Patient"}.
-        -------
-        """
-
-        default_qualifiers = {
-            name: max(counts, key=lambda item: counts[item])
-            for name, counts in self.qualifier_counts().items()
-        }
-
-        warnings.warn(
-            f"Inferred the following qualifier defaults from the majority "
-            f"classes: {default_qualifiers}. ",
-            UserWarning,
-            stacklevel=2,
-        )
-
-        for doc in self.docs:
-            for annotation in doc.annotations:
-                for qualifier in annotation.qualifiers:
-                    qualifier["is_default"] = (
-                        default_qualifiers[qualifier["name"]] == qualifier["value"]
-                    )
-
-        return default_qualifiers
-
     @staticmethod
     def from_medcattrainer(
         data: dict,
+        *,
         strip_spans: bool = True,
         default_qualifiers: Optional[dict[str, str]] = None,
     ) -> "InfoExtractionDataset":
         """
         Creates a new dataset from medcattrainer output, by converting downloaded json.
 
         Parameters
@@ -328,17 +330,16 @@
         Returns
         -------
         A Dataset, corresponding to the provided data that medcattrainer produced.
 
         """
 
         if len(data["projects"]) > 1:
-            raise ValueError(
-                "Cannot read MedCATTrainer exports with more than 1 project."
-            )
+            msg = "Cannot read MedCATTrainer exports with more than 1 project."
+            raise ValueError(msg)
 
         data = data["projects"][0]
         docs = []
 
         for doc in data["documents"]:
             annotations = []
 
@@ -393,15 +394,15 @@
         if they should be included, False otherwise.
 
         Returns
         -------
         A nested list of dictionaries corresponding to annotations.
         """
 
-        ann_filter = ann_filter or (lambda ann: True)
+        ann_filter = ann_filter or (lambda _: True)
 
         return [doc.to_nervaluate(ann_filter) for doc in self.docs]
 
     def num_docs(self) -> int:
         """
         The number of documents in this dataset.
 
@@ -532,53 +533,59 @@
 
 class InfoExtractionMetrics:
     """
     Use this class to implement metrics comparing datasets.
     """
 
     """ Compute these metrics for qualifiers. """
-    _QUALIFIER_METRICS = {
+    _QUALIFIER_METRICS: ClassVar[dict[str, Callable]] = {
         "precision": precision_score,
         "recall": recall_score,
         "f1": f1_score,
     }
 
-    def __init__(self, true: InfoExtractionDataset, pred: InfoExtractionDataset):
+    def __init__(
+        self, true: InfoExtractionDataset, pred: InfoExtractionDataset
+    ) -> None:
         """
         Initialize metrics.
 
         Parameters
         ----------
         true: The dataset containing true (annotated/gold standard) annotations.
         pred: The dataset containing pred (predicted/inferred) annotations.
         """
         self.true = true
         self.pred = pred
 
         self._validate_self()
 
-    def _validate_self(self):
+    def _validate_self(self) -> None:
         """
         Validate the two datasets. Will raise an ValueError when datasets don't contain
         the same documents.
         """
         if self.true.num_docs() != self.pred.num_docs():
-            raise ValueError("Can only compute metrics for Datasets with same size")
+            msg = "Can only compute metrics for Datasets with same size"
+            raise ValueError(msg)
 
         for true_doc, pred_doc in zip(self.true.docs, self.pred.docs):
             if true_doc.identifier != pred_doc.identifier:
-                raise ValueError(
+                msg = (
                     "Found two documents with non-matching ids "
                     f"(true={true_doc.identifier}, pred={pred_doc.identifier}). "
                     "Please make sure to present the same documents, "
                     "in the same order."
                 )
 
+                raise ValueError(msg)
+
     def entity_metrics(
         self,
+        *,
         ann_filter: Optional[Callable[[Annotation], bool]] = None,
         classes: bool = False,
     ) -> dict:
         """
         Compute metrics for entities, including precision, recall and f1-score.
         Returns all measures for exact, strict, partial, and type matching, based on
         the nervaluate libary (for more information, see:
@@ -594,15 +601,15 @@
 
         Returns
         -------
         A dictionary containing the relevant metrics.
 
         """
 
-        ann_filter = ann_filter or (lambda ann: True)
+        ann_filter = ann_filter or (lambda _: True)
 
         true_anns = self.true.to_nervaluate(ann_filter)
         pred_anns = self.pred.to_nervaluate(ann_filter)
 
         labels = list(
             set.union(
                 *[doc.labels(ann_filter) for doc in self.true.docs + self.pred.docs]
@@ -635,15 +642,15 @@
                     {"doc.identifier": 1, annotation: {"start": 0, "end": 5, "text":
                     "test"}, true_label: "Affirmed", pred_label: "Negated"}, ...]
             },
             ...
         }
         """
 
-        aggregation = defaultdict(lambda: defaultdict(list))
+        aggregation: dict = defaultdict(lambda: defaultdict(list))
 
         for true_doc, pred_doc in zip(self.true.docs, self.pred.docs):
             for true_annotation in true_doc.annotations:
                 pred_annotation = pred_doc.get_annotation_from_span(
                     start=true_annotation.start, end=true_annotation.end
                 )
 
@@ -669,15 +676,15 @@
                                 "true_qualifier": true_val,
                                 "pred_qualifier": pred_val,
                             }
                         )
 
         return aggregation
 
-    def qualifier_metrics(self, misses: bool = True) -> dict:
+    def qualifier_metrics(self, *, misses: bool = True) -> dict:
         """
         Computes metrics for qualifiers, including precision, recall and f1-score.
         Only computes metrics for combinations of annotations with the same start
         and end char, but regardless of whether the labels match.
 
         Parameters
         ----------
@@ -693,15 +700,16 @@
         result = {}
 
         for name, values in aggregation.items():
             true_unique_values = set(values["true"])
             pred_unique_values = set(values["pred"])
 
             if max(len(true_unique_values), len(pred_unique_values)) > 2:
-                raise ValueError("Can oly compute metrics for binary qualifier values")
+                msg = "Can oly compute metrics for binary qualifier values"
+                raise ValueError(msg)
 
             pos_label = next(
                 val
                 for val in true_unique_values
                 if val != self.true.default_qualifiers[name]
             )
```

### Comparing `clinlp-0.7.0/src/clinlp/normalizer.py` & `clinlp-0.8.0/src/clinlp/normalizer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,50 +1,53 @@
 import unicodedata
 
-from spacy import Language
+from spacy.pipeline import Pipe
 from spacy.tokens import Doc
 
-from clinlp.util import clinlp_autocomponent
+from clinlp.util import clinlp_component
 
 _defaults_normalizer = {"lowercase": True, "map_non_ascii": True}
 
 
-@Language.factory(
-    "clinlp_normalizer", assigns=["token.norm"], default_config=_defaults_normalizer
+@clinlp_component(
+    name="clinlp_normalizer",
+    assigns=["token.norm"],
+    default_config=_defaults_normalizer,
 )
-@clinlp_autocomponent
-class Normalizer:
+class Normalizer(Pipe):
     def __init__(
         self,
-        lowercase=_defaults_normalizer["lowercase"],
-        map_non_ascii=_defaults_normalizer["map_non_ascii"],
-    ):
+        lowercase: bool = _defaults_normalizer["lowercase"],  # noqa FBT001
+        map_non_ascii: bool = _defaults_normalizer["map_non_ascii"],  # noqa FBT001
+    ) -> None:
         self.lowercase = lowercase
         self.map_non_ascii = map_non_ascii
 
     @staticmethod
     def _lowercase(text: str) -> str:
         return text.lower()
 
     @staticmethod
     def _map_non_ascii_char(char: str) -> str:
         if len(char) != 1:
-            raise ValueError(
-                "Please only use the _map_non_ascii_char method on strings of length 1."
+            msg = (
+                "Please only use the _map_non_ascii_char method "
+                "on strings of length 1."
             )
+            raise ValueError(msg)
 
         normalized_char = unicodedata.normalize("NFD", char)
         normalized_char = str(normalized_char.encode("ascii", "ignore").decode("utf-8"))
 
         return normalized_char if len(normalized_char) > 0 else char
 
     def _map_non_ascii_string(self, text: str) -> str:
         return "".join(self._map_non_ascii_char(char) for char in text)
 
-    def __call__(self, doc: Doc):
+    def __call__(self, doc: Doc) -> Doc:
         if len(doc) == 0:
             return doc
 
         for token in doc:
             normalized_text = token.text
 
             if self.lowercase:
```

### Comparing `clinlp-0.7.0/src/clinlp/resources/context_rules.json` & `clinlp-0.8.0/src/clinlp/resources/context_rules.json`

 * *Files identical despite different names*

### Comparing `clinlp-0.7.0/src/clinlp/sentencizer.py` & `clinlp-0.8.0/src/clinlp/sentencizer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,63 +1,59 @@
 from typing import Optional
 
-import spacy.tokens
-from spacy.language import Language
+from spacy.pipeline import Pipe
+from spacy.tokens import Doc, Token
 
-from clinlp.util import clinlp_autocomponent
+from clinlp.util import clinlp_component
 
 _defaults_sentencizer = {
     "sent_end_chars": [".", "!", "?", "\n", "\r"],
     "sent_start_punct": ["-", "*", "[", "("],
 }
 
 
-@Language.factory(
-    "clinlp_sentencizer",
+@clinlp_component(
+    name="clinlp_sentencizer",
     assigns=["token.is_sent_start", "doc.sents"],
     default_config=_defaults_sentencizer,
 )
-@clinlp_autocomponent
-class Sentencizer:
+class Sentencizer(Pipe):
     def __init__(
         self,
         sent_end_chars: Optional[list[str]] = None,
         sent_start_punct: Optional[list[str]] = None,
-    ):
-        self.sent_end_chars = (
+    ) -> None:
+        self.sent_end_chars = set(
             _defaults_sentencizer["sent_end_chars"]
             if sent_end_chars is None
             else sent_end_chars
         )
-        self.sent_start_punct = (
+        self.sent_start_punct = set(
             _defaults_sentencizer["sent_start_punct"]
             if sent_start_punct is None
             else sent_start_punct
         )
 
-        self.sent_end_chars = set(self.sent_end_chars)
-        self.sent_start_punct = set(self.sent_start_punct)
-
-    def _token_can_start_sent(self, token: spacy.tokens.Token) -> bool:
+    def _token_can_start_sent(self, token: Token) -> bool:
         """
         Determines whether a token can start a sentence
         """
         return (
             token.text[0].isalnum()
             or (token.text[0] in {"["})
             or (token.text in self.sent_start_punct)
         )
 
-    def _token_can_end_sent(self, token: spacy.tokens.Token):
+    def _token_can_end_sent(self, token: Token) -> bool:
         """
         Determines whether a token can end a sentence
         """
         return token.text in self.sent_end_chars
 
-    def _get_sentence_starts(self, doc: spacy.tokens.Doc) -> list[bool]:
+    def _get_sentence_starts(self, doc: Doc) -> list[bool]:
         if len(doc) == 0:
             return []
 
         sentence_starts = [False] * len(doc)
 
         if self._token_can_start_sent(doc[0]):
             sentence_starts[0] = True
@@ -70,15 +66,15 @@
                 seen_end_char = False
 
             if self._token_can_end_sent(token):
                 seen_end_char = True
 
         return sentence_starts
 
-    def __call__(self, doc: spacy.tokens.Doc):
+    def __call__(self, doc: Doc) -> Doc:
         if len(doc) == 0:
             return doc
 
         sentence_starts = self._get_sentence_starts(doc)
 
         for is_sent_start, token in zip(sentence_starts, doc):
             token.is_sent_start = is_sent_start
```

### Comparing `clinlp-0.7.0/src/clinlp/util.py` & `clinlp-0.8.0/src/clinlp/util.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import inspect
 from inspect import Parameter, Signature
+from typing import Callable, Tuple, Type
 
 from makefun import with_signature
+from spacy.language import Language
 
 
 class _UnusedArgument:
     pass
 
 
-def get_class_init_signature(cls):
+def get_class_init_signature(cls: Type) -> Tuple[list, dict]:
     args = []
     kwargs = {}
 
     for mro_class in cls.__mro__:
         if "__init__" in mro_class.__dict__:
             argspec = inspect.getfullargspec(mro_class)
 
@@ -24,54 +26,60 @@
                 kwargs |= dict(
                     zip(argspec.args[first_arg_wit_default:], argspec.defaults)
                 )
 
     return args, kwargs
 
 
-def clinlp_autocomponent(cls):
-    component_args, component_kwargs = get_class_init_signature(cls)
+def clinlp_component(*args, register: bool = True, **kwargs) -> Callable:
+    def _clinlp_component(cls: Type) -> Callable:
+        component_args, component_kwargs = get_class_init_signature(cls)
 
-    params = []
+        make_component_args = component_args.copy()
 
-    make_component_args = component_args.copy()
+        if "nlp" not in make_component_args:
+            make_component_args = ["nlp", *make_component_args]
 
-    if "nlp" not in make_component_args:
-        make_component_args = ["nlp"] + make_component_args
+        if "name" not in make_component_args:
+            make_component_args = ["name", *make_component_args]
 
-    if "name" not in make_component_args:
-        make_component_args = ["name"] + make_component_args
-
-    for arg in make_component_args:
-        params.append(
+        params = [
             Parameter(
                 arg, kind=Parameter.POSITIONAL_OR_KEYWORD, default=_UnusedArgument()
             )
-        )
+            for arg in make_component_args
+        ]
+
+        for kwarg, default in component_kwargs.items():
+            params.append(
+                Parameter(kwarg, kind=Parameter.POSITIONAL_OR_KEYWORD, default=default)
+            )
+
+        @with_signature(Signature(params), func_name="make_component")
+        def make_component(*args, **kwargs) -> Type:
+            if len(args) > 0:
+                msg = "Please pass all arguments as keywords."
+                raise RuntimeError(msg)
+
+            cls_kwargs = {
+                k: v
+                for k, v in kwargs.items()
+                if (k in component_args or k in component_kwargs)
+                and (not isinstance(v, _UnusedArgument))
+            }
+
+            return cls(**cls_kwargs)
 
-    for kwarg, default in component_kwargs.items():
-        params.append(
-            Parameter(kwarg, kind=Parameter.POSITIONAL_OR_KEYWORD, default=default)
-        )
-
-    @with_signature(Signature(params), func_name="make_component")
-    def make_component(*args, **kwargs):
-        if len(args) > 0:
-            raise RuntimeError("Please pass all arguments as keywords.")
-
-        cls_kwargs = {
-            k: v
-            for k, v in kwargs.items()
-            if (k in component_args or k in component_kwargs)
-            and (not isinstance(v, _UnusedArgument))
-        }
+        if register:
+            Language.factory(*args, func=make_component, **kwargs)
 
-        return cls(**cls_kwargs)
+        return make_component
 
-    return make_component
+    return _clinlp_component
 
 
 def interval_dist(start_a: int, end_a: int, start_b: int, end_b: int) -> int:
     if (end_a < start_a) or (end_b < start_b):
-        raise ValueError("Input malformed interval.")
+        msg = "Input malformed interval."
+        raise ValueError(msg)
 
     return max(0, start_a - end_b, start_b - end_a)
```

### Comparing `clinlp-0.7.0/PKG-INFO` & `clinlp-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clinlp
-Version: 0.7.0
+Version: 0.8.0
 Summary: Performant and production-ready NLP pipelines for clinical text written in Dutch
 Author: UMCU DIT Analytics
 Author-email: analytics@umcutrecht.nl
 Requires-Python: >=3.10,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -70,15 +70,15 @@
         "hypotensie", Term("bd verlaagd", proximity=1)
     ],
     "veneus_infarct": [
         "veneus infarct", Term("VI", attr="TEXT")
     ]
 }
 
-entity_matcher = nlp.add_pipe("clinlp_entity_matcher", config={"attr": "NORM", "fuzzy": 1})
+entity_matcher = nlp.add_pipe("clinlp_rule_based_entity_matcher", config={"attr": "NORM", "fuzzy": 1})
 entity_matcher.load_concepts(concepts)
 
 # Qualifiers
 nlp.add_pipe("clinlp_context_algorithm", config={"phrase_matcher_attr": "NORM"})
 
 text = (
     "Preterme neonaat (<p3), bd enigszins verlaagd, familieanamnese vermeldt eveneens hypotensie "
@@ -98,15 +98,15 @@
 ```
 
 ![example_doc_render.png](media/example_doc_render.png)
 
 With relevant qualifiers (defaults omitted for readability):
 
 ```python
-for ent in doc.ents:
+for ent in doc.spans["ents"]:
   print(ent, ent._.qualifiers_str)
 ```
 
 * `Preterme` `set()`
 * `<p3` `set()`
 * `bd enigszins verlaagd` `set()`
 * `hypotensie` `{'Experiencer.Family'}`
@@ -168,15 +168,15 @@
 nlp.add_pipe("clinlp_sentencizer")
 ```
 
 It is designed to detect sentence boundaries in clinical text, whenever a character that demarks a sentence ending is matched (e.g. newline, period, question mark). It also correctly detects items in an enumerations (e.g. starting with `-` or `*`). 
 
 ### Entity matcher
 
-`clinlp` includes a `clinlp_entity_matcher` component that can be used for matching entities in text, based on a dictionary of known concepts and their terms/synonyms. It includes options for matching on different token attributes, proximity matching, fuzzy matching and matching pseudo/negative terms. 
+`clinlp` includes a `clinlp_rule_based_entity_matcher` component that can be used for matching entities in text, based on a dictionary of known concepts and their terms/synonyms. It includes options for matching on different token attributes, proximity matching, fuzzy matching and matching pseudo/negative terms. 
 
 The most basic example would be the following, with further options described below:
 
 ```python
 concepts = {
     "sepsis": [
         "sepsis",
@@ -186,50 +186,56 @@
     ],
     "veneus_infarct": [
         "veneus infarct",
         "VI",
     ]
 }
 
-entity_matcher = nlp.add_pipe("clinlp_entity_matcher")
+entity_matcher = nlp.add_pipe("clinlp_rule_based_entity_matcher")
 entity_matcher.load_concepts(concepts)
-
 ```
-> :bulb: The `clinlp_entity_matcher` component wraps the spaCy `Matcher` and `PhraseMatcher` components, adding some convenience and configurability. However, the `Matcher`, `PhraseMatcher` or `EntityRuler` can also be used directly with `clinlp` for those who prefer it.
+
+> :bulb: `clinlp` stores entities in `doc.spans`, specifically in `doc.spans["ents"]`. The reason for this is that spans can overlap, while the entities in `doc.ents` cannot. If you use other/custom components, make sure they read/write entities from/to the same span key if interoperability is needed.
+
+> :bulb: The `clinlp_rule_based_entity_matcher` component wraps the spaCy `Matcher` and `PhraseMatcher` components, adding some convenience and configurability. However, the `Matcher`, `PhraseMatcher` or `SpanRuler` can also be used directly with `clinlp` for those who prefer it. You can configure the `SpanRuler` to write to the same `SpanGroup` as follows: 
+> ```python
+> from clinlp.ie import SPAN_KEY
+> ruler = nlp.add_pipe('span_ruler', config={'span_key': SPAN_KEY})
+> ```
 
 #### Attribute
 
 Specify the token attribute the entity matcher should use as follows (by default `TEXT`):
 
 ```python
-entity_matcher = nlp.add_pipe("clinlp_entity_matcher", config={"attr": "NORM"})
+entity_matcher = nlp.add_pipe("clinlp_rule_based_entity_matcher", config={"attr": "NORM"})
 ```
 
 Any [Token attribute](https://spacy.io/api/token#attributes) can be used, but in the above example the `clinlp_normalizer` should be added before the entity matcher, or the `NORM` attribute is simply the literal text. `clinlp` does not include Part of Speech tags and dependency trees, at least not until a reliable model for Dutch clinical text is created, though it's always possible to add a relevant component from a trained (general) Dutch model if needed.
 
 #### Proximity matching
 
 The proxmity setting defines how many tokens can optionally be skipped between the tokens of a pattern. With `proxmity` set to `1`, the pattern `slaapt slecht` will also match `slaapt vaak slecht`, but not `slaapt al weken slecht`. 
 
 ```python
-entity_matcher = nlp.add_pipe("clinlp_entity_matcher", config={"proximity": 1})
+entity_matcher = nlp.add_pipe("clinlp_rule_based_entity_matcher", config={"proximity": 1})
 ```
 
 #### Fuzzy matching
 
 Fuzzy matching enables finding misspelled variants of terms. For instance, with `fuzzy` set to `1`, the pattern `diabetes` will also match `diabets`, `ddiabetes`, or `diabetis`, but not `diabetse` or `ddiabetess`. The threshold is based on Levenshtein distance with insertions, deletions and replacements (but not swaps).  
 
 ```python
-entity_matcher = nlp.add_pipe("clinlp_entity_matcher", config={"fuzzy": 1})
+entity_matcher = nlp.add_pipe("clinlp_rule_based_entity_matcher", config={"fuzzy": 1})
 ```
 
 Additionally, the `fuzzy_min_len` argument can be used to specify the minimum length of a phrase for fuzzy matching. This also works for multi-token phrases. For example, with `fuzzy` set to `1` and `fuzzy_min_len` set to `5`, the pattern `bloeding graad ii` would also match `bloedin graad ii`, but not `bloeding graad iii`. 
 
 ```python
-entity_matcher = nlp.add_pipe("clinlp_entity_matcher", config={"fuzzy": 1, "fuzzy_min_len": 5})
+entity_matcher = nlp.add_pipe("clinlp_rule_based_entity_matcher", config={"fuzzy": 1, "fuzzy_min_len": 5})
 ```
 
 #### Terms
 The settings above are described at the matcher level, but can all be overridden at the term level by adding a `Term` to a concept, rather than a literal phrase:
 
 ```python
 from clinlp.ie import Term
@@ -241,15 +247,15 @@
         Term("early onset", proximity=1),
         Term("late onset", proximity=1),
         Term("EOS", attr="TEXT", fuzzy=0),
         Term("LOS", attr="TEXT", fuzzy=0)
     ]
 }
 
-entity_matcher = nlp.add_pipe("clinlp_entity_matcher", config={"attr": "NORM", "fuzzy": 1})
+entity_matcher = nlp.add_pipe("clinlp_rule_based_entity_matcher", config={"attr": "NORM", "fuzzy": 1})
 entity_matcher.load_concepts(concepts)
 ```
 
 In the above example, by default the `NORM` attribute is used, and `fuzzy` is set to `1`. In addition, for the terms `early onset` and `late onset` proximity matching is set to `1`, in addition to matcher-level config of matching the `NORM` attribute and fuzzy matching. For the `EOS` and `LOS` abbreviations the `TEXT` attribute is used (so the matching is case sensitive), and fuzzy matching is disabled. 
 
 #### Pseudo/negative phrases
```

