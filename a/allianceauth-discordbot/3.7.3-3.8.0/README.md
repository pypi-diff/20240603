# Comparing `tmp/allianceauth_discordbot-3.7.3.tar.gz` & `tmp/allianceauth_discordbot-3.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "allianceauth_discordbot-3.7.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "allianceauth_discordbot-3.8.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `allianceauth_discordbot-3.7.3.tar` & `allianceauth_discordbot-3.8.0.tar`

### file list

```diff
@@ -1,72 +1,84 @@
--rw-r--r--   0        0        0     1322 2024-05-12 08:25:35.969976 allianceauth_discordbot-3.7.3/.github/workflows/main.yml
--rw-r--r--   0        0        0      719 2024-05-12 08:25:35.969976 allianceauth_discordbot-3.7.3/.github/workflows/publish.yml
--rw-r--r--   0        0        0      339 2024-05-12 08:25:35.969976 allianceauth_discordbot-3.7.3/.gitignore
--rw-r--r--   0        0        0      179 2024-05-12 08:25:35.969976 allianceauth_discordbot-3.7.3/.isort.cfg
--rw-r--r--   0        0        0     2553 2024-05-12 08:25:35.969976 allianceauth_discordbot-3.7.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0      272 2024-05-12 08:25:35.969976 allianceauth_discordbot-3.7.3/.tx/transifex.yml
--rw-r--r--   0        0        0     3318 2024-05-12 08:25:35.969976 allianceauth_discordbot-3.7.3/CHANGELOG.md
--rw-r--r--   0        0        0     1077 2024-05-12 08:25:35.973976 allianceauth_discordbot-3.7.3/LICENSE
--rw-r--r--   0        0        0      109 2024-05-12 08:25:35.973976 allianceauth_discordbot-3.7.3/MANIFEST.in
--rw-r--r--   0        0        0      636 2024-05-12 08:25:35.973976 allianceauth_discordbot-3.7.3/Makefile
--rw-r--r--   0        0        0    16093 2024-05-12 08:25:35.973976 allianceauth_discordbot-3.7.3/README.md
--rw-r--r--   0        0        0      176 2024-05-12 08:25:35.973976 allianceauth_discordbot-3.7.3/aadiscordbot/__init__.py
--rw-r--r--   0        0        0     2069 2024-05-12 08:25:35.973976 allianceauth_discordbot-3.7.3/aadiscordbot/admin.py
--rw-r--r--   0        0        0     4370 2024-05-12 08:25:35.973976 allianceauth_discordbot-3.7.3/aadiscordbot/app_settings.py
--rw-r--r--   0        0        0      263 2024-05-12 08:25:35.973976 allianceauth_discordbot-3.7.3/aadiscordbot/apps.py
--rw-r--r--   0        0        0      928 2024-05-12 08:25:35.973976 allianceauth_discordbot-3.7.3/aadiscordbot/auth_hooks.py
--rw-r--r--   0        0        0    17002 2024-05-12 08:25:35.973976 allianceauth_discordbot-3.7.3/aadiscordbot/bot.py
--rw-r--r--   0        0        0     4774 2024-05-12 08:25:35.973976 allianceauth_discordbot-3.7.3/aadiscordbot/bot_tasks.py
--rw-r--r--   0        0        0        0 2024-05-12 08:25:35.973976 allianceauth_discordbot-3.7.3/aadiscordbot/cogs/__init__.py
--rw-r--r--   0        0        0     3261 2024-05-12 08:25:35.973976 allianceauth_discordbot-3.7.3/aadiscordbot/cogs/about.py
--rw-r--r--   0        0        0     2931 2024-05-12 08:25:35.973976 allianceauth_discordbot-3.7.3/aadiscordbot/cogs/abuse.py
--rw-r--r--   0        0        0     1093 2024-05-12 08:25:35.973976 allianceauth_discordbot-3.7.3/aadiscordbot/cogs/abuse_two.py
--rw-r--r--   0        0        0    16421 2024-05-12 08:25:35.973976 allianceauth_discordbot-3.7.3/aadiscordbot/cogs/admin.py
--rw-r--r--   0        0        0     2694 2024-05-12 08:25:35.973976 allianceauth_discordbot-3.7.3/aadiscordbot/cogs/auth.py
--rw-r--r--   0        0        0      909 2024-05-12 08:25:35.973976 allianceauth_discordbot-3.7.3/aadiscordbot/cogs/eastereggs.py
--rw-r--r--   0        0        0     1459 2024-05-12 08:25:35.973976 allianceauth_discordbot-3.7.3/aadiscordbot/cogs/eightball.py
--rw-r--r--   0        0        0     3827 2024-05-12 08:25:35.973976 allianceauth_discordbot-3.7.3/aadiscordbot/cogs/facwar.py
--rw-r--r--   0        0        0    12709 2024-05-12 08:25:35.973976 allianceauth_discordbot-3.7.3/aadiscordbot/cogs/members.py
--rw-r--r--   0        0        0     3531 2024-05-12 08:25:35.973976 allianceauth_discordbot-3.7.3/aadiscordbot/cogs/models.py
--rw-r--r--   0        0        0     5703 2024-05-12 08:25:35.973976 allianceauth_discordbot-3.7.3/aadiscordbot/cogs/price_check.py
--rw-r--r--   0        0        0     1495 2024-05-12 08:25:35.973976 allianceauth_discordbot-3.7.3/aadiscordbot/cogs/prom_export.py
--rw-r--r--   0        0        0     5180 2024-05-12 08:25:35.973976 allianceauth_discordbot-3.7.3/aadiscordbot/cogs/quote.py
--rw-r--r--   0        0        0     6214 2024-05-12 08:25:35.973976 allianceauth_discordbot-3.7.3/aadiscordbot/cogs/reaction_roles.py
--rw-r--r--   0        0        0     1201 2024-05-12 08:25:35.973976 allianceauth_discordbot-3.7.3/aadiscordbot/cogs/remind.py
--rw-r--r--   0        0        0     6532 2024-05-12 08:25:35.973976 allianceauth_discordbot-3.7.3/aadiscordbot/cogs/services.py
--rw-r--r--   0        0        0    15830 2024-05-12 08:25:35.973976 allianceauth_discordbot-3.7.3/aadiscordbot/cogs/sov.py
--rw-r--r--   0        0        0     4650 2024-05-12 08:25:35.973976 allianceauth_discordbot-3.7.3/aadiscordbot/cogs/tickets.py
--rw-r--r--   0        0        0     1396 2024-05-12 08:25:35.973976 allianceauth_discordbot-3.7.3/aadiscordbot/cogs/time.py
--rw-r--r--   0        0        0     2171 2024-05-12 08:25:35.973976 allianceauth_discordbot-3.7.3/aadiscordbot/cogs/timers.py
--rw-r--r--   0        0        0        0 2024-05-12 08:25:35.973976 allianceauth_discordbot-3.7.3/aadiscordbot/cogs/utils/__init__.py
--rw-r--r--   0        0        0      207 2024-05-12 08:25:35.973976 allianceauth_discordbot-3.7.3/aadiscordbot/cogs/utils/context.py
--rw-r--r--   0        0        0     3883 2024-05-12 08:25:35.973976 allianceauth_discordbot-3.7.3/aadiscordbot/cogs/utils/decorators.py
--rw-r--r--   0        0        0      437 2024-05-12 08:25:35.973976 allianceauth_discordbot-3.7.3/aadiscordbot/cogs/utils/exceptions.py
--rw-r--r--   0        0        0     4831 2024-05-12 08:25:35.973976 allianceauth_discordbot-3.7.3/aadiscordbot/cogs/welcomegoodbye.py
--rw-r--r--   0        0        0      235 2024-05-12 08:25:35.973976 allianceauth_discordbot-3.7.3/aadiscordbot/launcher.py
--rw-r--r--   0        0        0     1235 2024-05-12 08:25:35.973976 allianceauth_discordbot-3.7.3/aadiscordbot/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      380 2024-05-12 08:25:35.973976 allianceauth_discordbot-3.7.3/aadiscordbot/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1027 2024-05-12 08:25:35.973976 allianceauth_discordbot-3.7.3/aadiscordbot/locale/en/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1621 2024-05-12 08:25:35.973976 allianceauth_discordbot-3.7.3/aadiscordbot/migrations/0001_initial.py
--rw-r--r--   0        0        0     1410 2024-05-12 08:25:35.973976 allianceauth_discordbot-3.7.3/aadiscordbot/migrations/0002_reactionrolebinding_reactionrolemessage.py
--rw-r--r--   0        0        0      636 2024-05-12 08:25:35.973976 allianceauth_discordbot-3.7.3/aadiscordbot/migrations/0003_authbotconfiguration.py
--rw-r--r--   0        0        0      485 2024-05-12 08:25:35.973976 allianceauth_discordbot-3.7.3/aadiscordbot/migrations/0004_settings.py
--rw-r--r--   0        0        0      759 2024-05-12 08:25:35.973976 allianceauth_discordbot-3.7.3/aadiscordbot/migrations/0005_rr_fixes_blank_admins.py
--rw-r--r--   0        0        0     1773 2024-05-12 08:25:35.973976 allianceauth_discordbot-3.7.3/aadiscordbot/migrations/0006_goodbyemessage_welcomemessage.py
--rw-r--r--   0        0        0     1219 2024-05-12 08:25:35.977976 allianceauth_discordbot-3.7.3/aadiscordbot/migrations/0007_quotemessage.py
--rw-r--r--   0        0        0      413 2024-05-12 08:25:35.977976 allianceauth_discordbot-3.7.3/aadiscordbot/migrations/0008_channels_deleted.py
--rw-r--r--   0        0        0      507 2024-05-12 08:25:35.977976 allianceauth_discordbot-3.7.3/aadiscordbot/migrations/0009_alter_quotemessage_options.py
--rw-r--r--   0        0        0     1056 2024-05-12 08:25:35.977976 allianceauth_discordbot-3.7.3/aadiscordbot/migrations/0010_alter_discordbot_options_ticketgroups.py
--rw-r--r--   0        0        0      805 2024-05-12 08:25:35.977976 allianceauth_discordbot-3.7.3/aadiscordbot/migrations/0011_alter_ticketgroups_options_and_more.py
--rw-r--r--   0        0        0      437 2024-05-12 08:25:35.977976 allianceauth_discordbot-3.7.3/aadiscordbot/migrations/0012_welcomemessage_guild_id.py
--rw-r--r--   0        0        0      425 2024-05-12 08:25:35.977976 allianceauth_discordbot-3.7.3/aadiscordbot/migrations/0013_goodbyemessage_guild_id.py
--rw-r--r--   0        0        0        0 2024-05-12 08:25:35.977976 allianceauth_discordbot-3.7.3/aadiscordbot/migrations/__init__.py
--rw-r--r--   0        0        0     5294 2024-05-12 08:25:35.977976 allianceauth_discordbot-3.7.3/aadiscordbot/models.py
--rw-r--r--   0        0        0      317 2024-05-12 08:25:35.977976 allianceauth_discordbot-3.7.3/aadiscordbot/providers.py
--rw-r--r--   0        0        0     3667 2024-05-12 08:25:35.977976 allianceauth_discordbot-3.7.3/aadiscordbot/tasks.py
--rw-r--r--   0        0        0       45 2024-05-12 08:25:35.977976 allianceauth_discordbot-3.7.3/aadiscordbot/urls.py
--rw-r--r--   0        0        0        0 2024-05-12 08:25:35.977976 allianceauth_discordbot-3.7.3/aadiscordbot/utils/__init__.py
--rw-r--r--   0        0        0     3349 2024-05-12 08:25:35.977976 allianceauth_discordbot-3.7.3/aadiscordbot/utils/auth.py
--rw-r--r--   0        0        0       15 2024-05-12 08:25:35.977976 allianceauth_discordbot-3.7.3/aadiscordbot/views.py
--rw-r--r--   0        0        0      315 2024-05-12 08:25:35.977976 allianceauth_discordbot-3.7.3/bot_conf.py
--rw-r--r--   0        0        0     2174 2024-05-12 08:25:35.977976 allianceauth_discordbot-3.7.3/pyproject.toml
--rw-r--r--   0        0        0    17687 1970-01-01 00:00:00.000000 allianceauth_discordbot-3.7.3/PKG-INFO
+-rw-r--r--   0        0        0      316 2024-06-03 10:24:55.056168 allianceauth_discordbot-3.8.0/.coveragerc
+-rw-r--r--   0        0        0     1308 2024-06-03 10:24:55.056168 allianceauth_discordbot-3.8.0/.github/workflows/main.yml
+-rw-r--r--   0        0        0      719 2024-06-03 10:24:55.056168 allianceauth_discordbot-3.8.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     1196 2024-06-03 10:24:55.056168 allianceauth_discordbot-3.8.0/.gitignore
+-rw-r--r--   0        0        0      179 2024-06-03 10:24:55.056168 allianceauth_discordbot-3.8.0/.isort.cfg
+-rw-r--r--   0        0        0     3125 2024-06-03 10:24:55.056168 allianceauth_discordbot-3.8.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      272 2024-06-03 10:24:55.056168 allianceauth_discordbot-3.8.0/.tx/transifex.yml
+-rw-r--r--   0        0        0     3318 2024-06-03 10:24:55.056168 allianceauth_discordbot-3.8.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1077 2024-06-03 10:24:55.056168 allianceauth_discordbot-3.8.0/LICENSE
+-rw-r--r--   0        0        0      109 2024-06-03 10:24:55.056168 allianceauth_discordbot-3.8.0/MANIFEST.in
+-rw-r--r--   0        0        0      636 2024-06-03 10:24:55.056168 allianceauth_discordbot-3.8.0/Makefile
+-rw-r--r--   0        0        0    16402 2024-06-03 10:24:55.056168 allianceauth_discordbot-3.8.0/README.md
+-rw-r--r--   0        0        0      116 2024-06-03 10:24:55.056168 allianceauth_discordbot-3.8.0/aadiscordbot/__init__.py
+-rw-r--r--   0        0        0     2069 2024-06-03 10:24:55.056168 allianceauth_discordbot-3.8.0/aadiscordbot/admin.py
+-rw-r--r--   0        0        0     4817 2024-06-03 10:24:55.056168 allianceauth_discordbot-3.8.0/aadiscordbot/app_settings.py
+-rw-r--r--   0        0        0      263 2024-06-03 10:24:55.056168 allianceauth_discordbot-3.8.0/aadiscordbot/apps.py
+-rw-r--r--   0        0        0      928 2024-06-03 10:24:55.056168 allianceauth_discordbot-3.8.0/aadiscordbot/auth_hooks.py
+-rw-r--r--   0        0        0    17131 2024-06-03 10:24:55.056168 allianceauth_discordbot-3.8.0/aadiscordbot/bot.py
+-rw-r--r--   0        0        0     4774 2024-06-03 10:24:55.056168 allianceauth_discordbot-3.8.0/aadiscordbot/bot_tasks.py
+-rw-r--r--   0        0        0        0 2024-06-03 10:24:55.056168 allianceauth_discordbot-3.8.0/aadiscordbot/cogs/__init__.py
+-rw-r--r--   0        0        0     3345 2024-06-03 10:24:55.056168 allianceauth_discordbot-3.8.0/aadiscordbot/cogs/about.py
+-rw-r--r--   0        0        0     2900 2024-06-03 10:24:55.056168 allianceauth_discordbot-3.8.0/aadiscordbot/cogs/abuse.py
+-rw-r--r--   0        0        0      879 2024-06-03 10:24:55.056168 allianceauth_discordbot-3.8.0/aadiscordbot/cogs/abuse_two.py
+-rw-r--r--   0        0        0    16421 2024-06-03 10:24:55.056168 allianceauth_discordbot-3.8.0/aadiscordbot/cogs/admin.py
+-rw-r--r--   0        0        0     2336 2024-06-03 10:24:55.060168 allianceauth_discordbot-3.8.0/aadiscordbot/cogs/auth.py
+-rw-r--r--   0        0        0      831 2024-06-03 10:24:55.060168 allianceauth_discordbot-3.8.0/aadiscordbot/cogs/eastereggs.py
+-rw-r--r--   0        0        0     1331 2024-06-03 10:24:55.060168 allianceauth_discordbot-3.8.0/aadiscordbot/cogs/eightball.py
+-rw-r--r--   0        0        0     3827 2024-06-03 10:24:55.060168 allianceauth_discordbot-3.8.0/aadiscordbot/cogs/facwar.py
+-rw-r--r--   0        0        0    12106 2024-06-03 10:24:55.060168 allianceauth_discordbot-3.8.0/aadiscordbot/cogs/members.py
+-rw-r--r--   0        0        0     3531 2024-06-03 10:24:55.060168 allianceauth_discordbot-3.8.0/aadiscordbot/cogs/models.py
+-rw-r--r--   0        0        0     5703 2024-06-03 10:24:55.060168 allianceauth_discordbot-3.8.0/aadiscordbot/cogs/price_check.py
+-rw-r--r--   0        0        0     1495 2024-06-03 10:24:55.060168 allianceauth_discordbot-3.8.0/aadiscordbot/cogs/prom_export.py
+-rw-r--r--   0        0        0     5180 2024-06-03 10:24:55.060168 allianceauth_discordbot-3.8.0/aadiscordbot/cogs/quote.py
+-rw-r--r--   0        0        0     6214 2024-06-03 10:24:55.060168 allianceauth_discordbot-3.8.0/aadiscordbot/cogs/reaction_roles.py
+-rw-r--r--   0        0        0     2474 2024-06-03 10:24:55.060168 allianceauth_discordbot-3.8.0/aadiscordbot/cogs/recruit_me.py
+-rw-r--r--   0        0        0     1201 2024-06-03 10:24:55.060168 allianceauth_discordbot-3.8.0/aadiscordbot/cogs/remind.py
+-rw-r--r--   0        0        0     6532 2024-06-03 10:24:55.060168 allianceauth_discordbot-3.8.0/aadiscordbot/cogs/services.py
+-rw-r--r--   0        0        0    15830 2024-06-03 10:24:55.060168 allianceauth_discordbot-3.8.0/aadiscordbot/cogs/sov.py
+-rw-r--r--   0        0        0     6580 2024-06-03 10:24:55.060168 allianceauth_discordbot-3.8.0/aadiscordbot/cogs/tickets.py
+-rw-r--r--   0        0        0     1396 2024-06-03 10:24:55.060168 allianceauth_discordbot-3.8.0/aadiscordbot/cogs/time.py
+-rw-r--r--   0        0        0     2171 2024-06-03 10:24:55.060168 allianceauth_discordbot-3.8.0/aadiscordbot/cogs/timers.py
+-rw-r--r--   0        0        0        0 2024-06-03 10:24:55.060168 allianceauth_discordbot-3.8.0/aadiscordbot/cogs/utils/__init__.py
+-rw-r--r--   0        0        0      207 2024-06-03 10:24:55.060168 allianceauth_discordbot-3.8.0/aadiscordbot/cogs/utils/context.py
+-rw-r--r--   0        0        0     5306 2024-06-03 10:24:55.060168 allianceauth_discordbot-3.8.0/aadiscordbot/cogs/utils/decorators.py
+-rw-r--r--   0        0        0      735 2024-06-03 10:24:55.060168 allianceauth_discordbot-3.8.0/aadiscordbot/cogs/utils/exceptions.py
+-rw-r--r--   0        0        0     5362 2024-06-03 10:24:55.060168 allianceauth_discordbot-3.8.0/aadiscordbot/cogs/welcomegoodbye.py
+-rw-r--r--   0        0        0      235 2024-06-03 10:24:55.060168 allianceauth_discordbot-3.8.0/aadiscordbot/launcher.py
+-rw-r--r--   0        0        0     1235 2024-06-03 10:24:55.060168 allianceauth_discordbot-3.8.0/aadiscordbot/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      380 2024-06-03 10:24:55.060168 allianceauth_discordbot-3.8.0/aadiscordbot/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1027 2024-06-03 10:24:55.060168 allianceauth_discordbot-3.8.0/aadiscordbot/locale/en/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1621 2024-06-03 10:24:55.060168 allianceauth_discordbot-3.8.0/aadiscordbot/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1410 2024-06-03 10:24:55.060168 allianceauth_discordbot-3.8.0/aadiscordbot/migrations/0002_reactionrolebinding_reactionrolemessage.py
+-rw-r--r--   0        0        0      636 2024-06-03 10:24:55.060168 allianceauth_discordbot-3.8.0/aadiscordbot/migrations/0003_authbotconfiguration.py
+-rw-r--r--   0        0        0      485 2024-06-03 10:24:55.060168 allianceauth_discordbot-3.8.0/aadiscordbot/migrations/0004_settings.py
+-rw-r--r--   0        0        0      759 2024-06-03 10:24:55.060168 allianceauth_discordbot-3.8.0/aadiscordbot/migrations/0005_rr_fixes_blank_admins.py
+-rw-r--r--   0        0        0     1773 2024-06-03 10:24:55.060168 allianceauth_discordbot-3.8.0/aadiscordbot/migrations/0006_goodbyemessage_welcomemessage.py
+-rw-r--r--   0        0        0     1219 2024-06-03 10:24:55.060168 allianceauth_discordbot-3.8.0/aadiscordbot/migrations/0007_quotemessage.py
+-rw-r--r--   0        0        0      413 2024-06-03 10:24:55.060168 allianceauth_discordbot-3.8.0/aadiscordbot/migrations/0008_channels_deleted.py
+-rw-r--r--   0        0        0      507 2024-06-03 10:24:55.060168 allianceauth_discordbot-3.8.0/aadiscordbot/migrations/0009_alter_quotemessage_options.py
+-rw-r--r--   0        0        0     1056 2024-06-03 10:24:55.060168 allianceauth_discordbot-3.8.0/aadiscordbot/migrations/0010_alter_discordbot_options_ticketgroups.py
+-rw-r--r--   0        0        0      805 2024-06-03 10:24:55.060168 allianceauth_discordbot-3.8.0/aadiscordbot/migrations/0011_alter_ticketgroups_options_and_more.py
+-rw-r--r--   0        0        0      437 2024-06-03 10:24:55.060168 allianceauth_discordbot-3.8.0/aadiscordbot/migrations/0012_welcomemessage_guild_id.py
+-rw-r--r--   0        0        0      425 2024-06-03 10:24:55.060168 allianceauth_discordbot-3.8.0/aadiscordbot/migrations/0013_goodbyemessage_guild_id.py
+-rw-r--r--   0        0        0      625 2024-06-03 10:24:55.060168 allianceauth_discordbot-3.8.0/aadiscordbot/migrations/0014_alter_goodbyemessage_guild_id_and_more.py
+-rw-r--r--   0        0        0        0 2024-06-03 10:24:55.060168 allianceauth_discordbot-3.8.0/aadiscordbot/migrations/__init__.py
+-rw-r--r--   0        0        0     5275 2024-06-03 10:24:55.060168 allianceauth_discordbot-3.8.0/aadiscordbot/models.py
+-rw-r--r--   0        0        0      317 2024-06-03 10:24:55.060168 allianceauth_discordbot-3.8.0/aadiscordbot/providers.py
+-rw-r--r--   0        0        0     3667 2024-06-03 10:24:55.060168 allianceauth_discordbot-3.8.0/aadiscordbot/tasks.py
+-rw-r--r--   0        0        0     1357 2024-06-03 10:24:55.060168 allianceauth_discordbot-3.8.0/aadiscordbot/tests/__init__.py
+-rw-r--r--   0        0        0     8065 2024-06-03 10:24:55.060168 allianceauth_discordbot-3.8.0/aadiscordbot/tests/test_utils_auth.py
+-rw-r--r--   0        0        0       45 2024-06-03 10:24:55.060168 allianceauth_discordbot-3.8.0/aadiscordbot/urls.py
+-rw-r--r--   0        0        0        0 2024-06-03 10:24:55.060168 allianceauth_discordbot-3.8.0/aadiscordbot/utils/__init__.py
+-rw-r--r--   0        0        0     4981 2024-06-03 10:24:55.064168 allianceauth_discordbot-3.8.0/aadiscordbot/utils/auth.py
+-rw-r--r--   0        0        0       15 2024-06-03 10:24:55.064168 allianceauth_discordbot-3.8.0/aadiscordbot/views.py
+-rw-r--r--   0        0        0      315 2024-06-03 10:24:55.064168 allianceauth_discordbot-3.8.0/bot_conf.py
+-rw-r--r--   0        0        0     2174 2024-06-03 10:24:55.064168 allianceauth_discordbot-3.8.0/pyproject.toml
+-rw-r--r--   0        0        0      847 2024-06-03 10:24:55.064168 allianceauth_discordbot-3.8.0/runtests.py
+-rw-r--r--   0        0        0       64 2024-06-03 10:24:55.064168 allianceauth_discordbot-3.8.0/tests/__init__.py
+-rw-r--r--   0        0        0      606 2024-06-03 10:24:55.064168 allianceauth_discordbot-3.8.0/tests/celery.py
+-rw-r--r--   0        0        0     1648 2024-06-03 10:24:55.064168 allianceauth_discordbot-3.8.0/tests/test_settings.py
+-rw-r--r--   0        0        0      325 2024-06-03 10:24:55.064168 allianceauth_discordbot-3.8.0/tests/urls.py
+-rw-r--r--   0        0        0       98 2024-06-03 10:24:55.064168 allianceauth_discordbot-3.8.0/tests/views.py
+-rw-r--r--   0        0        0      421 2024-06-03 10:24:55.064168 allianceauth_discordbot-3.8.0/tox.ini
+-rw-r--r--   0        0        0    17996 1970-01-01 00:00:00.000000 allianceauth_discordbot-3.8.0/PKG-INFO
```

### Comparing `allianceauth_discordbot-3.7.3/.github/workflows/main.yml` & `allianceauth_discordbot-3.8.0/.github/workflows/main.yml`

 * *Files 8% similar despite different names*

```diff
@@ -22,34 +22,34 @@
     runs-on: ubuntu-latest
     strategy:
       matrix:
         python-version: ["3.9", "3.10", "3.11"]
     steps:
       - uses: actions/checkout@v2
 
-      #- uses: shogo82148/actions-setup-redis@v1
-      #  with:
-      #    redis-version: "latest"
+      - uses: shogo82148/actions-setup-redis@v1
+        with:
+          redis-version: "latest"
 
-      #- run: redis-cli ping
+      - run: redis-cli ping
 
       - uses: actions/setup-python@v2
         with:
           python-version: ${{ matrix.python-version }}
 
       - name: install dependencies
         run: make dev
 
-      #- name: Run Tests
-      #  run: make test
+      - name: Run Tests
+        run: make test
 
-      #- name: Upload test coverage
-      #  if: ${{ !env.ACT }}
-      #  uses: actions/upload-artifact@v2.2.4
-      #  with:
-      #    # Artifact name
-      #    name: Python${{ matrix.python-version }} Test Coverage
-      #    # A file, directory or wildcard pattern that describes what to upload
-      #    path: htmlcov/
+      - name: Upload test coverage
+        if: ${{ !env.ACT }}
+        uses: actions/upload-artifact@v2.2.4
+        with:
+          # Artifact name
+          name: Python${{ matrix.python-version }} Test Coverage
+          # A file, directory or wildcard pattern that describes what to upload
+          path: htmlcov/
 
       - name: Build Projects
         run: make package
```

### Comparing `allianceauth_discordbot-3.7.3/.github/workflows/publish.yml` & `allianceauth_discordbot-3.8.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `allianceauth_discordbot-3.7.3/.pre-commit-config.yaml` & `allianceauth_discordbot-3.8.0/.pre-commit-config.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -91,7 +91,25 @@
     hooks:
       - id: flake8
         additional_dependencies: [Flake8-pyproject]
   - repo: https://github.com/asottile/yesqa
     rev: v1.5.0
     hooks:
       - id: yesqa
+  # Infrastructure
+  - repo: https://github.com/tox-dev/pyproject-fmt
+    rev: 1.7.0
+    hooks:
+      - id: pyproject-fmt
+        name: pyproject.toml formatter
+        description: "Format the pyproject.toml file."
+        args:
+          - --indent=4
+        additional_dependencies:
+          - tox==4.14.2 # https://github.com/tox-dev/tox/releases/latest
+
+  - repo: https://github.com/abravalheri/validate-pyproject
+    rev: v0.16
+    hooks:
+      - id: validate-pyproject
+        name: Validate pyproject.toml
+        description: "Validate the pyproject.toml file."
```

### Comparing `allianceauth_discordbot-3.7.3/CHANGELOG.md` & `allianceauth_discordbot-3.8.0/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `allianceauth_discordbot-3.7.3/LICENSE` & `allianceauth_discordbot-3.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `allianceauth_discordbot-3.7.3/Makefile` & `allianceauth_discordbot-3.8.0/Makefile`

 * *Files identical despite different names*

### Comparing `allianceauth_discordbot-3.7.3/README.md` & `allianceauth_discordbot-3.8.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -115,15 +115,19 @@
 
 ```bash
 wget https://raw.githubusercontent.com/pvyParts/allianceauth-discordbot/master/bot_conf.py
 ```
 
 ## Running Discordbot with Docker
 
-Update base image to have bot_conf.py mapped
+* To download the `bot_conf.py` file into your `conf/` folder, run the following from your aa-docker folder
+```bash
+wget https://raw.githubusercontent.com/pvyParts/allianceauth-discordbot/master/bot_conf.py -O conf/bot_conf.py
+```
+* Update base image to have bot_conf.py mapped
 
 ```dockerfile
 x-allianceauth-base:
 
 # image: ${AA_DOCKER_TAG?err}
 
   &allianceauth-base
@@ -182,16 +186,15 @@
 ```ini
 corputils.view_alliance_corpstats
 ```
 
 ## Optional Settings
 
 ### Built in Cogs
-
- ```python
+```python
 # Change the bots default Cogs, add or remove if you want to use any of the extra cogs.
 
 DISCORD_BOT_COGS = [
   "aadiscordbot.cogs.about", # about the bot
   "aadiscordbot.cogs.admin", # Discord server admin helpers
   "aadiscordbot.cogs.members", # Member lookup commands
   "aadiscordbot.cogs.timers", # timer board integration
@@ -205,14 +208,15 @@
   "aadiscordbot.cogs.price_check", # Price Checks
   "aadiscordbot.cogs.eightball", # 8ball should i install this cog
   "aadiscordbot.cogs.welcomegoodbye", # Customizable user join/leave messages
   "aadiscordbot.cogs.models", # Populate and Maintain Django Models for Channels and Servers
   "aadiscordbot.cogs.quote", # Save and recall messages
   "aadiscordbot.cogs.prom_export", # Admin Level Logging cog
   "aadiscordbot.cogs.tickets", # Private thread ticket system with pingable groups.
+  "aadiscordbot.cogs.recruit_me", # Private thread recruitment ticket system.
   ]
 ```
 
 ### Additional Rate Limiting
 
 ```python
 # configure the optional rate limited
```

### Comparing `allianceauth_discordbot-3.7.3/aadiscordbot/admin.py` & `allianceauth_discordbot-3.8.0/aadiscordbot/admin.py`

 * *Files identical despite different names*

### Comparing `allianceauth_discordbot-3.7.3/aadiscordbot/app_settings.py` & `allianceauth_discordbot-3.8.0/aadiscordbot/app_settings.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import re
-from inspect import getgeneratorlocals
 
 from django.apps import apps
 from django.conf import settings
 
 
 def get_site_url():  # regex sso url
     regex = r"^(.+)\/s.+"
@@ -46,14 +45,18 @@
     return apps.is_installed("allianceauth.services.modules.mumble")
 
 
 def discord_active():
     return apps.is_installed('allianceauth.services.modules.discord')
 
 
+def dmv_active():
+    return apps.is_installed('aadiscordmultiverse')
+
+
 DISCORD_BOT_PREFIX = getattr(settings, 'DISCORD_BOT_PREFIX', '!')
 
 DISCORD_BOT_COGS = getattr(settings, 'DISCORD_BOT_COGS',
                            [
                                "aadiscordbot.cogs.about",
                                "aadiscordbot.cogs.admin",
                                "aadiscordbot.cogs.members",
@@ -117,7 +120,21 @@
 DISCORD_BOT_SEND_FAILURE_MESSAGES = getattr(
     settings, 'DISCORD_BOT_SEND_FAILURE_MESSAGES', False)
 DISCORD_BOT_FAILURE_MESSAGES_CHANNEL = getattr(
     settings, 'DISCORD_BOT_FAILURE_MESSAGES_CHANNEL', False)
 
 PRICE_CHECK_HOSTNAME = getattr(
     settings, 'PRICE_CHECK_HOSTNAME', "evepraisal.com")
+
+# List of ints to sync commands to non global commands
+DISCORD_GUILD_IDS = getattr(settings, 'DISCORD_GUILD_IDS', [])
+
+DISCORD_GUILD_ID = getattr(settings, 'DISCORD_GUILD_ID', None)
+
+
+def get_all_servers():
+    servers = []
+    if DISCORD_GUILD_IDS:
+        servers += DISCORD_GUILD_IDS
+    if DISCORD_GUILD_ID and DISCORD_GUILD_ID not in servers:
+        servers.append(int(DISCORD_GUILD_ID))
+    return servers
```

### Comparing `allianceauth_discordbot-3.7.3/aadiscordbot/auth_hooks.py` & `allianceauth_discordbot-3.8.0/aadiscordbot/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `allianceauth_discordbot-3.7.3/aadiscordbot/bot.py` & `allianceauth_discordbot-3.8.0/aadiscordbot/bot.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,18 +25,17 @@
 
 import aadiscordbot
 from aadiscordbot import app_settings
 from aadiscordbot.app_settings import (
     DISCORD_BOT_ACCESS_DENIED_REACT, DISCORD_BOT_MESSAGE_INTENT,
     DISCORD_BOT_PREFIX,
 )
-from aadiscordbot.cogs.utils.exceptions import NotAuthenticated
+from aadiscordbot.cogs.utils.exceptions import NotAuthenticated, NotManaged
 
 from . import bot_tasks
-from .cogs.utils import context
 
 description = """
 AuthBot is watching...
 """
 
 logger = logging.getLogger(__name__)
 
@@ -281,39 +280,40 @@
 
     async def on_interaction(self, interaction):
         try:
             django.db.close_old_connections()
             await self.process_application_commands(interaction)
             django.db.close_old_connections()
         except Exception as e:
-            logger.error("Interaction Failed {e}", stack_info=True)
+            logger.error(f"Interaction Failed {e}", stack_info=True)
 
     async def on_message(self, message):
         if message.author.bot:
             return
         await self.process_commands(message)
 
     async def sync_commands(self, *args, **kwargs):
         try:
             return await super(__class__, self).sync_commands(*args, **kwargs)
-        except discord.Forbidden:
+        except discord.Forbidden as e:
             logger.error(
                 "******************************************************")
             logger.error("|   AuthBot was Unable to Sync Slash Commands!!!!")
             logger.error(
                 "|   Please ensure your bot was invited to the server with the correct scopes")
             logger.error("|")
             logger.error("|   To redo your scopes,")
             logger.error("|      1. Refresh Scopes with this link:")
             logger.error(f"|        {INVITE_URL}   ")
             logger.error(
                 "|      2. Move the bots role to top of the roles tree if its not there already")
             logger.error("|      3. Restart Bot")
             logger.error(
                 "******************************************************")
+            logger.error(e)
 
     @tasks.loop(seconds=1.0)
     async def poll_queue(self):
         message_avail = True
         while message_avail:
             try:
                 with self.message_consumer:
@@ -369,14 +369,16 @@
     async def on_application_command_error(self, context: ApplicationContext, exception: DiscordException) -> None:
         if isinstance(exception, commands.CheckFailure):
             await context.send_response(exception, ephemeral=True)
         elif isinstance(exception, commands.MissingPermissions):
             await context.send_response(exception, ephemeral=True)
         elif isinstance(exception, NotAuthenticated):
             await context.send_response(exception, ephemeral=True)
+        elif isinstance(exception, NotManaged):
+            await context.send_response(exception, ephemeral=True)
         else:  # Catch everything, and close out the interactions gracefully.
             logger.error(f"Unknown Error {exception}")
             logger.error("\n".join(traceback.format_tb(
                 exception.original.__traceback__)))
 
             if app_settings.DISCORD_BOT_SEND_FAILURE_MESSAGES and app_settings.DISCORD_BOT_FAILURE_MESSAGES_CHANNEL:
                 message = [f"`{context.command}` failed for `{context.author}`\n",
```

### Comparing `allianceauth_discordbot-3.7.3/aadiscordbot/bot_tasks.py` & `allianceauth_discordbot-3.8.0/aadiscordbot/bot_tasks.py`

 * *Files identical despite different names*

### Comparing `allianceauth_discordbot-3.7.3/aadiscordbot/cogs/about.py` & `allianceauth_discordbot-3.8.0/aadiscordbot/cogs/about.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,100 +1,103 @@
 import logging
 
 from discord.colour import Color
 from discord.commands import SlashCommandGroup
 from discord.embeds import Embed
 from discord.ext import commands
 
-from django.conf import settings
-
 from aadiscordbot import __branch__, __version__
 from aadiscordbot.app_settings import get_site_url
 
 logger = logging.getLogger(__name__)
 
 
 class About(commands.Cog):
     """
     All about me!
     """
 
     def __init__(self, bot):
         self.bot = bot
 
-    about_commands = SlashCommandGroup("about", "All about the Bot and Auth", guild_ids=[
-                                       int(settings.DISCORD_GUILD_ID)])
+    about_commands = SlashCommandGroup("about", "All about the Bot and Auth")
 
-    @about_commands.command(name="discordbot", description="About the Discord Bot", guild_ids=[int(settings.DISCORD_GUILD_ID)])
+    @about_commands.command(name="discordbot", description="About the Discord Bot")
     async def discordbot(self, ctx):
         """
         All about the bot
         """
         embed = Embed(title="AuthBot: The Authening")
         embed.set_thumbnail(
             url="https://cdn.discordapp.com/icons/516758158748811264/ae3991584b0f800b181c936cfc707880.webp?size=128"
         )
         embed.colour = Color.blue()
 
         embed.description = "This is a multi-de-functional discord bot tailored specifically for Alliance Auth Shenanigans."
-        regex = r"^(.+)\/d.+"
 
         embed.set_footer(
             text="Lovingly developed for Init.™ by AaronRin and ArielKable")
 
-        embed.add_field(
-            name="Number of Servers:", value=len(self.bot.guilds), inline=True
-        )
-        members = 0
-        for g in self.bot.guilds:
-            members += g.member_count
-        embed.add_field(name="Unwilling Monitorees:",
-                        value=members, inline=True)
-        embed.add_field(
-            name="Auth Link", value=get_site_url(), inline=False
-        )
+        if not ctx.guild:
+            embed.add_field(
+                name="Number of Servers:", value=len(self.bot.guilds), inline=True
+            )
+            members = 0
+            for g in self.bot.guilds:
+                members += g.member_count
+            embed.add_field(name="Unwilling Monitorees:",
+                            value=members, inline=True)
+            embed.add_field(
+                name="Auth Link", value=get_site_url(), inline=False
+            )
+
         embed.add_field(
             name="Version", value=f"{__version__}@{__branch__}", inline=False
         )
 
         return await ctx.respond(embed=embed)
 
-    @about_commands.command(name="server", description="About this Discord Server", guild_ids=[int(settings.DISCORD_GUILD_ID)])
+    @about_commands.command(name="server", description="About this Discord Server")
     async def server(self, ctx):
         """
         All about a server
         """
-        embed = Embed(title=ctx.guild.name)
+        if ctx.guild:
+            embed = Embed(title=ctx.guild.name)
 
-        if ctx.guild.icon:
-            embed.set_thumbnail(
-                url=ctx.guild.icon.url
-            )
-        embed.color = Color.blue()
-        embed.description = "Alliance Auth Managed EvE Online Discord Server!"
-        if ctx.guild.description:
-            embed.description = ctx.guild.description
-        embed.set_footer(
-            text="AuthBot Lovingly developed for Init.™ by AaronRin and ArielKable")
+            if ctx.guild.icon:
+                embed.set_thumbnail(
+                    url=ctx.guild.icon.url
+                )
+            embed.color = Color.blue()
+            embed.description = "Alliance Auth Managed EvE Online Discord Server!"
+            if ctx.guild.description:
+                embed.description = ctx.guild.description
+            embed.set_footer(
+                text="AuthBot Lovingly developed for Init.™ by AaronRin and ArielKable")
+
+            members = ctx.guild.member_count
+            embed.add_field(name="Unwilling Monitorees:",
+                            value=members, inline=True)
+
+            channels = len(ctx.guild.channels)
+            cats = len(ctx.guild.categories)
+            embed.add_field(name="Channel Count:",
+                            value=channels-cats, inline=True)
+
+            roles = len(ctx.guild.roles)
+            embed.add_field(name="Role Count:",
+                            value=roles, inline=True)
 
-        members = ctx.guild.member_count
-        embed.add_field(name="Unwilling Monitorees:",
-                        value=members, inline=True)
-
-        channels = len(ctx.guild.channels)
-        cats = len(ctx.guild.categories)
-        embed.add_field(name="Channel Count:",
-                        value=channels-cats, inline=True)
-
-        roles = len(ctx.guild.roles)
-        embed.add_field(name="Role Count:",
-                        value=roles, inline=True)
-
-        embed.add_field(
-            name="Auth Link", value=get_site_url(), inline=False
-        )
+            embed.add_field(
+                name="Auth Link", value=get_site_url(), inline=False
+            )
 
-        return await ctx.respond(embed=embed)
+            return await ctx.respond(embed=embed)
+        else:
+            return await ctx.respond(
+                "Sorry, this command cannot be used in DMs."
+            )
 
 
 def setup(bot):
     bot.add_cog(About(bot))
```

### Comparing `allianceauth_discordbot-3.7.3/aadiscordbot/cogs/abuse.py` & `allianceauth_discordbot-3.8.0/aadiscordbot/cogs/abuse.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,12 @@
 import logging
 from random import randrange
 
 from discord.ext import commands
 
-from django.conf import settings
-
-from aadiscordbot import __branch__, __version__
-
 logger = logging.getLogger(__name__)
 
 
 class Abuse(commands.Cog):
     """
     All about me!
     """
@@ -48,22 +44,22 @@
             "Stop trying to be a smart ass, you're just an ass.",
             "I'm busy now. Can I ignore you some other time?",
             "Why don't you slip into something more comfortable... like a coma.",
             "To make you laugh on Saturday, I need to you joke on Wednesday.",
             "Pardon me, but you've obviously mistaken me for someone who gives a damn.",
             "https://media.tenor.com/x8v1oNUOmg4AAAAC/rickroll-roll.gif"
         ]
-        rand = randrange(0, len(replies)-1)
-        if message.mention_everyone:
+        rand = randrange(0, len(replies) - 1)
+        if message.mention_everyone or message.author.id == self.bot.user.id:
             return
         try:
             if self.bot.user.mentioned_in(message):
                 if message.author.id == 318309023478972417:
                     await message.reply("https://media.tenor.com/x8v1oNUOmg4AAAAC/rickroll-roll.gif")
                 else:
                     await message.reply(replies[rand])
-        except:
+        except Exception:
             pass
 
 
 def setup(bot):
     bot.add_cog(Abuse(bot))
```

### Comparing `allianceauth_discordbot-3.7.3/aadiscordbot/cogs/abuse_two.py` & `allianceauth_discordbot-3.8.0/aadiscordbot/cogs/abuse_two.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,13 @@
 import logging
 
-from discord.colour import Color
-from discord.commands import SlashCommandGroup
-from discord.embeds import Embed
 from discord.ext import commands
 
 from django.conf import settings
 
-from aadiscordbot import __branch__, __version__
-from aadiscordbot.app_settings import get_site_url
-
 logger = logging.getLogger(__name__)
 
 
 class AbuseTwo(commands.Cog):
     """
     Emojis for abusing reasons...!
     """
```

### Comparing `allianceauth_discordbot-3.7.3/aadiscordbot/cogs/admin.py` & `allianceauth_discordbot-3.8.0/aadiscordbot/cogs/admin.py`

 * *Files identical despite different names*

### Comparing `allianceauth_discordbot-3.7.3/aadiscordbot/cogs/auth.py` & `allianceauth_discordbot-3.8.0/aadiscordbot/cogs/auth.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,16 @@
 # Cog Stuff
 import logging
 
 from discord.colour import Color
 from discord.embeds import Embed
 from discord.ext import commands
 
-from django.conf import settings
-
-from aadiscordbot import __branch__, __version__
 # AA Contexts
-from aadiscordbot.app_settings import get_admins, get_site_url
-
-from ..app_settings import discord_active, mumble_active
+from aadiscordbot.app_settings import get_site_url
 
 logger = logging.getLogger(__name__)
 
 
 class Auth(commands.Cog):
     """
     A Collection of Authentication Tools for Alliance Auth
@@ -24,15 +19,16 @@
     def __init__(self, bot):
         self.bot = bot
 
     @commands.command(pass_context=True)
     async def auth(self, ctx):
         """
         Returns a link to the AllianceAuth Install
-        Used by many other Bots and is a common command that users will attempt to run.
+        Used by many other Bots and is a common command that
+        users will attempt to run.
         """
         await ctx.trigger_typing()
 
         embed = Embed(title="AllianceAuth")
         embed.set_thumbnail(
             url="https://assets.gitlab-static.net/uploads/-/system/project/avatar/6840712/Alliance_auth.png?width=128"
         )
@@ -44,44 +40,41 @@
 
         embed.add_field(
             name="Auth Link", value=url, inline=False
         )
 
         return await ctx.send(embed=embed)
 
-    @commands.slash_command(name='auth', guild_ids=[int(settings.DISCORD_GUILD_ID)])
+    @commands.slash_command(name='auth')
     async def auth_slash(self, ctx):
         """
         Returns a link to the AllianceAuth Install
-        Used by many other Bots and is a common command that users will attempt to run.
-        """
-        embed = Embed(title="AllianceAuth")
-        embed.set_thumbnail(
-            url="https://assets.gitlab-static.net/uploads/-/system/project/avatar/6840712/Alliance_auth.png?width=128"
-        )
-        embed.colour = Color.blue()
-
-        embed.description = "All Authentication functions for this Discord server are handled through our Alliance Auth install"
-
-        url = get_site_url()
-
-        embed.add_field(
-            name="Auth Link", value=url, inline=False
-        )
+        Used by many other Bots and is a common command that
+        users will attempt to run.
         """
-        embed.add_field(
-            name="Number of Servers:", value=len(self.bot.guilds), inline=True
-        )
-        embed.add_field(name="Unwilling Monitorees:",
-                        value=len(self.bot.users), inline=True)
-        embed.add_field(
-            name="Version", value="{}@{}".format(__version__, __branch__), inline=False
-        )
-        """
-        embed.set_footer(
-            text="Lovingly developed for Init.™ by AaronRin and ArielKable")
-
-        return await ctx.respond(embed=embed)
+        if ctx.guild:
+            embed = Embed(title="AllianceAuth")
+            embed.set_thumbnail(
+                url="https://assets.gitlab-static.net/uploads/-/system/project/avatar/6840712/Alliance_auth.png?width=128"
+            )
+            embed.colour = Color.blue()
+
+            embed.description = "All Authentication functions for this Discord server are handled through our Alliance Auth install"
+
+            url = get_site_url()
+
+            embed.add_field(
+                name="Auth Link", value=url, inline=False
+            )
+            embed.set_footer(
+                text="Lovingly developed for Init.™ by AaronRin and ArielKable")
+
+            return await ctx.respond(embed=embed)
+
+        else:
+            return await ctx.respond(
+                "Sorry, this command cannot be used in DMs."
+            )
 
 
 def setup(bot):
     bot.add_cog(Auth(bot))
```

### Comparing `allianceauth_discordbot-3.7.3/aadiscordbot/cogs/eastereggs.py` & `allianceauth_discordbot-3.8.0/aadiscordbot/cogs/eastereggs.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 import logging
 
 from discord import User
 from discord.ext import commands
 
-from django.conf import settings
-
 logger = logging.getLogger(__name__)
 
 
 class EasterEggs(commands.Cog):
     """
     Stupid commands that don't belong anywhere
     These will not appear in Help menus
     Have limited to no real use
     I was bored
     """
 
     def __init__(self, bot):
         self.bot = bot
 
-    @commands.slash_command(name='happybirthday', guild_ids=[int(settings.DISCORD_GUILD_ID)])
+    @commands.slash_command(name='happybirthday')
     async def happybirthday(self, ctx,  user: User):
         """
         Takes one Discord User as an argument, Wishes this user a happy birthday
         If no user is passed, responds to the context user
         "Useful" to verify the bot is alive and functioning
         """
         await ctx.trigger_typing()
```

### Comparing `allianceauth_discordbot-3.7.3/aadiscordbot/cogs/eightball.py` & `allianceauth_discordbot-3.8.0/aadiscordbot/cogs/eightball.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,12 @@
 import logging
 from random import randrange
 
 from discord.ext import commands
 
-from django.conf import settings
-
-from aadiscordbot import __branch__, __version__
-
 logger = logging.getLogger(__name__)
 
 
 class EightBall(commands.Cog):
     """
     All about me!
     """
@@ -44,14 +40,14 @@
     @commands.command(pass_context=True, aliases=['8ball'])
     async def meb(self, message):
         """
         8 ball go brrrr
         """
         await message.reply(self.eightball())
 
-    @commands.slash_command(name='8ball', guild_ids=[int(settings.DISCORD_GUILD_ID)])
+    @commands.slash_command(name='8ball')
     async def meb_slash(self, ctx, question: str):
         await ctx.respond(f" You Asked: `{question}`\n\n{self.eightball()}")
 
 
 def setup(bot):
     bot.add_cog(EightBall(bot))
```

### Comparing `allianceauth_discordbot-3.7.3/aadiscordbot/cogs/facwar.py` & `allianceauth_discordbot-3.8.0/aadiscordbot/cogs/facwar.py`

 * *Files identical despite different names*

### Comparing `allianceauth_discordbot-3.7.3/aadiscordbot/cogs/members.py` & `allianceauth_discordbot-3.8.0/aadiscordbot/cogs/members.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from django.core.exceptions import ObjectDoesNotExist
 
 from allianceauth.eveonline.evelinks import evewho
 from allianceauth.eveonline.models import EveCharacter, EveCorporationInfo
 
 from aadiscordbot.app_settings import aastatistics_active
 from aadiscordbot.cogs.utils.decorators import (
-    has_any_perm, in_channels, message_in_channels, sender_has_any_perm,
+    is_guild_managed, message_in_channels, sender_has_any_perm,
 )
 
 logger = logging.getLogger(__name__)
 
 
 class Members(commands.Cog):
     """
@@ -151,70 +151,67 @@
             embed.description = (
                 "Character **{character_name}** does not exist in our Auth system"
             ).format(character_name=input_name)
 
             return embed
 
     @commands.command(pass_context=True)
+    @is_guild_managed()
     @sender_has_any_perm(['corputils.view_alliance_corpstats', 'corpstats.view_alliance_corpstats', 'aadiscordbot.member_command_access'])
     @message_in_channels(settings.ADMIN_DISCORD_BOT_CHANNELS)
     async def lookup(self, ctx):
         """
         Gets Auth data about a character
         Input: a Eve Character Name
         """
         input_name = ctx.message.content[8:]
         return await ctx.send(embed=self.get_lookup_embed(input_name))
 
     async def search_characters(ctx: AutocompleteContext):
         """Returns a list of colors that begin with the characters entered so far."""
         return list(EveCharacter.objects.filter(character_name__icontains=ctx.value).values_list('character_name', flat=True)[:10])
 
-    @commands.slash_command(name='lookup', guild_ids=[int(settings.DISCORD_GUILD_ID)])
+    @commands.slash_command(name='lookup')
+    @is_guild_managed()
+    @sender_has_any_perm(['corputils.view_alliance_corpstats', 'corpstats.view_alliance_corpstats', 'aadiscordbot.member_command_access'])
+    @message_in_channels(settings.ADMIN_DISCORD_BOT_CHANNELS)
     @option("character", description="Search for a Character!", autocomplete=search_characters)
     async def slash_lookup(
         self,
         ctx,
         character: str,
     ):
-        try:
-            in_channels(ctx.channel.id, settings.ADMIN_DISCORD_BOT_CHANNELS)
-            has_any_perm(ctx.author.id, ['corputils.view_alliance_corpstats',
-                         'corpstats.view_alliance_corpstats', 'aadiscordbot.member_command_access'])
-            await ctx.defer()
-            return await ctx.respond(embed=self.get_lookup_embed(character))
-        except commands.MissingPermissions as e:
-            return await ctx.respond(e.missing_permissions[0], ephemeral=True)
+        await ctx.defer()
+        return await ctx.respond(embed=self.get_lookup_embed(character))
 
     async def search_corps_on_characters(ctx: AutocompleteContext):
-        """Returns a list of colors that begin with the characters entered so far."""
+        """Returns a list of corporations that begin with the characters entered so far."""
         return list(EveCharacter.objects.filter(corporation_name__icontains=ctx.value).values_list('corporation_name', flat=True).distinct()[:10])
 
     def build_altcorp_embeds(self, input_name):
         chars = EveCharacter.objects.filter(corporation_name=input_name)
         if chars.count():
             corp_id = 0
             own_ids = [settings.DISCORD_BOT_MEMBER_ALLIANCES]
             alts_in_corp = []
             knowns = 0
             for c in chars:
                 corp_id = c.corporation_id
-                alliance = c.alliance_name
                 if c.alliance_id not in own_ids:
                     alts_in_corp.append(c)
 
             mains = {}
             for a in alts_in_corp:
                 try:
                     main = a.character_ownership.user.profile.main_character
                     if main.character_id not in mains:
                         mains[main.character_id] = [main, 0]
                     mains[main.character_id][1] += 1
                     knowns += 1
-                except Exception as e:
+                except Exception:
                     # logger.error(e)
                     pass
             output = []
             base_string = "[{}]({}) [ [{}]({}) ] has {} alt{}"
             for k, m in mains.items():
                 output.append(
                     base_string.format(
@@ -245,39 +242,39 @@
             for strings in [output[i:i + 10] for i in range(0, len(output), 10)]:
                 embed = Embed(title=input_name)
                 embed.colour = Color.blue()
                 embed.description = "\n".join(strings)
                 embeds.append(embed)
             return embeds
 
-    @commands.slash_command(name='altcorp', guild_ids=[int(settings.DISCORD_GUILD_ID)])
-    @option("corporation", description="Search for a Character!", autocomplete=search_corps_on_characters)
+    @commands.slash_command(name='altcorp')
+    @is_guild_managed()
+    @sender_has_any_perm(['aadiscordbot.member_command_access'])
+    @message_in_channels(settings.ADMIN_DISCORD_BOT_CHANNELS)
+    @option("corporation",
+            description="Search for a Character!",
+            autocomplete=search_corps_on_characters)
     async def slash_altcorp(
         self,
         ctx,
         corporation: str,
     ):
-        try:
-            in_channels(ctx.channel.id, settings.ADMIN_DISCORD_BOT_CHANNELS)
-            has_any_perm(ctx.author.id, ['corputils.view_alliance_corpstats',
-                         'corpstats.view_alliance_corpstats', 'aadiscordbot.member_command_access'])
-            await ctx.defer()
-            embeds = self.build_altcorp_embeds(corporation)
-            if len(embeds):
-                e = embeds.pop(0)
-                await ctx.respond(embed=e)
-                for e in embeds:
-                    await ctx.send(embed=e)
-            else:
-                await ctx.respond("No Members Found!")
-        except commands.MissingPermissions as e:
-            return await ctx.respond(e.missing_permissions[0], ephemeral=True)
+        await ctx.defer()
+        embeds = self.build_altcorp_embeds(corporation)
+        if len(embeds):
+            e = embeds.pop(0)
+            await ctx.respond(embed=e)
+            for e in embeds:
+                await ctx.send(embed=e)
+        else:
+            await ctx.respond("No Members Found!")
 
     @commands.command(pass_context=True)
-    @sender_has_any_perm(['corputils.view_alliance_corpstats', 'corpstats.view_alliance_corpstats', 'aadiscordbot.member_command_access'])
+    @is_guild_managed()
+    @sender_has_any_perm(['aadiscordbot.member_command_access'])
     @message_in_channels(settings.ADMIN_DISCORD_BOT_CHANNELS)
     async def altcorp(self, ctx):
         """
         Gets Auth data about an altcorp
         Input: a Eve Character Name
         """
         corporation = ctx.message.content[9:]
```

### Comparing `allianceauth_discordbot-3.7.3/aadiscordbot/cogs/models.py` & `allianceauth_discordbot-3.8.0/aadiscordbot/cogs/models.py`

 * *Files identical despite different names*

### Comparing `allianceauth_discordbot-3.7.3/aadiscordbot/cogs/price_check.py` & `allianceauth_discordbot-3.8.0/aadiscordbot/cogs/price_check.py`

 * *Files identical despite different names*

### Comparing `allianceauth_discordbot-3.7.3/aadiscordbot/cogs/prom_export.py` & `allianceauth_discordbot-3.8.0/aadiscordbot/cogs/prom_export.py`

 * *Files identical despite different names*

### Comparing `allianceauth_discordbot-3.7.3/aadiscordbot/cogs/quote.py` & `allianceauth_discordbot-3.8.0/aadiscordbot/cogs/quote.py`

 * *Files identical despite different names*

### Comparing `allianceauth_discordbot-3.7.3/aadiscordbot/cogs/reaction_roles.py` & `allianceauth_discordbot-3.8.0/aadiscordbot/cogs/reaction_roles.py`

 * *Files identical despite different names*

### Comparing `allianceauth_discordbot-3.7.3/aadiscordbot/cogs/remind.py` & `allianceauth_discordbot-3.8.0/aadiscordbot/cogs/remind.py`

 * *Files identical despite different names*

### Comparing `allianceauth_discordbot-3.7.3/aadiscordbot/cogs/services.py` & `allianceauth_discordbot-3.8.0/aadiscordbot/cogs/services.py`

 * *Files identical despite different names*

### Comparing `allianceauth_discordbot-3.7.3/aadiscordbot/cogs/sov.py` & `allianceauth_discordbot-3.8.0/aadiscordbot/cogs/sov.py`

 * *Files identical despite different names*

### Comparing `allianceauth_discordbot-3.7.3/aadiscordbot/cogs/time.py` & `allianceauth_discordbot-3.8.0/aadiscordbot/cogs/time.py`

 * *Files identical despite different names*

### Comparing `allianceauth_discordbot-3.7.3/aadiscordbot/cogs/timers.py` & `allianceauth_discordbot-3.8.0/aadiscordbot/cogs/timers.py`

 * *Files identical despite different names*

### Comparing `allianceauth_discordbot-3.7.3/aadiscordbot/cogs/welcomegoodbye.py` & `allianceauth_discordbot-3.8.0/aadiscordbot/cogs/welcomegoodbye.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,60 +3,69 @@
 """
 import asyncio
 import logging
 
 import discord
 from discord.ext import commands
 
+from django.db.models import Q
+
 from aadiscordbot.app_settings import get_site_url
 from aadiscordbot.models import GoodbyeMessage, WelcomeMessage
-from aadiscordbot.utils.auth import user_is_authenticated
+from aadiscordbot.utils.auth import is_user_authenticated
 
 logger = logging.getLogger(__name__)
 
 
 class Welcome(commands.Cog):
     """
     Responds to on_member_join events from discord
     """
 
     def __init__(self, bot):
         self.bot = bot
 
     @commands.Cog.listener("on_member_join")
     async def on_member_join(self, member: discord.Member):
+        logger.info(
+            f"{member} joined {member.guild.name}"
+        )
         channel = member.guild.system_channel
         if channel is not None:
             try:
                 # Give AA a chance to save the UID for a joiner.
                 await asyncio.sleep(3)
-                authenticated = user_is_authenticated(member, member.guild)
+                authenticated = is_user_authenticated(member, member.guild)
             except Exception:
                 authenticated = False
             if authenticated:
                 try:
                     message = WelcomeMessage.objects.filter(
+                        Q(
+                            Q(guild_id=member.guild.id) | Q(guild_id=None)
+                        ),
                         authenticated=True,
-                        guild_id=member.guild.id
                     ).order_by('?').first().message
                     message_formatted = message.format(
                         user_mention=member.mention,
                         guild_name=member.guild.name,
                         auth_url=get_site_url(),)
                     await channel.send(message_formatted)
                 except IndexError:
                     logger.error(
                         'No Welcome Message configured for Discordbot Welcome cog')
                 except Exception as e:
                     logger.error(e)
             else:
                 try:
                     message = WelcomeMessage.objects.filter(
+                        Q(
+                            Q(guild_id=member.guild.id) | Q(guild_id=None)
+                        ),
                         unauthenticated=True,
-                        guild_id=member.guild.id
                     ).order_by('?').first().message
                     message_formatted = message.format(
                         user_mention=member.mention,
                         guild_name=member.guild.name,
                         auth_url=get_site_url(),)
                     await channel.send(message_formatted)
                 except IndexError:
@@ -72,27 +81,32 @@
     """
 
     def __init__(self, bot):
         self.bot = bot
 
     @commands.Cog.listener("on_member_remove")
     async def on_member_remove(self, member: discord.Member):
+        logger.info(
+            f"{member} Left {member.guild.name}"
+        )
         channel = member.guild.system_channel
         if channel is not None:
             try:
                 # Give AA a chance to save the UID for a joiner.
-                authenticated = user_is_authenticated(member, member.guild)
+                authenticated = is_user_authenticated(member, member.guild)
             except Exception:
                 authenticated = False
             if authenticated:
                 # Authenticated
                 try:
                     message = GoodbyeMessage.objects.filter(
+                        Q(
+                            Q(guild_id=member.guild.id) | Q(guild_id=None)
+                        ),
                         authenticated=True,
-                        guild_id=member.guild.id
                     ).order_by('?').first().message
                     message_formatted = message.format(
                         user_mention=member.mention,
                         guild_name=member.guild.name,
                         auth_url=get_site_url(),)
                     await channel.send(message_formatted)
                 except IndexError:
@@ -101,27 +115,29 @@
                 except Exception as e:
                     logger.error(e)
 
             else:
                 # Un-Authenticated
                 try:
                     message = GoodbyeMessage.objects.filter(
+                        Q(
+                            Q(guild_id=member.guild.id) | Q(guild_id=None)
+                        ),
                         unauthenticated=True,
-                        guild_id=member.guild.id
                     ).order_by('?').first().message
                     message_formatted = message.format(
                         user_mention=member.mention,
                         guild_name=member.guild.name,
                         auth_url=get_site_url(),)
                     await channel.send(message_formatted)
                 except IndexError:
                     logger.error(
                         'No Leave Message configured for Discordbot Goodbye cog')
                 except Exception as e:
-                    logger.error(e)
+                    logger.error(e, stack_info=True)
 
 
 def setup(bot):
     """
     setup the cog
     :param bot:
     """
```

### Comparing `allianceauth_discordbot-3.7.3/aadiscordbot/locale/de/LC_MESSAGES/django.po` & `allianceauth_discordbot-3.8.0/aadiscordbot/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `allianceauth_discordbot-3.7.3/aadiscordbot/locale/en/LC_MESSAGES/django.po` & `allianceauth_discordbot-3.8.0/aadiscordbot/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `allianceauth_discordbot-3.7.3/aadiscordbot/migrations/0001_initial.py` & `allianceauth_discordbot-3.8.0/aadiscordbot/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `allianceauth_discordbot-3.7.3/aadiscordbot/migrations/0002_reactionrolebinding_reactionrolemessage.py` & `allianceauth_discordbot-3.8.0/aadiscordbot/migrations/0002_reactionrolebinding_reactionrolemessage.py`

 * *Files identical despite different names*

### Comparing `allianceauth_discordbot-3.7.3/aadiscordbot/migrations/0003_authbotconfiguration.py` & `allianceauth_discordbot-3.8.0/aadiscordbot/migrations/0003_authbotconfiguration.py`

 * *Files identical despite different names*

### Comparing `allianceauth_discordbot-3.7.3/aadiscordbot/migrations/0005_rr_fixes_blank_admins.py` & `allianceauth_discordbot-3.8.0/aadiscordbot/migrations/0005_rr_fixes_blank_admins.py`

 * *Files identical despite different names*

### Comparing `allianceauth_discordbot-3.7.3/aadiscordbot/migrations/0006_goodbyemessage_welcomemessage.py` & `allianceauth_discordbot-3.8.0/aadiscordbot/migrations/0006_goodbyemessage_welcomemessage.py`

 * *Files identical despite different names*

### Comparing `allianceauth_discordbot-3.7.3/aadiscordbot/migrations/0007_quotemessage.py` & `allianceauth_discordbot-3.8.0/aadiscordbot/migrations/0007_quotemessage.py`

 * *Files identical despite different names*

### Comparing `allianceauth_discordbot-3.7.3/aadiscordbot/migrations/0010_alter_discordbot_options_ticketgroups.py` & `allianceauth_discordbot-3.8.0/aadiscordbot/migrations/0010_alter_discordbot_options_ticketgroups.py`

 * *Files identical despite different names*

### Comparing `allianceauth_discordbot-3.7.3/aadiscordbot/migrations/0011_alter_ticketgroups_options_and_more.py` & `allianceauth_discordbot-3.8.0/aadiscordbot/migrations/0011_alter_ticketgroups_options_and_more.py`

 * *Files identical despite different names*

### Comparing `allianceauth_discordbot-3.7.3/aadiscordbot/models.py` & `allianceauth_discordbot-3.8.0/aadiscordbot/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from solo.models import SingletonModel
 
-from django.conf import settings
 from django.contrib.auth.models import Group
 from django.core.exceptions import ValidationError
 from django.db import models
 from django.utils.translation import gettext_lazy as _
 
 from allianceauth.services.modules.discord.models import DiscordUser
 
@@ -77,15 +76,15 @@
     emoji = models.CharField(max_length=100)
     emoji_text = models.CharField(max_length=100)
     message = models.ForeignKey(ReactionRoleMessage, on_delete=models.CASCADE)
 
     def __str__(self):
         try:
             b = eval(self.emoji_text).decode('utf-8')
-        except:
+        except Exception:
             b = self.emoji_text
         return f'{self.message.name}: {b} ({self.group})'
 
 
 class AuthBotConfiguration(models.Model):
 
     admin_users = models.ManyToManyField(DiscordUser, blank=True)
@@ -103,28 +102,28 @@
 
 
 class WelcomeMessage(models.Model):
     message = models.TextField(_("Welcome Message"))
     authenticated = models.BooleanField(_("Valid for Authenticated Users"))
     unauthenticated = models.BooleanField(
         _("Valid for Un-Authenticated Users"))
-    guild_id = models.BigIntegerField(default=settings.DISCORD_GUILD_ID)
+    guild_id = models.BigIntegerField(default=None, null=True, blank=True)
 
     class Meta:
         default_permissions = ()
         verbose_name = 'Welcome Message'
         verbose_name_plural = 'Welcome Messages'
 
 
 class GoodbyeMessage(models.Model):
     message = models.TextField(_("Goodbye Message"))
     authenticated = models.BooleanField(_("Valid for Authenticated Users"))
     unauthenticated = models.BooleanField(
         _("Valid for Un-Authenticated Users"))
-    guild_id = models.BigIntegerField(default=settings.DISCORD_GUILD_ID)
+    guild_id = models.BigIntegerField(default=None, null=True, blank=True)
 
     class Meta:
         default_permissions = ()
         verbose_name = 'Goodbye Message'
         verbose_name_plural = 'Goodbye Messages'
```

### Comparing `allianceauth_discordbot-3.7.3/aadiscordbot/tasks.py` & `allianceauth_discordbot-3.8.0/aadiscordbot/tasks.py`

 * *Files identical despite different names*

### Comparing `allianceauth_discordbot-3.7.3/aadiscordbot/utils/auth.py` & `allianceauth_discordbot-3.8.0/aadiscordbot/utils/auth.py`

 * *Files 26% similar despite different names*

```diff
@@ -6,136 +6,197 @@
       - https://gitlab.com/allianceauth/allianceauth/
     - aadiscordmultiverse
       - https://github.com/Solar-Helix-Independent-Transport/allianceauth-discord-multiverse
 
 """
 
 import logging
+import warnings
 
 from discord import Guild, User
 
 from django.conf import settings
 
-from allianceauth.services.modules.discord.models import DiscordUser
+from aadiscordbot.app_settings import discord_active, dmv_active, get_admins
 
 logger = logging.getLogger(__name__)
 
-DMV_ACTIVE = False
+DMV_ACTIVE = dmv_active()
+DISCORD_ACTIVE = discord_active()
+
 
 try:
-    from aadiscordmultiverse.models import (
-        DiscordManagedServer, MultiDiscordUser,
-    )
-    DMV_ACTIVE = True
+    if DISCORD_ACTIVE:
+        # this needs to be imported safely incase only DMV installed
+        from allianceauth.services.modules.discord.models import DiscordUser
+except ImportError:
+    logger.debug("Discord not installed?")
+
+
+try:
+    if DMV_ACTIVE:
+        # this needs to be imported safely incase only Core service installed
+        from aadiscordmultiverse.models import (
+            DiscordManagedServer, MultiDiscordUser,
+        )
 except ImportError:
-    logger.debug("DMV not installed")
+    logger.debug("DMV not installed?")
 
 
-def get_dmv_discord_user(user_id, guild_id):
+def _get_dmv_discord_user(user_id, guild_id):
     if DMV_ACTIVE:
         try:
             return MultiDiscordUser.objects.get(
                 guild_id=guild_id,
                 uid=user_id
             )
         except MultiDiscordUser.DoesNotExist:
             return None
     else:
         return None
 
 
-def check_for_dmv_user(user: User, guild: Guild):
+def _check_for_dmv_user(user: User, guild: Guild):
     """
         Return `True` if a discord user is authenticated to
         the DMV service module `False` Otherwise
     """
-    user = get_dmv_discord_user(user.id, guild.id)
+    user = _get_dmv_discord_user(user.id, guild.id)
     if user:
         return True
     else:
         return False
 
 
-def get_core_discord_user(user_id):
-    try:
-        return DiscordUser.objects.get(uid=user_id)
-    except DiscordUser.DoesNotExist:
+def _get_core_discord_user(user_id):
+    if DISCORD_ACTIVE:
+        try:
+            return DiscordUser.objects.get(uid=user_id)
+        except DiscordUser.DoesNotExist:
+            return None
+    else:
         return None
 
 
-def check_for_core_user(user: User):
+def _check_for_core_user(user: User):
     """
         Return `True` if a discord user is authenticated to
         the core auth service module `False` Otherwise
     """
-    user = get_core_discord_user(user.id)
+    user = _get_core_discord_user(user.id)
     if user:
         return True
     else:
         return False
 
 
-def guild_is_core_module(guild_id):
+def _guild_is_core_module(guild_id):
     """
         Check if the guild_id matches the core auth service module's guild
     """
-    return id == getattr(settings, "DISCORD_GUILD_ID", -1)
+    # May be string in settings so cast to int for check.
+    # discord returns int for guild.id
+    gid = int(getattr(settings, "DISCORD_GUILD_ID", -1))
 
+    return guild_id == gid and DISCORD_ACTIVE
 
-def guild_is_dmv_module(guild_id):
+
+def _guild_is_dmv_module(guild_id):
     """
         Check if the guild_id matches the any of the DMV servers
     """
-    guild = get_dmv_guild(guild_id)
+    guild = _get_dmv_guild(guild_id)
     if guild:
         return True
     else:
         return False
 
 
-def get_dmv_guild(guild_id):
+def _get_dmv_guild(guild_id):
     """
         Return DMV Guild model if DMV installed and
     """
     if DMV_ACTIVE:
         try:
             return DiscordManagedServer.objects.get(
                 guild_id=guild_id,
             )
         except DiscordManagedServer.DoesNotExist:
             return None
     else:
         return None
 
 
+def is_user_bot_admin(user: User):
+    """
+        Is user a configured Bot Admin
+        TODO: Make this work with DNV somehow.
+    """
+    if user.id in get_admins():
+        return True
+    else:
+        return False
+
+
+def is_guild_managed(guild: Guild):
+    core = _guild_is_core_module(guild.id)
+    dmv = _guild_is_dmv_module(guild.id)
+    return core or dmv
+
+
 def user_is_authenticated(user: User, guild: Guild):
+    warnings.warn(
+        "user_is_authenticated is deprecated use is_user_authenticated instead",
+        DeprecationWarning,
+        stacklevel=2
+    )
+    logger.warning("user_is_authenticated is deprecated use is_user_authenticated instead")
+    return is_user_authenticated(user, guild)
+
+
+def is_user_authenticated(user: User, guild: Guild):
     """
         Return `True` if a discord user is authenticated to the
         any service module `False` Otherwise
 
         Checks these services depending on the guild_id
     """
-    if guild_is_core_module(guild.id):
-        return check_for_core_user(user)
+    if _guild_is_core_module(guild.id):
+        return _check_for_core_user(user)
 
-    elif guild_is_dmv_module(guild.id):
-        return check_for_dmv_user(user, guild)
+    elif _guild_is_dmv_module(guild.id):
+        return _check_for_dmv_user(user, guild)
 
     else:
         return False
 
 
-def get_auth_user(user: User, guild: Guild):
+def get_auth_user(user: User | int, guild: Guild | int = None):
     """
         Get auth user from any service module
     """
+    guild_id = None
+    user_id = None
+
+    if isinstance(user, int):
+        user_id = user
+    else:
+        user_id = user.id
+
+    if guild:
+        if isinstance(guild, int):
+            guild_id = guild
+        else:
+            guild_id = guild.id
+
     discord_user = None
-    if guild_is_core_module(guild.id):
-        discord_user = get_core_discord_user(user.id)
 
-    elif guild_is_dmv_module(guild.id):
-        discord_user = get_dmv_discord_user(user.id, guild.id)
+    if guild_id is None or _guild_is_core_module(guild_id):
+        discord_user = _get_core_discord_user(user_id)
+
+    elif _guild_is_dmv_module(guild_id):
+        discord_user = _get_dmv_discord_user(user_id, guild_id)
 
     if discord_user:
         return discord_user.user
     else:
         return None
```

### Comparing `allianceauth_discordbot-3.7.3/pyproject.toml` & `allianceauth_discordbot-3.8.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `allianceauth_discordbot-3.7.3/PKG-INFO` & `allianceauth_discordbot-3.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: allianceauth-discordbot
-Version: 3.7.3
+Version: 3.8.0
 Summary: Alliance Auth Modular Discord Bot
 Keywords: allianceauth,eveonline
 Author-email: AaronKable <aaronkable@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Celery
@@ -150,15 +150,19 @@
 
 ```bash
 wget https://raw.githubusercontent.com/pvyParts/allianceauth-discordbot/master/bot_conf.py
 ```
 
 ## Running Discordbot with Docker
 
-Update base image to have bot_conf.py mapped
+* To download the `bot_conf.py` file into your `conf/` folder, run the following from your aa-docker folder
+```bash
+wget https://raw.githubusercontent.com/pvyParts/allianceauth-discordbot/master/bot_conf.py -O conf/bot_conf.py
+```
+* Update base image to have bot_conf.py mapped
 
 ```dockerfile
 x-allianceauth-base:
 
 # image: ${AA_DOCKER_TAG?err}
 
   &allianceauth-base
@@ -217,16 +221,15 @@
 ```ini
 corputils.view_alliance_corpstats
 ```
 
 ## Optional Settings
 
 ### Built in Cogs
-
- ```python
+```python
 # Change the bots default Cogs, add or remove if you want to use any of the extra cogs.
 
 DISCORD_BOT_COGS = [
   "aadiscordbot.cogs.about", # about the bot
   "aadiscordbot.cogs.admin", # Discord server admin helpers
   "aadiscordbot.cogs.members", # Member lookup commands
   "aadiscordbot.cogs.timers", # timer board integration
@@ -240,14 +243,15 @@
   "aadiscordbot.cogs.price_check", # Price Checks
   "aadiscordbot.cogs.eightball", # 8ball should i install this cog
   "aadiscordbot.cogs.welcomegoodbye", # Customizable user join/leave messages
   "aadiscordbot.cogs.models", # Populate and Maintain Django Models for Channels and Servers
   "aadiscordbot.cogs.quote", # Save and recall messages
   "aadiscordbot.cogs.prom_export", # Admin Level Logging cog
   "aadiscordbot.cogs.tickets", # Private thread ticket system with pingable groups.
+  "aadiscordbot.cogs.recruit_me", # Private thread recruitment ticket system.
   ]
 ```
 
 ### Additional Rate Limiting
 
 ```python
 # configure the optional rate limited
```

