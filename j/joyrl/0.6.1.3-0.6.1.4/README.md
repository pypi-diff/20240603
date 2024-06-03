# Comparing `tmp/joyrl-0.6.1.3.tar.gz` & `tmp/joyrl-0.6.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "joyrl-0.6.1.3.tar", last modified: Sun Jun  2 02:57:40 2024, max compression
+gzip compressed data, was "joyrl-0.6.1.4.tar", last modified: Mon Jun  3 05:27:38 2024, max compression
```

## Comparing `joyrl-0.6.1.3.tar` & `joyrl-0.6.1.4.tar`

### file list

```diff
@@ -1,105 +1,105 @@
-drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-02 02:57:40.477568 joyrl-0.6.1.3/
--rw-r--r--   0 johnjim    (501) staff       (20)     1077 2024-02-25 07:46:04.000000 joyrl-0.6.1.3/LICENSE
--rw-r--r--   0 johnjim    (501) staff       (20)    11639 2024-06-02 02:57:40.477474 joyrl-0.6.1.3/PKG-INFO
--rw-r--r--   0 johnjim    (501) staff       (20)    10670 2024-06-01 08:59:02.000000 joyrl-0.6.1.3/README.md
-drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-02 02:57:40.462928 joyrl-0.6.1.3/joyrl/
--rw-r--r--   0 johnjim    (501) staff       (20)      357 2024-06-02 02:56:22.000000 joyrl-0.6.1.3/joyrl/__init__.py
-drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-02 02:57:40.463910 joyrl-0.6.1.3/joyrl/algos/
-drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-02 02:57:40.464772 joyrl-0.6.1.3/joyrl/algos/DDPG/
--rw-r--r--   0 johnjim    (501) staff       (20)        0 2024-02-25 07:46:04.000000 joyrl-0.6.1.3/joyrl/algos/DDPG/__init__.py
--rw-r--r--   0 johnjim    (501) staff       (20)     1517 2024-02-25 07:46:04.000000 joyrl-0.6.1.3/joyrl/algos/DDPG/config.py
--rw-r--r--   0 johnjim    (501) staff       (20)      152 2024-02-25 07:46:04.000000 joyrl-0.6.1.3/joyrl/algos/DDPG/data_handler.py
--rw-r--r--   0 johnjim    (501) staff       (20)     5540 2024-02-25 07:46:04.000000 joyrl-0.6.1.3/joyrl/algos/DDPG/policy.py
-drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-02 02:57:40.465370 joyrl-0.6.1.3/joyrl/algos/DQN/
--rw-r--r--   0 johnjim    (501) staff       (20)        0 2024-02-25 07:46:04.000000 joyrl-0.6.1.3/joyrl/algos/DQN/__init__.py
--rw-r--r--   0 johnjim    (501) staff       (20)     1950 2024-06-02 02:51:34.000000 joyrl-0.6.1.3/joyrl/algos/DQN/config.py
--rw-r--r--   0 johnjim    (501) staff       (20)      158 2024-02-25 07:46:04.000000 joyrl-0.6.1.3/joyrl/algos/DQN/data_handler.py
--rw-r--r--   0 johnjim    (501) staff       (20)     3627 2024-06-02 02:14:32.000000 joyrl-0.6.1.3/joyrl/algos/DQN/policy.py
-drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-02 02:57:40.466033 joyrl-0.6.1.3/joyrl/algos/DoubleDQN/
--rw-r--r--   0 johnjim    (501) staff       (20)        0 2024-02-25 07:46:04.000000 joyrl-0.6.1.3/joyrl/algos/DoubleDQN/__init__.py
--rw-r--r--   0 johnjim    (501) staff       (20)     1703 2024-02-25 07:46:04.000000 joyrl-0.6.1.3/joyrl/algos/DoubleDQN/config.py
--rw-r--r--   0 johnjim    (501) staff       (20)      350 2024-02-25 07:46:04.000000 joyrl-0.6.1.3/joyrl/algos/DoubleDQN/data_handler.py
--rw-r--r--   0 johnjim    (501) staff       (20)     3512 2024-06-02 02:34:38.000000 joyrl-0.6.1.3/joyrl/algos/DoubleDQN/policy.py
-drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-02 02:57:40.466617 joyrl-0.6.1.3/joyrl/algos/DuelingDQN/
--rw-r--r--   0 johnjim    (501) staff       (20)        0 2024-02-25 07:46:04.000000 joyrl-0.6.1.3/joyrl/algos/DuelingDQN/__init__.py
--rw-r--r--   0 johnjim    (501) staff       (20)     1773 2024-06-01 16:33:50.000000 joyrl-0.6.1.3/joyrl/algos/DuelingDQN/config.py
--rw-r--r--   0 johnjim    (501) staff       (20)      337 2024-02-25 07:46:04.000000 joyrl-0.6.1.3/joyrl/algos/DuelingDQN/data_handler.py
--rw-r--r--   0 johnjim    (501) staff       (20)     3626 2024-06-02 02:19:04.000000 joyrl-0.6.1.3/joyrl/algos/DuelingDQN/policy.py
-drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-02 02:57:40.467243 joyrl-0.6.1.3/joyrl/algos/NoisyDQN/
--rw-r--r--   0 johnjim    (501) staff       (20)      184 2024-02-25 07:46:04.000000 joyrl-0.6.1.3/joyrl/algos/NoisyDQN/__init__.py
--rw-r--r--   0 johnjim    (501) staff       (20)     1071 2024-02-25 07:46:04.000000 joyrl-0.6.1.3/joyrl/algos/NoisyDQN/config.py
--rw-r--r--   0 johnjim    (501) staff       (20)      341 2024-02-25 07:46:04.000000 joyrl-0.6.1.3/joyrl/algos/NoisyDQN/data_handler.py
--rw-r--r--   0 johnjim    (501) staff       (20)     4445 2024-02-25 07:46:04.000000 joyrl-0.6.1.3/joyrl/algos/NoisyDQN/policy.py
-drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-02 02:57:40.467785 joyrl-0.6.1.3/joyrl/algos/PPO/
--rw-r--r--   0 johnjim    (501) staff       (20)        0 2024-02-25 07:46:04.000000 joyrl-0.6.1.3/joyrl/algos/PPO/__init__.py
--rw-r--r--   0 johnjim    (501) staff       (20)     2071 2024-06-01 16:35:55.000000 joyrl-0.6.1.3/joyrl/algos/PPO/config.py
--rw-r--r--   0 johnjim    (501) staff       (20)     2979 2024-06-01 09:19:48.000000 joyrl-0.6.1.3/joyrl/algos/PPO/data_handler.py
--rw-r--r--   0 johnjim    (501) staff       (20)     6921 2024-06-01 10:23:56.000000 joyrl-0.6.1.3/joyrl/algos/PPO/policy.py
-drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-02 02:57:40.468399 joyrl-0.6.1.3/joyrl/algos/QLearning/
--rw-r--r--   0 johnjim    (501) staff       (20)        0 2024-02-25 07:46:04.000000 joyrl-0.6.1.3/joyrl/algos/QLearning/__init__.py
--rw-r--r--   0 johnjim    (501) staff       (20)      431 2024-02-25 07:46:04.000000 joyrl-0.6.1.3/joyrl/algos/QLearning/config.py
--rw-r--r--   0 johnjim    (501) staff       (20)     1302 2024-05-27 05:48:19.000000 joyrl-0.6.1.3/joyrl/algos/QLearning/data_handler.py
--rw-r--r--   0 johnjim    (501) staff       (20)     1964 2024-02-25 07:46:04.000000 joyrl-0.6.1.3/joyrl/algos/QLearning/policy.py
-drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-02 02:57:40.468979 joyrl-0.6.1.3/joyrl/algos/Sarsa/
--rw-r--r--   0 johnjim    (501) staff       (20)        0 2024-02-25 07:46:04.000000 joyrl-0.6.1.3/joyrl/algos/Sarsa/__init__.py
--rw-r--r--   0 johnjim    (501) staff       (20)      431 2024-02-25 07:46:04.000000 joyrl-0.6.1.3/joyrl/algos/Sarsa/config.py
--rw-r--r--   0 johnjim    (501) staff       (20)     1302 2024-05-27 05:48:19.000000 joyrl-0.6.1.3/joyrl/algos/Sarsa/data_handler.py
--rw-r--r--   0 johnjim    (501) staff       (20)     2144 2024-02-25 07:46:04.000000 joyrl-0.6.1.3/joyrl/algos/Sarsa/policy.py
-drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-02 02:57:40.469494 joyrl-0.6.1.3/joyrl/algos/TD3/
--rw-r--r--   0 johnjim    (501) staff       (20)        0 2024-02-25 07:46:04.000000 joyrl-0.6.1.3/joyrl/algos/TD3/__init__.py
--rw-r--r--   0 johnjim    (501) staff       (20)     1277 2024-02-25 07:46:04.000000 joyrl-0.6.1.3/joyrl/algos/TD3/config.py
--rw-r--r--   0 johnjim    (501) staff       (20)      153 2024-02-25 07:46:04.000000 joyrl-0.6.1.3/joyrl/algos/TD3/data_handler.py
--rw-r--r--   0 johnjim    (501) staff       (20)     7726 2024-02-25 07:46:04.000000 joyrl-0.6.1.3/joyrl/algos/TD3/policy.py
--rw-r--r--   0 johnjim    (501) staff       (20)      366 2024-02-25 07:46:04.000000 joyrl-0.6.1.3/joyrl/algos/__init__.py
-drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-02 02:57:40.472017 joyrl-0.6.1.3/joyrl/algos/base/
--rw-r--r--   0 johnjim    (501) staff       (20)        0 2024-02-25 07:46:04.000000 joyrl-0.6.1.3/joyrl/algos/base/__init__.py
--rw-r--r--   0 johnjim    (501) staff       (20)    10114 2024-06-01 16:17:16.000000 joyrl-0.6.1.3/joyrl/algos/base/action_layer.py
--rw-r--r--   0 johnjim    (501) staff       (20)     8643 2024-02-25 07:46:04.000000 joyrl-0.6.1.3/joyrl/algos/base/base_layer.py
--rw-r--r--   0 johnjim    (501) staff       (20)    86101 2024-06-02 02:50:43.000000 joyrl-0.6.1.3/joyrl/algos/base/buffer.py
--rw-r--r--   0 johnjim    (501) staff       (20)     2711 2024-06-02 02:50:56.000000 joyrl-0.6.1.3/joyrl/algos/base/data_handler.py
--rw-r--r--   0 johnjim    (501) staff       (20)      131 2024-02-25 07:46:04.000000 joyrl-0.6.1.3/joyrl/algos/base/experience.py
--rw-r--r--   0 johnjim    (501) staff       (20)    13934 2024-06-02 02:51:15.000000 joyrl-0.6.1.3/joyrl/algos/base/network.py
--rw-r--r--   0 johnjim    (501) staff       (20)     1313 2024-02-25 07:46:04.000000 joyrl-0.6.1.3/joyrl/algos/base/noise.py
--rw-r--r--   0 johnjim    (501) staff       (20)     2407 2024-02-25 07:46:04.000000 joyrl-0.6.1.3/joyrl/algos/base/optm.py
--rw-r--r--   0 johnjim    (501) staff       (20)     7793 2024-06-02 02:32:38.000000 joyrl-0.6.1.3/joyrl/algos/base/policy.py
-drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-02 02:57:40.473830 joyrl-0.6.1.3/joyrl/envs/
--rw-r--r--   0 johnjim    (501) staff       (20)       51 2024-02-25 07:46:04.000000 joyrl-0.6.1.3/joyrl/envs/__init__.py
--rw-r--r--   0 johnjim    (501) staff       (20)     4258 2024-02-25 07:46:04.000000 joyrl-0.6.1.3/joyrl/envs/blackjack.py
--rw-r--r--   0 johnjim    (501) staff       (20)     2706 2024-02-25 07:46:04.000000 joyrl-0.6.1.3/joyrl/envs/cliff_walking.py
--rw-r--r--   0 johnjim    (501) staff       (20)     3871 2024-02-25 07:46:04.000000 joyrl-0.6.1.3/joyrl/envs/gridworld.py
--rw-r--r--   0 johnjim    (501) staff       (20)     3485 2024-02-25 07:46:04.000000 joyrl-0.6.1.3/joyrl/envs/gridworld_env.py
-drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-02 02:57:40.474339 joyrl-0.6.1.3/joyrl/envs/gym/
--rw-r--r--   0 johnjim    (501) staff       (20)      221 2024-02-25 07:46:04.000000 joyrl-0.6.1.3/joyrl/envs/gym/__init__.py
--rw-r--r--   0 johnjim    (501) staff       (20)      525 2024-02-25 07:46:04.000000 joyrl-0.6.1.3/joyrl/envs/gym/config.py
--rw-r--r--   0 johnjim    (501) staff       (20)    11068 2024-05-09 16:41:09.000000 joyrl-0.6.1.3/joyrl/envs/gym/wrappers.py
--rw-r--r--   0 johnjim    (501) staff       (20)     9890 2024-02-25 07:46:04.000000 joyrl-0.6.1.3/joyrl/envs/racetrack.py
--rw-r--r--   0 johnjim    (501) staff       (20)     1445 2024-02-25 07:46:04.000000 joyrl-0.6.1.3/joyrl/envs/register.py
--rw-r--r--   0 johnjim    (501) staff       (20)     1311 2024-02-25 07:46:04.000000 joyrl-0.6.1.3/joyrl/envs/stochastic_mdp.py
--rw-r--r--   0 johnjim    (501) staff       (20)     2615 2024-02-25 07:46:04.000000 joyrl-0.6.1.3/joyrl/envs/windy_gridworld.py
-drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-02 02:57:40.476096 joyrl-0.6.1.3/joyrl/framework/
--rw-r--r--   0 johnjim    (501) staff       (20)        0 2024-02-25 07:46:04.000000 joyrl-0.6.1.3/joyrl/framework/__init__.py
--rw-r--r--   0 johnjim    (501) staff       (20)     1073 2024-06-02 02:50:42.000000 joyrl-0.6.1.3/joyrl/framework/base.py
--rw-r--r--   0 johnjim    (501) staff       (20)     4376 2024-06-02 02:57:10.000000 joyrl-0.6.1.3/joyrl/framework/collector.py
--rw-r--r--   0 johnjim    (501) staff       (20)     2295 2024-06-02 02:03:30.000000 joyrl-0.6.1.3/joyrl/framework/config.py
--rw-r--r--   0 johnjim    (501) staff       (20)     5561 2024-06-02 02:57:23.000000 joyrl-0.6.1.3/joyrl/framework/interactor.py
--rw-r--r--   0 johnjim    (501) staff       (20)     2782 2024-06-02 02:57:37.000000 joyrl-0.6.1.3/joyrl/framework/learner.py
--rw-r--r--   0 johnjim    (501) staff       (20)      821 2024-05-28 01:37:10.000000 joyrl-0.6.1.3/joyrl/framework/message.py
--rw-r--r--   0 johnjim    (501) staff       (20)     2927 2024-06-02 02:50:38.000000 joyrl-0.6.1.3/joyrl/framework/policy_mgr.py
--rw-r--r--   0 johnjim    (501) staff       (20)     5276 2024-06-02 02:50:37.000000 joyrl-0.6.1.3/joyrl/framework/recorder.py
--rw-r--r--   0 johnjim    (501) staff       (20)     3965 2024-06-02 02:50:36.000000 joyrl-0.6.1.3/joyrl/framework/tester.py
--rw-r--r--   0 johnjim    (501) staff       (20)     2242 2024-02-25 07:46:04.000000 joyrl-0.6.1.3/joyrl/framework/tracker.py
--rw-r--r--   0 johnjim    (501) staff       (20)     7028 2024-06-02 02:50:35.000000 joyrl-0.6.1.3/joyrl/framework/trainer.py
--rw-r--r--   0 johnjim    (501) staff       (20)    39479 2024-06-02 02:50:21.000000 joyrl-0.6.1.3/joyrl/framework/utils.py
--rw-r--r--   0 johnjim    (501) staff       (20)     8007 2024-06-02 02:48:05.000000 joyrl-0.6.1.3/joyrl/run.py
-drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-02 02:57:40.476659 joyrl-0.6.1.3/joyrl/scripts/
--rw-r--r--   0 johnjim    (501) staff       (20)      184 2024-02-25 07:46:04.000000 joyrl-0.6.1.3/joyrl/scripts/__init__.py
--rw-r--r--   0 johnjim    (501) staff       (20)      520 2024-02-25 07:46:04.000000 joyrl-0.6.1.3/joyrl/scripts/scripts.py
-drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-02 02:57:40.476942 joyrl-0.6.1.3/joyrl.egg-info/
--rw-r--r--   0 johnjim    (501) staff       (20)    11639 2024-06-02 02:57:40.000000 joyrl-0.6.1.3/joyrl.egg-info/PKG-INFO
--rw-r--r--   0 johnjim    (501) staff       (20)     2390 2024-06-02 02:57:40.000000 joyrl-0.6.1.3/joyrl.egg-info/SOURCES.txt
--rw-r--r--   0 johnjim    (501) staff       (20)        1 2024-06-02 02:57:40.000000 joyrl-0.6.1.3/joyrl.egg-info/dependency_links.txt
--rw-r--r--   0 johnjim    (501) staff       (20)       53 2024-06-02 02:57:40.000000 joyrl-0.6.1.3/joyrl.egg-info/entry_points.txt
--rw-r--r--   0 johnjim    (501) staff       (20)      256 2024-06-02 02:57:40.000000 joyrl-0.6.1.3/joyrl.egg-info/requires.txt
--rw-r--r--   0 johnjim    (501) staff       (20)        6 2024-06-02 02:57:40.000000 joyrl-0.6.1.3/joyrl.egg-info/top_level.txt
--rw-r--r--   0 johnjim    (501) staff       (20)      940 2024-06-02 02:57:40.477876 joyrl-0.6.1.3/setup.cfg
--rw-r--r--   0 johnjim    (501) staff       (20)     1886 2024-06-01 09:01:11.000000 joyrl-0.6.1.3/setup.py
+drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-03 05:27:38.219935 joyrl-0.6.1.4/
+-rw-r--r--   0 johnjim    (501) staff       (20)     1077 2024-02-25 07:46:04.000000 joyrl-0.6.1.4/LICENSE
+-rw-r--r--   0 johnjim    (501) staff       (20)    11639 2024-06-03 05:27:38.219801 joyrl-0.6.1.4/PKG-INFO
+-rw-r--r--   0 johnjim    (501) staff       (20)    10670 2024-06-01 08:59:02.000000 joyrl-0.6.1.4/README.md
+drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-03 05:27:38.205500 joyrl-0.6.1.4/joyrl/
+-rw-r--r--   0 johnjim    (501) staff       (20)      357 2024-06-03 05:27:33.000000 joyrl-0.6.1.4/joyrl/__init__.py
+drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-03 05:27:38.206481 joyrl-0.6.1.4/joyrl/algos/
+drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-03 05:27:38.207243 joyrl-0.6.1.4/joyrl/algos/DDPG/
+-rw-r--r--   0 johnjim    (501) staff       (20)        0 2024-02-25 07:46:04.000000 joyrl-0.6.1.4/joyrl/algos/DDPG/__init__.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     1517 2024-02-25 07:46:04.000000 joyrl-0.6.1.4/joyrl/algos/DDPG/config.py
+-rw-r--r--   0 johnjim    (501) staff       (20)      152 2024-02-25 07:46:04.000000 joyrl-0.6.1.4/joyrl/algos/DDPG/data_handler.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     5540 2024-02-25 07:46:04.000000 joyrl-0.6.1.4/joyrl/algos/DDPG/policy.py
+drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-03 05:27:38.207852 joyrl-0.6.1.4/joyrl/algos/DQN/
+-rw-r--r--   0 johnjim    (501) staff       (20)        0 2024-02-25 07:46:04.000000 joyrl-0.6.1.4/joyrl/algos/DQN/__init__.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     1950 2024-06-02 02:51:34.000000 joyrl-0.6.1.4/joyrl/algos/DQN/config.py
+-rw-r--r--   0 johnjim    (501) staff       (20)      158 2024-02-25 07:46:04.000000 joyrl-0.6.1.4/joyrl/algos/DQN/data_handler.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     3629 2024-06-03 05:13:02.000000 joyrl-0.6.1.4/joyrl/algos/DQN/policy.py
+drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-03 05:27:38.208437 joyrl-0.6.1.4/joyrl/algos/DoubleDQN/
+-rw-r--r--   0 johnjim    (501) staff       (20)        0 2024-02-25 07:46:04.000000 joyrl-0.6.1.4/joyrl/algos/DoubleDQN/__init__.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     1703 2024-02-25 07:46:04.000000 joyrl-0.6.1.4/joyrl/algos/DoubleDQN/config.py
+-rw-r--r--   0 johnjim    (501) staff       (20)      350 2024-02-25 07:46:04.000000 joyrl-0.6.1.4/joyrl/algos/DoubleDQN/data_handler.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     3512 2024-06-02 02:34:38.000000 joyrl-0.6.1.4/joyrl/algos/DoubleDQN/policy.py
+drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-03 05:27:38.209039 joyrl-0.6.1.4/joyrl/algos/DuelingDQN/
+-rw-r--r--   0 johnjim    (501) staff       (20)        0 2024-02-25 07:46:04.000000 joyrl-0.6.1.4/joyrl/algos/DuelingDQN/__init__.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     1773 2024-06-01 16:33:50.000000 joyrl-0.6.1.4/joyrl/algos/DuelingDQN/config.py
+-rw-r--r--   0 johnjim    (501) staff       (20)      337 2024-02-25 07:46:04.000000 joyrl-0.6.1.4/joyrl/algos/DuelingDQN/data_handler.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     3626 2024-06-02 02:19:04.000000 joyrl-0.6.1.4/joyrl/algos/DuelingDQN/policy.py
+drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-03 05:27:38.209581 joyrl-0.6.1.4/joyrl/algos/NoisyDQN/
+-rw-r--r--   0 johnjim    (501) staff       (20)      184 2024-02-25 07:46:04.000000 joyrl-0.6.1.4/joyrl/algos/NoisyDQN/__init__.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     1065 2024-06-03 05:24:52.000000 joyrl-0.6.1.4/joyrl/algos/NoisyDQN/config.py
+-rw-r--r--   0 johnjim    (501) staff       (20)      341 2024-02-25 07:46:04.000000 joyrl-0.6.1.4/joyrl/algos/NoisyDQN/data_handler.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     3632 2024-06-03 05:25:20.000000 joyrl-0.6.1.4/joyrl/algos/NoisyDQN/policy.py
+drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-03 05:27:38.210162 joyrl-0.6.1.4/joyrl/algos/PPO/
+-rw-r--r--   0 johnjim    (501) staff       (20)        0 2024-02-25 07:46:04.000000 joyrl-0.6.1.4/joyrl/algos/PPO/__init__.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     2071 2024-06-01 16:35:55.000000 joyrl-0.6.1.4/joyrl/algos/PPO/config.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     2979 2024-06-01 09:19:48.000000 joyrl-0.6.1.4/joyrl/algos/PPO/data_handler.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     6921 2024-06-01 10:23:56.000000 joyrl-0.6.1.4/joyrl/algos/PPO/policy.py
+drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-03 05:27:38.210657 joyrl-0.6.1.4/joyrl/algos/QLearning/
+-rw-r--r--   0 johnjim    (501) staff       (20)        0 2024-02-25 07:46:04.000000 joyrl-0.6.1.4/joyrl/algos/QLearning/__init__.py
+-rw-r--r--   0 johnjim    (501) staff       (20)      431 2024-02-25 07:46:04.000000 joyrl-0.6.1.4/joyrl/algos/QLearning/config.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     1302 2024-05-27 05:48:19.000000 joyrl-0.6.1.4/joyrl/algos/QLearning/data_handler.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     1964 2024-02-25 07:46:04.000000 joyrl-0.6.1.4/joyrl/algos/QLearning/policy.py
+drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-03 05:27:38.211116 joyrl-0.6.1.4/joyrl/algos/Sarsa/
+-rw-r--r--   0 johnjim    (501) staff       (20)        0 2024-02-25 07:46:04.000000 joyrl-0.6.1.4/joyrl/algos/Sarsa/__init__.py
+-rw-r--r--   0 johnjim    (501) staff       (20)      431 2024-02-25 07:46:04.000000 joyrl-0.6.1.4/joyrl/algos/Sarsa/config.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     1302 2024-05-27 05:48:19.000000 joyrl-0.6.1.4/joyrl/algos/Sarsa/data_handler.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     2144 2024-02-25 07:46:04.000000 joyrl-0.6.1.4/joyrl/algos/Sarsa/policy.py
+drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-03 05:27:38.211560 joyrl-0.6.1.4/joyrl/algos/TD3/
+-rw-r--r--   0 johnjim    (501) staff       (20)        0 2024-02-25 07:46:04.000000 joyrl-0.6.1.4/joyrl/algos/TD3/__init__.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     1277 2024-02-25 07:46:04.000000 joyrl-0.6.1.4/joyrl/algos/TD3/config.py
+-rw-r--r--   0 johnjim    (501) staff       (20)      153 2024-02-25 07:46:04.000000 joyrl-0.6.1.4/joyrl/algos/TD3/data_handler.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     7726 2024-02-25 07:46:04.000000 joyrl-0.6.1.4/joyrl/algos/TD3/policy.py
+-rw-r--r--   0 johnjim    (501) staff       (20)      366 2024-02-25 07:46:04.000000 joyrl-0.6.1.4/joyrl/algos/__init__.py
+drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-03 05:27:38.213979 joyrl-0.6.1.4/joyrl/algos/base/
+-rw-r--r--   0 johnjim    (501) staff       (20)        0 2024-02-25 07:46:04.000000 joyrl-0.6.1.4/joyrl/algos/base/__init__.py
+-rw-r--r--   0 johnjim    (501) staff       (20)    10114 2024-06-01 16:17:16.000000 joyrl-0.6.1.4/joyrl/algos/base/action_layer.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     8643 2024-02-25 07:46:04.000000 joyrl-0.6.1.4/joyrl/algos/base/base_layer.py
+-rw-r--r--   0 johnjim    (501) staff       (20)    86101 2024-06-02 02:50:43.000000 joyrl-0.6.1.4/joyrl/algos/base/buffer.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     2711 2024-06-02 02:50:56.000000 joyrl-0.6.1.4/joyrl/algos/base/data_handler.py
+-rw-r--r--   0 johnjim    (501) staff       (20)      131 2024-02-25 07:46:04.000000 joyrl-0.6.1.4/joyrl/algos/base/experience.py
+-rw-r--r--   0 johnjim    (501) staff       (20)    13934 2024-06-02 02:51:15.000000 joyrl-0.6.1.4/joyrl/algos/base/network.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     1313 2024-02-25 07:46:04.000000 joyrl-0.6.1.4/joyrl/algos/base/noise.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     2407 2024-02-25 07:46:04.000000 joyrl-0.6.1.4/joyrl/algos/base/optm.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     7793 2024-06-02 02:32:38.000000 joyrl-0.6.1.4/joyrl/algos/base/policy.py
+drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-03 05:27:38.215467 joyrl-0.6.1.4/joyrl/envs/
+-rw-r--r--   0 johnjim    (501) staff       (20)       51 2024-02-25 07:46:04.000000 joyrl-0.6.1.4/joyrl/envs/__init__.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     4258 2024-02-25 07:46:04.000000 joyrl-0.6.1.4/joyrl/envs/blackjack.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     2706 2024-02-25 07:46:04.000000 joyrl-0.6.1.4/joyrl/envs/cliff_walking.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     3871 2024-02-25 07:46:04.000000 joyrl-0.6.1.4/joyrl/envs/gridworld.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     3485 2024-02-25 07:46:04.000000 joyrl-0.6.1.4/joyrl/envs/gridworld_env.py
+drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-03 05:27:38.215976 joyrl-0.6.1.4/joyrl/envs/gym/
+-rw-r--r--   0 johnjim    (501) staff       (20)      221 2024-02-25 07:46:04.000000 joyrl-0.6.1.4/joyrl/envs/gym/__init__.py
+-rw-r--r--   0 johnjim    (501) staff       (20)      525 2024-02-25 07:46:04.000000 joyrl-0.6.1.4/joyrl/envs/gym/config.py
+-rw-r--r--   0 johnjim    (501) staff       (20)    11068 2024-05-09 16:41:09.000000 joyrl-0.6.1.4/joyrl/envs/gym/wrappers.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     9890 2024-02-25 07:46:04.000000 joyrl-0.6.1.4/joyrl/envs/racetrack.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     1445 2024-02-25 07:46:04.000000 joyrl-0.6.1.4/joyrl/envs/register.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     1311 2024-02-25 07:46:04.000000 joyrl-0.6.1.4/joyrl/envs/stochastic_mdp.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     2615 2024-02-25 07:46:04.000000 joyrl-0.6.1.4/joyrl/envs/windy_gridworld.py
+drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-03 05:27:38.218688 joyrl-0.6.1.4/joyrl/framework/
+-rw-r--r--   0 johnjim    (501) staff       (20)        0 2024-02-25 07:46:04.000000 joyrl-0.6.1.4/joyrl/framework/__init__.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     1073 2024-06-02 02:50:42.000000 joyrl-0.6.1.4/joyrl/framework/base.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     4376 2024-06-02 02:57:10.000000 joyrl-0.6.1.4/joyrl/framework/collector.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     2295 2024-06-02 02:03:30.000000 joyrl-0.6.1.4/joyrl/framework/config.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     5561 2024-06-02 02:57:23.000000 joyrl-0.6.1.4/joyrl/framework/interactor.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     2782 2024-06-02 02:57:37.000000 joyrl-0.6.1.4/joyrl/framework/learner.py
+-rw-r--r--   0 johnjim    (501) staff       (20)      821 2024-05-28 01:37:10.000000 joyrl-0.6.1.4/joyrl/framework/message.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     2927 2024-06-02 02:50:38.000000 joyrl-0.6.1.4/joyrl/framework/policy_mgr.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     5276 2024-06-02 02:50:37.000000 joyrl-0.6.1.4/joyrl/framework/recorder.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     3965 2024-06-02 02:50:36.000000 joyrl-0.6.1.4/joyrl/framework/tester.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     2242 2024-02-25 07:46:04.000000 joyrl-0.6.1.4/joyrl/framework/tracker.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     7028 2024-06-02 02:50:35.000000 joyrl-0.6.1.4/joyrl/framework/trainer.py
+-rw-r--r--   0 johnjim    (501) staff       (20)    39479 2024-06-02 02:50:21.000000 joyrl-0.6.1.4/joyrl/framework/utils.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     8007 2024-06-02 02:48:05.000000 joyrl-0.6.1.4/joyrl/run.py
+drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-03 05:27:38.219116 joyrl-0.6.1.4/joyrl/scripts/
+-rw-r--r--   0 johnjim    (501) staff       (20)      184 2024-02-25 07:46:04.000000 joyrl-0.6.1.4/joyrl/scripts/__init__.py
+-rw-r--r--   0 johnjim    (501) staff       (20)      520 2024-02-25 07:46:04.000000 joyrl-0.6.1.4/joyrl/scripts/scripts.py
+drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-03 05:27:38.219288 joyrl-0.6.1.4/joyrl.egg-info/
+-rw-r--r--   0 johnjim    (501) staff       (20)    11639 2024-06-03 05:27:38.000000 joyrl-0.6.1.4/joyrl.egg-info/PKG-INFO
+-rw-r--r--   0 johnjim    (501) staff       (20)     2390 2024-06-03 05:27:38.000000 joyrl-0.6.1.4/joyrl.egg-info/SOURCES.txt
+-rw-r--r--   0 johnjim    (501) staff       (20)        1 2024-06-03 05:27:38.000000 joyrl-0.6.1.4/joyrl.egg-info/dependency_links.txt
+-rw-r--r--   0 johnjim    (501) staff       (20)       53 2024-06-03 05:27:38.000000 joyrl-0.6.1.4/joyrl.egg-info/entry_points.txt
+-rw-r--r--   0 johnjim    (501) staff       (20)      256 2024-06-03 05:27:38.000000 joyrl-0.6.1.4/joyrl.egg-info/requires.txt
+-rw-r--r--   0 johnjim    (501) staff       (20)        6 2024-06-03 05:27:38.000000 joyrl-0.6.1.4/joyrl.egg-info/top_level.txt
+-rw-r--r--   0 johnjim    (501) staff       (20)      940 2024-06-03 05:27:38.220250 joyrl-0.6.1.4/setup.cfg
+-rw-r--r--   0 johnjim    (501) staff       (20)     1886 2024-06-01 09:01:11.000000 joyrl-0.6.1.4/setup.py
```

### Comparing `joyrl-0.6.1.3/LICENSE` & `joyrl-0.6.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1.3/PKG-INFO` & `joyrl-0.6.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: joyrl
-Version: 0.6.1.3
+Version: 0.6.1.4
 Summary: A Library for Deep Reinforcement Learning
 Home-page: https://github.com/datawhalechina/joyrl
 Author: johnjim0816
 Author-email: johnjim0816@gmail.com
 License: MIT
 Keywords: reinforcement learning platform pytorch
 Platform: any
```

### Comparing `joyrl-0.6.1.3/README.md` & `joyrl-0.6.1.4/README.md`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1.3/joyrl/algos/DDPG/config.py` & `joyrl-0.6.1.4/joyrl/algos/DDPG/config.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1.3/joyrl/algos/DDPG/policy.py` & `joyrl-0.6.1.4/joyrl/algos/DDPG/policy.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1.3/joyrl/algos/DQN/config.py` & `joyrl-0.6.1.4/joyrl/algos/DQN/config.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1.3/joyrl/algos/DQN/policy.py` & `joyrl-0.6.1.4/joyrl/algos/DQN/policy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # coding=utf-8
 '''
 Author: JiangJi
 Email: johnjim0816@gmail.com
 Date: 2024-01-25 09:58:33
 LastEditor: JiangJi
-LastEditTime: 2024-06-02 10:14:18
+LastEditTime: 2024-06-03 13:13:02
 Discription: 
 '''
 import torch
 import torch.nn as nn
 import math,random
 import numpy as np
 from joyrl.algos.base.policy import BasePolicy
@@ -24,16 +24,16 @@
         self.epsilon_end = cfg.epsilon_end
         self.epsilon_decay = cfg.epsilon_decay
         self.target_update = cfg.target_update
         self.sample_count = 0
         self.update_step = 0
         
     def create_model(self):
-        self.model = QNetwork(self.cfg,self.state_size_list).to(self.device)
-        self.target_model = QNetwork(self.cfg,self.state_size_list).to(self.device)
+        self.model = QNetwork(self.cfg, self.state_size_list).to(self.device)
+        self.target_model = QNetwork(self.cfg, self.state_size_list).to(self.device)
         self.target_model.load_state_dict(self.model.state_dict()) # or use this to copy parameters
 
     def sample_action(self, state,  **kwargs):
         ''' sample action
         '''
         # epsilon must decay(linear,exponential and etc.) for balancing exploration and exploitation
         self.sample_count += 1
```

### Comparing `joyrl-0.6.1.3/joyrl/algos/DoubleDQN/config.py` & `joyrl-0.6.1.4/joyrl/algos/DoubleDQN/config.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1.3/joyrl/algos/DoubleDQN/policy.py` & `joyrl-0.6.1.4/joyrl/algos/DoubleDQN/policy.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1.3/joyrl/algos/DuelingDQN/config.py` & `joyrl-0.6.1.4/joyrl/algos/DuelingDQN/config.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1.3/joyrl/algos/DuelingDQN/policy.py` & `joyrl-0.6.1.4/joyrl/algos/DuelingDQN/policy.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1.3/joyrl/algos/NoisyDQN/config.py` & `joyrl-0.6.1.4/joyrl/algos/NoisyDQN/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # coding=utf-8
 '''
 Author: JiangJi
 Email: johnjim0816@gmail.com
 Date: 2023-02-21 20:32:11
 LastEditor: JiangJi
-LastEditTime: 2023-05-18 13:38:56
+LastEditTime: 2024-06-03 13:24:36
 Discription: 
 '''
 class AlgoConfig(object):
     ''' algorithm parameters
     '''
     def __init__(self) -> None:
         # set epsilon_start=epsilon_end to get fixed epsilon, i.e. epsilon=epsilon_end
@@ -17,12 +17,12 @@
         self.epsilon_end = 0.01  # epsilon end value
         self.epsilon_decay = 500  # epsilon decay
         self.gamma = 0.95  # reward discount factor
         self.lr = 0.0001  # learning rate
         self.max_buffer_size = 100000  # replay buffer size
         self.batch_size = 64  # batch size
         self.target_update = 4  # target network update frequency
-        # value network layers config
-        self.value_layers = [
+        self.branch_layers = []
+        self.merge_layers = [
             {'layer_type': 'noisy_linear', 'layer_size': [64], 'activation': 'ReLU','std_init': 0.4},
             {'layer_type': 'noisy_linear', 'layer_size': [64], 'activation': 'ReLU','std_init': 0.4},
         ]
```

### Comparing `joyrl-0.6.1.3/joyrl/algos/PPO/config.py` & `joyrl-0.6.1.4/joyrl/algos/PPO/config.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1.3/joyrl/algos/PPO/data_handler.py` & `joyrl-0.6.1.4/joyrl/algos/PPO/data_handler.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1.3/joyrl/algos/PPO/policy.py` & `joyrl-0.6.1.4/joyrl/algos/PPO/policy.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1.3/joyrl/algos/QLearning/data_handler.py` & `joyrl-0.6.1.4/joyrl/algos/QLearning/data_handler.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1.3/joyrl/algos/QLearning/policy.py` & `joyrl-0.6.1.4/joyrl/algos/QLearning/policy.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1.3/joyrl/algos/Sarsa/data_handler.py` & `joyrl-0.6.1.4/joyrl/algos/Sarsa/data_handler.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1.3/joyrl/algos/Sarsa/policy.py` & `joyrl-0.6.1.4/joyrl/algos/Sarsa/policy.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1.3/joyrl/algos/TD3/config.py` & `joyrl-0.6.1.4/joyrl/algos/TD3/config.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1.3/joyrl/algos/TD3/policy.py` & `joyrl-0.6.1.4/joyrl/algos/TD3/policy.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1.3/joyrl/algos/base/action_layer.py` & `joyrl-0.6.1.4/joyrl/algos/base/action_layer.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1.3/joyrl/algos/base/base_layer.py` & `joyrl-0.6.1.4/joyrl/algos/base/base_layer.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1.3/joyrl/algos/base/buffer.py` & `joyrl-0.6.1.4/joyrl/algos/base/buffer.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1.3/joyrl/algos/base/data_handler.py` & `joyrl-0.6.1.4/joyrl/algos/base/data_handler.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1.3/joyrl/algos/base/network.py` & `joyrl-0.6.1.4/joyrl/algos/base/network.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1.3/joyrl/algos/base/noise.py` & `joyrl-0.6.1.4/joyrl/algos/base/noise.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1.3/joyrl/algos/base/optm.py` & `joyrl-0.6.1.4/joyrl/algos/base/optm.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1.3/joyrl/algos/base/policy.py` & `joyrl-0.6.1.4/joyrl/algos/base/policy.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1.3/joyrl/envs/blackjack.py` & `joyrl-0.6.1.4/joyrl/envs/blackjack.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1.3/joyrl/envs/cliff_walking.py` & `joyrl-0.6.1.4/joyrl/envs/cliff_walking.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1.3/joyrl/envs/gridworld.py` & `joyrl-0.6.1.4/joyrl/envs/gridworld.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1.3/joyrl/envs/gridworld_env.py` & `joyrl-0.6.1.4/joyrl/envs/gridworld_env.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1.3/joyrl/envs/gym/config.py` & `joyrl-0.6.1.4/joyrl/envs/gym/config.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1.3/joyrl/envs/gym/wrappers.py` & `joyrl-0.6.1.4/joyrl/envs/gym/wrappers.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1.3/joyrl/envs/racetrack.py` & `joyrl-0.6.1.4/joyrl/envs/racetrack.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1.3/joyrl/envs/register.py` & `joyrl-0.6.1.4/joyrl/envs/register.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1.3/joyrl/envs/stochastic_mdp.py` & `joyrl-0.6.1.4/joyrl/envs/stochastic_mdp.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1.3/joyrl/envs/windy_gridworld.py` & `joyrl-0.6.1.4/joyrl/envs/windy_gridworld.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1.3/joyrl/framework/base.py` & `joyrl-0.6.1.4/joyrl/framework/base.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1.3/joyrl/framework/collector.py` & `joyrl-0.6.1.4/joyrl/framework/collector.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1.3/joyrl/framework/config.py` & `joyrl-0.6.1.4/joyrl/framework/config.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1.3/joyrl/framework/interactor.py` & `joyrl-0.6.1.4/joyrl/framework/interactor.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1.3/joyrl/framework/learner.py` & `joyrl-0.6.1.4/joyrl/framework/learner.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1.3/joyrl/framework/message.py` & `joyrl-0.6.1.4/joyrl/framework/message.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1.3/joyrl/framework/policy_mgr.py` & `joyrl-0.6.1.4/joyrl/framework/policy_mgr.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1.3/joyrl/framework/recorder.py` & `joyrl-0.6.1.4/joyrl/framework/recorder.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1.3/joyrl/framework/tester.py` & `joyrl-0.6.1.4/joyrl/framework/tester.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1.3/joyrl/framework/tracker.py` & `joyrl-0.6.1.4/joyrl/framework/tracker.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1.3/joyrl/framework/trainer.py` & `joyrl-0.6.1.4/joyrl/framework/trainer.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1.3/joyrl/framework/utils.py` & `joyrl-0.6.1.4/joyrl/framework/utils.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1.3/joyrl/run.py` & `joyrl-0.6.1.4/joyrl/run.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1.3/joyrl/scripts/scripts.py` & `joyrl-0.6.1.4/joyrl/scripts/scripts.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1.3/joyrl.egg-info/PKG-INFO` & `joyrl-0.6.1.4/joyrl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: joyrl
-Version: 0.6.1.3
+Version: 0.6.1.4
 Summary: A Library for Deep Reinforcement Learning
 Home-page: https://github.com/datawhalechina/joyrl
 Author: johnjim0816
 Author-email: johnjim0816@gmail.com
 License: MIT
 Keywords: reinforcement learning platform pytorch
 Platform: any
```

### Comparing `joyrl-0.6.1.3/joyrl.egg-info/SOURCES.txt` & `joyrl-0.6.1.4/joyrl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1.3/setup.cfg` & `joyrl-0.6.1.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.1.3/setup.py` & `joyrl-0.6.1.4/setup.py`

 * *Files identical despite different names*

