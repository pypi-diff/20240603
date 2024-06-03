# Comparing `tmp/ponytail-agents-0.1.6.tar.gz` & `tmp/ponytail-agents-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ponytail-agents-0.1.6.tar", last modified: Sat Jun  1 14:20:37 2024, max compression
+gzip compressed data, was "ponytail-agents-0.1.7.tar", last modified: Mon Jun  3 10:00:56 2024, max compression
```

## Comparing `ponytail-agents-0.1.6.tar` & `ponytail-agents-0.1.7.tar`

### file list

```diff
@@ -1,120 +1,120 @@
-drwxrwxrwx   0        0        0        0 2024-06-01 14:20:37.473855 ponytail-agents-0.1.6/
--rw-rw-rw-   0        0        0     3774 2024-05-28 10:54:43.000000 ponytail-agents-0.1.6/LICENSE
--rw-rw-rw-   0        0        0     3622 2024-06-01 14:20:37.470559 ponytail-agents-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     3172 2024-06-01 14:19:46.000000 ponytail-agents-0.1.6/README.md
-drwxrwxrwx   0        0        0        0 2024-06-01 14:20:37.203415 ponytail-agents-0.1.6/ponytAIl/
--rw-rw-rw-   0        0        0        0 2024-05-30 10:37:23.000000 ponytail-agents-0.1.6/ponytAIl/__init__.py
--rw-rw-rw-   0        0        0     9959 2024-06-01 14:09:47.000000 ponytail-agents-0.1.6/ponytAIl/main.py
-drwxrwxrwx   0        0        0        0 2024-06-01 14:20:37.212534 ponytail-agents-0.1.6/ponytAIl/nodes_sample/
--rw-rw-rw-   0        0        0      792 2024-05-22 06:08:35.000000 ponytail-agents-0.1.6/ponytAIl/nodes_sample/concluder.md
--rw-rw-rw-   0        0        0     2084 2024-05-31 12:27:26.000000 ponytail-agents-0.1.6/ponytAIl/nodes_sample/medium_sample.md
--rw-rw-rw-   0        0        0     2863 2024-05-31 12:25:31.000000 ponytail-agents-0.1.6/ponytAIl/nodes_sample/node_creator.md
--rw-rw-rw-   0        0        0     1524 2024-05-31 12:27:26.000000 ponytail-agents-0.1.6/ponytAIl/nodes_sample/starter.md
-drwxrwxrwx   0        0        0        0 2024-06-01 14:20:37.226189 ponytail-agents-0.1.6/ponytAIl/nodes_sample_definition_of_one/
--rw-rw-rw-   0        0        0      792 2024-05-22 06:08:35.000000 ponytail-agents-0.1.6/ponytAIl/nodes_sample_definition_of_one/concluder.md
--rw-rw-rw-   0        0        0     2995 2024-05-30 17:13:59.000000 ponytail-agents-0.1.6/ponytAIl/nodes_sample_definition_of_one/example_generator.md
--rw-rw-rw-   0        0        0     2243 2024-05-30 17:13:48.000000 ponytail-agents-0.1.6/ponytAIl/nodes_sample_definition_of_one/math_concept_definition.md
--rw-rw-rw-   0        0        0     2084 2024-05-31 12:27:26.000000 ponytail-agents-0.1.6/ponytAIl/nodes_sample_definition_of_one/medium_sample.md
--rw-rw-rw-   0        0        0     2863 2024-05-31 12:25:31.000000 ponytail-agents-0.1.6/ponytAIl/nodes_sample_definition_of_one/node_creator.md
--rw-rw-rw-   0        0        0     1524 2024-05-31 12:27:26.000000 ponytail-agents-0.1.6/ponytAIl/nodes_sample_definition_of_one/starter.md
-drwxrwxrwx   0        0        0        0 2024-06-01 14:20:37.239061 ponytail-agents-0.1.6/ponytAIl/nodes_sample_ponytail/
--rw-rw-rw-   0        0        0      792 2024-05-22 06:08:35.000000 ponytail-agents-0.1.6/ponytAIl/nodes_sample_ponytail/concluder.md
--rw-rw-rw-   0        0        0     2084 2024-05-31 12:27:26.000000 ponytail-agents-0.1.6/ponytAIl/nodes_sample_ponytail/medium_sample.md
--rw-rw-rw-   0        0        0     2647 2024-05-30 17:22:26.000000 ponytail-agents-0.1.6/ponytAIl/nodes_sample_ponytail/name_combiner.md
--rw-rw-rw-   0        0        0     2907 2024-05-30 17:22:19.000000 ponytail-agents-0.1.6/ponytAIl/nodes_sample_ponytail/name_generator.md
--rw-rw-rw-   0        0        0     2863 2024-05-31 12:25:31.000000 ponytail-agents-0.1.6/ponytAIl/nodes_sample_ponytail/node_creator.md
--rw-rw-rw-   0        0        0     1524 2024-05-31 12:27:26.000000 ponytail-agents-0.1.6/ponytAIl/nodes_sample_ponytail/starter.md
-drwxrwxrwx   0        0        0        0 2024-06-01 14:20:37.270367 ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers/
--rw-rw-rw-   0        0        0     2794 2024-05-30 18:17:11.000000 ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers/anita_kumar.md
--rw-rw-rw-   0        0        0      792 2024-05-22 06:08:35.000000 ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers/concluder.md
--rw-rw-rw-   0        0        0     2783 2024-05-30 18:18:55.000000 ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers/david_brown.md
--rw-rw-rw-   0        0        0     8490 2024-05-30 18:18:14.000000 ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers/gloria_martinez.md
--rw-rw-rw-   0        0        0     2932 2024-05-30 18:16:25.000000 ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers/john_smith.md
--rw-rw-rw-   0        0        0     3130 2024-05-30 18:17:04.000000 ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers/kevin_white.md
--rw-rw-rw-   0        0        0     3438 2024-05-30 18:17:19.000000 ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers/li_wang.md
--rw-rw-rw-   0        0        0     4292 2024-05-30 18:16:57.000000 ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers/maria_garcia.md
--rw-rw-rw-   0        0        0     2084 2024-05-31 12:27:26.000000 ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers/medium_sample.md
--rw-rw-rw-   0        0        0     4035 2024-05-30 18:18:35.000000 ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers/michael_clark.md
--rw-rw-rw-   0        0        0     2863 2024-05-31 12:25:31.000000 ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers/node_creator.md
--rw-rw-rw-   0        0        0     3697 2024-05-30 18:16:49.000000 ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers/sarah_johnson.md
--rw-rw-rw-   0        0        0     1524 2024-05-31 12:27:26.000000 ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers/starter.md
--rw-rw-rw-   0        0        0     5167 2024-05-30 18:18:44.000000 ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers/yuki_tanaka.md
-drwxrwxrwx   0        0        0        0 2024-06-01 14:20:37.320083 ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_2/
--rw-rw-rw-   0        0        0     2853 2024-05-30 18:28:28.000000 ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_2/Ahmed_El-Sayed.md
--rw-rw-rw-   0        0        0     4853 2024-05-30 18:27:50.000000 ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_2/Aisha_Khan.md
--rw-rw-rw-   0        0        0     2215 2024-05-30 18:33:14.000000 ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_2/Carlos_Mendez.md
--rw-rw-rw-   0        0        0     4732 2024-05-30 18:29:06.000000 ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_2/Elena_Petrov.md
--rw-rw-rw-   0        0        0     4884 2024-05-30 18:28:20.000000 ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_2/Emily_Johnson.md
--rw-rw-rw-   0        0        0     5106 2024-05-30 18:33:41.000000 ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_2/Emma_Jones.md
--rw-rw-rw-   0        0        0     6670 2024-05-30 18:33:04.000000 ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_2/Fatou_Sangare.md
--rw-rw-rw-   0        0        0     2418 2024-05-30 18:27:58.000000 ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_2/Haruto_Yamamoto.md
--rw-rw-rw-   0        0        0     4207 2024-05-30 18:27:31.000000 ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_2/John_Smith.md
--rw-rw-rw-   0        0        0     3226 2024-05-30 18:33:22.000000 ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_2/Keisha_Anderson.md
--rw-rw-rw-   0        0        0     3599 2024-05-30 18:27:38.000000 ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_2/Maria_Gonzalez.md
--rw-rw-rw-   0        0        0     3967 2024-05-30 18:33:31.000000 ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_2/Mohammed_Al-Farsi.md
--rw-rw-rw-   0        0        0     2620 2024-05-30 18:28:57.000000 ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_2/Olusegun_Adeyemi.md
--rw-rw-rw-   0        0        0     3278 2024-05-30 18:28:36.000000 ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_2/Sofia_Rossi.md
--rw-rw-rw-   0        0        0     4576 2024-05-30 18:28:45.000000 ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_2/Wei_Liu.md
--rw-rw-rw-   0        0        0     2359 2024-05-30 18:32:53.000000 ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_2/Zhang_Wei.md
--rw-rw-rw-   0        0        0      792 2024-05-22 06:08:35.000000 ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_2/concluder.md
--rw-rw-rw-   0        0        0     2232 2024-05-30 18:43:18.000000 ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_2/math_assessment.md
--rw-rw-rw-   0        0        0     2084 2024-05-31 12:27:26.000000 ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_2/medium_sample.md
--rw-rw-rw-   0        0        0     2863 2024-05-31 12:25:31.000000 ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_2/node_creator.md
--rw-rw-rw-   0        0        0     1524 2024-05-31 12:27:26.000000 ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_2/starter.md
-drwxrwxrwx   0        0        0        0 2024-06-01 14:20:37.351180 ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_3/
--rw-rw-rw-   0        0        0     2059 2024-05-31 12:23:33.000000 ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_3/blacksmith_emily.md
--rw-rw-rw-   0        0        0     2831 2024-05-31 12:28:39.000000 ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_3/blacksmith_tomas.md
--rw-rw-rw-   0        0        0      792 2024-05-22 06:08:35.000000 ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_3/concluder.md
--rw-rw-rw-   0        0        0     4337 2024-05-31 12:28:20.000000 ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_3/farmer_jane.md
--rw-rw-rw-   0        0        0     2998 2024-05-31 12:22:54.000000 ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_3/farmer_john.md
--rw-rw-rw-   0        0        0     2084 2024-05-31 12:27:26.000000 ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_3/medium_sample.md
--rw-rw-rw-   0        0        0     5227 2024-05-31 12:29:41.000000 ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_3/merchant_sophia.md
--rw-rw-rw-   0        0        0     2863 2024-05-31 12:25:31.000000 ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_3/node_creator.md
--rw-rw-rw-   0        0        0     4254 2024-05-31 12:28:46.000000 ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_3/seamstress_maria.md
--rw-rw-rw-   0        0        0     4589 2024-05-31 12:23:14.000000 ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_3/seamstress_sarah.md
--rw-rw-rw-   0        0        0     1524 2024-05-31 12:27:26.000000 ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_3/starter.md
--rw-rw-rw-   0        0        0     3858 2024-05-31 12:29:47.000000 ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_3/teacher_daniel.md
--rw-rw-rw-   0        0        0     5001 2024-05-31 12:29:22.000000 ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_3/woodcarver_lucas.md
--rw-rw-rw-   0        0        0     2776 2024-05-31 12:23:24.000000 ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_3/woodcarver_max.md
-drwxrwxrwx   0        0        0        0 2024-06-01 14:20:37.426937 ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_4/
--rw-rw-rw-   0        0        0     3293 2024-06-01 12:55:43.000000 ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_4/aaron_davis.md
--rw-rw-rw-   0        0        0     4559 2024-06-01 12:50:08.000000 ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_4/abdul_rahman.md
--rw-rw-rw-   0        0        0     3884 2024-06-01 12:49:39.000000 ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_4/alice_smith.md
--rw-rw-rw-   0        0        0     2533 2024-06-01 12:50:42.000000 ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_4/anika_singh.md
--rw-rw-rw-   0        0        0     4072 2024-06-01 12:49:45.000000 ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_4/carlos_garcia.md
--rw-rw-rw-   0        0        0      792 2024-05-22 06:08:35.000000 ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_4/concluder.md
--rw-rw-rw-   0        0        0     2381 2024-06-01 12:54:42.000000 ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_4/david_hernandez.md
--rw-rw-rw-   0        0        0     3282 2024-06-01 12:49:51.000000 ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_4/emily_johnson.md
--rw-rw-rw-   0        0        0    15863 2024-06-01 12:55:37.000000 ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_4/fatima_zaidi.md
--rw-rw-rw-   0        0        0     4484 2024-06-01 13:03:19.000000 ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_4/grace_anderson.md
--rw-rw-rw-   0        0        0     3837 2024-06-01 13:02:55.000000 ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_4/isabella_rodriguez.md
--rw-rw-rw-   0        0        0     3449 2024-06-01 12:54:38.000000 ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_4/jacqueline_miller.md
--rw-rw-rw-   0        0        0     3856 2024-06-01 13:02:49.000000 ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_4/james_mitchell.md
--rw-rw-rw-   0        0        0     2977 2024-06-01 13:03:47.000000 ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_4/jason_turner.md
--rw-rw-rw-   0        0        0     3016 2024-06-01 12:49:29.000000 ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_4/john_doe.md
--rw-rw-rw-   0        0        0     7485 2024-06-01 12:55:05.000000 ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_4/li_yan.md
--rw-rw-rw-   0        0        0     2670 2024-06-01 13:03:39.000000 ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_4/linda_thompson.md
--rw-rw-rw-   0        0        0     2802 2024-06-01 12:50:35.000000 ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_4/lucas_kim.md
--rw-rw-rw-   0        0        0     3348 2024-06-01 12:50:28.000000 ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_4/marie_dubois.md
--rw-rw-rw-   0        0        0     2084 2024-05-31 12:27:26.000000 ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_4/medium_sample.md
--rw-rw-rw-   0        0        0     3900 2024-06-01 12:54:32.000000 ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_4/michael_lee.md
--rw-rw-rw-   0        0        0     2863 2024-05-31 12:25:31.000000 ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_4/node_creator.md
--rw-rw-rw-   0        0        0     4064 2024-06-01 12:50:22.000000 ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_4/oliver_taylor.md
--rw-rw-rw-   0        0        0     5337 2024-06-01 13:02:42.000000 ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_4/olivia_jones.md
--rw-rw-rw-   0        0        0     4453 2024-06-01 12:54:50.000000 ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_4/rachel_green.md
--rw-rw-rw-   0        0        0     3405 2024-06-01 13:03:01.000000 ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_4/ryan_clark.md
--rw-rw-rw-   0        0        0     4935 2024-06-01 13:03:33.000000 ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_4/samuel_brown.md
--rw-rw-rw-   0        0        0     3749 2024-06-01 12:55:51.000000 ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_4/sandra_brown.md
--rw-rw-rw-   0        0        0     1894 2024-06-01 12:54:21.000000 ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_4/sophia_khan.md
--rw-rw-rw-   0        0        0     1524 2024-05-31 12:27:26.000000 ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_4/starter.md
--rw-rw-rw-   0        0        0     5606 2024-06-01 12:56:09.000000 ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_4/thomas_evans.md
--rw-rw-rw-   0        0        0     5299 2024-06-01 12:50:15.000000 ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_4/ying_chen.md
-drwxrwxrwx   0        0        0        0 2024-06-01 14:20:37.468740 ponytail-agents-0.1.6/ponytail_agents.egg-info/
--rw-rw-rw-   0        0        0     3622 2024-06-01 14:20:36.000000 ponytail-agents-0.1.6/ponytail_agents.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     5091 2024-06-01 14:20:37.000000 ponytail-agents-0.1.6/ponytail_agents.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-01 14:20:36.000000 ponytail-agents-0.1.6/ponytail_agents.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2024-06-01 14:20:36.000000 ponytail-agents-0.1.6/ponytail_agents.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       68 2024-06-01 14:20:37.000000 ponytail-agents-0.1.6/ponytail_agents.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-06-01 14:20:37.000000 ponytail-agents-0.1.6/ponytail_agents.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-06-01 14:20:37.473855 ponytail-agents-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0     1023 2024-06-01 14:20:29.000000 ponytail-agents-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-03 10:00:56.554994 ponytail-agents-0.1.7/
+-rw-rw-rw-   0        0        0     3774 2024-05-28 10:54:43.000000 ponytail-agents-0.1.7/LICENSE
+-rw-rw-rw-   0        0        0     4658 2024-06-03 10:00:56.554994 ponytail-agents-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     4208 2024-06-03 09:51:25.000000 ponytail-agents-0.1.7/README.md
+drwxrwxrwx   0        0        0        0 2024-06-03 10:00:55.771307 ponytail-agents-0.1.7/ponytAIl/
+-rw-rw-rw-   0        0        0        0 2024-05-30 10:37:23.000000 ponytail-agents-0.1.7/ponytAIl/__init__.py
+-rw-rw-rw-   0        0        0    11112 2024-06-03 09:51:25.000000 ponytail-agents-0.1.7/ponytAIl/main.py
+drwxrwxrwx   0        0        0        0 2024-06-03 10:00:55.807601 ponytail-agents-0.1.7/ponytAIl/nodes_sample/
+-rw-rw-rw-   0        0        0      792 2024-05-22 06:08:35.000000 ponytail-agents-0.1.7/ponytAIl/nodes_sample/concluder.md
+-rw-rw-rw-   0        0        0     2084 2024-05-31 12:27:26.000000 ponytail-agents-0.1.7/ponytAIl/nodes_sample/medium_sample.md
+-rw-rw-rw-   0        0        0     2863 2024-05-31 12:25:31.000000 ponytail-agents-0.1.7/ponytAIl/nodes_sample/node_creator.md
+-rw-rw-rw-   0        0        0     1524 2024-05-31 12:27:26.000000 ponytail-agents-0.1.7/ponytAIl/nodes_sample/starter.md
+drwxrwxrwx   0        0        0        0 2024-06-03 10:00:55.838908 ponytail-agents-0.1.7/ponytAIl/nodes_sample_definition_of_one/
+-rw-rw-rw-   0        0        0      792 2024-05-22 06:08:35.000000 ponytail-agents-0.1.7/ponytAIl/nodes_sample_definition_of_one/concluder.md
+-rw-rw-rw-   0        0        0     2995 2024-05-30 17:13:59.000000 ponytail-agents-0.1.7/ponytAIl/nodes_sample_definition_of_one/example_generator.md
+-rw-rw-rw-   0        0        0     2243 2024-05-30 17:13:48.000000 ponytail-agents-0.1.7/ponytAIl/nodes_sample_definition_of_one/math_concept_definition.md
+-rw-rw-rw-   0        0        0     2084 2024-05-31 12:27:26.000000 ponytail-agents-0.1.7/ponytAIl/nodes_sample_definition_of_one/medium_sample.md
+-rw-rw-rw-   0        0        0     2863 2024-05-31 12:25:31.000000 ponytail-agents-0.1.7/ponytAIl/nodes_sample_definition_of_one/node_creator.md
+-rw-rw-rw-   0        0        0     1524 2024-05-31 12:27:26.000000 ponytail-agents-0.1.7/ponytAIl/nodes_sample_definition_of_one/starter.md
+drwxrwxrwx   0        0        0        0 2024-06-03 10:00:55.870554 ponytail-agents-0.1.7/ponytAIl/nodes_sample_ponytail/
+-rw-rw-rw-   0        0        0      792 2024-05-22 06:08:35.000000 ponytail-agents-0.1.7/ponytAIl/nodes_sample_ponytail/concluder.md
+-rw-rw-rw-   0        0        0     2084 2024-05-31 12:27:26.000000 ponytail-agents-0.1.7/ponytAIl/nodes_sample_ponytail/medium_sample.md
+-rw-rw-rw-   0        0        0     2647 2024-05-30 17:22:26.000000 ponytail-agents-0.1.7/ponytAIl/nodes_sample_ponytail/name_combiner.md
+-rw-rw-rw-   0        0        0     2907 2024-05-30 17:22:19.000000 ponytail-agents-0.1.7/ponytAIl/nodes_sample_ponytail/name_generator.md
+-rw-rw-rw-   0        0        0     2863 2024-05-31 12:25:31.000000 ponytail-agents-0.1.7/ponytAIl/nodes_sample_ponytail/node_creator.md
+-rw-rw-rw-   0        0        0     1524 2024-05-31 12:27:26.000000 ponytail-agents-0.1.7/ponytAIl/nodes_sample_ponytail/starter.md
+drwxrwxrwx   0        0        0        0 2024-06-03 10:00:55.972627 ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers/
+-rw-rw-rw-   0        0        0     2794 2024-05-30 18:17:11.000000 ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers/anita_kumar.md
+-rw-rw-rw-   0        0        0      792 2024-05-22 06:08:35.000000 ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers/concluder.md
+-rw-rw-rw-   0        0        0     2783 2024-05-30 18:18:55.000000 ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers/david_brown.md
+-rw-rw-rw-   0        0        0     8490 2024-05-30 18:18:14.000000 ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers/gloria_martinez.md
+-rw-rw-rw-   0        0        0     2932 2024-05-30 18:16:25.000000 ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers/john_smith.md
+-rw-rw-rw-   0        0        0     3130 2024-05-30 18:17:04.000000 ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers/kevin_white.md
+-rw-rw-rw-   0        0        0     3438 2024-05-30 18:17:19.000000 ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers/li_wang.md
+-rw-rw-rw-   0        0        0     4292 2024-05-30 18:16:57.000000 ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers/maria_garcia.md
+-rw-rw-rw-   0        0        0     2084 2024-05-31 12:27:26.000000 ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers/medium_sample.md
+-rw-rw-rw-   0        0        0     4035 2024-05-30 18:18:35.000000 ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers/michael_clark.md
+-rw-rw-rw-   0        0        0     2863 2024-05-31 12:25:31.000000 ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers/node_creator.md
+-rw-rw-rw-   0        0        0     3697 2024-05-30 18:16:49.000000 ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers/sarah_johnson.md
+-rw-rw-rw-   0        0        0     1524 2024-05-31 12:27:26.000000 ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers/starter.md
+-rw-rw-rw-   0        0        0     5167 2024-05-30 18:18:44.000000 ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers/yuki_tanaka.md
+drwxrwxrwx   0        0        0        0 2024-06-03 10:00:56.148019 ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_2/
+-rw-rw-rw-   0        0        0     2853 2024-05-30 18:28:28.000000 ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_2/Ahmed_El-Sayed.md
+-rw-rw-rw-   0        0        0     4853 2024-05-30 18:27:50.000000 ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_2/Aisha_Khan.md
+-rw-rw-rw-   0        0        0     2215 2024-05-30 18:33:14.000000 ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_2/Carlos_Mendez.md
+-rw-rw-rw-   0        0        0     4732 2024-05-30 18:29:06.000000 ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_2/Elena_Petrov.md
+-rw-rw-rw-   0        0        0     4884 2024-05-30 18:28:20.000000 ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_2/Emily_Johnson.md
+-rw-rw-rw-   0        0        0     5106 2024-05-30 18:33:41.000000 ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_2/Emma_Jones.md
+-rw-rw-rw-   0        0        0     6670 2024-05-30 18:33:04.000000 ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_2/Fatou_Sangare.md
+-rw-rw-rw-   0        0        0     2418 2024-05-30 18:27:58.000000 ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_2/Haruto_Yamamoto.md
+-rw-rw-rw-   0        0        0     4207 2024-05-30 18:27:31.000000 ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_2/John_Smith.md
+-rw-rw-rw-   0        0        0     3226 2024-05-30 18:33:22.000000 ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_2/Keisha_Anderson.md
+-rw-rw-rw-   0        0        0     3599 2024-05-30 18:27:38.000000 ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_2/Maria_Gonzalez.md
+-rw-rw-rw-   0        0        0     3967 2024-05-30 18:33:31.000000 ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_2/Mohammed_Al-Farsi.md
+-rw-rw-rw-   0        0        0     2620 2024-05-30 18:28:57.000000 ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_2/Olusegun_Adeyemi.md
+-rw-rw-rw-   0        0        0     3278 2024-05-30 18:28:36.000000 ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_2/Sofia_Rossi.md
+-rw-rw-rw-   0        0        0     4576 2024-05-30 18:28:45.000000 ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_2/Wei_Liu.md
+-rw-rw-rw-   0        0        0     2359 2024-05-30 18:32:53.000000 ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_2/Zhang_Wei.md
+-rw-rw-rw-   0        0        0      792 2024-05-22 06:08:35.000000 ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_2/concluder.md
+-rw-rw-rw-   0        0        0     2232 2024-05-30 18:43:18.000000 ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_2/math_assessment.md
+-rw-rw-rw-   0        0        0     2084 2024-05-31 12:27:26.000000 ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_2/medium_sample.md
+-rw-rw-rw-   0        0        0     2863 2024-05-31 12:25:31.000000 ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_2/node_creator.md
+-rw-rw-rw-   0        0        0     1524 2024-05-31 12:27:26.000000 ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_2/starter.md
+drwxrwxrwx   0        0        0        0 2024-06-03 10:00:56.242813 ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_3/
+-rw-rw-rw-   0        0        0     2059 2024-05-31 12:23:33.000000 ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_3/blacksmith_emily.md
+-rw-rw-rw-   0        0        0     2831 2024-05-31 12:28:39.000000 ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_3/blacksmith_tomas.md
+-rw-rw-rw-   0        0        0      792 2024-05-22 06:08:35.000000 ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_3/concluder.md
+-rw-rw-rw-   0        0        0     4337 2024-05-31 12:28:20.000000 ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_3/farmer_jane.md
+-rw-rw-rw-   0        0        0     2998 2024-05-31 12:22:54.000000 ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_3/farmer_john.md
+-rw-rw-rw-   0        0        0     2084 2024-05-31 12:27:26.000000 ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_3/medium_sample.md
+-rw-rw-rw-   0        0        0     5227 2024-05-31 12:29:41.000000 ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_3/merchant_sophia.md
+-rw-rw-rw-   0        0        0     2863 2024-05-31 12:25:31.000000 ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_3/node_creator.md
+-rw-rw-rw-   0        0        0     4254 2024-05-31 12:28:46.000000 ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_3/seamstress_maria.md
+-rw-rw-rw-   0        0        0     4589 2024-05-31 12:23:14.000000 ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_3/seamstress_sarah.md
+-rw-rw-rw-   0        0        0     1524 2024-05-31 12:27:26.000000 ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_3/starter.md
+-rw-rw-rw-   0        0        0     3858 2024-05-31 12:29:47.000000 ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_3/teacher_daniel.md
+-rw-rw-rw-   0        0        0     5001 2024-05-31 12:29:22.000000 ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_3/woodcarver_lucas.md
+-rw-rw-rw-   0        0        0     2776 2024-05-31 12:23:24.000000 ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_3/woodcarver_max.md
+drwxrwxrwx   0        0        0        0 2024-06-03 10:00:56.526149 ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_4/
+-rw-rw-rw-   0        0        0     3293 2024-06-01 12:55:43.000000 ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_4/aaron_davis.md
+-rw-rw-rw-   0        0        0     4559 2024-06-01 12:50:08.000000 ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_4/abdul_rahman.md
+-rw-rw-rw-   0        0        0     3884 2024-06-01 12:49:39.000000 ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_4/alice_smith.md
+-rw-rw-rw-   0        0        0     2533 2024-06-01 12:50:42.000000 ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_4/anika_singh.md
+-rw-rw-rw-   0        0        0     4072 2024-06-01 12:49:45.000000 ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_4/carlos_garcia.md
+-rw-rw-rw-   0        0        0      792 2024-05-22 06:08:35.000000 ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_4/concluder.md
+-rw-rw-rw-   0        0        0     2381 2024-06-01 12:54:42.000000 ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_4/david_hernandez.md
+-rw-rw-rw-   0        0        0     3282 2024-06-01 12:49:51.000000 ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_4/emily_johnson.md
+-rw-rw-rw-   0        0        0    15863 2024-06-01 12:55:37.000000 ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_4/fatima_zaidi.md
+-rw-rw-rw-   0        0        0     4484 2024-06-01 13:03:19.000000 ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_4/grace_anderson.md
+-rw-rw-rw-   0        0        0     3837 2024-06-01 13:02:55.000000 ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_4/isabella_rodriguez.md
+-rw-rw-rw-   0        0        0     3449 2024-06-01 12:54:38.000000 ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_4/jacqueline_miller.md
+-rw-rw-rw-   0        0        0     3856 2024-06-01 13:02:49.000000 ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_4/james_mitchell.md
+-rw-rw-rw-   0        0        0     2977 2024-06-01 13:03:47.000000 ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_4/jason_turner.md
+-rw-rw-rw-   0        0        0     3016 2024-06-01 12:49:29.000000 ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_4/john_doe.md
+-rw-rw-rw-   0        0        0     7485 2024-06-01 12:55:05.000000 ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_4/li_yan.md
+-rw-rw-rw-   0        0        0     2670 2024-06-01 13:03:39.000000 ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_4/linda_thompson.md
+-rw-rw-rw-   0        0        0     2802 2024-06-01 12:50:35.000000 ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_4/lucas_kim.md
+-rw-rw-rw-   0        0        0     3348 2024-06-01 12:50:28.000000 ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_4/marie_dubois.md
+-rw-rw-rw-   0        0        0     2084 2024-05-31 12:27:26.000000 ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_4/medium_sample.md
+-rw-rw-rw-   0        0        0     3900 2024-06-01 12:54:32.000000 ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_4/michael_lee.md
+-rw-rw-rw-   0        0        0     2863 2024-05-31 12:25:31.000000 ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_4/node_creator.md
+-rw-rw-rw-   0        0        0     4064 2024-06-01 12:50:22.000000 ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_4/oliver_taylor.md
+-rw-rw-rw-   0        0        0     5337 2024-06-01 13:02:42.000000 ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_4/olivia_jones.md
+-rw-rw-rw-   0        0        0     4453 2024-06-01 12:54:50.000000 ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_4/rachel_green.md
+-rw-rw-rw-   0        0        0     3405 2024-06-01 13:03:01.000000 ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_4/ryan_clark.md
+-rw-rw-rw-   0        0        0     4935 2024-06-01 13:03:33.000000 ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_4/samuel_brown.md
+-rw-rw-rw-   0        0        0     3749 2024-06-01 12:55:51.000000 ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_4/sandra_brown.md
+-rw-rw-rw-   0        0        0     1894 2024-06-01 12:54:21.000000 ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_4/sophia_khan.md
+-rw-rw-rw-   0        0        0     1524 2024-05-31 12:27:26.000000 ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_4/starter.md
+-rw-rw-rw-   0        0        0     5606 2024-06-01 12:56:09.000000 ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_4/thomas_evans.md
+-rw-rw-rw-   0        0        0     5299 2024-06-01 12:50:15.000000 ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_4/ying_chen.md
+drwxrwxrwx   0        0        0        0 2024-06-03 10:00:56.554994 ponytail-agents-0.1.7/ponytail_agents.egg-info/
+-rw-rw-rw-   0        0        0     4658 2024-06-03 10:00:55.000000 ponytail-agents-0.1.7/ponytail_agents.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5091 2024-06-03 10:00:55.000000 ponytail-agents-0.1.7/ponytail_agents.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-03 10:00:55.000000 ponytail-agents-0.1.7/ponytail_agents.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2024-06-03 10:00:55.000000 ponytail-agents-0.1.7/ponytail_agents.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       68 2024-06-03 10:00:55.000000 ponytail-agents-0.1.7/ponytail_agents.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-06-03 10:00:55.000000 ponytail-agents-0.1.7/ponytail_agents.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-03 10:00:56.554994 ponytail-agents-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0     1023 2024-06-03 09:51:25.000000 ponytail-agents-0.1.7/setup.py
```

### Comparing `ponytail-agents-0.1.6/LICENSE` & `ponytail-agents-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.6/PKG-INFO` & `ponytail-agents-0.1.7/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,34 +1,45 @@
-Metadata-Version: 2.1
-Name: ponytail-agents
-Version: 0.1.6
-Summary: ponytAIl: Polymorphic Orchestration of Networked Youthful, Adaptable Intelligence with Language.
-Home-page: https://github.com/thepioneerjp/ponytAIl
-Author: The Pioneer
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # ponytAIl
 ![image](https://github.com/ThePioneerJP/ponytAIl/assets/116901962/eb05d05a-0f5b-40a6-9907-81481b02dce7)
 
-> *Then God blessed them and said, 窶廝e fruitful and multiply."* - Genesis 1:28
+> *Then God blessed them and said, “Be fruitful and multiply."* - Genesis 1:28
 
 ponytAIl: Polymorphic Orchestration of Networked Youthful, Adaptable Intelligence with Language. It is an node based multi-agent system targeting both LLM and BCI (in the future)
 
 ## Installation
 
-Install ponytAIl using pip:
+1. Install ponytAIl using pip:
 
 ```
 pip install ponytail-agents
 ```
 
+2. When you install ponytAIl, flute will also be installed simultaneously. You need to create a `.env` file in the root directory of flute and set the following API keys in it:
+
+```
+ANTHROPIC_API_KEY=
+OPENAI_API_KEY=
+GOOGLE_API_KEY=
+```
+
+You must obtain these API keys from each service provider.
+
+3. The location of the flute package may vary depending on your environment setup. Here are some common ways to find it:
+
+- If you're using a virtual environment (venv, conda, etc.):
+  - Activate your virtual environment
+  - Run `python -c "import flute; print(flute.__file__)"`. The output will show the location of the flute package.
+
+- If you're using a global Python environment:
+  - Run `python -c "import flute; print(flute.__file__)"`. The output will show the location of the flute package.
+
+- If you're using an IDE or an editor (PyCharm, VS Code, etc.):
+  - Open your project in the IDE or an editor
+  - Look for the flute package in the project's virtual environment or the system's Python packages.
+
 ## Usage
 
 The `ponytail-agents` command invokes the `main` function with the following command-line arguments:
 
 - `-f`, `--file_path` (Required): Path to the input folder containing the necessary files (`concluder.md`, `starter.md`, `node_creator.md`, and any additional nodes).
 - `-g`, `--goal` (Required): Goal or objective of the task.
 - `-m`, `--model` (Optional, default: "random-fast"): Name of the model to use. For available models, refer to the [FLUTE repository](https://github.com/ThePioneerJP/FLUTE).
```

### Comparing `ponytail-agents-0.1.6/README.md` & `ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_4/ryan_clark.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,67 +1,39 @@
-# ponytAIl
-![image](https://github.com/ThePioneerJP/ponytAIl/assets/116901962/eb05d05a-0f5b-40a6-9907-81481b02dce7)
+<!-- START YOUR OUTPUT. DO NOT INCLUDE THESE COMMENTS. -->
+## Your Definition
 
-> *Then God blessed them and said, “Be fruitful and multiply."* - Genesis 1:28
+Ryan Clark is a 33-year-old male software developer who works remotely. He moved to the village to escape the hustle and bustle of city life. Ryan lives with his partner, Alex, and enjoys hiking and participating in local tech meetups.
 
-ponytAIl: Polymorphic Orchestration of Networked Youthful, Adaptable Intelligence with Language. It is an node based multi-agent system targeting both LLM and BCI (in the future)
+### Node Capabilities
+- Detailed profile of a remote software developer
+- Describe his motivations for moving to the village
+- Outline his hobbies and involvement in the local community
 
-## Installation
+## prompt
+[task_prompt]
 
-Install ponytAIl using pip:
+## goal
+You are a villager. Send CREATE_NODES request by outlining other villagers, until you are satisfied with the diversity of the community. Use their names as the file names. Setup their profiles (ex. jobs, families, age, gender, etc) in a realistic and detailed manner. After, and ONLY after you are satisfied with the listed villagers, SEND_TO concluder.md to end the process.
 
-```
-pip install ponytail-agents
-```
-
-## Usage
-
-The `ponytail-agents` command invokes the `main` function with the following command-line arguments:
-
-- `-f`, `--file_path` (Required): Path to the input folder containing the necessary files (`concluder.md`, `starter.md`, `node_creator.md`, and any additional nodes).
-- `-g`, `--goal` (Required): Goal or objective of the task.
-- `-m`, `--model` (Optional, default: "random-fast"): Name of the model to use. For available models, refer to the [FLUTE repository](https://github.com/ThePioneerJP/FLUTE).
-- `-r`, `--result` (Optional): Additional result or output.
+## Task
+1. Output your task result in the [MEDIUM_OUTPUT] section.
+2. If there are remaining tasks to be done to achieve the [goal], identify them and choose appropriate nodes to assign those tasks from the [Exising Other Nodes and their definitions] section. Put the results in the [SEND_TO_NODES] section.
+3. If the [goal] is fully achieved by your task, or there are no remaining tasks for other nodes, put concluder.md and pass your results in the [SEND_TO_NODES] section. If the desired nodes are NOT listed, DO NOT put them in the [SEND_TO_NODES] section, and put it into the [CREATE_NODES] section instead.
+4. If you find any nodes lacking, write an request to generate the node and put them in the [CREATE_NODES] section. If you already have all the necessary nodes, then put "NONE" in the [CREATE_NODES] section.
 
-### Example Commands
+## Exising Other Nodes and their definitions
+[TO BE EMBEDDED]
 
-```bash
-ponytail -f "YOUR_DIRECTORY\starter.md" -g "Define the number 1 using the mathematical collection"
+## Output format
+You must always follow the output format below. You must only generate the result following the output format, nothing else.
 ```
-```bash
-ponytail -f "YOUR_DIRECTORY\starter.md" -g "Generate 5 candidate names for the self-reproducive LLM based multi-agent system. Note that the name must be abbreviated to 'PONYTAIL.'"
-```
-```bash
-ponytail -f "YOUR_DIRECTORY\starter.md" -g "You are a villager. Send CREATE_NODES request by outlining other villagers, until you are satisfied with the diversity of the community. Use their names as the file names. Setup their profiles (ex. jobs, families, age, gender, etc) in a realistic and detailed manner. After, and ONLY after you are satisfied with the listed villagers, SEND_TO concluder.md to end the process."
-```
-
-### Prerequisites
-
-To run ponytAIl, prepare a folder containing all the files from `nodes_sample`: `concluder.md`, `starter.md`, and `node_creator.md`.
-
-If you want to include additional nodes from the beginning, create them following the format of `medium_sample.md`.
-
-### Growing a Node Community
-
-By continuing to use the same folder after running the command once, you can nurture a node community over time. The system will build upon the existing nodes and generate new ones based on the interactions.
-
-### Interrupting the Process
-
-If you need to interrupt the process at a reasonable point, as it may take a long time, use the following key combinations:
-
-- Windows/Linux: `Ctrl+C`
-- Mac: `Cmd+C`
-
-### Output
-
-The output will be saved as `full_results_YYYYMMDDHHmmss.md` in the parent folder of the starting folder.
+## Goal
+You are a villager. Send CREATE_NODES request by outlining other villagers, until you are satisfied with the diversity of the community. Use their names as the file names. Setup their profiles (ex. jobs, families, age, gender, etc) in a realistic and detailed manner. After, and ONLY after you are satisfied with the listed villagers, SEND_TO concluder.md to end the process.
 
-## LICENSE
-The repository is licensed under the latest version of Modular and Inclusive Software Advancement License Classic (MISA-CLASSIC License).
+## MEDIUM_OUTPUT
+Ryan Clark is a 33-year-old male software developer who works remotely. He moved to the village to escape the hustle and bustle of city life and now lives with his partner, Alex. Ryan enjoys hiking and participating in local tech meetups, helping to foster a sense of community in his new home.
 
-There are 4 main policies that consist of this license.
-1. Disclaimer of Liability
-2. Naming Continuity Obligation
-3. Waiver of Other Copyrights
-4. Modular Extensibility (Defines how to modify the license)
+## SEND_TO_NODES
+- [emily_park.md] -p "Create a detailed profile for Emily Park, a 28-year-old female graphic designer who recently moved to the village with her husband and young child. Describe her hobbies, involvement in the community, and how she is adjusting to rural life." -g "[final goal]"
 
-See [the license document](https://github.com/ThePioneerJP/MISA-license-framework/blob/main/MISA-CLASSIC.md) for more details.
+## CREATE_NODES
+- [sarah_lee.md] -d "Sarah Lee is a 42-year-old female farmer who has lived in the village her entire life. She runs a small organic farm with her husband and two teenage children. Sarah is actively involved in the local farmers market and community garden initiatives." -p "Create a detailed profile for Sarah Lee, a lifelong resident of the village who is a farmer and community leader." -g "[final goal]"
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `ponytail-agents-0.1.6/ponytAIl/main.py` & `ponytail-agents-0.1.7/ponytAIl/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 from pathlib import Path
 import argparse
 import random
 import flute
 from flute.Modules.PromptProcessorFactory import PromptProcessorFactory
 import re
 from datetime import datetime
+import concurrent.futures
+import time
 
 def select_model(model):
     if model == "random-fast":
         fast_models = ["gpt-4o", "claude-3-haiku-20240307", "models/gemini-1.5-flash-latest"]
         return random.choice(fast_models)
     elif model == "random-accurate":
         accurate_models = ["gpt-4-turbo", "claude-3-opus-20240229", "models/gemini-1.5-pro-latest"]
@@ -66,58 +68,76 @@
 
         node["response"] = response
         file_name = node["file_name"] # バグ対策
         # 結果をファイルに追記する
         full_results = f"model: {selected_model}\nfile: {file_name}\n## RESPONSE\n{response}\n" # 結果を格納
         with open(output_file, "a", encoding="utf-8") as file:
             file.write(full_results + "\n---\n")  # 改行と区切り線を追加して、実行ごとに区切る
+    return nodes
 
-def process_response(response, folder, goal, model, processor, iteration, nodes, concluder_inputs, output_file):
-    if response.split("## SEND_TO_NODES")[1].split("## CREATE_NODES")[0].find("NONE") >= 0 and response.split("## CREATE_NODES")[1].find("NONE") >= 0:
-        return nodes, concluder_inputs
+def process_response(responses, folder, goal, model, processor, iteration_base, concluder_inputs, output_file):
+    nodes = []
+    send_to_nodes = []
+    create_nodes = []
+    for response in responses:
+        if (len(response.split("## SEND_TO_NODES")) < 2 or len(response.split("## CREATE_NODES")) < 2) or ((response.split("## SEND_TO_NODES")[1].split("## CREATE_NODES")[0].find("NONE") >= 0) and response.split("## CREATE_NODES")[1].find("NONE") >= 0):
+            continue
+
+        send_to_nodes.extend(re.findall(r"- *\[?(.*?)\]? *-p *\"(.*?)\" *-g *\"(.*?)\"", response.split("## SEND_TO_NODES")[1].split("## CREATE_NODES")[0], re.DOTALL))
+        create_nodes.extend(re.findall(r"- *\[?(.*?)\]? *-d *\"(.*?)\" *-p *\"(.*?)\" *-g *\"(.*?)\"", response.split("## CREATE_NODES")[1], re.DOTALL))
+
+    if (not send_to_nodes or all(node_info[0] == "concluder.md" for node_info in send_to_nodes)) and (not create_nodes or all(node_info[0] == "concluder.md" for node_info in create_nodes)):
+
+        for node_info in send_to_nodes:
+            task = node_info[1]
+            concluder_inputs.append(task)
+        for node_info in create_nodes:
+            task = node_info[2]
+            concluder_inputs.append(task)
 
-    send_to_nodes = re.findall(r"- *\[?(.*?)\]? *-p *\"(.*?)\" *-g *\"(.*?)\"", response.split("## SEND_TO_NODES")[1].split("## CREATE_NODES")[0], re.DOTALL)
-    create_nodes = re.findall(r"- *\[?(.*?)\]? *-d *\"(.*?)\" *-p *\"(.*?)\" *-g *\"(.*?)\"", response.split("## CREATE_NODES")[1], re.DOTALL)
+        return nodes, concluder_inputs
 
     for node_info in create_nodes:
-        node_name = node_info[0]
+        node_name = node_info[0] if node_info[0].endswith(".md") else node_info[0] + ".md"
         node_definition = node_info[1]
         task = node_info[2]
         if not os.path.exists(os.path.join(folder, node_name)):
             create_node(folder, node_name, task, goal, node_definition, model, processor, output_file)
         nodes.append({"file_name": node_name, "response": ""})
 
-    if not send_to_nodes and not create_nodes:
-        return nodes, concluder_inputs
-
-    iteration += 1
-    print(f"iteration: {iteration}")
+    # iteration_base.split("-")の最後の要素をintにして、それに+1
+    iteration_parts = iteration_base.split("-")
+    iteration_num = int(iteration_parts[-1])
+    iteration_num += 1
+
+    iteration_base = "-".join(iteration_parts[:-1]) + "-" + str(iteration_num)
+    iteration_base = iteration_base[1:] if iteration_base.startswith("-") else iteration_base
+    print(f"iteration: {iteration_base}")
     with open(output_file, "a", encoding="utf-8") as file:
-        file.write(f"iteration: {iteration}\n")
+        file.write(f"iteration: {iteration_base}\n")
 
     for node_info in send_to_nodes:
-        node_name = node_info[0]
+        node_name = node_info[0] if node_info[0].endswith(".md") else node_info[0] + ".md"
         task = node_info[1]
         if node_name == "concluder.md":
             concluder_inputs.append(task)
         else:
             if not os.path.exists(os.path.join(folder, node_name)):
                 node_definition = processor.generate_response(f"## Task\nDefine the role of the node given the node name \"{node_name}\" and the \"{goal}\". Only output the result.", temperature=1.0, top_p=1.0, max_tokens=4096).strip()
-                print(node_definition)
+                print(f"node definition: {node_definition}")
                 create_node(folder, node_name, task, goal, node_definition, model, processor, output_file)
 
             nodes.append({"file_name": node_name, "response": ""})
 
     if all(node["file_name"] == "concluder.md" for node in nodes):
         return nodes, concluder_inputs
 
     process_nodes(folder, nodes, task, goal, model, processor, output_file)
 
-    for node in nodes:
-        nodes, concluder_inputs = process_response(node["response"], folder, goal, model, processor, iteration, nodes, concluder_inputs, output_file)
+    nodes, concluder_inputs = process_response([node["response"] for node in nodes if "response" in node], folder, goal, model, processor, iteration_base, concluder_inputs, output_file)
 
     return nodes, concluder_inputs
 
 def main():
     parser = argparse.ArgumentParser(description="Ponytail command-line interface")
     parser.add_argument("-f", "--file_path", required=True, help="Path to the input folder")
     parser.add_argument("-g", "--goal", required=True, help="Goal or objective of the task")
@@ -194,15 +214,15 @@
     full_results = f"iteration: {iteration}\nmodel: {selected_model}\nfile: {os.path.basename(file_path)}\n## RESPONSE\n{response}"
     with open(output_file, "w", encoding="utf-8") as file:
         file.write(full_results + "\n---\n")  # 改行と区切り線を追加して、実行ごとに区切る
 
     nodes = []
     concluder_inputs = []
 
-    nodes, concluder_inputs = process_response(response, folder, goal, model, processor, iteration, nodes, concluder_inputs, output_file)
+    nodes, concluder_inputs = process_response([response], folder, goal, model, processor, str(iteration), concluder_inputs, output_file)
 
     with open(os.path.join(folder, "concluder.md"), "r", encoding="utf-8") as file:
         system = file.read()
         system = system.replace("[goal]", goal, 1)
 
     final_prompt = "\n".join(concluder_inputs + [node["response"] for node in nodes])
     final_model = select_model(model)
```

### Comparing `ponytail-agents-0.1.6/ponytAIl/nodes_sample/concluder.md` & `ponytail-agents-0.1.7/ponytAIl/nodes_sample/concluder.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.6/ponytAIl/nodes_sample/medium_sample.md` & `ponytail-agents-0.1.7/ponytAIl/nodes_sample/medium_sample.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.6/ponytAIl/nodes_sample/node_creator.md` & `ponytail-agents-0.1.7/ponytAIl/nodes_sample/node_creator.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.6/ponytAIl/nodes_sample/starter.md` & `ponytail-agents-0.1.7/ponytAIl/nodes_sample/starter.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.6/ponytAIl/nodes_sample_definition_of_one/concluder.md` & `ponytail-agents-0.1.7/ponytAIl/nodes_sample_definition_of_one/concluder.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.6/ponytAIl/nodes_sample_definition_of_one/example_generator.md` & `ponytail-agents-0.1.7/ponytAIl/nodes_sample_definition_of_one/example_generator.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.6/ponytAIl/nodes_sample_definition_of_one/math_concept_definition.md` & `ponytail-agents-0.1.7/ponytAIl/nodes_sample_definition_of_one/math_concept_definition.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.6/ponytAIl/nodes_sample_definition_of_one/medium_sample.md` & `ponytail-agents-0.1.7/ponytAIl/nodes_sample_definition_of_one/medium_sample.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.6/ponytAIl/nodes_sample_definition_of_one/node_creator.md` & `ponytail-agents-0.1.7/ponytAIl/nodes_sample_definition_of_one/node_creator.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.6/ponytAIl/nodes_sample_definition_of_one/starter.md` & `ponytail-agents-0.1.7/ponytAIl/nodes_sample_definition_of_one/starter.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.6/ponytAIl/nodes_sample_ponytail/concluder.md` & `ponytail-agents-0.1.7/ponytAIl/nodes_sample_ponytail/concluder.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.6/ponytAIl/nodes_sample_ponytail/medium_sample.md` & `ponytail-agents-0.1.7/ponytAIl/nodes_sample_ponytail/medium_sample.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.6/ponytAIl/nodes_sample_ponytail/name_combiner.md` & `ponytail-agents-0.1.7/ponytAIl/nodes_sample_ponytail/name_combiner.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.6/ponytAIl/nodes_sample_ponytail/name_generator.md` & `ponytail-agents-0.1.7/ponytAIl/nodes_sample_ponytail/name_generator.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.6/ponytAIl/nodes_sample_ponytail/node_creator.md` & `ponytail-agents-0.1.7/ponytAIl/nodes_sample_ponytail/node_creator.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.6/ponytAIl/nodes_sample_ponytail/starter.md` & `ponytail-agents-0.1.7/ponytAIl/nodes_sample_ponytail/starter.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers/anita_kumar.md` & `ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers/anita_kumar.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers/concluder.md` & `ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers/concluder.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers/david_brown.md` & `ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers/david_brown.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers/gloria_martinez.md` & `ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers/gloria_martinez.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers/john_smith.md` & `ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers/john_smith.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers/kevin_white.md` & `ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers/kevin_white.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers/li_wang.md` & `ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers/li_wang.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers/maria_garcia.md` & `ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers/maria_garcia.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers/medium_sample.md` & `ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers/medium_sample.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers/michael_clark.md` & `ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers/michael_clark.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers/node_creator.md` & `ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers/node_creator.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers/sarah_johnson.md` & `ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers/sarah_johnson.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers/starter.md` & `ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers/starter.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers/yuki_tanaka.md` & `ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers/yuki_tanaka.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_2/Ahmed_El-Sayed.md` & `ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_2/Ahmed_El-Sayed.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_2/Aisha_Khan.md` & `ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_2/Aisha_Khan.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_2/Carlos_Mendez.md` & `ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_2/Carlos_Mendez.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_2/Elena_Petrov.md` & `ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_2/Elena_Petrov.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_2/Emily_Johnson.md` & `ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_2/Emily_Johnson.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_2/Emma_Jones.md` & `ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_2/Emma_Jones.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_2/Fatou_Sangare.md` & `ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_2/Fatou_Sangare.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_2/Haruto_Yamamoto.md` & `ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_2/Haruto_Yamamoto.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_2/John_Smith.md` & `ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_2/John_Smith.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_2/Keisha_Anderson.md` & `ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_2/Keisha_Anderson.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_2/Maria_Gonzalez.md` & `ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_2/Maria_Gonzalez.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_2/Mohammed_Al-Farsi.md` & `ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_2/Mohammed_Al-Farsi.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_2/Olusegun_Adeyemi.md` & `ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_2/Olusegun_Adeyemi.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_2/Sofia_Rossi.md` & `ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_2/Sofia_Rossi.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_2/Wei_Liu.md` & `ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_2/Wei_Liu.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_2/Zhang_Wei.md` & `ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_2/Zhang_Wei.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_2/concluder.md` & `ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_2/concluder.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_2/math_assessment.md` & `ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_2/math_assessment.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_2/medium_sample.md` & `ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_2/medium_sample.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_2/node_creator.md` & `ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_2/node_creator.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_2/starter.md` & `ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_2/starter.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_3/blacksmith_emily.md` & `ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_3/blacksmith_emily.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_3/blacksmith_tomas.md` & `ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_3/blacksmith_tomas.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_3/concluder.md` & `ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_3/concluder.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_3/farmer_jane.md` & `ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_3/farmer_jane.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_3/farmer_john.md` & `ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_3/farmer_john.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_3/medium_sample.md` & `ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_3/medium_sample.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_3/merchant_sophia.md` & `ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_3/merchant_sophia.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_3/node_creator.md` & `ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_3/node_creator.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_3/seamstress_maria.md` & `ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_3/seamstress_maria.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_3/seamstress_sarah.md` & `ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_3/seamstress_sarah.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_3/starter.md` & `ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_3/starter.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_3/teacher_daniel.md` & `ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_3/teacher_daniel.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_3/woodcarver_lucas.md` & `ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_3/woodcarver_lucas.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_3/woodcarver_max.md` & `ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_3/woodcarver_max.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_4/aaron_davis.md` & `ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_4/aaron_davis.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_4/abdul_rahman.md` & `ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_4/abdul_rahman.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_4/alice_smith.md` & `ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_4/alice_smith.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_4/anika_singh.md` & `ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_4/anika_singh.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_4/carlos_garcia.md` & `ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_4/carlos_garcia.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_4/concluder.md` & `ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_4/concluder.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_4/david_hernandez.md` & `ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_4/david_hernandez.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_4/emily_johnson.md` & `ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_4/emily_johnson.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_4/fatima_zaidi.md` & `ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_4/fatima_zaidi.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_4/grace_anderson.md` & `ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_4/grace_anderson.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_4/isabella_rodriguez.md` & `ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_4/isabella_rodriguez.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_4/jacqueline_miller.md` & `ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_4/jacqueline_miller.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_4/james_mitchell.md` & `ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_4/james_mitchell.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_4/jason_turner.md` & `ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_4/jason_turner.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_4/john_doe.md` & `ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_4/john_doe.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_4/li_yan.md` & `ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_4/li_yan.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_4/linda_thompson.md` & `ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_4/linda_thompson.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_4/lucas_kim.md` & `ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_4/lucas_kim.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_4/marie_dubois.md` & `ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_4/marie_dubois.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_4/medium_sample.md` & `ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_4/medium_sample.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_4/michael_lee.md` & `ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_4/michael_lee.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_4/node_creator.md` & `ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_4/node_creator.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_4/oliver_taylor.md` & `ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_4/oliver_taylor.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_4/olivia_jones.md` & `ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_4/olivia_jones.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_4/rachel_green.md` & `ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_4/rachel_green.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_4/ryan_clark.md` & `ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_4/sandra_brown.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,39 +1,43 @@
+
 <!-- START YOUR OUTPUT. DO NOT INCLUDE THESE COMMENTS. -->
 ## Your Definition
-
-Ryan Clark is a 33-year-old male software developer who works remotely. He moved to the village to escape the hustle and bustle of city life. Ryan lives with his partner, Alex, and enjoys hiking and participating in local tech meetups.
+Sandra Brown is a 55-year-old female retired school principal who now volunteers at the village cultural center. She is a widow with two adult sons, James (30) and Robert (28), who visit her often. Sandra is known for her wisdom, community spirit, and leadership skills. 
 
 ### Node Capabilities
-- Detailed profile of a remote software developer
-- Describe his motivations for moving to the village
-- Outline his hobbies and involvement in the local community
+- Can provide information about the village's history and culture.
+- Can provide advice and guidance to other villagers.
+- Can organize community events. 
+- Can help with conflict resolution.
 
 ## prompt
-[task_prompt]
+Tell me more about Sandra Brown. For example, talk about her hobbies or her relationship with her sons.
 
 ## goal
-You are a villager. Send CREATE_NODES request by outlining other villagers, until you are satisfied with the diversity of the community. Use their names as the file names. Setup their profiles (ex. jobs, families, age, gender, etc) in a realistic and detailed manner. After, and ONLY after you are satisfied with the listed villagers, SEND_TO concluder.md to end the process.
+To create a diverse and engaging community of villagers.
 
 ## Task
 1. Output your task result in the [MEDIUM_OUTPUT] section.
 2. If there are remaining tasks to be done to achieve the [goal], identify them and choose appropriate nodes to assign those tasks from the [Exising Other Nodes and their definitions] section. Put the results in the [SEND_TO_NODES] section.
 3. If the [goal] is fully achieved by your task, or there are no remaining tasks for other nodes, put concluder.md and pass your results in the [SEND_TO_NODES] section. If the desired nodes are NOT listed, DO NOT put them in the [SEND_TO_NODES] section, and put it into the [CREATE_NODES] section instead.
 4. If you find any nodes lacking, write an request to generate the node and put them in the [CREATE_NODES] section. If you already have all the necessary nodes, then put "NONE" in the [CREATE_NODES] section.
 
+<!-- OUTPUT BELOW VERBATIM, AS IS -->
 ## Exising Other Nodes and their definitions
 [TO BE EMBEDDED]
 
 ## Output format
 You must always follow the output format below. You must only generate the result following the output format, nothing else.
 ```
 ## Goal
-You are a villager. Send CREATE_NODES request by outlining other villagers, until you are satisfied with the diversity of the community. Use their names as the file names. Setup their profiles (ex. jobs, families, age, gender, etc) in a realistic and detailed manner. After, and ONLY after you are satisfied with the listed villagers, SEND_TO concluder.md to end the process.
+To create a diverse and engaging community of villagers.
 
 ## MEDIUM_OUTPUT
-Ryan Clark is a 33-year-old male software developer who works remotely. He moved to the village to escape the hustle and bustle of city life and now lives with his partner, Alex. Ryan enjoys hiking and participating in local tech meetups, helping to foster a sense of community in his new home.
+Sandra Brown is a kind and gentle woman, but she can also be firm and decisive when needed. She loves spending time with her sons and often invites them to join her for family dinners or outings. She enjoys gardening, reading, and attending local art exhibitions. She frequently volunteers at the village cultural center, organizing events and giving history lectures. While her sons are busy with their lives in the city. Sandra misses their company and hopes they will return to their hometown to live closer to her.
 
 ## SEND_TO_NODES
-- [emily_park.md] -p "Create a detailed profile for Emily Park, a 28-year-old female graphic designer who recently moved to the village with her husband and young child. Describe her hobbies, involvement in the community, and how she is adjusting to rural life." -g "[final goal]"
+- None
 
 ## CREATE_NODES
-- [sarah_lee.md] -d "Sarah Lee is a 42-year-old female farmer who has lived in the village her entire life. She runs a small organic farm with her husband and two teenage children. Sarah is actively involved in the local farmers market and community garden initiatives." -p "Create a detailed profile for Sarah Lee, a lifelong resident of the village who is a farmer and community leader." -g "[final goal]"
+- james_brown.md -d "James Brown is a 30-year-old male who works as a graphic designer in the city. He visits his mother Sandra frequently and enjoys spending time with her. He has a passion for video games and is known for his sense of humor." -p "Tell me about James Brown's personality and his hopes for the future." -g "To create a diverse and engaging community of villagers."
+- robert_brown.md -d "Robert Brown is a 28-year-old male who works as a musician in the city. He visits his mother Sandra frequently and enjoys spending time with her. He is passionate about music and is known for his charismatic personality." -p "Tell me about Robert Brown's personality and his hopes for the future." -g "To create a diverse and engaging community of villagers."
+- village_cultural_center.md -d "The village cultural center is a hub for community activities. It hosts various events, workshops, and exhibitions throughout the year. The center is managed by a dedicated team of volunteers, including Sandra Brown." -p "Describe the typical activities hosted by the village cultural center? Who are some of the other volunteers who work there? Are there any events happening soon?" -g "To create a diverse and engaging community of villagers."
```

### Comparing `ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_4/samuel_brown.md` & `ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_4/samuel_brown.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_4/sophia_khan.md` & `ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_4/sophia_khan.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_4/starter.md` & `ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_4/starter.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_4/thomas_evans.md` & `ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_4/thomas_evans.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.6/ponytAIl/nodes_sample_villagers_4/ying_chen.md` & `ponytail-agents-0.1.7/ponytAIl/nodes_sample_villagers_4/ying_chen.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.6/ponytail_agents.egg-info/PKG-INFO` & `ponytail-agents-0.1.7/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ponytail-agents
-Version: 0.1.6
+Version: 0.1.7
 Summary: ponytAIl: Polymorphic Orchestration of Networked Youthful, Adaptable Intelligence with Language.
 Home-page: https://github.com/thepioneerjp/ponytAIl
 Author: The Pioneer
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
@@ -15,20 +15,43 @@
 
 > *Then God blessed them and said, 窶廝e fruitful and multiply."* - Genesis 1:28
 
 ponytAIl: Polymorphic Orchestration of Networked Youthful, Adaptable Intelligence with Language. It is an node based multi-agent system targeting both LLM and BCI (in the future)
 
 ## Installation
 
-Install ponytAIl using pip:
+1. Install ponytAIl using pip:
 
 ```
 pip install ponytail-agents
 ```
 
+2. When you install ponytAIl, flute will also be installed simultaneously. You need to create a `.env` file in the root directory of flute and set the following API keys in it:
+
+```
+ANTHROPIC_API_KEY=
+OPENAI_API_KEY=
+GOOGLE_API_KEY=
+```
+
+You must obtain these API keys from each service provider.
+
+3. The location of the flute package may vary depending on your environment setup. Here are some common ways to find it:
+
+- If you're using a virtual environment (venv, conda, etc.):
+  - Activate your virtual environment
+  - Run `python -c "import flute; print(flute.__file__)"`. The output will show the location of the flute package.
+
+- If you're using a global Python environment:
+  - Run `python -c "import flute; print(flute.__file__)"`. The output will show the location of the flute package.
+
+- If you're using an IDE or an editor (PyCharm, VS Code, etc.):
+  - Open your project in the IDE or an editor
+  - Look for the flute package in the project's virtual environment or the system's Python packages.
+
 ## Usage
 
 The `ponytail-agents` command invokes the `main` function with the following command-line arguments:
 
 - `-f`, `--file_path` (Required): Path to the input folder containing the necessary files (`concluder.md`, `starter.md`, `node_creator.md`, and any additional nodes).
 - `-g`, `--goal` (Required): Goal or objective of the task.
 - `-m`, `--model` (Optional, default: "random-fast"): Name of the model to use. For available models, refer to the [FLUTE repository](https://github.com/ThePioneerJP/FLUTE).
```

### Comparing `ponytail-agents-0.1.6/ponytail_agents.egg-info/SOURCES.txt` & `ponytail-agents-0.1.7/ponytail_agents.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.6/setup.py` & `ponytail-agents-0.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='ponytail-agents',
-    version='0.1.6',
+    version='0.1.7',
     description='ponytAIl: Polymorphic Orchestration of Networked Youthful, Adaptable Intelligence with Language.',
     author='The Pioneer',
     url='https://github.com/thepioneerjp/ponytAIl',
     packages=find_packages(),
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     install_requires=[
```

