# Comparing `tmp/asmek_authcogs-1.1.1.tar.gz` & `tmp/asmek_authcogs-1.1.2.tar.gz`

## Comparing `asmek_authcogs-1.1.1.tar` & `asmek_authcogs-1.1.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.1/CHANGELOG.md
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.1/.github/workflows/publish.yml
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.1/asmek_authcogs/__init__.py
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.1/asmek_authcogs/app_settings.py
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.1/asmek_authcogs/apps.py
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.1/asmek_authcogs/auth_hooks.py
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.1/asmek_authcogs/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.1/asmek_authcogs/Images/__init__.py
--rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.1/asmek_authcogs/Images/eve-o-4.png
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.1/asmek_authcogs/Images/smt_bomb_icon-1.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.1/asmek_authcogs/cogs/__init__.py
--rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.1/asmek_authcogs/cogs/about.py
--rw-r--r--   0        0        0     4916 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.1/asmek_authcogs/cogs/auth.py
--rw-r--r--   0        0        0     8254 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.1/asmek_authcogs/cogs/links.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.1/asmek_authcogs/cogs/siege.py
--rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.1/asmek_authcogs/migrations/0001_initial.py
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.1/asmek_authcogs/migrations/0002_alter_link_name.py
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.1/asmek_authcogs/migrations/0003_alter_general_options.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.1/asmek_authcogs/migrations/__init__.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.1/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.1/LICENSE
--rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.1/README.md
--rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     2096 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.2/CHANGELOG.md
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.2/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.2/asmek_authcogs/__init__.py
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.2/asmek_authcogs/app_settings.py
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.2/asmek_authcogs/apps.py
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.2/asmek_authcogs/auth_hooks.py
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.2/asmek_authcogs/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.2/asmek_authcogs/Images/__init__.py
+-rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.2/asmek_authcogs/Images/eve-o-4.png
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.2/asmek_authcogs/Images/smt_bomb_icon-1.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.2/asmek_authcogs/cogs/__init__.py
+-rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.2/asmek_authcogs/cogs/about.py
+-rw-r--r--   0        0        0     4916 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.2/asmek_authcogs/cogs/auth.py
+-rw-r--r--   0        0        0     8254 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.2/asmek_authcogs/cogs/links.py
+-rw-r--r--   0        0        0     2696 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.2/asmek_authcogs/cogs/siege.py
+-rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.2/asmek_authcogs/migrations/0001_initial.py
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.2/asmek_authcogs/migrations/0002_alter_link_name.py
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.2/asmek_authcogs/migrations/0003_alter_general_options.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.2/asmek_authcogs/migrations/__init__.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.2/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.2/LICENSE
+-rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.2/README.md
+-rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2096 2020-02-02 00:00:00.000000 asmek_authcogs-1.1.2/PKG-INFO
```

### Comparing `asmek_authcogs-1.1.1/CHANGELOG.md` & `asmek_authcogs-1.1.2/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `asmek_authcogs-1.1.1/.github/workflows/publish.yml` & `asmek_authcogs-1.1.2/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `asmek_authcogs-1.1.1/asmek_authcogs/models.py` & `asmek_authcogs-1.1.2/asmek_authcogs/models.py`

 * *Files identical despite different names*

### Comparing `asmek_authcogs-1.1.1/asmek_authcogs/Images/eve-o-4.png` & `asmek_authcogs-1.1.2/asmek_authcogs/Images/eve-o-4.png`

 * *Files identical despite different names*

### Comparing `asmek_authcogs-1.1.1/asmek_authcogs/Images/smt_bomb_icon-1.png` & `asmek_authcogs-1.1.2/asmek_authcogs/Images/smt_bomb_icon-1.png`

 * *Files identical despite different names*

### Comparing `asmek_authcogs-1.1.1/asmek_authcogs/cogs/about.py` & `asmek_authcogs-1.1.2/asmek_authcogs/cogs/about.py`

 * *Files identical despite different names*

### Comparing `asmek_authcogs-1.1.1/asmek_authcogs/cogs/auth.py` & `asmek_authcogs-1.1.2/asmek_authcogs/cogs/auth.py`

 * *Files identical despite different names*

### Comparing `asmek_authcogs-1.1.1/asmek_authcogs/cogs/links.py` & `asmek_authcogs-1.1.2/asmek_authcogs/cogs/links.py`

 * *Files identical despite different names*

### Comparing `asmek_authcogs-1.1.1/asmek_authcogs/cogs/siege.py` & `asmek_authcogs-1.1.2/asmek_authcogs/cogs/siege.py`

 * *Files 23% similar despite different names*

```diff
@@ -29,48 +29,40 @@
         All Clear
         """
         if len(msg) == 0:
             msg = 'SIEGE GREEN - Crab on!'
         siege_channel = self.bot.get_channel(int(settings.ASMEK_SIEGE_CHANNEL))
         await siege_channel.purge()
         await siege_channel.send(' @here '+ msg + '\nhttps://media.discordapp.net/attachments/478100446238474282/671250121178218496/Green_w_Excav.gif')
+        await siege_channel.edit(name = 'delve-status-💸')
         return await ctx.respond("Siege status updated to GREEN", ephemeral=True)
     
     @siege_commands.command(name="amber", guild_ids=[int(settings.DISCORD_GUILD_ID)])
     @sender_has_perm("general.siege_control")
     async def amber(self, ctx,*,msg=''):
         """
         Ratting caps should dock, rorqs max tank
         """
         if len(msg) == 0:
             msg = 'SIEGE AMBER - Caps dock / Rorqs max tank!'
         siege_channel = self.bot.get_channel(int(settings.ASMEK_SIEGE_CHANNEL))
         await siege_channel.purge()
         await siege_channel.send('@here '+ msg + '\nhttps://media.discordapp.net/attachments/726469660916318218/829165923436331039/unknown.png')
+        await siege_channel.edit(name = 'delve-status-🟠')
         return await ctx.respond("Siege status updated to AMBER", ephemeral=True)
     
     @siege_commands.command(name="red", guild_ids=[int(settings.DISCORD_GUILD_ID)])
     @sender_has_perm("general.siege_control")
-    async def red(self, ctx):
+    async def red(self, ctx,*,msg=''):
         """
         Everyone should dock up
         """
         if len(msg) == 0:
             msg = 'SIEGE RED - Delve is dangerous!'
         siege_channel = self.bot.get_channel(int(settings.ASMEK_SIEGE_CHANNEL))
         await siege_channel.purge()
         await siege_channel.send('@here '+ msg + '\nhttps://media.discordapp.net/attachments/478100446238474282/671250121345728542/Red_Final.gif')
+        await siege_channel.edit(name = 'delve-status-🔴')
         return await ctx.respond("Siege status updated to RED", ephemeral=True)
-    
-    @siege_commands.command(name="cta", guild_ids=[int(settings.DISCORD_GUILD_ID)])
-    @sender_has_perm("general.siege_control")
-    async def red(self, ctx):
-        """
-        CTA dock up
-        """
-        siege_channel = self.bot.get_channel(int(settings.ASMEK_SIEGE_CHANNEL))
-        await siege_channel.purge()
-        await siege_channel.send('@here SIEGE RED - CTA IS MUST ATTEND! \nhttps://media.discordapp.net/attachments/478100446238474282/671250121345728542/Red_Final.gif')
-        return await ctx.respond("Siege status updated to RED/CTA", ephemeral=True)
-    
+        
 def setup(bot):
     bot.add_cog(Siege(bot))
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `asmek_authcogs-1.1.1/asmek_authcogs/migrations/0001_initial.py` & `asmek_authcogs-1.1.2/asmek_authcogs/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `asmek_authcogs-1.1.1/.gitignore` & `asmek_authcogs-1.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `asmek_authcogs-1.1.1/LICENSE` & `asmek_authcogs-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `asmek_authcogs-1.1.1/README.md` & `asmek_authcogs-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `asmek_authcogs-1.1.1/pyproject.toml` & `asmek_authcogs-1.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `asmek_authcogs-1.1.1/PKG-INFO` & `asmek_authcogs-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asmek-authcogs
-Version: 1.1.1
+Version: 1.1.2
 Summary: ASMEK customized cogs for aa-discordbot
 Project-URL: Documentation, https://github.com/AstrumMechanica/asmek-authcogs#readme
 Project-URL: Issues, https://github.com/AstrumMechanica/asmek-authcogs/issues
 Project-URL: Source, https://github.com/AstrumMechanica/asmek-authcogs
 Author-email: AstrumMechanica <astrummechanica@gmail.com>
 License-Expression: GPL-3.0
 License-File: LICENSE
```

