# Comparing `tmp/tnnt_discordbot_cogs-0.4.0.tar.gz` & `tmp/tnnt_discordbot_cogs-0.5.0.tar.gz`

## Comparing `tnnt_discordbot_cogs-0.4.0.tar` & `tnnt_discordbot_cogs-0.5.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 tnnt_discordbot_cogs-0.4.0/tnnt_discordbot_cogs/__init__.py
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 tnnt_discordbot_cogs-0.4.0/tnnt_discordbot_cogs/apps.py
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 tnnt_discordbot_cogs-0.4.0/tnnt_discordbot_cogs/auth_hooks.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 tnnt_discordbot_cogs-0.4.0/tnnt_discordbot_cogs/cogs/__init__.py
--rw-r--r--   0        0        0     6856 2020-02-02 00:00:00.000000 tnnt_discordbot_cogs-0.4.0/tnnt_discordbot_cogs/cogs/about.py
--rw-r--r--   0        0        0     4059 2020-02-02 00:00:00.000000 tnnt_discordbot_cogs-0.4.0/tnnt_discordbot_cogs/cogs/auth.py
--rw-r--r--   0        0        0     9717 2020-02-02 00:00:00.000000 tnnt_discordbot_cogs-0.4.0/tnnt_discordbot_cogs/cogs/members.py
--rw-r--r--   0        0        0     6986 2020-02-02 00:00:00.000000 tnnt_discordbot_cogs-0.4.0/tnnt_discordbot_cogs/cogs/price_check.py
--rw-r--r--   0        0        0     4558 2020-02-02 00:00:00.000000 tnnt_discordbot_cogs-0.4.0/tnnt_discordbot_cogs/cogs/timers.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 tnnt_discordbot_cogs-0.4.0/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 tnnt_discordbot_cogs-0.4.0/LICENSE
--rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 tnnt_discordbot_cogs-0.4.0/README.md
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 tnnt_discordbot_cogs-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     2483 2020-02-02 00:00:00.000000 tnnt_discordbot_cogs-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 tnnt_discordbot_cogs-0.5.0/tnnt_discordbot_cogs/__init__.py
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 tnnt_discordbot_cogs-0.5.0/tnnt_discordbot_cogs/apps.py
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 tnnt_discordbot_cogs-0.5.0/tnnt_discordbot_cogs/auth_hooks.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 tnnt_discordbot_cogs-0.5.0/tnnt_discordbot_cogs/cogs/__init__.py
+-rw-r--r--   0        0        0     2937 2020-02-02 00:00:00.000000 tnnt_discordbot_cogs-0.5.0/tnnt_discordbot_cogs/cogs/about.py
+-rw-r--r--   0        0        0     4450 2020-02-02 00:00:00.000000 tnnt_discordbot_cogs-0.5.0/tnnt_discordbot_cogs/cogs/auth.py
+-rw-r--r--   0        0        0    10200 2020-02-02 00:00:00.000000 tnnt_discordbot_cogs-0.5.0/tnnt_discordbot_cogs/cogs/members.py
+-rw-r--r--   0        0        0     7164 2020-02-02 00:00:00.000000 tnnt_discordbot_cogs-0.5.0/tnnt_discordbot_cogs/cogs/price_check.py
+-rw-r--r--   0        0        0     4880 2020-02-02 00:00:00.000000 tnnt_discordbot_cogs-0.5.0/tnnt_discordbot_cogs/cogs/timers.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 tnnt_discordbot_cogs-0.5.0/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 tnnt_discordbot_cogs-0.5.0/LICENSE
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 tnnt_discordbot_cogs-0.5.0/README.md
+-rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 tnnt_discordbot_cogs-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     2529 2020-02-02 00:00:00.000000 tnnt_discordbot_cogs-0.5.0/PKG-INFO
```

### Comparing `tnnt_discordbot_cogs-0.4.0/tnnt_discordbot_cogs/cogs/auth.py` & `tnnt_discordbot_cogs-0.5.0/tnnt_discordbot_cogs/cogs/auth.py`

 * *Files 16% similar despite different names*

```diff
@@ -34,53 +34,67 @@
         self.bot = bot
 
     @commands.command(pass_context=True)
     async def auth(self, ctx):
         """
         Returns a link to TN-NT Auth
         Used by many other Bots and is a common command that users will attempt to run.
+
+        :param ctx:
+        :type ctx:
+        :return:
+        :rtype:
         """
 
         await ctx.trigger_typing()
 
-        embed = Embed(title="Alliance Auth")
+        auth_url = get_site_url()
+        embed = Embed(title="Terra Nanotech Auth")
 
         try:
             if settings.TNNT_TEMPLATE_ENTITY_ID == 1:
-                embed.set_thumbnail(url=get_site_url + "static/icons/allianceauth.png")
+                aa_icon = f"{auth_url}/static/allianceauth/icons/allianceauth.png"
+                embed.set_thumbnail(url=aa_icon)
             else:
                 if settings.TNNT_TEMPLATE_ENTITY_TYPE == "alliance":
                     embed.set_thumbnail(
-                        url=alliance_logo_url(settings.TNNT_TEMPLATE_ENTITY_ID, 256)
+                        url=alliance_logo_url(
+                            alliance_id=settings.TNNT_TEMPLATE_ENTITY_ID, size=256
+                        )
                     )
                 elif settings.TNNT_TEMPLATE_ENTITY_TYPE == "corporation":
                     embed.set_thumbnail(
-                        url=corporation_logo_url(settings.TNNT_TEMPLATE_ENTITY_ID, 256)
+                        url=corporation_logo_url(
+                            corporation_id=settings.TNNT_TEMPLATE_ENTITY_ID, size=256
+                        )
                     )
         except AttributeError:
             pass
 
         embed.colour = Color.blue()
 
         embed.description = (
             "All authentication functions for this Discord "
-            "server are handled through our Alliance Auth instance."
+            "server are handled through our Auth system."
         )
 
-        auth_url = get_site_url()
-
         embed.add_field(name="Auth Link", value=auth_url, inline=False)
 
         return await ctx.send(embed=embed)
 
     @commands.command(pass_context=True)
     @sender_is_admin()
     async def orphans(self, ctx):
         """
         Returns a list of users on this server, who are unknown to TN-NT Auth
+
+        :param ctx:
+        :type ctx:
+        :return:
+        :rtype:
         """
 
         await ctx.trigger_typing()
         await ctx.send("Searching for Orphaned Discord Users")
         await ctx.trigger_typing()
 
         payload = "The following Users cannot be located in Alliance Auth\n"
@@ -90,15 +104,15 @@
         for member in member_list:
             discord_member_id = member.id
             discord_member_is_bot = member.bot
 
             try:
                 discord_member_exists = DiscordUser.objects.get(uid=discord_member_id)
             except DiscordUser.DoesNotExist as exception:
-                logger.error(exception)
+                logger.error(msg=exception)
                 discord_member_exists = False
 
             if discord_member_exists is not False:
                 # Nothing to do, the user exists. Move on with ur life dude.
                 pass
 
             elif discord_member_is_bot is True:
@@ -109,28 +123,32 @@
                 if len(payload) > 1000:
                     try:
                         await ctx.send(payload)
 
                         payload = (
                             "The following Users cannot be located in Alliance Auth\n"
                         )
-                    except Exception as e:
-                        logger.error(e)
+                    except Exception as exc:
+                        logger.error(msg=exc)
 
                 # keep building the payload
                 payload = payload + member.mention + "\n"
 
         try:
             await ctx.send(payload)
-        except Exception as e:
-            logger.error(e)
+        except Exception as exc:
+            logger.error(msg=exc)
             # await ctx.send(payload[0:1999])
             # await ctx.send("Maximum Discord message length reached")
 
 
 def setup(bot):
     """
-    setup the cog
+    Set up the cog
+
     :param bot:
+    :type bot:
+    :return:
+    :rtype:
     """
 
     bot.add_cog(Auth(bot))
```

### Comparing `tnnt_discordbot_cogs-0.4.0/tnnt_discordbot_cogs/cogs/members.py` & `tnnt_discordbot_cogs-0.5.0/tnnt_discordbot_cogs/cogs/members.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+"""
+"Members" cog for discordbot - https://github.com/pvyParts/allianceauth-discordbot
+"""
+
 # Standard Library
 import logging
 
 # Third Party
 from aadiscordbot.app_settings import (
     ADMIN_DISCORD_BOT_CHANNELS,
     DISCORD_BOT_MEMBER_ALLIANCES,
@@ -35,108 +39,110 @@
     @sender_has_any_perm(
         ["corputils.view_alliance_corpstats", "corpstats.view_alliance_corpstats"]
     )
     @message_in_channels(ADMIN_DISCORD_BOT_CHANNELS)
     async def lookup(self, ctx):
         """
         Gets Auth data about a character
-        Input: a Eve Character Name
+        Input: An Eve Character Name
+
+        :param ctx:
+        :type ctx:
+        :return:
+        :rtype:
         """
 
         input_name = ctx.message.content[8:]
-
         embed = Embed(title=f"Character Lookup {input_name}")
 
         try:
             char = EveCharacter.objects.get(character_name=input_name)
 
             try:
                 main = char.character_ownership.user.profile.main_character
                 state = char.character_ownership.user.profile.state.name
                 groups = char.character_ownership.user.groups.all().values_list(
                     "name", flat=True
                 )
 
                 try:
-                    discord_string = "<@{}>".format(
-                        char.character_ownership.user.discord.uid
-                    )
+                    discord_string = f"<@{char.character_ownership.user.discord.uid}>"
                 except Exception as e:
-                    logger.error(e)
+                    logger.error(msg=e)
                     discord_string = "unknown"
 
                 if aastatistics_active():
-                    alts = (
+                    alt_characters = (
                         char.character_ownership.user.character_ownerships.all()
                         .select_related("character", "character_stats")
                         .values_list(
                             "character__character_name",
                             "character__corporation_ticker",
                             "character__character_id",
                             "character__corporation_id",
                             "character__character_stats__zk_12m",
                             "character__character_stats__zk_3m",
                         )
                     )
                     zk12 = 0
                     zk3 = 0
                 else:
-                    alts = (
+                    alt_characters = (
                         char.character_ownership.user.character_ownerships.all()
                         .select_related("character")
                         .values_list(
                             "character__character_name",
                             "character__corporation_ticker",
                             "character__character_id",
                             "character__corporation_id",
                         )
                     )
                     zk12 = "Not Installed"
                     zk3 = "Not Installed"
 
                 if aastatistics_active():
-                    for alt in alts:
-                        if alt[4]:
-                            zk12 += alt[4]
-                            zk3 += alt[5]
+                    for alt_character in alt_characters:
+                        if alt_character[4]:
+                            zk12 += alt_character[4]
+                            zk3 += alt_character[5]
 
                 embed.colour = Color.blue()
-                embed.description = (
-                    "**{character}** is linked to **{main} "
-                    "[{corp_ticker}]** (State: {state})"
-                ).format(
-                    character=char,
-                    main=main,
-                    corp_ticker=main.corporation_ticker,
-                    state=state,
-                )
 
-                alt_list = [
-                    (
-                        "[{}](https://evewho.com/character/{}) "
-                        "[[{}](https://evewho.com/corporation/{})]"
-                    ).format(a[0], a[2], a[1], a[3])
-                    for a in alts
-                ]
+                if main is None:
+                    embed.description = (
+                        f"**{char}** is not associated with any Auth account …"
+                    )
+                else:
+                    embed.description = (
+                        f"**{char}** is linked to **{main} "
+                        f"[{main.corporation_ticker}]** (State: {state})"
+                    )
+
+                alt_list = []
+                for alt_character in alt_characters:
+                    alt_list.append(
+                        f"[{alt_character[0]}](https://evewho.com/character/{alt_character[2]}) "  # pylint: disable=line-too-long
+                        f"[[{alt_character[1]}](https://evewho.com/corporation/{alt_character[3]})]"  # pylint: disable=line-too-long
+                    )
 
                 for idx, names in enumerate(
                     [alt_list[i : i + 6] for i in range(0, len(alt_list), 6)]
                 ):
                     if idx < 6:
                         embed.add_field(
                             name=f"Linked Characters {idx + 1}",
                             value="\n".join(names),
                             inline=False,
                         )
                     else:
                         embed.add_field(
                             name=(
-                                "Linked Characters {} "
+                                f"Linked Characters {idx} "
                                 "**(Discord Limited There are More)**"
-                            ).format(idx),
+                            ),
                             value="\n".join(names),
                             inline=False,
                         )
                         break
 
                 if len(groups) > 0:
                     embed.add_field(
@@ -156,118 +162,124 @@
                 characters = EveCharacter.objects.filter(
                     ownership_records__user__in=users
                 ).distinct()
                 embed = Embed(title="Character Lookup")
                 embed.colour = Color.blue()
 
                 embed.description = (
-                    "**{}** is unlinked, searching for any "
+                    f"**{char}** is unlinked, searching for any "
                     "characters linked to known users"
-                ).format(char)
+                )
                 user_names = [f"{user.username}" for user in users]
                 embed.add_field(
                     name="Old Users", value="\n".join(user_names), inline=False
                 )
 
-                alt_list = [
-                    (
-                        "[{}](https://evewho.com/character/{}) "
-                        "[[{}](https://evewho.com/corporation/{})]"
-                    ).format(
-                        a.character_name,
-                        a.character_id,
-                        a.corporation_ticker,
-                        a.corporation_id,
+                alt_list = []
+                for character in characters:
+                    alt_list.append(
+                        f"[{character.character_name}](https://evewho.com/character/{character.character_id}) "  # pylint: disable=line-too-long
+                        f"[[{character.corporation_ticker}](https://evewho.com/corporation/{character.corporation_id})]"  # pylint: disable=line-too-long
                     )
-                    for a in characters
-                ]
 
                 for idx, names in enumerate(
                     [alt_list[i : i + 6] for i in range(0, len(alt_list), 6)]
                 ):
                     if idx < 6:
                         embed.add_field(
                             name=f"Found Characters {idx + 1}",
                             value="\n".join(names),
                             inline=False,
                         )
                     else:
                         embed.add_field(
                             name=(
-                                "Found Characters {} "
+                                f"Found Characters {idx} "
                                 "**(Discord Limited There are More)**"
-                            ).format(idx),
+                            ),
                             value="\n".join(names),
                             inline=False,
                         )
                         break
 
                 return await ctx.send(embed=embed)
         except EveCharacter.DoesNotExist:
             embed.colour = Color.red()
 
             embed.description = (
-                "Character **{character_name}** does not exist in our Auth system"
-            ).format(character_name=input_name)
+                f"Character **{input_name}** does not exist in our Auth system"
+            )
 
             return await ctx.send(embed=embed)
 
     @commands.command(pass_context=True)
     @sender_has_any_perm(
         ["corputils.view_alliance_corpstats", "corpstats.view_alliance_corpstats"]
     )
     @message_in_channels(ADMIN_DISCORD_BOT_CHANNELS)
     async def altcorp(self, ctx):
         """
         Gets Auth data about an altcorp
-        Input: a Eve Character Name
+        Input: An Eve Corporation Name
+
+        :param ctx:
+        :type ctx:
+        :return:
+        :rtype:
         """
 
         input_name = ctx.message.content[9:]
         chars = EveCharacter.objects.filter(corporation_name=input_name)
         own_ids = [DISCORD_BOT_MEMBER_ALLIANCES]
         alts_in_corp = []
 
-        for c in chars:
-            if c.alliance_id not in own_ids:
-                alts_in_corp.append(c)
+        for char in chars:
+            if char.alliance_id not in own_ids:
+                alts_in_corp.append(char)
 
         mains = {}
 
-        for a in alts_in_corp:
+        for alt_char in alts_in_corp:
             try:
-                main = a.character_ownership.user.profile.main_character
+                main = alt_char.character_ownership.user.profile.main_character
 
                 if main.character_id not in mains:
                     mains[main.character_id] = [main, 0]
 
                 mains[main.character_id][1] += 1
                 # alt_corp_id = a.corporation_id
             except Exception as e:
-                logger.error(e)
-                pass
+                logger.error(msg=e)
 
         output = []
-        base_string = "[{}]({}) [ [{}]({}) ] has {} alt{}"
+        base_string = "[{}]({}) [[{}]({})] has {} alt{}"
 
-        for k, m in mains.items():
+        for _, main_char in mains.items():
             output.append(
                 base_string.format(
-                    m[0],
-                    evewho.character_url(m[0].character_id),
-                    m[0].corporation_ticker,
-                    evewho.corporation_url(m[0].corporation_id),
-                    m[1],
-                    "s" if m[1] > 1 else "",
+                    main_char[0],
+                    evewho.character_url(main_char[0].character_id),
+                    main_char[0].corporation_ticker,
+                    evewho.corporation_url(main_char[0].corporation_id),
+                    main_char[1],
+                    "s" if main_char[1] > 1 else "",
                 )
             )
 
         for strings in [output[i : i + 10] for i in range(0, len(output), 10)]:
             embed = Embed(title=input_name)
             embed.colour = Color.blue()
             embed.description = "\n".join(strings)
 
             await ctx.send(embed=embed)
 
 
 def setup(bot):
+    """
+    Set up the cog
+
+    :param bot:
+    :type bot:
+    :return:
+    :rtype:
+    """
     bot.add_cog(Members(bot))
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `tnnt_discordbot_cogs-0.4.0/tnnt_discordbot_cogs/cogs/price_check.py` & `tnnt_discordbot_cogs-0.5.0/tnnt_discordbot_cogs/cogs/price_check.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
-Market Price Checks
+Market Price Checks cog for discordbot - https://github.com/pvyParts/allianceauth-discordbot
 """
+
 # Standard Library
 import locale
 import logging
 
 # Third Party
 import requests
 from discord.colour import Color
@@ -27,16 +28,19 @@
     def __init__(self, bot):
         self.bot = bot
 
     @commands.command(pass_context=True)
     async def price(self, ctx):
         """
         Check an item price on all major market hubs
+
         :param ctx:
+        :type ctx:
         :return:
+        :rtype:
         """
 
         markets = [
             {"name": "Jita", "system_id": 30000142},
             {"name": "Amarr", "system_id": 30002187},
             {"name": "Rens", "system_id": 60004588},
             {"name": "Hek", "system_id": 60005686},
@@ -49,57 +53,63 @@
 
         await self.price_check(ctx=ctx, markets=markets, item_name=item_name)
 
     @commands.command(pass_context=True)
     async def jita(self, ctx):
         """
         Check an item price on Jita market
+
         :param ctx:
+        :type ctx:
         :return:
+        :rtype:
         """
 
-        markets = [
-            {"name": "Jita", "system_id": 30000142},
-        ]
+        markets = [{"name": "Jita", "system_id": 30000142}]
 
         await ctx.trigger_typing()
 
         item_name = ctx.message.content[6:]
 
         await self.price_check(ctx=ctx, markets=markets, item_name=item_name)
 
     @commands.command(pass_context=True)
     async def amarr(self, ctx):
         """
         Check an item price on Amarr market
+
         :param ctx:
+        :type ctx:
         :return:
+        :rtype:
         """
 
-        markets = [
-            {"name": "Amarr", "system_id": 60008494},
-        ]
+        markets = [{"name": "Amarr", "system_id": 60008494}]
 
         await ctx.trigger_typing()
 
         item_name = ctx.message.content[7:]
 
         await self.price_check(ctx=ctx, markets=markets, item_name=item_name)
 
     async def price_check(self, ctx, markets, item_name: str = None):
         """
         Do the price checks and post to Discord
+
         :param ctx:
+        :type ctx:
         :param markets:
+        :type markets:
         :param item_name:
+        :type item_name:
         :return:
+        :rtype:
         """
 
         has_thumbnail = False
-        eve_type_id = None
 
         await ctx.trigger_typing()
 
         if item_name != "":
             try:
                 eve_type = (
                     EveEntity.objects.fetch_by_names_esi([item_name])
@@ -153,49 +163,48 @@
                             f"{self.imageserver_url}/types/{eve_type_id}/icon?size=64"
                         )
 
                         if has_thumbnail is False:
                             embed.set_thumbnail(url=thumbnail_url)
                             has_thumbnail = True
 
-                        # locale.setlocale(locale.LC_ALL, "de_DE.UTF-8")
-                        locale.setlocale(locale.LC_ALL, "")
+                        locale.setlocale(category=locale.LC_ALL, locale="")
 
                         # Sell order price
                         market_min_sell_order_price = locale.format_string(
-                            "%.2f", float(sell_min), grouping=True
+                            f="%.2f", val=float(sell_min), grouping=True
                         )
 
                         if sell_order_count == 0:
                             market_min_sell_order_price = "No sell orders found"
 
                         embed.add_field(
                             name=f"Sell Order Price ({sell_order_count} Orders)",
                             value=f"{market_min_sell_order_price} ISK",
                             inline=True,
                         )
 
                         # Buy order price
                         market_max_buy_order_price = locale.format_string(
-                            "%.2f", float(buy_max), grouping=True
+                            f="%.2f", val=float(buy_max), grouping=True
                         )
 
                         if buy_order_count == 0:
                             market_max_buy_order_price = "No buy orders found"
 
                         embed.add_field(
                             name=f"Buy Order Price ({buy_order_count} Orders)",
                             value=f"{market_max_buy_order_price} ISK",
                             inline=True,
                         )
                     else:
                         embed.add_field(
                             name="API Error",
                             value=(
-                                f"Could not not fetch the price "
+                                "Could not not fetch the price "
                                 f'for the {market["name"]} market.'
                             ),
                             inline=False,
                         )
         else:
             embed = Embed(
                 title="Price Lookup",
@@ -211,13 +220,16 @@
             )
 
         return await ctx.send(embed=embed)
 
 
 def setup(bot):
     """
-    Add the cogg
+    Set up the cogg
+
     :param bot:
+    :type bot:
     :return:
+    :rtype:
     """
 
     bot.add_cog(PriceCheck(bot))
```

### Comparing `tnnt_discordbot_cogs-0.4.0/tnnt_discordbot_cogs/cogs/timers.py` & `tnnt_discordbot_cogs-0.5.0/tnnt_discordbot_cogs/cogs/timers.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 """
-All about the timers ....
+All about the timers …
 """
 
 # Standard Library
 import datetime
 import logging
 
 # Third Party
-from aadiscordbot.app_settings import ADMIN_DISCORD_BOT_CHANNELS, get_site_url
+from aadiscordbot.app_settings import ADMIN_DISCORD_BOT_CHANNELS
 from aadiscordbot.cogs.utils.decorators import message_in_channels
 from discord.colour import Color
 from discord.embeds import Embed
 from discord.ext import commands
 from structuretimers.models import Timer
 
 # Django
 from django.apps import apps
 from django.utils import timezone
 
 # Alliance Auth
 from allianceauth.eveonline.templatetags.evelinks import dotlan_solar_system_url
 
+# Alliance Auth (External Libs)
+from app_utils.urls import reverse_absolute
+
 logger = logging.getLogger(__name__)
 
 
 def structuretimers_active():
     """
     Check if "structuretimers" is installed
     :return:
@@ -40,29 +43,49 @@
     :return:
     :rtype:
     """
 
     return apps.is_installed("timezones")
 
 
+def add_empty_line(embed: Embed) -> None:
+    """
+    Adding an empty line to the embed
+
+    :param embed:
+    :type embed:
+    :return:
+    :rtype:
+    """
+
+    embed.add_field(
+        name="\u200b",
+        value="\u200b",
+        inline=False,
+    )
+
+
 class Timers(commands.Cog):
     """
     TimerBoard Stuffs!
     """
 
     def __init__(self, bot):
         self.bot = bot
 
     @commands.command(pass_context=True)
     @message_in_channels(ADMIN_DISCORD_BOT_CHANNELS)
     async def timer(self, ctx):
         """
         Gets the Next Timer!
+
         :param ctx:
+        :type ctx:
         :return:
+        :rtype:
         """
 
         embed = Embed(title="Next Timer")
 
         next_timer = Timer.objects.filter(
             is_opsec=False,
             visibility=Timer.VISIBILITY_UNRESTRICTED,
@@ -77,15 +100,15 @@
             elif next_timer.objective == Timer.OBJECTIVE_HOSTILE:
                 embed.colour = Color.red()
             elif next_timer.objective == Timer.OBJECTIVE_NEUTRAL:
                 embed.colour = Color.light_gray()
             elif next_timer.objective == Timer.OBJECTIVE_UNDEFINED:
                 embed.colour = Color.dark_gray()
             else:
-                embed.colour = Color.from_rgb(255, 255, 255)
+                embed.colour = Color.from_rgb(r=255, g=255, b=255)
 
             user_has_profile = True
 
             if next_timer.user is not None:
                 creator_name = next_timer.user.username
 
                 try:
@@ -93,62 +116,67 @@
                 except Exception:
                     user_has_profile = False
 
                 if user_has_profile is True:
                     if creator_profile.main_character is not None:
                         creator_name = creator_profile.main_character.character_name
 
-                embed.set_footer(
-                    text="Timer added by {creator_name}".format(
-                        creator_name=creator_name
-                    )
-                )
+                embed.set_footer(text=f"Timer added by {creator_name}")
 
             embed.add_field(name="Structure:", value=next_timer.structure_type.name)
 
+            solar_system_name = next_timer.eve_solar_system.name
+            solar_system_link = dotlan_solar_system_url(next_timer.eve_solar_system)
+            solar_system_md_link = f"[{solar_system_name}]({solar_system_link})"
+            location_details = next_timer.location_details
+
             embed.add_field(
-                name="Location:",
-                value="{system}\n{location}".format(
-                    system="[{solar_system_name}]({solar_system_link})".format(
-                        solar_system_name=next_timer.eve_solar_system.name,
-                        solar_system_link=dotlan_solar_system_url(
-                            next_timer.eve_solar_system
-                        ),
-                    ),
-                    location=next_timer.location_details,
-                ),
+                name="Location:", value=f"{solar_system_md_link}\n{location_details}"
             )
 
+            add_empty_line(embed=embed)
+
+            timer_timestamp = str(int(next_timer.date.timestamp()))
+
             if timezones_active():
+                timezones_url = reverse_absolute(
+                    viewname="timezones:index",
+                    args=[timer_timestamp],
+                )
+                timezones_md_link = f"[TZ Conversion]({timezones_url})"
+                timer_eve_time = next_timer.date.strftime("%Y-%m-%d %H:%M")
+
                 embed.add_field(
                     name="Eve Time:",
-                    value="{eve_time} ({tz_link})".format(
-                        eve_time=next_timer.date.strftime("%Y-%m-%d %H:%M"),
-                        tz_link="[{tz_lnk_text}]({tz_link_url}/)".format(
-                            tz_lnk_text="Time Zone Conversion",
-                            tz_link_url=get_site_url()
-                            + "/timezones/"
-                            + str(int(next_timer.date.timestamp())),
-                        ),
-                    ),
-                    inline=False,
+                    value=f"{timer_eve_time} ({timezones_md_link})",
+                    inline=True,
                 )
             else:
                 embed.add_field(
                     name="Eve Time:",
                     value=next_timer.eve_time.strftime("%Y-%m-%d %H:%M"),
-                    inline=False,
+                    inline=True,
                 )
 
+            embed.add_field(
+                name="Local Time:",
+                value=f"<t:{timer_timestamp}:F>",
+                inline=True,
+            )
+
         return await ctx.send(embed=embed)
 
 
 def setup(bot):
     """
-    Setup the cog
+    Set up the cog
+
     :param bot:
+    :type bot:
+    :return:
+    :rtype:
     """
 
     if structuretimers_active():
         bot.add_cog(Timers(bot))
     else:
         logger.debug("Timerboard not installed")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `tnnt_discordbot_cogs-0.4.0/LICENSE` & `tnnt_discordbot_cogs-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tnnt_discordbot_cogs-0.4.0/README.md` & `tnnt_discordbot_cogs-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `tnnt_discordbot_cogs-0.4.0/pyproject.toml` & `tnnt_discordbot_cogs-0.5.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "tnnt-discordbot-cogs"
-version = "0.4.0"
+version = "0.5.0"
 description = "TN-NT customized cogs for aa-discordbot"
 readme = "README.md"
 license = "GPL-3.0"
 requires-python = "~=3.8"
 authors = [
     { name = "Peter Pfeufer", email = "develop@ppfeufer.de" },
 ]
@@ -31,16 +31,17 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Internet :: WWW/HTTP",
     "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
 ]
 dependencies = [
-    "allianceauth-discordbot",
     "allianceauth>=3.0.0",
+    "allianceauth-discordbot",
+    "allianceauth-app-utils>=1.14.1",
     "django-eveuniverse>=1.3.0",
 ]
 
 [project.urls]
 Homepage = "https://github.com/terra-nanotech/tn-nt-discordbot-cogs"
 Documentation = "https://github.com/terra-nanotech/tn-nt-discordbot-cogs/blob/master/README.md"
 Source = "https://github.com/terra-nanotech/tn-nt-discordbot-cogs.git"
```

### Comparing `tnnt_discordbot_cogs-0.4.0/PKG-INFO` & `tnnt_discordbot_cogs-0.5.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tnnt-discordbot-cogs
-Version: 0.4.0
+Version: 0.5.0
 Summary: TN-NT customized cogs for aa-discordbot
 Project-URL: Homepage, https://github.com/terra-nanotech/tn-nt-discordbot-cogs
 Project-URL: Documentation, https://github.com/terra-nanotech/tn-nt-discordbot-cogs/blob/master/README.md
 Project-URL: Source, https://github.com/terra-nanotech/tn-nt-discordbot-cogs.git
 Project-URL: Changelog, https://github.com/terra-nanotech/tn-nt-discordbot-cogs/blob/master/CHANGELOG.md
 Project-URL: Tracker, https://github.com/terra-nanotech/tn-nt-discordbot-cogs/issues
 Author-email: Peter Pfeufer <develop@ppfeufer.de>
@@ -22,14 +22,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: ~=3.8
+Requires-Dist: allianceauth-app-utils>=1.14.1
 Requires-Dist: allianceauth-discordbot
 Requires-Dist: allianceauth>=3.0.0
 Requires-Dist: django-eveuniverse>=1.3.0
 Description-Content-Type: text/markdown
 
 # Terra Nanotech Discordbot Cogs
```

