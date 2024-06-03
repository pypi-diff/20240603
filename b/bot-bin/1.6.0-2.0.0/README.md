# Comparing `tmp/bot-bin-1.6.0.tar.gz` & `tmp/bot-bin-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bot-bin-1.6.0.tar", last modified: Fri Jul 24 19:41:28 2020, max compression
+gzip compressed data, was "bot-bin-2.0.0.tar", last modified: Mon Jun  3 00:50:24 2024, max compression
```

## Comparing `bot-bin-1.6.0.tar` & `bot-bin-2.0.0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2020-07-24 19:41:28.428770 bot-bin-1.6.0/
--rw-r--r--   0 user      (1000) user      (1000)       16 2019-05-11 17:27:50.000000 bot-bin-1.6.0/MANIFEST.in
--rw-r--r--   0 user      (1000) user      (1000)     3306 2020-07-24 19:41:28.428770 bot-bin-1.6.0/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)     2179 2019-09-10 18:05:48.000000 bot-bin-1.6.0/README.md
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2020-07-24 19:41:28.425437 bot-bin-1.6.0/bot_bin/
--rw-r--r--   0 user      (1000) user      (1000)      161 2020-07-24 19:40:04.000000 bot-bin-1.6.0/bot_bin/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)     6487 2020-07-24 19:38:29.000000 bot-bin-1.6.0/bot_bin/bot.py
--rw-r--r--   0 user      (1000) user      (1000)     4075 2019-09-05 20:46:53.000000 bot-bin-1.6.0/bot_bin/debug.py
--rw-r--r--   0 user      (1000) user      (1000)     7373 2020-05-12 23:28:29.000000 bot-bin-1.6.0/bot_bin/misc.py
--rw-r--r--   0 user      (1000) user      (1000)     8571 2020-06-23 23:04:14.000000 bot-bin-1.6.0/bot_bin/socket.py
--rw-r--r--   0 user      (1000) user      (1000)     3334 2019-10-03 00:11:19.000000 bot-bin-1.6.0/bot_bin/sql.py
--rw-r--r--   0 user      (1000) user      (1000)     4410 2020-06-23 23:04:55.000000 bot-bin-1.6.0/bot_bin/stats.py
--rw-r--r--   0 user      (1000) user      (1000)      849 2020-07-24 19:38:29.000000 bot-bin-1.6.0/bot_bin/systemd.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2020-07-24 19:41:28.428770 bot-bin-1.6.0/bot_bin.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)     3306 2020-07-24 19:41:28.000000 bot-bin-1.6.0/bot_bin.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)      321 2020-07-24 19:41:28.000000 bot-bin-1.6.0/bot_bin.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2020-07-24 19:41:28.000000 bot-bin-1.6.0/bot_bin.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) user      (1000)      140 2020-07-24 19:41:28.000000 bot-bin-1.6.0/bot_bin.egg-info/requires.txt
--rw-r--r--   0 user      (1000) user      (1000)        8 2020-07-24 19:41:28.000000 bot-bin-1.6.0/bot_bin.egg-info/top_level.txt
--rw-r--r--   0 user      (1000) user      (1000)       38 2020-07-24 19:41:28.428770 bot-bin-1.6.0/setup.cfg
--rwxr-xr-x   0 user      (1000) user      (1000)     1237 2020-07-24 19:38:29.000000 bot-bin-1.6.0/setup.py
+drwxr-x---   0 user      (1000) user      (1000)        0 2024-06-03 00:50:24.948242 bot-bin-2.0.0/
+-rw-r-----   0 user      (1000) user      (1000)     1551 2024-05-27 23:20:36.000000 bot-bin-2.0.0/LICENSE.md
+-rw-r-----   0 user      (1000) user      (1000)       16 2024-05-27 23:20:36.000000 bot-bin-2.0.0/MANIFEST.in
+-rw-r--r--   0 user      (1000) user      (1000)     3257 2024-06-03 00:50:24.948242 bot-bin-2.0.0/PKG-INFO
+-rw-r-----   0 user      (1000) user      (1000)     2179 2024-05-27 23:20:36.000000 bot-bin-2.0.0/README.md
+drwxr-x---   0 user      (1000) user      (1000)        0 2024-06-03 00:50:24.948242 bot-bin-2.0.0/bot_bin/
+-rw-r-----   0 user      (1000) user      (1000)      148 2024-06-03 00:49:36.000000 bot-bin-2.0.0/bot_bin/__init__.py
+-rw-r-----   0 user      (1000) user      (1000)     7103 2024-06-03 00:49:36.000000 bot-bin-2.0.0/bot_bin/bot.py
+-rw-r-----   0 user      (1000) user      (1000)     4086 2024-06-03 00:49:36.000000 bot-bin-2.0.0/bot_bin/debug.py
+-rw-r-----   0 user      (1000) user      (1000)     7385 2024-06-03 00:49:36.000000 bot-bin-2.0.0/bot_bin/misc.py
+-rw-r-----   0 user      (1000) user      (1000)     8571 2024-05-27 23:20:36.000000 bot-bin-2.0.0/bot_bin/socket.py
+-rw-r-----   0 user      (1000) user      (1000)     3346 2024-06-03 00:49:36.000000 bot-bin-2.0.0/bot_bin/sql.py
+-rw-r-----   0 user      (1000) user      (1000)     4495 2024-06-03 00:49:36.000000 bot-bin-2.0.0/bot_bin/stats.py
+-rw-r-----   0 user      (1000) user      (1000)      861 2024-06-03 00:49:36.000000 bot-bin-2.0.0/bot_bin/systemd.py
+drwxr-x---   0 user      (1000) user      (1000)        0 2024-06-03 00:50:24.948242 bot-bin-2.0.0/bot_bin.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)     3257 2024-06-03 00:50:24.000000 bot-bin-2.0.0/bot_bin.egg-info/PKG-INFO
+-rw-r-----   0 user      (1000) user      (1000)      332 2024-06-03 00:50:24.000000 bot-bin-2.0.0/bot_bin.egg-info/SOURCES.txt
+-rw-r-----   0 user      (1000) user      (1000)        1 2024-06-03 00:50:24.000000 bot-bin-2.0.0/bot_bin.egg-info/dependency_links.txt
+-rw-r-----   0 user      (1000) user      (1000)      140 2024-06-03 00:50:24.000000 bot-bin-2.0.0/bot_bin.egg-info/requires.txt
+-rw-r-----   0 user      (1000) user      (1000)        8 2024-06-03 00:50:24.000000 bot-bin-2.0.0/bot_bin.egg-info/top_level.txt
+-rw-r-----   0 user      (1000) user      (1000)       38 2024-06-03 00:50:24.948242 bot-bin-2.0.0/setup.cfg
+-rwxr-x---   0 user      (1000) user      (1000)     1236 2024-06-03 00:49:36.000000 bot-bin-2.0.0/setup.py
```

### Comparing `bot-bin-1.6.0/PKG-INFO` & `bot-bin-2.0.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,67 +1,44 @@
-Metadata-Version: 2.1
-Name: bot-bin
-Version: 1.6.0
-Summary: Shared cogs and utilities for use in Discord bots
-Home-page: https://github.com/bmintz/bot-bin
-Author: lambda#0987
-License: BlueOak-1.0.0
-Download-URL: https://github.com/bot-bin/cogs/archive/v1.6.0.tar.gz
-Description: # Bot Bin
-        Shared cogs and utilities for use in Discord bots.
-        Some cogs require bot configuration; those that do expect a `bot.config` dict attribute.
-        
-        ## bot_bin.bot
-        
-        Contains an AutoShardedBot subclass. Contains custom error logging, customizable on_message bot ignoring,
-        case insensitive prefixes, and database setup if the setup_db kwarg is set to True. Requires the config kwarg
-        to be set to a dict. bot.config['tokens']['discord'] should be the bot's Discord token.
-        
-        ## bot_bin.debug
-        
-        Contains memory usage and performance debugging commands. Most other debug functionality is already provided
-        by [jishaku](https://pypi.org/project/jishaku/).
-        
-        ## bot_bin.misc
-        
-        Contains an uptime, ping, and copyright command. The latter requires bot.config['copyright_license_file'] to be
-        set to a path to a text file, the contents of which will be sent when the user runs the copyright command.
-        
-        Also contains various utilities:
-        - `codeblock` wraps text in a markdown code block
-        - `absolute_natural_timedelta` returns an English string representing an amount of seconds
-        - `natural_timedelta` returns an English string representing the difference between two dates.
-          This function differs from `absolute_natural_timedelta` in that it also supports years and months.
-        - `natural_rate` returns an English string representing a rate of occurence.
-        - `plural` is a format object which pluralizes strings. For example: `f'Found {plural(len(results)):weapon}'`
-        - `natural_join` joins a sequence of strings according to English grammar
-        - `timeit` is a context manager that times the code in the `with` block
-        
-        ## bot_bin.sql
-        
-        Contains SQL execution commands for asyncpg.
-        Requires `bot.pool` to be set to either an asyncpg Connection or a ConnectionPool.
-        Requires the `bot_bin[sql]` extra.
-        
-        ## bot_bin.stats
-        
-        Implements the guild count API for DBL, DBots, Bots For Discord, LBots, and Discord Boats.
-        This is configured using `bot.config['tokens']['stats']`.
-        Each key should be a domain, e.g. `bot.config['tokens']['stats']['discordbots.org']` would be the bot's DBL token.
-        
-        Defines a `send-stats` owner only command which sends the current guild counts to the configured APIs
-        and reports any errors.
-        
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: Framework :: AsyncIO
-Classifier: Intended Audience :: Developers
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Topic :: Internet
-Classifier: Topic :: Utilities
-Requires-Python: >=3.6.0
-Description-Content-Type: text/markdown
-Provides-Extra: sql
-Provides-Extra: uvloop
+# Bot Bin
+Shared cogs and utilities for use in Discord bots.
+Some cogs require bot configuration; those that do expect a `bot.config` dict attribute.
+
+## bot_bin.bot
+
+Contains an AutoShardedBot subclass. Contains custom error logging, customizable on_message bot ignoring,
+case insensitive prefixes, and database setup if the setup_db kwarg is set to True. Requires the config kwarg
+to be set to a dict. bot.config['tokens']['discord'] should be the bot's Discord token.
+
+## bot_bin.debug
+
+Contains memory usage and performance debugging commands. Most other debug functionality is already provided
+by [jishaku](https://pypi.org/project/jishaku/).
+
+## bot_bin.misc
+
+Contains an uptime, ping, and copyright command. The latter requires bot.config['copyright_license_file'] to be
+set to a path to a text file, the contents of which will be sent when the user runs the copyright command.
+
+Also contains various utilities:
+- `codeblock` wraps text in a markdown code block
+- `absolute_natural_timedelta` returns an English string representing an amount of seconds
+- `natural_timedelta` returns an English string representing the difference between two dates.
+  This function differs from `absolute_natural_timedelta` in that it also supports years and months.
+- `natural_rate` returns an English string representing a rate of occurence.
+- `plural` is a format object which pluralizes strings. For example: `f'Found {plural(len(results)):weapon}'`
+- `natural_join` joins a sequence of strings according to English grammar
+- `timeit` is a context manager that times the code in the `with` block
+
+## bot_bin.sql
+
+Contains SQL execution commands for asyncpg.
+Requires `bot.pool` to be set to either an asyncpg Connection or a ConnectionPool.
+Requires the `bot_bin[sql]` extra.
+
+## bot_bin.stats
+
+Implements the guild count API for DBL, DBots, Bots For Discord, LBots, and Discord Boats.
+This is configured using `bot.config['tokens']['stats']`.
+Each key should be a domain, e.g. `bot.config['tokens']['stats']['discordbots.org']` would be the bot's DBL token.
+
+Defines a `send-stats` owner only command which sends the current guild counts to the configured APIs
+and reports any errors.
```

### Comparing `bot-bin-1.6.0/bot_bin/bot.py` & `bot-bin-2.0.0/bot_bin/bot.py`

 * *Files 7% similar despite different names*

```diff
@@ -129,36 +129,46 @@
 				message = 'Sorry. This command is disabled and cannot be used.'
 				try:
 					await ctx.author.send(message)
 				except discord.Forbidden:
 					await ctx.send(message)
 			elif isinstance(error, commands.NotOwner):
 				logger.error('%s tried to run %s but is not the owner', ctx.author, ctx.command.name)
-				await ctx.message.add_reaction(self.config['success_emojis'][False])
+				await ctx.send(self.config['success_emojis'][False], ephemeral=True, delete_after=3.0)
 			elif isinstance(error, (commands.UserInputError, commands.CheckFailure)):
 				await ctx.send(error)
 			elif (
-				isinstance(error, commands.CommandInvokeError)
+				isinstance(error, (commands.HybridCommandError, commands.CommandInvokeError))
 				and (not ctx.cog or type(ctx.cog).cog_command_error is commands.Cog.cog_command_error)  # not overridden
 				and not hasattr(ctx.command, 'on_error')
 			):
-				logger.error('"%s" caused an exception <%s>', ctx.message.content, ctx.message.jump_url)
-				logger.error(''.join(traceback.format_tb(error.original.__traceback__)))
-				# pylint: disable=logging-format-interpolation
-				logger.error('{0.__class__.__name__}: {0}'.format(error.original))
+				if ctx.interaction:
+					formatted = ' '.join(
+						f'{param}: “{argument}”'
+						for param, argument
+						in ctx.interaction.namespace
+					)
+					if ctx.interaction.command:
+						logger.exception('"/%s %s" caused an exception', ctx.interaction.command.name, formatted, exc_info=error)
+					else:
+						logger.exception('Non-command interaction "%s" caused an exception', formatted, exc_info=error)
+				else:
+					logger.exception('"%s" caused an exception <%s>', ctx.message.content, ctx.message.jump_url, exc_info=error)
 
-				await ctx.send('An internal error occured while trying to run that command.')
+				await ctx.send('An internal error occured while trying to run that command.', ephemeral=True)
 
 	### Utility functions
 
 	def should_reply(self, message):
 		"""return whether the bot should reply to a given message"""
-		return not (
-			message.author == self.user
-			or (message.author.bot and not self.should_reply_to_bot(message)))
+		if message.author == self.user:
+			return False
+		if message.author.bot and not self.should_reply_to_bot(message):
+			return False
+		return True
 
 	def should_reply_to_bot(self, message):
 		should_reply = not self.config['ignore_bots'].get('default')
 		overrides = self.config['ignore_bots']['overrides']
 
 		def check_override(location, overrides_key):
 			return location and location.id in overrides[overrides_key]
@@ -169,33 +179,46 @@
 		return should_reply
 
 	async def is_privileged(self, member):
 		return member.guild_permissions.administrator or await self.is_owner(member)
 
 	### Init / Shutdown
 
-	async def start(self):
+	def run(self, *, reconnect: bool = True):
+		async def runner():
+			async with self:
+				await self.start(reconnect=reconnect)
+
+		try:
+			asyncio.run(runner())
+		except KeyboardInterrupt:
+			return
+
+	async def start(self, *, reconnect: bool = True):
 		if self._should_setup_db:
 			await self.init_db()
-		self.load_extensions()
+		await self.load_extensions()
 
-		await super().start(self.config['tokens'].pop('discord'))
+		await super().start(
+			self.config['tokens'].pop('discord'),
+			reconnect=reconnect,
+		)
 
 	async def close(self):
 		if self._should_setup_db:
 			with contextlib.suppress(AttributeError):
 				await self.pool.close()
 		await super().close()
 
 	async def init_db(self):
 		credentials = self.config['database']
 		self.pool = await asyncpg.create_pool(**credentials)
 
-	def load_extensions(self):
+	async def load_extensions(self):
 		for extension in self.startup_extensions:  # subclasses must define this
-			self.load_extension(extension)
+			await self.load_extension(extension)
 
 def convert_emoji(s) -> discord.PartialEmoji:
 	match = re.search(r'<?(a?):([A-Za-z0-9_]+):([0-9]{17,})>?', s)
 	if match:
 		return discord.PartialEmoji(animated=match[1], name=match[2], id=int(match[3]))
 	return discord.PartialEmoji(animated=None, name=s, id=None)
```

### Comparing `bot-bin-1.6.0/bot_bin/debug.py` & `bot-bin-2.0.0/bot_bin/debug.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,14 +136,13 @@
 				await context.send(f'```py\n{traceback.format_exc()}\n```')
 		else:
 			end = time.perf_counter()
 			success = '✅'
 
 		await context.send(f'Status: {success} Time: {(end - start) * 1000:.2f}ms')
 
-
-def setup(bot):
-	bot.add_cog(BotBinDebug())
+async def setup(bot):
+	await bot.add_cog(BotBinDebug())
 
 	if not HAVE_PSUTIL:
 		for command in 'objgrowth', 'most-common-types', 'mem':
 			bot.remove_command(command)
```

### Comparing `bot-bin-1.6.0/bot_bin/misc.py` & `bot-bin-2.0.0/bot_bin/misc.py`

 * *Files 0% similar despite different names*

```diff
@@ -242,12 +242,12 @@
 		reply = await context.send('Ping')
 		if context.message.created_at < reply.created_at:
 			# the messages appeared in the correct order
 			await reply.delete()
 		# due to loose snowflake ordering, we time travelled
 		# so leave the reply message alone
 
-def setup(bot):
+async def setup(bot):
 	cog = BotBinMisc(bot)
-	bot.add_cog(cog)
+	await bot.add_cog(cog)
 	if not hasattr(cog, 'license_message'):
 		bot.remove_command('copyright')
```

### Comparing `bot-bin-1.6.0/bot_bin/socket.py` & `bot-bin-2.0.0/bot_bin/socket.py`

 * *Files identical despite different names*

### Comparing `bot-bin-1.6.0/bot_bin/sql.py` & `bot-bin-2.0.0/bot_bin/sql.py`

 * *Files 4% similar despite different names*

```diff
@@ -91,11 +91,11 @@
 		elapsed = round(timer.elapsed * 1000, 2)
 
 		# fetchval returns a native python result
 		# so its repr is probably python code
 		message = codeblock(repr(result), lang='python')
 		await context.send(f'{message}\n*Retrieved in {elapsed}ms.*')
 
-def setup(bot):
+async def setup(bot):
 	if bot.case_insensitive:
 		BotBinSql.sql_command.aliases.clear()
-	bot.add_cog(BotBinSql(bot.pool))
+	await bot.add_cog(BotBinSql(bot.pool))
```

### Comparing `bot-bin-1.6.0/bot_bin/stats.py` & `bot-bin-2.0.0/bot_bin/stats.py`

 * *Files 5% similar despite different names*

```diff
@@ -80,15 +80,17 @@
 		if self.bot.owner_id:
 			owners = [self.bot.get_user(self.bot.owner_id)]
 		elif self.bot.owner_ids:
 			owners = map(self.bot.get_user, self.bot.owner_ids)
 
 		async def send(user):
 			await user.send(f'Guild count ({guild_count}) is a power of 2!')
-		await asyncio.gather(*map(send, owners))
+		async with asyncio.TaskGroup() as tg:
+			for user in owners:
+				tg.create_task(send(user))
 
 	async def guild_count(self):
 		"""Return the guild count for the bot associated with this cog.
 		Override this if your guild count needs manipulation.
 		"""
 		return len(self.bot.guilds)
 
@@ -100,43 +102,39 @@
 
 		succeeded = []
 		failed = []
 		for config_key, (status, text) in statuses.items():
 			(succeeded if status in range(200, 300) else failed).append((config_key, status, text))
 
 		if not failed:
-			await context.message.add_reaction('✅')
+			await context.message.add_reaction(bot.config['success_emojis'][True])
 
 		def format(apis):
 			return '\n'.join(
 				f'• {config_key}: **{status}**\n{textwrap.shorten(text, 150)}'
 				for config_key, status, text in apis
 			)
 
 		message = []
 		if succeeded:
 			message.append('The following APIs succeeded:\n' + format(succeeded))
 		if failed:
 			message.append('The following APIs failed:\n' + format(failed))
 		if not message:
-			await asyncio.gather(
-				context.message.add_reaction('❌'),
-				context.send(
+			async with asyncio.TaskGroup() as tg:
+				tg.create_task(context.message.add_reaction(self.bot.config['success_emojis'][False]))
+				tg.create_task(context.send(
 					'No APIs are currently configured. '
 					"Please double check that `bot.config['tokens']['stats']` is correctly set."
-				)
-			)
+				))
 			return
 
-		await asyncio.gather(
-			context.message.add_reaction('❌' if failed else '✅'),
-			context.send('\n\n'.join(message))
-		)
+		await context.send('\n\n'.join(message))
 
 	@commands.Cog.listener(name='on_guild_join')
 	@commands.Cog.listener(name='on_guild_remove')
 	async def on_guild_change(self, _):
 		await self.notify_owners()
 		await self.send()
 
-def setup(bot):
-	bot.add_cog(BotBinStats(bot))
+async def setup(bot):
+	await bot.add_cog(BotBinStats(bot))
```

### Comparing `bot-bin-1.6.0/bot_bin/systemd.py` & `bot-bin-2.0.0/bot_bin/systemd.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,10 +25,10 @@
 	async def on_shard_ready(self, shard_id):
 		self.send(b'STATUS=Ready on shard %d' % shard_id)
 
 	@commands.Cog.listener()
 	async def on_ready(self):
 		self.send(b'READY=1')
 
-def setup(bot):
+async def setup(bot):
 	if 'NOTIFY_SOCKET' in os.environ:
-		bot.add_cog(BotBinSystemdNotifier())
+		await bot.add_cog(BotBinSystemdNotifier())
```

### Comparing `bot-bin-1.6.0/bot_bin.egg-info/PKG-INFO` & `bot-bin-2.0.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,67 +1,75 @@
 Metadata-Version: 2.1
 Name: bot-bin
-Version: 1.6.0
+Version: 2.0.0
 Summary: Shared cogs and utilities for use in Discord bots
 Home-page: https://github.com/bmintz/bot-bin
-Author: lambda#0987
+Download-URL: https://github.com/bot-bin/cogs/archive/v2.0.0.tar.gz
+Author: lambda0987
 License: BlueOak-1.0.0
-Download-URL: https://github.com/bot-bin/cogs/archive/v1.6.0.tar.gz
-Description: # Bot Bin
-        Shared cogs and utilities for use in Discord bots.
-        Some cogs require bot configuration; those that do expect a `bot.config` dict attribute.
-        
-        ## bot_bin.bot
-        
-        Contains an AutoShardedBot subclass. Contains custom error logging, customizable on_message bot ignoring,
-        case insensitive prefixes, and database setup if the setup_db kwarg is set to True. Requires the config kwarg
-        to be set to a dict. bot.config['tokens']['discord'] should be the bot's Discord token.
-        
-        ## bot_bin.debug
-        
-        Contains memory usage and performance debugging commands. Most other debug functionality is already provided
-        by [jishaku](https://pypi.org/project/jishaku/).
-        
-        ## bot_bin.misc
-        
-        Contains an uptime, ping, and copyright command. The latter requires bot.config['copyright_license_file'] to be
-        set to a path to a text file, the contents of which will be sent when the user runs the copyright command.
-        
-        Also contains various utilities:
-        - `codeblock` wraps text in a markdown code block
-        - `absolute_natural_timedelta` returns an English string representing an amount of seconds
-        - `natural_timedelta` returns an English string representing the difference between two dates.
-          This function differs from `absolute_natural_timedelta` in that it also supports years and months.
-        - `natural_rate` returns an English string representing a rate of occurence.
-        - `plural` is a format object which pluralizes strings. For example: `f'Found {plural(len(results)):weapon}'`
-        - `natural_join` joins a sequence of strings according to English grammar
-        - `timeit` is a context manager that times the code in the `with` block
-        
-        ## bot_bin.sql
-        
-        Contains SQL execution commands for asyncpg.
-        Requires `bot.pool` to be set to either an asyncpg Connection or a ConnectionPool.
-        Requires the `bot_bin[sql]` extra.
-        
-        ## bot_bin.stats
-        
-        Implements the guild count API for DBL, DBots, Bots For Discord, LBots, and Discord Boats.
-        This is configured using `bot.config['tokens']['stats']`.
-        Each key should be a domain, e.g. `bot.config['tokens']['stats']['discordbots.org']` would be the bot's DBL token.
-        
-        Defines a `send-stats` owner only command which sends the current guild counts to the configured APIs
-        and reports any errors.
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Internet
 Classifier: Topic :: Utilities
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
+License-File: LICENSE.md
+Requires-Dist: discord.py<3.0.0,>=2.0.0
+Requires-Dist: humanize
+Requires-Dist: python-dateutil
+Requires-Dist: objgraph
 Provides-Extra: sql
+Requires-Dist: aiocontextvars>=0.2.2; extra == "sql"
+Requires-Dist: asyncpg; extra == "sql"
+Requires-Dist: prettytable; extra == "sql"
 Provides-Extra: uvloop
+Requires-Dist: uvloop<1.0.0,>=0.14.0; extra == "uvloop"
+
+# Bot Bin
+Shared cogs and utilities for use in Discord bots.
+Some cogs require bot configuration; those that do expect a `bot.config` dict attribute.
+
+## bot_bin.bot
+
+Contains an AutoShardedBot subclass. Contains custom error logging, customizable on_message bot ignoring,
+case insensitive prefixes, and database setup if the setup_db kwarg is set to True. Requires the config kwarg
+to be set to a dict. bot.config['tokens']['discord'] should be the bot's Discord token.
+
+## bot_bin.debug
+
+Contains memory usage and performance debugging commands. Most other debug functionality is already provided
+by [jishaku](https://pypi.org/project/jishaku/).
+
+## bot_bin.misc
+
+Contains an uptime, ping, and copyright command. The latter requires bot.config['copyright_license_file'] to be
+set to a path to a text file, the contents of which will be sent when the user runs the copyright command.
+
+Also contains various utilities:
+- `codeblock` wraps text in a markdown code block
+- `absolute_natural_timedelta` returns an English string representing an amount of seconds
+- `natural_timedelta` returns an English string representing the difference between two dates.
+  This function differs from `absolute_natural_timedelta` in that it also supports years and months.
+- `natural_rate` returns an English string representing a rate of occurence.
+- `plural` is a format object which pluralizes strings. For example: `f'Found {plural(len(results)):weapon}'`
+- `natural_join` joins a sequence of strings according to English grammar
+- `timeit` is a context manager that times the code in the `with` block
+
+## bot_bin.sql
+
+Contains SQL execution commands for asyncpg.
+Requires `bot.pool` to be set to either an asyncpg Connection or a ConnectionPool.
+Requires the `bot_bin[sql]` extra.
+
+## bot_bin.stats
+
+Implements the guild count API for DBL, DBots, Bots For Discord, LBots, and Discord Boats.
+This is configured using `bot.config['tokens']['stats']`.
+Each key should be a domain, e.g. `bot.config['tokens']['stats']['discordbots.org']` would be the bot's DBL token.
+
+Defines a `send-stats` owner only command which sends the current guild counts to the configured APIs
+and reports any errors.
```

### Comparing `bot-bin-1.6.0/setup.py` & `bot-bin-2.0.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,24 +7,24 @@
     version = re.search(r'^__version__\s*=\s*[\'"]([^\'"]*)[\'"]', f.read(), re.MULTILINE).group(1)
 
 with open('README.md') as f:
 	long_description = f.read()
 
 setup(
 	name='bot-bin',
-	author='lambda#0987',
+	author='lambda0987',
 	description='Shared cogs and utilities for use in Discord bots',
 	long_description=long_description,
 	long_description_content_type='text/markdown',
 	url='https://github.com/bmintz/bot-bin',
 	download_url='https://github.com/bot-bin/cogs/archive/v{}.tar.gz'.format(version),
 	version=version,
 	packages=['bot_bin'],
 	install_requires=[
-		'discord.py>=1.3.3,<2.0.0',
+		'discord.py>=2.0.0,<3.0.0',
 		'humanize',
 		'python-dateutil',
 		'objgraph'],
 	extras_require={
 		'sql': [
 			'aiocontextvars>=0.2.2',
 			'asyncpg',
```

