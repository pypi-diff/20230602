# Comparing `tmp/discordLevelingSystem-1.2.0.tar.gz` & `tmp/discordLevelingSystem-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discordLevelingSystem-1.2.0.tar", last modified: Mon Aug 22 10:28:54 2022, max compression
+gzip compressed data, was "discordLevelingSystem-1.2.1.tar", last modified: Fri Jun  2 14:57:50 2023, max compression
```

## Comparing `discordLevelingSystem-1.2.0.tar` & `discordLevelingSystem-1.2.1.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxrwxrwx   0        0        0        0 2022-08-22 10:28:54.529590 discordLevelingSystem-1.2.0/
--rw-rw-rw-   0        0        0     1099 2021-08-24 22:55:36.000000 discordLevelingSystem-1.2.0/LICENSE
--rw-rw-rw-   0        0        0    49168 2022-08-22 10:28:54.528594 discordLevelingSystem-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0    48125 2022-08-22 10:28:08.000000 discordLevelingSystem-1.2.0/README.md
-drwxrwxrwx   0        0        0        0 2022-08-22 10:28:54.519616 discordLevelingSystem-1.2.0/discordLevelingSystem/
--rw-rw-rw-   0        0        0      598 2022-08-22 09:07:43.000000 discordLevelingSystem-1.2.0/discordLevelingSystem/__init__.py
--rw-rw-rw-   0        0        0    12223 2022-08-22 09:52:55.000000 discordLevelingSystem-1.2.0/discordLevelingSystem/announcement.py
--rw-rw-rw-   0        0        0     4861 2022-08-22 09:07:43.000000 discordLevelingSystem-1.2.0/discordLevelingSystem/decorators.py
--rw-rw-rw-   0        0        0     3632 2021-08-24 22:55:36.000000 discordLevelingSystem-1.2.0/discordLevelingSystem/errors.py
--rw-rw-rw-   0        0        0    95454 2022-08-22 09:39:28.000000 discordLevelingSystem-1.2.0/discordLevelingSystem/leveling_system.py
--rw-rw-rw-   0        0        0     3894 2022-08-22 09:39:28.000000 discordLevelingSystem-1.2.0/discordLevelingSystem/levels_xp_needed.py
--rw-rw-rw-   0        0        0     2845 2022-08-22 09:46:59.000000 discordLevelingSystem-1.2.0/discordLevelingSystem/member_data.py
--rw-rw-rw-   0        0        0     6624 2022-08-22 09:07:43.000000 discordLevelingSystem-1.2.0/discordLevelingSystem/role_awards.py
-drwxrwxrwx   0        0        0        0 2022-08-22 10:28:54.526599 discordLevelingSystem-1.2.0/discordLevelingSystem.egg-info/
--rw-rw-rw-   0        0        0    49168 2022-08-22 10:28:54.000000 discordLevelingSystem-1.2.0/discordLevelingSystem.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      547 2022-08-22 10:28:54.000000 discordLevelingSystem-1.2.0/discordLevelingSystem.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-08-22 10:28:54.000000 discordLevelingSystem-1.2.0/discordLevelingSystem.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2022-08-22 10:28:54.000000 discordLevelingSystem-1.2.0/discordLevelingSystem.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2022-08-22 10:28:54.000000 discordLevelingSystem-1.2.0/discordLevelingSystem.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-08-22 10:28:54.529590 discordLevelingSystem-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0     2637 2022-08-22 10:00:31.000000 discordLevelingSystem-1.2.0/setup.py
+drwxr-xr-x   0 jaggenneil   (501) staff       (20)        0 2023-06-02 14:57:50.710412 discordLevelingSystem-1.2.1/
+-rw-r--r--   0 jaggenneil   (501) staff       (20)     1079 2022-08-05 07:18:15.000000 discordLevelingSystem-1.2.1/LICENSE
+-rw-r--r--   0 jaggenneil   (501) staff       (20)    48695 2023-06-02 14:57:50.710263 discordLevelingSystem-1.2.1/PKG-INFO
+-rw-r--r--   0 jaggenneil   (501) staff       (20)    47636 2022-09-27 10:31:34.000000 discordLevelingSystem-1.2.1/README.md
+drwxr-xr-x   0 jaggenneil   (501) staff       (20)        0 2023-06-02 14:57:50.708953 discordLevelingSystem-1.2.1/discordLevelingSystem/
+-rw-r--r--   0 jaggenneil   (501) staff       (20)      575 2022-09-27 10:43:24.000000 discordLevelingSystem-1.2.1/discordLevelingSystem/__init__.py
+-rw-r--r--   0 jaggenneil   (501) staff       (20)    11960 2022-08-19 15:22:51.000000 discordLevelingSystem-1.2.1/discordLevelingSystem/announcement.py
+-rw-r--r--   0 jaggenneil   (501) staff       (20)     4754 2022-08-19 15:04:35.000000 discordLevelingSystem-1.2.1/discordLevelingSystem/decorators.py
+-rw-r--r--   0 jaggenneil   (501) staff       (20)     3564 2022-09-27 10:43:24.000000 discordLevelingSystem-1.2.1/discordLevelingSystem/errors.py
+-rw-r--r--   0 jaggenneil   (501) staff       (20)    93498 2023-06-02 13:37:20.000000 discordLevelingSystem-1.2.1/discordLevelingSystem/leveling_system.py
+-rw-r--r--   0 jaggenneil   (501) staff       (20)     3735 2022-08-05 07:18:15.000000 discordLevelingSystem-1.2.1/discordLevelingSystem/levels_xp_needed.py
+-rw-r--r--   0 jaggenneil   (501) staff       (20)     2768 2022-08-05 07:18:15.000000 discordLevelingSystem-1.2.1/discordLevelingSystem/member_data.py
+-rw-r--r--   0 jaggenneil   (501) staff       (20)     6485 2022-08-19 15:10:26.000000 discordLevelingSystem-1.2.1/discordLevelingSystem/role_awards.py
+drwxr-xr-x   0 jaggenneil   (501) staff       (20)        0 2023-06-02 14:57:50.709936 discordLevelingSystem-1.2.1/discordLevelingSystem.egg-info/
+-rw-r--r--   0 jaggenneil   (501) staff       (20)    48695 2023-06-02 14:57:50.000000 discordLevelingSystem-1.2.1/discordLevelingSystem.egg-info/PKG-INFO
+-rw-r--r--   0 jaggenneil   (501) staff       (20)      562 2023-06-02 14:57:50.000000 discordLevelingSystem-1.2.1/discordLevelingSystem.egg-info/SOURCES.txt
+-rw-r--r--   0 jaggenneil   (501) staff       (20)        1 2023-06-02 14:57:50.000000 discordLevelingSystem-1.2.1/discordLevelingSystem.egg-info/dependency_links.txt
+-rw-r--r--   0 jaggenneil   (501) staff       (20)       36 2023-06-02 14:57:50.000000 discordLevelingSystem-1.2.1/discordLevelingSystem.egg-info/requires.txt
+-rw-r--r--   0 jaggenneil   (501) staff       (20)       22 2023-06-02 14:57:50.000000 discordLevelingSystem-1.2.1/discordLevelingSystem.egg-info/top_level.txt
+-rw-r--r--   0 jaggenneil   (501) staff       (20)     1369 2023-06-02 14:55:31.000000 discordLevelingSystem-1.2.1/pyproject.toml
+-rw-r--r--   0 jaggenneil   (501) staff       (20)       38 2023-06-02 14:57:50.710452 discordLevelingSystem-1.2.1/setup.cfg
+-rw-r--r--   0 jaggenneil   (501) staff       (20)       69 2023-06-02 14:25:17.000000 discordLevelingSystem-1.2.1/setup.py
```

### Comparing `discordLevelingSystem-1.2.0/LICENSE` & `discordLevelingSystem-1.2.1/LICENSE`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2021-present Defxult#8269
-
-Permission is hereby granted, free of charge, to any person obtaining a
-copy of this software and associated documentation files (the "Software"),
-to deal in the Software without restriction, including without limitation
-the rights to use, copy, modify, merge, publish, distribute, sublicense,
-and/or sell copies of the Software, and to permit persons to whom the
-Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in
-all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS
-OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER 
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING 
-FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER 
+MIT License
+
+Copyright (c) 2021-present Defxult#8269
+
+Permission is hereby granted, free of charge, to any person obtaining a
+copy of this software and associated documentation files (the "Software"),
+to deal in the Software without restriction, including without limitation
+the rights to use, copy, modify, merge, publish, distribute, sublicense,
+and/or sell copies of the Software, and to permit persons to whom the
+Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in
+all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS
+OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER 
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING 
+FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER 
 DEALINGS IN THE SOFTWARE.
```

### Comparing `discordLevelingSystem-1.2.0/PKG-INFO` & `discordLevelingSystem-1.2.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,856 +1,841 @@
-Metadata-Version: 2.1
-Name: discordLevelingSystem
-Version: 1.2.0
-Summary: A library to implement a leveling system into a discord bot. Contains features such as XP, level, ranks, and role awards.
-Home-page: https://github.com/Defxult/discordLevelingSystem
-Author: Defxult#8269
-License: MIT
-Project-URL: Changelog, https://github.com/Defxult/discordLevelingSystem/blob/main/CHANGELOG.md
-Keywords: database,discord,discord bot,discord.py,discord py,discord level,discord leveling,discord leveling system,level,levels,leveling,level up,level system,mee6,rank,ranking,role award,xp
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-A library to implement a leveling system into a discord bot. One of the most popular discord bots out there is MEE6 and it's leveling system. This library provides ways to easily implement one for yourself. It uses SQLite (aiosqlite) to locally query things such as their XP, rank, and level. Various amounts of other methods and classes are also provided so you can access or remove contents from the database file.
-
-<!-- ## Installing
-You can install the latest [PyPI version](https://pypi.org/project/discordLevelingSystem/) of the library by doing:
-
-`$ pip install discordLevelingSystem`
-
-Or the development version:
-
-`$ pip install git+https://github.com/Defxult/discordLevelingSystem` -->
-
----
-
-## Showcase
-![showcase](https://cdn.discordapp.com/attachments/655186216060321816/835010159092039680/leveling_showcase.gif)
-
----
-## How to import
-```py
-from discordLevelingSystem import DiscordLevelingSystem, LevelUpAnnouncement, RoleAward
-```
-
----
-## Intents
-[Intents](https://discordpy.readthedocs.io/en/stable/intents.html) are required for proper functionality
-```py
-bot = commands.Bot(..., intents=discord.Intents(messages=True, guilds=True, members=True))
-```
----
-
-
-## DiscordLevelingSystem
-```class DiscordLevelingSystem(rate=1, per=60.0, awards=None, **kwargs)```
-
----
-### Parameters of the DiscordLevelingSystem constructor
-* `rate` (`int`) The amount of messages each member can send before the cooldown triggers
-* `per` (`float`) The amount of seconds each member has to wait before gaining more XP, aka the cooldown
-* `awards` (`Optional[Dict[int, List[RoleAward]]]`) The role given to a member when they reach a `RoleAward` level requirement
----
-### Kwargs of the DiscordLevelingSystem constructor
-| Name | Type | Default Value | Info
-|------|------|---------------|-----
-| `no_xp_roles` | `Sequence[int]` | `None` | A sequence of role ID's. Any member with any of those roles will not gain XP when sending messages
-| `no_xp_channels` | `Sequence[int]` | `None` | A sequence of text channel ID's. Any member sending messages in any of those text channels will not gain XP
-| `announce_level_up` | `bool` | `True` | If `True`, level up messages will be sent when a member levels up
-| `stack_awards` | `bool` | `True` | If this is `True`, when the member levels up the assigned role award will be applied. If `False`, the previous role award will be removed and the level up assigned role will also be applied
-| `level_up_announcement` | `Union[LevelUpAnnouncement, Sequence[LevelUpAnnouncement]]` | `LevelUpAnnouncement()` | The message that is sent when someone levels up. If this is a sequence of `LevelUpAnnouncement`, one is selected at random
-|`bot` | ` Union[AutoShardedBot, Bot]` | `None` | Your bot instance variable. Used only if you'd like to use the `on_dls_level_up` event
-
----
-### Attributes
-* `no_xp_roles`
-* `no_xp_channels`
-* `announce_level_up`
-* `stack_awards`
-* `level_up_announcement`
-* `bot`
-* `rate` (`int`) Read only property from the constructor
-* `per` (`float`) Read only property from the constructor
-* `database_file_path` (`str`) Read only property
-* `active` (`bool`) Enable/disable the leveling system. If `False`, nobody can gain XP when sending messages unless this is set back to `True`
-
-> NOTE: All attributes can be set during initialization
----
-## Initial Setup
-When setting up the leveling system, a database file needs to be created in order for the library to function. 
-* Associated static method
-  * `DiscordLevelingSystem.create_database_file(path: str)`
-
-The above static method is used to create the database file for you in the path you specify. This method only needs to be called once. Example:
-```py
-DiscordLevelingSystem.create_database_file(r'C:\Users\Defxult\Documents')
-```
-Once created, there is no need to ever run that method again unless you want to create a new database file from scratch. Now that you have the database file, you can use the leveling system.
-
----
-## Connecting to the Database
-* Associated method
-  * `DiscordLevelingSystem.connect_to_database_file(path: str)`
-
-Since the database file has already been created, all you need to do is connect to it. 
-> NOTE: When connecting to the database file, the event loop must not be running
-<div align="left"><sub>EXAMPLE</sub></div>
-
-```py
-from discord.ext import commands
-from discordLevelingSystem import DiscordLevelingSystem
-
-bot = commands.Bot(...)
-lvl = DiscordLevelingSystem()
-lvl.connect_to_database_file(r'C:\Users\Defxult\Documents\DiscordLevelingSystem.db')
-
-bot.run(...)
-```
----
-
-## RoleAward
-```class RoleAward(role_id: int, level_requirement: int, role_name=None)```
-
-You can assign roles to the system so when someone levels up to a certain level, they are given that role. `RoleAward` is how that is accomplished.
-
----
-### Parameters of the RoleAward constructor
-* `role_id` (`int`) ID of the role that is to be awarded.
-* `level_requirement` (`int`) What level is required for a member to be awarded the role.
-* `role_name` (`Optional[str]`) A name you can set for the award. Nothing is done with this value, it is used for visual identification purposes only.
----
-### Attributes
-* `role_id`
-* `level_requirement`
-* `role_name`
-* `mention` (`str`) The discord role mention string
-
-When creating role awards, all role IDs and level requirements must be unique. Level requirements must also be in ascending order. It is also possible to assign different role awards for different guilds. If you don't want any role awards, set the `awards` parameter to `None`. When setting `awards`, it accepts a `dict` where the keys are guild IDs and the values are a `list` of `RoleAward`
-<div align="left"><sub>EXAMPLE</sub></div>
-
-```py
-from discordLevelingSystem import DiscordLevelingSystem, RoleAward
-
-johns_server = 587937522043060224
-janes_server = 850809412011950121
-
-my_awards = {
-    johns_server : [
-        RoleAward(role_id=831672678586777601, level_requirement=1, role_name='Rookie'),
-        RoleAward(role_id=831672730583171073, level_requirement=2, role_name='Associate'),
-        RoleAward(role_id=831672814419050526, level_requirement=3, role_name='Legend')
-    ],
-    janes_server : [
-        RoleAward(role_id=851400453904400385, level_requirement=1, role_name='Silver'),
-        RoleAward(role_id=851379776111116329, level_requirement=2, role_name='Gold'),
-        RoleAward(role_id=851959077071880202, level_requirement=3, role_name='Diamond')
-    ]
-}
-
-lvl = DiscordLevelingSystem(..., awards=my_awards)
-```
----
-
-## LevelUpAnnouncement
-```class LevelUpAnnouncement(message=default_message, level_up_channel_ids=None, allowed_mentions=default_mentions, tts=False, delete_after=None)```
-
-Level up announcements are for when you want to implement your own level up messages. It provides access to who leveled up, their rank, level and much more. It also uses some of discord.py's kwargs from it's `Messageable.send` such as `allowed_mentions`, `tts`, and `delete_after` to give you more control over the sent message.
-
----
-### Parameters of the LevelUpAnnouncement constructor
-
-* `message` (`Union[str, discord.Embed]`) The message that is sent when someone levels up. Defaults to `"<mention>, you are now **level <level>!**"`
-
-* `level_up_channel_ids` (`Optional[Sequence[int]]`) The text channel IDs where all level up messages will be sent for each server. If `None`, the level up message will be sent in the channel where they sent the message (example below).
-
-* `allowed_mentions` (`discord.AllowedMentions`) Used to determine who can be pinged in the level up message. Defaults to `discord.AllowedMentions(everyone=False, users=True, roles=False, replied_user=False)`
-
-* `tts` (`bool`) When the level up message is sent, have discord read the level up message aloud.
-
-* `delete_after` (`Optional[float]`) Delete the level up message after an x amount of seconds.
-
-### Class Attributes
-The `LevelUpAnnouncement` class provides a set of markdown attributes for you to use so you can access certain information in a level up message.
-
-* `LevelUpAnnouncement.TOTAL_XP` The members current total XP amount
-* `LevelUpAnnouncement.LEVEL` The members current level
-* `LevelUpAnnouncement.RANK` The members current rank
-
-The below markdown attributes takes the information from a `discord.Member` object so you can access member information in the level up message.
-
-* `LevelUpAnnouncement.Member.avatar_url`
-* `LevelUpAnnouncement.Member.banner_url`
-* `LevelUpAnnouncement.Member.created_at`
-* `LevelUpAnnouncement.Member.default_avatar_url`
-* `LevelUpAnnouncement.Member.discriminator`
-* `LevelUpAnnouncement.Member.display_avatar_url`
-* `LevelUpAnnouncement.Member.display_name`
-* `LevelUpAnnouncement.Member.id`
-* `LevelUpAnnouncement.Member.joined_at`
-* `LevelUpAnnouncement.Member.mention`
-* `LevelUpAnnouncement.Member.name`
-* `LevelUpAnnouncement.Member.nick`
-* `LevelUpAnnouncement.Member.Guild.icon_url`
-* `LevelUpAnnouncement.Member.Guild.id`
-* `LevelUpAnnouncement.Member.Guild.name`
-
-<div align="left"><sub>EXAMPLE</sub></div>
-
-```py
-from discordLevelingSystem import DiscordLevelingSystem, LevelUpAnnouncement
-
-embed = discord.Embed()
-embed.set_author(name=LevelUpAnnouncement.Member.name, icon_url=LevelUpAnnouncement.Member.avatar_url)
-embed.description = f'Congrats {LevelUpAnnouncement.Member.mention}! You are now level {LevelUpAnnouncement.LEVEL} 😎'
-
-announcement = LevelUpAnnouncement(embed)
-
-lvl = DiscordLevelingSystem(..., level_up_announcement=announcement)
-
-# NOTE: You can have multiple level up announcements by setting the parameter to a sequence of LevelUpAnnouncement
-lvl = DiscordLevelingSystem(..., level_up_announcement=[announcement_1, announcement_2, ...])
-```
-When it comes to `level_up_channel_ids`, you can set a designated channel for each server. If you don't set a level up channel ID for a specific server, the level up message will be sent in the channel where the member leveled up. You don't have to specify a level up channel ID for each server unless you'd like to.
-```py
-johns_bot_commands = 489374746737648734 # text channel ID from server A
-janes_levelup_channel = 58498304930493094 # text channel ID from server B
-
-announcement = LevelUpAnnouncement(..., level_up_channel_ids=[johns_bot_commands, janes_levelup_channel])
-lvl = DiscordLevelingSystem(..., level_up_announcement=announcement)
-```
----
-## Handling XP
-Method `award_xp` is how members gain XP. This method is placed inside the `on_message` event of your bot. Members will gain XP if they send a message and if they're *not* on cooldown. Spamming messages will not give them XP.
-> NOTE: Members cannot gain XP in DM's
-* Associated methods
-  * `await DiscordLevelingSystem.add_xp(member: Member, amount: int)`
-  * `await DiscordLevelingSystem.remove_xp(member: Member, amount: int)`
-  * `await DiscordLevelingSystem.set_level(member: Member, level: int)`
-  * `await DiscordLevelingSystem.award_xp(*, amount=[15, 25], message: Message, refresh_name=True, **kwargs)`
-
-
-### Parameters for award_xp
-* `amount` (`Union[int, Sequence[int]]`) The amount of XP to award to the member per message. Must be from 1-25. Can be a sequence with a minimum and maximum length of two. If `amount` is a sequence of two integers, it will randomly pick a number in between those numbers including the numbers provided.
-* `message` (`discord.Message`) A discord message object
-* `refresh_name` (`bool`) Everytime the member sends a message, check if their name still matches the name in the database. If it doesn't match, update the database to match their current name. It is suggested to leave this as `True` so the database can always have the most up-to-date record.
-
-### Kwargs for award_xp
-* `bonus` (`DiscordLevelingSystem.Bonus`) Used to set the roles that will be awarded bonus XP.
-  * `class Bonus(role_ids: Sequence[int], bonus_amount: int, multiply: bool)`
-  * **Parameters of the DiscordLevelingSystem.Bonus constructor**
-    * `role_ids` (`Sequence[int]`) The role(s) a member must have to be able to get bonus XP. They only need to have one of these roles to get the bonus
-    * `bonus_amount` (`int`) Amount of extra XP to be awarded
-    * `multiply` (`bool`) If set to `True`, this will operate on a x2, x3 basis. Meaning if you have the awarded XP amount set to 10 and you want the bonus XP role to be awarded 20, it must be set to 2, not 10. If `False`, it operates purely on the given value. Meaning if you have the awarded XP set to 10 and you want the bonus XP role to be awarded 20, it must be set to 10.
-
-<div align="left"><sub>EXAMPLE</sub></div>
-
-```py
-lvl = DiscordLevelingSystem(...)
-
-nitro_booster = 851379776111116329
-associate_role = 851400453904400385
-
-@bot.event
-async def on_message(message):
-    await lvl.award_xp(amount=[15, 25], message=message, bonus=DiscordLevelingSystem.Bonus([nitro_booster, associate_role], 20, multiply=False))
-```
----
-
-## MemberData
-Accessing the raw information inside the database file can look a bit messy if you don't know exactly what you're looking at. To make things easier, this library comes with the `MemberData` class. A class which returns information about a specific member in the database.
-
-* Associated methods
-  * `await DiscordLevelingSystem.get_data_for(member: Member) -> MemberData`
-  * `await DiscordLevelingSystem.each_member_data(guild: Guild, sort_by=None, limit=None) -> List[MemberData]`
-
-### Attributes
-* `id_number` (`int`) The members ID
-* `name` (`str`) The members name
-* `level` (`int`) The members level
-* `xp` (`int`) The members xp
-* `total_xp` (`int`) The members total xp
-* `rank` (`Optional[int]`) The members rank
-* `mention` (`str`) The discord member mention string
-
-### Methods
-* `MemberData.to_dict() -> dict`
-
-<div align="left"><sub>EXAMPLE</sub></div>
-
-```py
-lvl = DiscordLevelingSystem(...)
-
-@bot.command()
-async def rank(ctx):
-    data = await lvl.get_data_for(ctx.author)
-    await ctx.send(f'You are level {data.level} and your rank is {data.rank}')
-
-@bot.command()
-async def leaderboard(ctx):
-    data = await lvl.each_member_data(ctx.guild, sort_by='rank')
-    # show the leaderboard whichever way you'd like
-```
----
-## Events
-You can set an event to be called when a member levels up. Using the event is considered as an enhanced `LevelUpAnnouncement` because it provides more capabilities rather than simply sending a message with only text/an embed. The `on_dls_level_up` event takes three parameters:
-* `member` (`discord.Member`) The member that leveled up
-* `message` (`discord.Message`) The message that triggered the level up
-* `data` (`MemberData`) The database information for that member
-
-```py
-bot = commands.Bot(...)
-lvl = DiscordLevelingSystem(..., bot=bot) # your bot instance variable is needed
-
-@bot.event
-async def on_dls_level_up(member: discord.Member, message: discord.Message, data: MemberData):
-    # You can do a lot more here compared to LevelUpAnnouncement
-    # - create a level up image and send it with discord.File
-    # - call additional functions that you may need
-    # - access to all attributes/methods that are available within discord.Member and discord.Message
-```
-> NOTE: `LevelUpAnnouncement` and `on_dls_level_up` are not the same. Level up messages are sent by default by the library. If you'd like to only use `on_dls_level_up`, you need to disable level up announcements (`lvl.announce_level_up = False`)
-
----
-## Full Example
-With all classes and core methods introduced, here is a basic implementation of this library.
-```py
-from discord.ext import commands
-from discordLevelingSystem import DiscordLevelingSystem, RoleAward, LevelUpAnnouncement
-
-bot = commands.Bot(...)
-
-main_guild_id = 850809412011950121
-
-my_awards = {
-    main_guild_id : [
-        RoleAward(role_id=831672678586777601, level_requirement=1, role_name='Rookie'),
-        RoleAward(role_id=831672730583171073, level_requirement=2, role_name='Associate'),
-        RoleAward(role_id=831672814419050526, level_requirement=3, role_name='Legend')
-    ]
-}
-
-announcement = LevelUpAnnouncement(f'{LevelUpAnnouncement.Member.mention} just leveled up to level {LevelUpAnnouncement.LEVEL} 😎')
-
-# DiscordLevelingSystem.create_database_file(r'C:\Users\Defxult\Documents') database file already created
-lvl = DiscordLevelingSystem(awards=my_awards, level_up_announcement=announcement)
-lvl.connect_to_database_file(r'C:\Users\Defxult\Documents\DiscordLevelingSystem.db')
-
-@bot.event
-async def on_message(message):
-    await lvl.award_xp(amount=15, message=message)
-
-bot.run(...)
-```
----
-
-## All methods for DiscordLevelingSystem
-<details>
-    <summary>Click to show all methods</summary>
-
-* *await* **add_record**(`guild_id, member_id, member_name, level`) - Manually add a record to the database. If the record already exists (the `guild_id` and `member_id` was found), only the level will be updated. If there were no records that matched those values, all provided information will be added
-  * **Parameters**
-    * **guild_id** (`int`) The guild ID to register
-    * **member_id** (`int`) The member ID to register
-    * **member_name** (`str`) The member name to register
-    * **level** (`int`) The member level to register. Must be from 0-100
-  * **Raises**
-    * `DiscordLevelingSystemError` - The value given from a parameter was not of the correct type or "level" was not 0-100
-
-
-* *await* **add_xp**(`member, amount`) - Give XP to a member. This also changes their level so it matches the associated XP
-  * **Parameters**
-    * **member** (`discord.Member`) The member to give XP to
-    * **amount** (`int`) Amount of XP to give to the member
-  * **Raises**
-    * `DatabaseFileNotFound` - The database file was not found
-    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
-    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
-    * `NotConnected` - Attempted to use a method that requires a connection to a database file
-    * `DiscordLevelingSystemError` - Parameter "amount" was less than or equal to zero. The minimum value is 1 
-
-
-* *await* **award_xp**(`*, amount = [15, 25], message, refresh_name = True, **kwargs`) - Give XP to the member that sent a message
-  * **Parameters**
-    * **amount** (`Union[int, Sequence[int]]`)
-    * **message** (`discord.Message`) A message object
-    * **refresh_name** (`bool`) Everytime the member sends a message, check if their name still matches the name in the database. If it doesn't match, update the database to match their current name. It is suggested to leave this as `True` so the database can always have the most up-to-date record
-  * **Kwargs**
-    * **bonus** (`DiscordLevelingSystem.Bonus`) Set the bonus values. Read the `DiscordLevelingSystem.Bonus` doc string for more details (defaults to `None`)
-  * **Raises**
-    * `DatabaseFileNotFound` - The database file was not found
-    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
-    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
-    * `NotConnected` - Attempted to use a method that requires a connection to a database file
-
-
-* **backup_database_file**(`path, with_timestamp = False`) - Create a copy of the database file to the specified path. If a copy of the backup file is already in the specified path it will be overwritten
-  * **Parameters**
-    * **path** (`str`) The path to copy the database file to
-    * **with_timestamp** (`bool`) Creates a unique file name that has the date and time of when the backup file was created. This is useful when you want multiple backup files
-  * **Raises**
-    * `DiscordLevelingSystemError` - Path doesn't exist or points to another file
-    * `NotConnected` - Attempted to use a method that requires a connection to a database file
-
-
-* *await* **change_cooldown**(`rate, per`) - Update the cooldown rate
-  * **Parameters**
-    * **rate** (`int`) The amount of messages each member can send before the cooldown triggers
-    * **per** (`float`) The amount of seconds each member has to wait before gaining more XP, aka the cooldown
-  * **Raises**
-    * `DatabaseFileNotFound` - The database file was not found
-    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
-    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
-    * `NotConnected` - Attempted to use a method that requires a connection to a database file
-    * `DiscordLevelingSystemError` - The rate or per value was not greater than zero
-
-
-* *await* **clean_database**(`guild`) - Removes the data for members that are no longer in the guild, thus reducing the database file size. It is recommended to have this method in a background loop in order to keep the database file free of records that are no longer in use
-  * **Parameters**
-    * **guild** (`discord.Guild`) The guild records to clean
-  * **Returns**
-    * (`Optional[int]`) The amount of records that were removed from the database
-  * **Raises**
-    * `DatabaseFileNotFound` - The database file was not found
-    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
-    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
-    * `NotConnected` - Attempted to use a method that requires a connection to a database file
-
-
-* **connect_to_database_file**(`path`) - Connect to the existing database file in the specified path
-  * **Parameters**
-    * **path** (`str`) The location of the database file
-  * **Raises**
-    * `ConnectionFailure` - Attempted to connect to the database file when the event loop is already running
-    * `DatabaseFileNotFound` - The database file was not found
-
-
-* *static method* **create_database_file**(`path = None`) - Create the database file and implement the SQL data for the database
-  * **Parameters**
-    * **path** (`Optional[str]`) The location to create the database file. If `None`, the file is created in the current working directory
-  * **Raises**
-    * `ConnectionFailure` - Attempted to create the database file when the event loop is already running
-    * `DiscordLevelingSystemError` - The path does not exist or the path points to a file instead of a directory
-
-
-* *await* **each_member_data**(`guild, sort_by = None, limit = None`) - Return each member in the database as a `MemberData` object for easy access to their XP, level, etc. You can sort the data with `sort_by` with the below values
-  * **Parameters**
-    * **guild** (`discord.Guild`) A guild object
-    * **sort_by** (`Optional[str]`) Return each member sorted by: "name", "level", "xp", "rank". If `None`, it will return in the order they were added to the database
-    * **limit** (`Optional[int]`) Restrict the amount of records returned to the specified amount
-  * **Returns**
-    * `List[MemberData]`
-  * **Raises**
-    * `DatabaseFileNotFound` - The database file was not found
-    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
-    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
-    * `NotConnected` - Attempted to use a method that requires a connection to a database file
-    * `DiscordLevelingSystemError` - The value of `sort_by` was not recognized or `guild` was not of type `discord.Guild`
-
-
-* *await* **export_as_json**(`path, guild`) - Export a json file that represents the database to the path specified
-  * **Parameters**
-    * **path** (`str`) Path to copy the json file to
-    * **guild** (`discord.Guild`) The guild for which the data should be extracted from. If `None`, all guild information will be extracted from the database
-  * **Raises**
-    * `DatabaseFileNotFound` - The database file was not found
-    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
-    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
-    * `NotConnected` - Attempted to use a method that requires a connection to a database file
-    * `DiscordLevelingSystemError` - The path does not exist or does not point to a directory
-
-
-* **get_awards**(`guild = None`) - Get all `RoleAward`'s or only the `RoleAward`'s assigned to the specified guild
-  * **Parameters**
-    * **guild** (`Optional[Union[discord.Guild, int]]`) A guild object or a guild ID
-  * **Returns**
-    * (`Union[Dict[int, List[RoleAward]], List[RoleAward]]`) If `guild` is `None`, this return the awards `dict` that was set in constructor. If `guild` is specified, it returns a List[`RoleAward`] that matches the specified guild ID. Can also return `None` if awards were never set or if the awards for the specified guild was not found
-
-
-* *await* **get_data_for**(`member`) - Get the `MemberData` object that represents the specified member
-  * **Parameters**
-    * **member** (`discord.Member`) The member to get the data for
-  * **Returns**
-    * (`MemberData`) Can be `None` if the member isn't in the database
-  * **Raises**
-    * `DatabaseFileNotFound` - The database file was not found
-    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
-    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
-    * `NotConnected` - Attempted to use a method that requires a connection to a database file
-
-
-* *await* **get_level_for**(`member`) - Get the level for the specified member
-  * **Parameters**
-    * **member** (`discord.Member`) Member to get the level for
-  * **Returns**
-    * (`int`) Can be `None` if the member isn't in the database
-  * **Raises**
-    * `DatabaseFileNotFound` - The database file was not found
-    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
-    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
-    * `NotConnected` - Attempted to use a method that requires a connection to a database file
-
-
-* *await* **get_rank_for**(`member`) - Get the rank for the specified member
-  * **Parameters**
-    * **member** (`discord.Member`) Member to get the rank for
-  * **Returns**
-    * (`int`) Can be `None` if the member isn't ranked yet
-  * **Raises**
-    * `DatabaseFileNotFound` - The database file was not found
-    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
-    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
-    * `NotConnected` - Attempted to use a method that requires a connection to a database file
-
-
-* *await* **get_record_count**(`guild = None`) - Get the amount of members that are registered in the database. If `guild` is set to `None`, ALL members in the database will be counted
-  * **Parameters**
-    * **guild** (`Optional[discord.Guild]`) The guild for which to count the amount of records
-  * **Returns**
-    * (`int`)
-  * **Raises**
-    * `DatabaseFileNotFound` - The database file was not found
-    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
-    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
-    * `NotConnected` - Attempted to use a method that requires a connection to a database file
-
-
-* *await* **get_total_xp_for**(`member`) - Get the total XP for the specified member
-  * **Parameters**
-    * **member** (`discord.Member`) Member to get the total XP for
-  * **Returns**
-    * (`int`) Can be `None` if the member isn't in the database
-  * **Raises**
-    * `DatabaseFileNotFound` - The database file was not found
-    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
-    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
-    * `NotConnected` - Attempted to use a method that requires a connection to a database file
-
-
-* *await* **get_xp_for**(`member`) - Get the XP for the specified member
-  * **Parameters**
-    * **member** (`discord.Member`) Member to get the XP for
-  * **Returns**
-    * (`int`) Can be `None` if the member isn't in the database
-  * **Raises**
-    * `DatabaseFileNotFound` - The database file was not found
-    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
-    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
-    * `NotConnected` - Attempted to use a method that requires a connection to a database file
-
-
-* *static method* **get_xp_for_level**(`level`) - Returns the total amount of XP needed for the specified level. Levels go from 0-100
-  * **Parameters**
-    * **level** (`int`) The level XP information to retrieve
-  * **Returns**
-    * (`int`)
-  * **Raises**
-    * `DiscordLevelingSystemError` - The level specified does not exist
-
-
-* *await* **insert**(`bot, guild_id, users, using, overwrite = False, show_results = True`) - Insert the records from your own leveling system into the library. A lot of leveling system tutorials out there use json files to store information. Although it might work, it is insufficient because json files are not made to act as a database. Using an actual database file has many benefits over a json file
-  * **Parameters**
-    * **bot** (`Union[discord.ext.commands.Bot, discord.ext.commands.AutoShardedBot]`) Your bot instance variable
-    * **guild_id** (`int`) ID of the guild that you used your leveling system with
-    * **users** (`Dict[int, int]`) This is the information that will be added to the database. The keys are user ID's, and the values are the users total XP or level. Note: This library only uses levels 0-100 and XP 0-1899250. If any number in this dict are over the levels/XP threshold, it is implicitly set back to this libraries maximum value
-    * **using** (`str`) What structure your leveling system used. Options: "xp" or "levels". Some leveling systems give users only XP and they are ranked up based on that XP value. Others use a combination of levels and XP. If all the values in the `users` dict are based on XP, set this to "xp". If they are based on a users level, set this to "levels"
-    * **overwrite** (`bool`) If a user you've specified in the `users` dict already has a record in the database, overwrite their current record with the one your inserting
-    * **show_results** (`bool`) Print the results for how many of the `users` were successfully added to the database file. If any are unsuccessful, their ID along with the value you provided will also be shown
-  * **Raises**
-      * `DiscordLevelingSystemError` - The value given from a parameter was not of the correct type. The `users` dict was empty. Or your bot is not in the guild associated with `guild_id`       
-
-
-* *await* **is_in_database**(`member, guild = None`) - A quick check to see if a member is in the database. This is not guild specific although it can be if `guild` is specified
-  * **Parameters**
-    * **member** (`Union[discord.Member, int]`) The member to check for. Can be the member object or that members ID
-    * **guild** (`Optional[discord.Guild]`) The guild to check if the member is registered in
-  * **Returns**
-    * (`bool`)
-  * **Raises**
-    * `DatabaseFileNotFound` - The database file was not found
-    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
-    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
-    * `NotConnected` - Attempted to use a method that requires a connection to a database file
-    * `DiscordLevelingSystemError` - Parameter `member` was not of type `discord.Member` or `int`
-
-
-* *static method* **levels_and_xp**( ) -  Get the raw `dict` representation for the amount of levels/XP in the system. The keys in the `dict` returned is each level, and the values are the amount of XP needed to be awarded that level
-  * **Returns**
-    * (`Dict[str, int]`)
-
-
-* *await* **next_level**(`member`) - Get the next level for the specified member
-  * **Parameters**
-    * **member** (`discord.Member`) Member to get the next level for
-  * **Returns**
-    * (`int`) If the member is currently max level (100), it will return 100. This can also return `None` if the member is not in the database
-  * **Raises**
-    * `DatabaseFileNotFound` - The database file was not found
-    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
-    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
-    * `NotConnected` - Attempted to use a method that requires a connection to a database file
-
-
-* *await* **next_level_up**(`member`) - Get the amount of XP needed for the specified member to level up
-  * **Parameters**
-    * **member** (`discord.Member`) Member to get the amount of XP needed for a level up
-  * **Returns**
-    * (`int`) Returns 0 if the member is currently at max level. Can return `None` if the member is not in the database.
-  * **Raises**
-    * `DatabaseFileNotFound` - The database file was not found
-    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
-    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
-    * `NotConnected` - Attempted to use a method that requires a connection to a database file
-
-
-* *await* **raw_database_contents**(`guild = None`) - Returns everything in the database. Can specify which guild information will be extracted
-  * **Parameters**
-    * **guild** (`Optional[discord.Guild]`) The guild to extract the raw database contents from. If `None`, information about all guilds will be extracted
-  * **Returns**
-    * `List[Tuple[int, int, str, int, int, int]]` The tuples inside the list represents each row of the database:
-      * Index 0 is the guild ID
-      * Index 1 is their ID
-      * Index 2 is their name
-      * Index 3 is their level
-      * Index 4 is their XP
-      * Index 5 is their total xp
-      * Can be an empty list if nothing is in the database
-  * **Raises**
-    * `DatabaseFileNotFound` - The database file was not found
-    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
-    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
-    * `NotConnected` - Attempted to use a method that requires a connection to a database file
-
-
-* *await* **refresh_names**(`guild`) - Update names inside the database. This does not add anything new. It simply verifies if the name in the database matches their current name, and if they don't match, update the database name
-  * **Parameters**
-    * **guild** (`discord.Guild`) A guild object
-  * **Returns**
-    * `(Optional[int])` The amount of records in the database that were updated
-  * **Raises**
-    * `DatabaseFileNotFound` - The database file was not found
-    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
-    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
-    * `NotConnected` - Attempted to use a method that requires a connection to a database file
-
-
-* *await* **remove_from_database**(`member, guild = None`) - Remove a member from the database. This is not guild specific although it can be if `guild` is specified
-  * **Parameters**
-    * **member** (`Union[discord.Member, int]`) The member to remove. Can be the member object or that members ID
-    * **guild** (`Optional[discord.Guild]`) If this parameter is given, it will remove the record of the specified member only from the specified guild record. If `None`, it will remove all records no matter the guild
-  * **Returns**
-    * (`Optional[bool]`) Returns `True` if the member was successfully removed from the database. `False` if the member was not in the database so there was nothing to remove
-  * **Raises**
-      * `DatabaseFileNotFound` - The database file was not found
-      * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
-      * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
-      * `DiscordLevelingSystemError` - Parameter `member` was not of type `discord.Member` or `int`
-      * `NotConnected` - Attempted to use a method that requires a connection to a database file
-
-
-* *await* **remove_xp**(`member, amount`) - Remove XP from a member. This also changes their level so it matches the associated XP
-  * **Parameters**
-      * **member** (`discord.Member`) The member to remove XP from
-      * **amount** (`int`) Amount of XP to remove from the member
-  * **Raises**
-    * `DatabaseFileNotFound` - The database file was not found
-    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
-    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
-    * `NotConnected` - Attempted to use a method that requires a connection to a database file
-    * `DiscordLevelingSystemError` - Parameter "amount" was less than or equal to zero. The minimum value is 1
-
-
-* *await* **reset_everyone**(`guild, *, intentional = False`) - Sets EVERYONES XP, total XP, and level to zero in the database. Can specify which guild to reset
-  * **Parameters**
-      * **guild** (`Union[discord.Guild, None]`) The guild for which everyone will be reset. If this is set to `None`, everyone in the entire database will be reset
-      * **intentional** (`bool`) A simple kwarg to try and ensure that this action is indeed what you want to do. Once executed, this cannot be undone
-  * **Raises**
-    * `DatabaseFileNotFound` - The database file was not found
-    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
-    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
-    * `NotConnected` - Attempted to use a method that requires a connection to a database file
-    * `FailSafe` - "intentional" argument for this method was set to `False` in case you called this method by mistake
-
-
-* *await* **reset_member**(`member`) - Sets the members XP, total XP, and level to zero
-  * **Parameters**
-    * **member** (`discord.Member`) The member to reset
-  * **Raises**
-    * `DatabaseFileNotFound` The database file was not found
-    * `LeaderboardNotFound` Table "leaderboard" in the database file is missing
-    * `ImproperLeaderboard` Leaderboard table was altered. Components changed or deleted
-    * `NotConnected` Attempted to use a method that requires a connection to a database file
-
-
-* *await* **set_level**(`member, level`) - Sets the level for the member. This also changes their total XP so it matches the associated level
-  * **Parameters**
-    * **member** (`discord.Member`) The member who's level will be set
-    * **level** (`int`) Level to set. Must be from 0-100     
-  * **Raises**
-    * `DatabaseFileNotFound` - The database file was not found
-    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
-    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
-    * `NotConnected` - Attempted to use a method that requires a connection to a database file
-    * `DiscordLevelingSystemError` - Parameter "level" was not from 0-100
-
-
-* *await* **sql_query_get**(`sql, parameters = None, fetch = 'ALL'`) - Query and return something from the database using SQL. The following columns are apart of the "leaderboard" table: guild_id, member_id, member_name, member_level, member_xp, member_total_xp
-  * **Parameters**
-    * **sql** (`str`) SQL string used to query the database
-    * **parameters** (`Optional[Tuple[Union[str ,int]]]`) The parameters used for the database query
-    * **fetch** (`Union[str, int]`) The amount of rows you would like back from the query. Options: 'ALL', 'ONE', or an integer value that is greater than zero
-  * **Returns**
-    * (`Union[List[tuple], tuple]`)
-      * Using `fetch='ALL'` returns `List[tuple]`
-      * Using `fetch='ONE'` returns `tuple`
-      * Using `fetch=4` returns `List[tuple]` with only four values
-      * Can also return an empty list if the query was valid but got nothing from it
-  * **Raises**
-    * `DatabaseFileNotFound` - The database file was not found
-    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
-    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
-    * `NotConnected` - Attempted to use a method that requires a connection to a database file
-    * `DiscordLevelingSystemError` - Argument "fetch" was the wrong type or used an invalid value
-    * `aiosqlite.Error` - Base aiosqlite error. Multiple errors can arise from this if the SQL query was invalid
-
-
-* *await* **switch_connection**(`path`) - Connect to a different leveling system database file
-  * **Parameters**
-    * **path** (`str`) The location of the database file
-  * **Raises**
-    * `DatabaseFileNotFound` - The database file was not found
-
-
-* *static method* **transfer**(`old, new, guild_id`) - Transfer the database records from a database file created from v0.0.1 to a blank database file created using v0.0.2+. If you were already using a v0.0.2+ database file, there's no need to use this method
-  * **Parameters**
-    * **old** (`str`) The path of the v0.0.1 database file
-    * **new** (`str`) The path of the v0.0.2+ database file
-    * **guild_id** (`int`) ID of the guild that was originally used with this library
-  * **Raises**
-    - `ConnectionFailure` - The event loop is already running
-    - `DatabaseFileNotFound` - "old" or "new" database file was not found
-    - `DiscordLevelingSystemError` - One of the databases is missing the "leaderboard" table. A v0.0.2+ database file contains records, or there was an attempt to transfer records from a v0.0.2+ file to another v0.0.2+ file
-
-
-* *await* **wipe_database**(`guild = None, *, intentional = False`) - Delete EVERYTHING from the database. If `guild` is specified, only the information related to that guild will be deleted
-  * **Parameters**
-    * **guild** (`Optional[discord.Guild]`) The guild for which all information that is related to that guild will be deleted. If `None`, everything will be deleted
-    * **intentional** (`bool`) A simple kwarg to try and ensure that this action is indeed what you want to do. Once executed, this cannot be undone
-  * **Raises**
-    * `DatabaseFileNotFound` - The database file was not found
-    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
-    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
-    * `NotConnected` - Attempted to use a method that requires a connection to a database file
-    * `FailSafe` - "intentional" argument for this method was set to `False` in case you called this method by mistake
-
-</details>
-
-## Migrating from v0.0.1 to v0.0.2+
-<details>
-    <summary>Click to show details</summary>
-
-This library was not originally designed with the use of multiple servers in mind, so all the data you might have currently (your database file was created in `v0.0.1`) should be from a single server. With `v0.0.2`, the structure of the database file was changed to accommodate this fix. That means if you are currently using a `v0.0.1` database file and update to `v0.0.2+`, a vast majority of the library will be broken. To avoid this, you need to transfer all your `v0.0.1` database file records to a `v0.0.2+` database file. This can be done using the `transfer` method.
-
-* Associated static method
-  * `DiscordLevelingSystem.transfer(old: str, new: str, guild_id: int)`
-
-### Parameters
-* `old` (`str`) The path of the `v0.0.1` database file
-* `new` (`str`) The path of the `v0.0.2+` database file (a brand new file from using `DiscordLevelingSystem.create_database_file(path: str)`)
-* `guild_id` (`int`) ID of the guild that was originally used with this library
-
-<div align="left"><sub>EXAMPLE</sub></div>
-
-```py
-from discordLevelingSystem import DiscordLevelingSystem
-
-old = r'C:\Users\Defxult\Documents\DiscordLevelingSystem.db'
-new = r'C:\Users\Defxult\Desktop\DiscordLevelingSystem.db'
-
-DiscordLevelingSystem.transfer(old, new, guild_id=850809412011950121)
-```
-
-</details>
-
-## Inserting your own leveling system information
-<details>
-    <summary>Click to show details</summary>
-
-Insert the records from your leveling system into this one. A lot of leveling system tutorials out there use json files to store information. Although it might work, it is insufficient because json files are not made to act as a database. Using a database file has many benefits over a json file. If you previously watched a tutorial for your leveling system and would like to import your records over to use with this library, you can do so with the below method.
-
-* Associated static method
-  * `await DiscordLevelingSystem.insert(bot: Union[Bot, AutoShardedBot], guild_id: int, users: Dict[int, int], using: str, overwrite=False, show_results=True)`
-
-### Parameters
-- `bot` (`Union[discord.ext.commands.Bot, discord.ext.commands.AutoShardedBot]`) Your bot instance variable
-
-- `guild_id` (`int`) ID of the guild that you used your leveling system with
-
-- `users` (`Dict[int, int]`) This is the information that will be added to the database. The keys are user ID's, and the values are the users total XP or level. Note: This library only uses levels 0-100 and XP 0-1899250. If any number in this dict are over the levels/XP threshold, it is implicitly set back to this libraries maximum value
-
-- `using` (`str`) What structure your leveling system used. Options: "xp" or "levels". Some leveling systems give users only XP and they are ranked up based on that XP value. Others use a combination of levels and XP. If all the values in the `users` dict are based on XP, set this to "xp". If they are based on a users level, set this to "levels"
-
-- `overwrite` (`bool`) If a user you've specified in the `users` dict already has a record in the database, overwrite their current record with the one your inserting
-
-- `show_results` (`bool`) Print the results for how many of the `users` were successfully added to the database file. If any are unsuccessful, their ID along with the value you provided will also be shown
-
-> NOTE: If the users you've provided in the `users` dict is not currently in the guild (`guild_id`), their information will not be inserted. If you'd like, you can manually add those records with method `DiscordLevelingSystem.add_record()`, but that is discouraged because it is better to discard information that is no longer in use (the user is no longer in the guild)
-
-<div align="left"><sub>EXAMPLE</sub></div>
-
-```py
-# leveling_system.json
-[
-  {
-      "5748392849348934" : {
-          "xp" : 373,
-          "level" : 4
-      }
-  },
-  {
-      "89283659820948923" : {
-          "xp" : 23,
-          "level" : 1
-      }
-  }
-]
-
-
-# bot.py
-import json
-from discord.ext import commands
-from discordLevelingSystem import DiscordLevelingSystem
-
-bot = commands.Bot(...)
-
-lvl = DiscordLevelingSystem(...)
-lvl.connect_to_database_file(...)
-
-def json_to_dict() -> dict:
-    with open('leveling_system.json') as fp:
-        data = json.load(fp)
-        formatted: Dict[int, int] = ... # format the data so all keys and values are associated with the user ID and level
-        
-        """
-        In the end, the formatted dict should look like so:
-        
-        formatted = {
-            5748392849348934 : 4,
-            89283659820948923 : 1
-        }
-        """
-        return formatted
-
-@bot.command()
-async def insert(ctx):
-    await lvl.insert(ctx.bot, guild_id=12345678901234, users=json_to_dict(), using='levels')
-
-bot.run(...)
-```
-
-</details>
+A library to implement a leveling system into a discord bot. One of the most popular discord bots out there is MEE6 and it's leveling system. This library provides ways to easily implement one for yourself. It uses SQLite ([aiosqlite](https://pypi.org/project/aiosqlite/)) to locally query things such as their XP, rank, and level. Various amounts of other methods and classes are also provided so you can access or remove contents from the database file.
+
+[![Downloads](https://pepy.tech/badge/discordlevelingsystem)](https://pepy.tech/project/discordlevelingsystem)
+[![Downloads](https://pepy.tech/badge/discordlevelingsystem/month)](https://pepy.tech/project/discordlevelingsystem)
+![python_version](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10-blue)
+
+## Installing
+You can install the latest [PyPI version](https://pypi.org/project/discordLevelingSystem/) of the library by doing:
+
+`$ pip install discordLevelingSystem`
+
+Or the development version:
+
+`$ pip install git+https://github.com/Defxult/discordLevelingSystem`
+
+---
+
+## Showcase
+![showcase](https://cdn.discordapp.com/attachments/655186216060321816/835010159092039680/leveling_showcase.gif)
+
+---
+## How to import
+```py
+from discordLevelingSystem import DiscordLevelingSystem, LevelUpAnnouncement, RoleAward
+```
+
+---
+## Intents
+[Intents](https://discordpy.readthedocs.io/en/stable/intents.html) are required for proper functionality
+```py
+bot = commands.Bot(..., intents=discord.Intents(messages=True, guilds=True, members=True))
+```
+---
+
+
+## DiscordLevelingSystem
+```class DiscordLevelingSystem(rate=1, per=60.0, awards=None, **kwargs)```
+
+---
+### Parameters of the DiscordLevelingSystem constructor
+* `rate` (`int`) The amount of messages each member can send before the cooldown triggers
+* `per` (`float`) The amount of seconds each member has to wait before gaining more XP, aka the cooldown
+* `awards` (`Optional[Dict[int, List[RoleAward]]]`) The role given to a member when they reach a `RoleAward` level requirement
+---
+### Kwargs of the DiscordLevelingSystem constructor
+| Name | Type | Default Value | Info
+|------|------|---------------|-----
+| `no_xp_roles` | `Sequence[int]` | `None` | A sequence of role ID's. Any member with any of those roles will not gain XP when sending messages
+| `no_xp_channels` | `Sequence[int]` | `None` | A sequence of text channel ID's. Any member sending messages in any of those text channels will not gain XP
+| `announce_level_up` | `bool` | `True` | If `True`, level up messages will be sent when a member levels up
+| `stack_awards` | `bool` | `True` | If this is `True`, when the member levels up the assigned role award will be applied. If `False`, the previous role award will be removed and the level up assigned role will also be applied
+| `level_up_announcement` | `Union[LevelUpAnnouncement, Sequence[LevelUpAnnouncement]]` | `LevelUpAnnouncement()` | The message that is sent when someone levels up. If this is a sequence of `LevelUpAnnouncement`, one is selected at random
+|`bot` | ` Union[AutoShardedBot, Bot]` | `None` | Your bot instance variable. Used only if you'd like to use the `on_dls_level_up` event
+
+---
+### Attributes
+* `no_xp_roles`
+* `no_xp_channels`
+* `announce_level_up`
+* `stack_awards`
+* `level_up_announcement`
+* `bot`
+* `rate` (`int`) Read only property from the constructor
+* `per` (`float`) Read only property from the constructor
+* `database_file_path` (`str`) Read only property
+* `active` (`bool`) Enable/disable the leveling system. If `False`, nobody can gain XP when sending messages unless this is set back to `True`
+
+> NOTE: All attributes can be set during initialization
+---
+## Initial Setup
+When setting up the leveling system, a database file needs to be created in order for the library to function. 
+* Associated static method
+  * `DiscordLevelingSystem.create_database_file(path: str)`
+
+The above static method is used to create the database file for you in the path you specify. This method only needs to be called once. Example:
+```py
+DiscordLevelingSystem.create_database_file(r'C:\Users\Defxult\Documents')
+```
+Once created, there is no need to ever run that method again unless you want to create a new database file from scratch. Now that you have the database file, you can use the leveling system.
+
+---
+## Connecting to the Database
+* Associated method
+  * `DiscordLevelingSystem.connect_to_database_file(path: str)`
+
+Since the database file has already been created, all you need to do is connect to it. 
+> NOTE: When connecting to the database file, the event loop must not be running
+<div align="left"><sub>EXAMPLE</sub></div>
+
+```py
+from discord.ext import commands
+from discordLevelingSystem import DiscordLevelingSystem
+
+bot = commands.Bot(...)
+lvl = DiscordLevelingSystem()
+lvl.connect_to_database_file(r'C:\Users\Defxult\Documents\DiscordLevelingSystem.db')
+
+bot.run(...)
+```
+---
+
+## RoleAward
+```class RoleAward(role_id: int, level_requirement: int, role_name=None)```
+
+You can assign roles to the system so when someone levels up to a certain level, they are given that role. `RoleAward` is how that is accomplished.
+
+---
+### Parameters of the RoleAward constructor
+* `role_id` (`int`) ID of the role that is to be awarded.
+* `level_requirement` (`int`) What level is required for a member to be awarded the role.
+* `role_name` (`Optional[str]`) A name you can set for the award. Nothing is done with this value, it is used for visual identification purposes only.
+---
+### Attributes
+* `role_id`
+* `level_requirement`
+* `role_name`
+* `mention` (`str`) The discord role mention string
+
+When creating role awards, all role IDs and level requirements must be unique. Level requirements must also be in ascending order. It is also possible to assign different role awards for different guilds. If you don't want any role awards, set the `awards` parameter to `None`. When setting `awards`, it accepts a `dict` where the keys are guild IDs and the values are a `list` of `RoleAward`
+<div align="left"><sub>EXAMPLE</sub></div>
+
+```py
+from discordLevelingSystem import DiscordLevelingSystem, RoleAward
+
+johns_server = 587937522043060224
+janes_server = 850809412011950121
+
+my_awards = {
+    johns_server : [
+        RoleAward(role_id=831672678586777601, level_requirement=1, role_name='Rookie'),
+        RoleAward(role_id=831672730583171073, level_requirement=2, role_name='Associate'),
+        RoleAward(role_id=831672814419050526, level_requirement=3, role_name='Legend')
+    ],
+    janes_server : [
+        RoleAward(role_id=851400453904400385, level_requirement=1, role_name='Silver'),
+        RoleAward(role_id=851379776111116329, level_requirement=2, role_name='Gold'),
+        RoleAward(role_id=851959077071880202, level_requirement=3, role_name='Diamond')
+    ]
+}
+
+lvl = DiscordLevelingSystem(..., awards=my_awards)
+```
+---
+
+## LevelUpAnnouncement
+```class LevelUpAnnouncement(message=default_message, level_up_channel_ids=None, allowed_mentions=default_mentions, tts=False, delete_after=None)```
+
+Level up announcements are for when you want to implement your own level up messages. It provides access to who leveled up, their rank, level and much more. It also uses some of discord.py's kwargs from it's `Messageable.send` such as `allowed_mentions`, `tts`, and `delete_after` to give you more control over the sent message.
+
+---
+### Parameters of the LevelUpAnnouncement constructor
+
+* `message` (`Union[str, discord.Embed]`) The message that is sent when someone levels up. Defaults to `"<mention>, you are now **level <level>!**"`
+
+* `level_up_channel_ids` (`Optional[Sequence[int]]`) The text channel IDs where all level up messages will be sent for each server. If `None`, the level up message will be sent in the channel where they sent the message (example below).
+
+* `allowed_mentions` (`discord.AllowedMentions`) Used to determine who can be pinged in the level up message. Defaults to `discord.AllowedMentions(everyone=False, users=True, roles=False, replied_user=False)`
+
+* `tts` (`bool`) When the level up message is sent, have discord read the level up message aloud.
+
+* `delete_after` (`Optional[float]`) Delete the level up message after an x amount of seconds.
+
+### Class Attributes
+The `LevelUpAnnouncement` class provides a set of markdown attributes for you to use so you can access certain information in a level up message.
+
+* `LevelUpAnnouncement.TOTAL_XP` The members current total XP amount
+* `LevelUpAnnouncement.LEVEL` The members current level
+* `LevelUpAnnouncement.RANK` The members current rank
+
+The below markdown attributes takes the information from a `discord.Member` object so you can access member information in the level up message.
+
+* `LevelUpAnnouncement.Member.avatar_url`
+* `LevelUpAnnouncement.Member.banner_url`
+* `LevelUpAnnouncement.Member.created_at`
+* `LevelUpAnnouncement.Member.default_avatar_url`
+* `LevelUpAnnouncement.Member.discriminator`
+* `LevelUpAnnouncement.Member.display_avatar_url`
+* `LevelUpAnnouncement.Member.display_name`
+* `LevelUpAnnouncement.Member.id`
+* `LevelUpAnnouncement.Member.joined_at`
+* `LevelUpAnnouncement.Member.mention`
+* `LevelUpAnnouncement.Member.name`
+* `LevelUpAnnouncement.Member.nick`
+* `LevelUpAnnouncement.Member.Guild.icon_url`
+* `LevelUpAnnouncement.Member.Guild.id`
+* `LevelUpAnnouncement.Member.Guild.name`
+
+<div align="left"><sub>EXAMPLE</sub></div>
+
+```py
+from discordLevelingSystem import DiscordLevelingSystem, LevelUpAnnouncement
+
+embed = discord.Embed()
+embed.set_author(name=LevelUpAnnouncement.Member.name, icon_url=LevelUpAnnouncement.Member.avatar_url)
+embed.description = f'Congrats {LevelUpAnnouncement.Member.mention}! You are now level {LevelUpAnnouncement.LEVEL} 😎'
+
+announcement = LevelUpAnnouncement(embed)
+
+lvl = DiscordLevelingSystem(..., level_up_announcement=announcement)
+
+# NOTE: You can have multiple level up announcements by setting the parameter to a sequence of LevelUpAnnouncement
+lvl = DiscordLevelingSystem(..., level_up_announcement=[announcement_1, announcement_2, ...])
+```
+When it comes to `level_up_channel_ids`, you can set a designated channel for each server. If you don't set a level up channel ID for a specific server, the level up message will be sent in the channel where the member leveled up. You don't have to specify a level up channel ID for each server unless you'd like to.
+```py
+johns_bot_commands = 489374746737648734 # text channel ID from server A
+janes_levelup_channel = 58498304930493094 # text channel ID from server B
+
+announcement = LevelUpAnnouncement(..., level_up_channel_ids=[johns_bot_commands, janes_levelup_channel])
+lvl = DiscordLevelingSystem(..., level_up_announcement=announcement)
+```
+---
+## Handling XP
+Method `award_xp` is how members gain XP. This method is placed inside the `on_message` event of your bot. Members will gain XP if they send a message and if they're *not* on cooldown. Spamming messages will not give them XP.
+> NOTE: Members cannot gain XP in DM's
+* Associated methods
+  * `await DiscordLevelingSystem.add_xp(member: Member, amount: int)`
+  * `await DiscordLevelingSystem.remove_xp(member: Member, amount: int)`
+  * `await DiscordLevelingSystem.set_level(member: Member, level: int)`
+  * `await DiscordLevelingSystem.award_xp(*, amount=[15, 25], message: Message, refresh_name=True, **kwargs)`
+
+
+### Parameters for award_xp
+* `amount` (`Union[int, Sequence[int]]`) The amount of XP to award to the member per message. Must be from 1-25. Can be a sequence with a minimum and maximum length of two. If `amount` is a sequence of two integers, it will randomly pick a number in between those numbers including the numbers provided.
+* `message` (`discord.Message`) A discord message object
+* `refresh_name` (`bool`) Everytime the member sends a message, check if their name still matches the name in the database. If it doesn't match, update the database to match their current name. It is suggested to leave this as `True` so the database can always have the most up-to-date record.
+
+### Kwargs for award_xp
+* `bonus` (`DiscordLevelingSystem.Bonus`) Used to set the roles that will be awarded bonus XP.
+  * `class Bonus(role_ids: Sequence[int], bonus_amount: int, multiply: bool)`
+  * **Parameters of the DiscordLevelingSystem.Bonus constructor**
+    * `role_ids` (`Sequence[int]`) The role(s) a member must have to be able to get bonus XP. They only need to have one of these roles to get the bonus
+    * `bonus_amount` (`int`) Amount of extra XP to be awarded
+    * `multiply` (`bool`) If set to `True`, this will operate on a x2, x3 basis. Meaning if you have the awarded XP amount set to 10 and you want the bonus XP role to be awarded 20, it must be set to 2, not 10. If `False`, it operates purely on the given value. Meaning if you have the awarded XP set to 10 and you want the bonus XP role to be awarded 20, it must be set to 10.
+
+<div align="left"><sub>EXAMPLE</sub></div>
+
+```py
+lvl = DiscordLevelingSystem(...)
+
+nitro_booster = 851379776111116329
+associate_role = 851400453904400385
+
+@bot.event
+async def on_message(message):
+    await lvl.award_xp(amount=[15, 25], message=message, bonus=DiscordLevelingSystem.Bonus([nitro_booster, associate_role], 20, multiply=False))
+```
+---
+
+## MemberData
+Accessing the raw information inside the database file can look a bit messy if you don't know exactly what you're looking at. To make things easier, this library comes with the `MemberData` class. A class which returns information about a specific member in the database.
+
+* Associated methods
+  * `await DiscordLevelingSystem.get_data_for(member: Member) -> MemberData`
+  * `await DiscordLevelingSystem.each_member_data(guild: Guild, sort_by=None, limit=None) -> List[MemberData]`
+
+### Attributes
+* `id_number` (`int`) The members ID
+* `name` (`str`) The members name
+* `level` (`int`) The members level
+* `xp` (`int`) The members xp
+* `total_xp` (`int`) The members total xp
+* `rank` (`Optional[int]`) The members rank
+* `mention` (`str`) The discord member mention string
+
+### Methods
+* `MemberData.to_dict() -> dict`
+
+<div align="left"><sub>EXAMPLE</sub></div>
+
+```py
+lvl = DiscordLevelingSystem(...)
+
+@bot.command()
+async def rank(ctx):
+    data = await lvl.get_data_for(ctx.author)
+    await ctx.send(f'You are level {data.level} and your rank is {data.rank}')
+
+@bot.command()
+async def leaderboard(ctx):
+    data = await lvl.each_member_data(ctx.guild, sort_by='rank')
+    # show the leaderboard whichever way you'd like
+```
+---
+## Events
+You can set an event to be called when a member levels up. Using the event is considered as an enhanced `LevelUpAnnouncement` because it provides more capabilities rather than simply sending a message with only text/an embed. The `on_dls_level_up` event takes three parameters:
+* `member` (`discord.Member`) The member that leveled up
+* `message` (`discord.Message`) The message that triggered the level up
+* `data` (`MemberData`) The database information for that member
+
+```py
+bot = commands.Bot(...)
+lvl = DiscordLevelingSystem(..., bot=bot) # your bot instance variable is needed
+
+@bot.event
+async def on_dls_level_up(member: discord.Member, message: discord.Message, data: MemberData):
+    # You can do a lot more here compared to LevelUpAnnouncement
+    # - create a level up image and send it with discord.File
+    # - call additional functions that you may need
+    # - access to all attributes/methods that are available within discord.Member and discord.Message
+```
+> NOTE: `LevelUpAnnouncement` and `on_dls_level_up` are not the same. Level up messages are sent by default by the library. If you'd like to only use `on_dls_level_up`, you need to disable level up announcements (`lvl.announce_level_up = False`)
+
+---
+## Full Example
+With all classes and core methods introduced, here is a basic implementation of this library.
+```py
+from discord.ext import commands
+from discordLevelingSystem import DiscordLevelingSystem, RoleAward, LevelUpAnnouncement
+
+bot = commands.Bot(...)
+
+main_guild_id = 850809412011950121
+
+my_awards = {
+    main_guild_id : [
+        RoleAward(role_id=831672678586777601, level_requirement=1, role_name='Rookie'),
+        RoleAward(role_id=831672730583171073, level_requirement=2, role_name='Associate'),
+        RoleAward(role_id=831672814419050526, level_requirement=3, role_name='Legend')
+    ]
+}
+
+announcement = LevelUpAnnouncement(f'{LevelUpAnnouncement.Member.mention} just leveled up to level {LevelUpAnnouncement.LEVEL} 😎')
+
+# DiscordLevelingSystem.create_database_file(r'C:\Users\Defxult\Documents') database file already created
+lvl = DiscordLevelingSystem(awards=my_awards, level_up_announcement=announcement)
+lvl.connect_to_database_file(r'C:\Users\Defxult\Documents\DiscordLevelingSystem.db')
+
+@bot.event
+async def on_message(message):
+    await lvl.award_xp(amount=15, message=message)
+
+bot.run(...)
+```
+---
+
+## All methods for DiscordLevelingSystem
+<details>
+    <summary>Click to show all methods</summary>
+
+* *await* **add_record**(`guild_id, member_id, member_name, level`) - Manually add a record to the database. If the record already exists (the `guild_id` and `member_id` was found), only the level will be updated. If there were no records that matched those values, all provided information will be added
+  * **Parameters**
+    * **guild_id** (`int`) The guild ID to register
+    * **member_id** (`int`) The member ID to register
+    * **member_name** (`str`) The member name to register
+    * **level** (`int`) The member level to register. Must be from 0-100
+  * **Raises**
+    * `DiscordLevelingSystemError` - The value given from a parameter was not of the correct type or "level" was not 0-100
+
+
+* *await* **add_xp**(`member, amount`) - Give XP to a member. This also changes their level so it matches the associated XP
+  * **Parameters**
+    * **member** (`discord.Member`) The member to give XP to
+    * **amount** (`int`) Amount of XP to give to the member
+  * **Raises**
+    * `DatabaseFileNotFound` - The database file was not found
+    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
+    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
+    * `NotConnected` - Attempted to use a method that requires a connection to a database file
+    * `DiscordLevelingSystemError` - Parameter "amount" was less than or equal to zero. The minimum value is 1 
+
+
+* *await* **award_xp**(`*, amount = [15, 25], message, refresh_name = True, **kwargs`) - Give XP to the member that sent a message
+  * **Parameters**
+    * **amount** (`Union[int, Sequence[int]]`)
+    * **message** (`discord.Message`) A message object
+    * **refresh_name** (`bool`) Everytime the member sends a message, check if their name still matches the name in the database. If it doesn't match, update the database to match their current name. It is suggested to leave this as `True` so the database can always have the most up-to-date record
+  * **Kwargs**
+    * **bonus** (`DiscordLevelingSystem.Bonus`) Set the bonus values. Read the `DiscordLevelingSystem.Bonus` doc string for more details (defaults to `None`)
+  * **Raises**
+    * `DatabaseFileNotFound` - The database file was not found
+    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
+    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
+    * `NotConnected` - Attempted to use a method that requires a connection to a database file
+
+
+* **backup_database_file**(`path, with_timestamp = False`) - Create a copy of the database file to the specified path. If a copy of the backup file is already in the specified path it will be overwritten
+  * **Parameters**
+    * **path** (`str`) The path to copy the database file to
+    * **with_timestamp** (`bool`) Creates a unique file name that has the date and time of when the backup file was created. This is useful when you want multiple backup files
+  * **Raises**
+    * `DiscordLevelingSystemError` - Path doesn't exist or points to another file
+    * `NotConnected` - Attempted to use a method that requires a connection to a database file
+
+
+* *await* **change_cooldown**(`rate, per`) - Update the cooldown rate
+  * **Parameters**
+    * **rate** (`int`) The amount of messages each member can send before the cooldown triggers
+    * **per** (`float`) The amount of seconds each member has to wait before gaining more XP, aka the cooldown
+  * **Raises**
+    * `DatabaseFileNotFound` - The database file was not found
+    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
+    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
+    * `NotConnected` - Attempted to use a method that requires a connection to a database file
+    * `DiscordLevelingSystemError` - The rate or per value was not greater than zero
+
+
+* *await* **clean_database**(`guild`) - Removes the data for members that are no longer in the guild, thus reducing the database file size. It is recommended to have this method in a background loop in order to keep the database file free of records that are no longer in use
+  * **Parameters**
+    * **guild** (`discord.Guild`) The guild records to clean
+  * **Returns**
+    * (`Optional[int]`) The amount of records that were removed from the database
+  * **Raises**
+    * `DatabaseFileNotFound` - The database file was not found
+    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
+    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
+    * `NotConnected` - Attempted to use a method that requires a connection to a database file
+
+
+* **connect_to_database_file**(`path`) - Connect to the existing database file in the specified path
+  * **Parameters**
+    * **path** (`str`) The location of the database file
+  * **Raises**
+    * `ConnectionFailure` - Attempted to connect to the database file when the event loop is already running
+    * `DatabaseFileNotFound` - The database file was not found
+
+
+* *static method* **create_database_file**(`path = None`) - Create the database file and implement the SQL data for the database
+  * **Parameters**
+    * **path** (`Optional[str]`) The location to create the database file. If `None`, the file is created in the current working directory
+  * **Raises**
+    * `ConnectionFailure` - Attempted to create the database file when the event loop is already running
+    * `DiscordLevelingSystemError` - The path does not exist or the path points to a file instead of a directory
+
+
+* *await* **each_member_data**(`guild, sort_by = None, limit = None`) - Return each member in the database as a `MemberData` object for easy access to their XP, level, etc. You can sort the data with `sort_by` with the below values
+  * **Parameters**
+    * **guild** (`discord.Guild`) A guild object
+    * **sort_by** (`Optional[str]`) Return each member sorted by: "name", "level", "xp", "rank". If `None`, it will return in the order they were added to the database
+    * **limit** (`Optional[int]`) Restrict the amount of records returned to the specified amount
+  * **Returns**
+    * `List[MemberData]`
+  * **Raises**
+    * `DatabaseFileNotFound` - The database file was not found
+    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
+    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
+    * `NotConnected` - Attempted to use a method that requires a connection to a database file
+    * `DiscordLevelingSystemError` - The value of `sort_by` was not recognized or `guild` was not of type `discord.Guild`
+
+
+* *await* **export_as_json**(`path, guild`) - Export a json file that represents the database to the path specified
+  * **Parameters**
+    * **path** (`str`) Path to copy the json file to
+    * **guild** (`discord.Guild`) The guild for which the data should be extracted from. If `None`, all guild information will be extracted from the database
+  * **Raises**
+    * `DatabaseFileNotFound` - The database file was not found
+    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
+    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
+    * `NotConnected` - Attempted to use a method that requires a connection to a database file
+    * `DiscordLevelingSystemError` - The path does not exist or does not point to a directory
+
+
+* **get_awards**(`guild = None`) - Get all `RoleAward`'s or only the `RoleAward`'s assigned to the specified guild
+  * **Parameters**
+    * **guild** (`Optional[Union[discord.Guild, int]]`) A guild object or a guild ID
+  * **Returns**
+    * (`Union[Dict[int, List[RoleAward]], List[RoleAward]]`) If `guild` is `None`, this return the awards `dict` that was set in constructor. If `guild` is specified, it returns a List[`RoleAward`] that matches the specified guild ID. Can also return `None` if awards were never set or if the awards for the specified guild was not found
+
+
+* *await* **get_data_for**(`member`) - Get the `MemberData` object that represents the specified member
+  * **Parameters**
+    * **member** (`discord.Member`) The member to get the data for
+  * **Returns**
+    * (`MemberData`) Can be `None` if the member isn't in the database
+  * **Raises**
+    * `DatabaseFileNotFound` - The database file was not found
+    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
+    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
+    * `NotConnected` - Attempted to use a method that requires a connection to a database file
+
+
+* *await* **get_level_for**(`member`) - Get the level for the specified member
+  * **Parameters**
+    * **member** (`discord.Member`) Member to get the level for
+  * **Returns**
+    * (`int`) Can be `None` if the member isn't in the database
+  * **Raises**
+    * `DatabaseFileNotFound` - The database file was not found
+    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
+    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
+    * `NotConnected` - Attempted to use a method that requires a connection to a database file
+
+
+* *await* **get_rank_for**(`member`) - Get the rank for the specified member
+  * **Parameters**
+    * **member** (`discord.Member`) Member to get the rank for
+  * **Returns**
+    * (`int`) Can be `None` if the member isn't ranked yet
+  * **Raises**
+    * `DatabaseFileNotFound` - The database file was not found
+    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
+    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
+    * `NotConnected` - Attempted to use a method that requires a connection to a database file
+
+
+* *await* **get_record_count**(`guild = None`) - Get the amount of members that are registered in the database. If `guild` is set to `None`, ALL members in the database will be counted
+  * **Parameters**
+    * **guild** (`Optional[discord.Guild]`) The guild for which to count the amount of records
+  * **Returns**
+    * (`int`)
+  * **Raises**
+    * `DatabaseFileNotFound` - The database file was not found
+    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
+    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
+    * `NotConnected` - Attempted to use a method that requires a connection to a database file
+
+
+* *await* **get_total_xp_for**(`member`) - Get the total XP for the specified member
+  * **Parameters**
+    * **member** (`discord.Member`) Member to get the total XP for
+  * **Returns**
+    * (`int`) Can be `None` if the member isn't in the database
+  * **Raises**
+    * `DatabaseFileNotFound` - The database file was not found
+    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
+    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
+    * `NotConnected` - Attempted to use a method that requires a connection to a database file
+
+
+* *await* **get_xp_for**(`member`) - Get the XP for the specified member
+  * **Parameters**
+    * **member** (`discord.Member`) Member to get the XP for
+  * **Returns**
+    * (`int`) Can be `None` if the member isn't in the database
+  * **Raises**
+    * `DatabaseFileNotFound` - The database file was not found
+    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
+    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
+    * `NotConnected` - Attempted to use a method that requires a connection to a database file
+
+
+* *static method* **get_xp_for_level**(`level`) - Returns the total amount of XP needed for the specified level. Levels go from 0-100
+  * **Parameters**
+    * **level** (`int`) The level XP information to retrieve
+  * **Returns**
+    * (`int`)
+  * **Raises**
+    * `DiscordLevelingSystemError` - The level specified does not exist
+
+
+* *await* **insert**(`bot, guild_id, users, using, overwrite = False, show_results = True`) - Insert the records from your own leveling system into the library. A lot of leveling system tutorials out there use json files to store information. Although it might work, it is insufficient because json files are not made to act as a database. Using an actual database file has many benefits over a json file
+  * **Parameters**
+    * **bot** (`Union[discord.ext.commands.Bot, discord.ext.commands.AutoShardedBot]`) Your bot instance variable
+    * **guild_id** (`int`) ID of the guild that you used your leveling system with
+    * **users** (`Dict[int, int]`) This is the information that will be added to the database. The keys are user ID's, and the values are the users total XP or level. Note: This library only uses levels 0-100 and XP 0-1899250. If any number in this dict are over the levels/XP threshold, it is implicitly set back to this libraries maximum value
+    * **using** (`str`) What structure your leveling system used. Options: "xp" or "levels". Some leveling systems give users only XP and they are ranked up based on that XP value. Others use a combination of levels and XP. If all the values in the `users` dict are based on XP, set this to "xp". If they are based on a users level, set this to "levels"
+    * **overwrite** (`bool`) If a user you've specified in the `users` dict already has a record in the database, overwrite their current record with the one your inserting
+    * **show_results** (`bool`) Print the results for how many of the `users` were successfully added to the database file. If any are unsuccessful, their ID along with the value you provided will also be shown
+  * **Raises**
+      * `DiscordLevelingSystemError` - The value given from a parameter was not of the correct type. The `users` dict was empty. Or your bot is not in the guild associated with `guild_id`       
+
+
+* *await* **is_in_database**(`member, guild = None`) - A quick check to see if a member is in the database. This is not guild specific although it can be if `guild` is specified
+  * **Parameters**
+    * **member** (`Union[discord.Member, int]`) The member to check for. Can be the member object or that members ID
+    * **guild** (`Optional[discord.Guild]`) The guild to check if the member is registered in
+  * **Returns**
+    * (`bool`)
+  * **Raises**
+    * `DatabaseFileNotFound` - The database file was not found
+    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
+    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
+    * `NotConnected` - Attempted to use a method that requires a connection to a database file
+    * `DiscordLevelingSystemError` - Parameter `member` was not of type `discord.Member` or `int`
+
+
+* *static method* **levels_and_xp**( ) -  Get the raw `dict` representation for the amount of levels/XP in the system. The keys in the `dict` returned is each level, and the values are the amount of XP needed to be awarded that level
+  * **Returns**
+    * (`Dict[str, int]`)
+
+
+* *await* **next_level**(`member`) - Get the next level for the specified member
+  * **Parameters**
+    * **member** (`discord.Member`) Member to get the next level for
+  * **Returns**
+    * (`int`) If the member is currently max level (100), it will return 100. This can also return `None` if the member is not in the database
+  * **Raises**
+    * `DatabaseFileNotFound` - The database file was not found
+    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
+    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
+    * `NotConnected` - Attempted to use a method that requires a connection to a database file
+
+
+* *await* **next_level_up**(`member`) - Get the amount of XP needed for the specified member to level up
+  * **Parameters**
+    * **member** (`discord.Member`) Member to get the amount of XP needed for a level up
+  * **Returns**
+    * (`int`) Returns 0 if the member is currently at max level. Can return `None` if the member is not in the database.
+  * **Raises**
+    * `DatabaseFileNotFound` - The database file was not found
+    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
+    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
+    * `NotConnected` - Attempted to use a method that requires a connection to a database file
+
+
+* *await* **raw_database_contents**(`guild = None`) - Returns everything in the database. Can specify which guild information will be extracted
+  * **Parameters**
+    * **guild** (`Optional[discord.Guild]`) The guild to extract the raw database contents from. If `None`, information about all guilds will be extracted
+  * **Returns**
+    * `List[Tuple[int, int, str, int, int, int]]` The tuples inside the list represents each row of the database:
+      * Index 0 is the guild ID
+      * Index 1 is their ID
+      * Index 2 is their name
+      * Index 3 is their level
+      * Index 4 is their XP
+      * Index 5 is their total xp
+      * Can be an empty list if nothing is in the database
+  * **Raises**
+    * `DatabaseFileNotFound` - The database file was not found
+    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
+    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
+    * `NotConnected` - Attempted to use a method that requires a connection to a database file
+
+
+* *await* **refresh_names**(`guild`) - Update names inside the database. This does not add anything new. It simply verifies if the name in the database matches their current name, and if they don't match, update the database name
+  * **Parameters**
+    * **guild** (`discord.Guild`) A guild object
+  * **Returns**
+    * `(Optional[int])` The amount of records in the database that were updated
+  * **Raises**
+    * `DatabaseFileNotFound` - The database file was not found
+    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
+    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
+    * `NotConnected` - Attempted to use a method that requires a connection to a database file
+
+
+* *await* **remove_from_database**(`member, guild = None`) - Remove a member from the database. This is not guild specific although it can be if `guild` is specified
+  * **Parameters**
+    * **member** (`Union[discord.Member, int]`) The member to remove. Can be the member object or that members ID
+    * **guild** (`Optional[discord.Guild]`) If this parameter is given, it will remove the record of the specified member only from the specified guild record. If `None`, it will remove all records no matter the guild
+  * **Returns**
+    * (`Optional[bool]`) Returns `True` if the member was successfully removed from the database. `False` if the member was not in the database so there was nothing to remove
+  * **Raises**
+      * `DatabaseFileNotFound` - The database file was not found
+      * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
+      * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
+      * `DiscordLevelingSystemError` - Parameter `member` was not of type `discord.Member` or `int`
+      * `NotConnected` - Attempted to use a method that requires a connection to a database file
+
+
+* *await* **remove_xp**(`member, amount`) - Remove XP from a member. This also changes their level so it matches the associated XP
+  * **Parameters**
+      * **member** (`discord.Member`) The member to remove XP from
+      * **amount** (`int`) Amount of XP to remove from the member
+  * **Raises**
+    * `DatabaseFileNotFound` - The database file was not found
+    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
+    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
+    * `NotConnected` - Attempted to use a method that requires a connection to a database file
+    * `DiscordLevelingSystemError` - Parameter "amount" was less than or equal to zero. The minimum value is 1
+
+
+* *await* **reset_everyone**(`guild, *, intentional = False`) - Sets EVERYONES XP, total XP, and level to zero in the database. Can specify which guild to reset
+  * **Parameters**
+      * **guild** (`Union[discord.Guild, None]`) The guild for which everyone will be reset. If this is set to `None`, everyone in the entire database will be reset
+      * **intentional** (`bool`) A simple kwarg to try and ensure that this action is indeed what you want to do. Once executed, this cannot be undone
+  * **Raises**
+    * `DatabaseFileNotFound` - The database file was not found
+    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
+    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
+    * `NotConnected` - Attempted to use a method that requires a connection to a database file
+    * `FailSafe` - "intentional" argument for this method was set to `False` in case you called this method by mistake
+
+
+* *await* **reset_member**(`member`) - Sets the members XP, total XP, and level to zero
+  * **Parameters**
+    * **member** (`discord.Member`) The member to reset
+  * **Raises**
+    * `DatabaseFileNotFound` The database file was not found
+    * `LeaderboardNotFound` Table "leaderboard" in the database file is missing
+    * `ImproperLeaderboard` Leaderboard table was altered. Components changed or deleted
+    * `NotConnected` Attempted to use a method that requires a connection to a database file
+
+
+* *await* **set_level**(`member, level`) - Sets the level for the member. This also changes their total XP so it matches the associated level
+  * **Parameters**
+    * **member** (`discord.Member`) The member who's level will be set
+    * **level** (`int`) Level to set. Must be from 0-100     
+  * **Raises**
+    * `DatabaseFileNotFound` - The database file was not found
+    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
+    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
+    * `NotConnected` - Attempted to use a method that requires a connection to a database file
+    * `DiscordLevelingSystemError` - Parameter "level" was not from 0-100
+
+
+* *await* **sql_query_get**(`sql, parameters = None, fetch = 'ALL'`) - Query and return something from the database using SQL. The following columns are apart of the "leaderboard" table: guild_id, member_id, member_name, member_level, member_xp, member_total_xp
+  * **Parameters**
+    * **sql** (`str`) SQL string used to query the database
+    * **parameters** (`Optional[Tuple[Union[str ,int]]]`) The parameters used for the database query
+    * **fetch** (`Union[str, int]`) The amount of rows you would like back from the query. Options: 'ALL', 'ONE', or an integer value that is greater than zero
+  * **Returns**
+    * (`Union[List[tuple], tuple]`)
+      * Using `fetch='ALL'` returns `List[tuple]`
+      * Using `fetch='ONE'` returns `tuple`
+      * Using `fetch=4` returns `List[tuple]` with only four values
+      * Can also return an empty list if the query was valid but got nothing from it
+  * **Raises**
+    * `DatabaseFileNotFound` - The database file was not found
+    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
+    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
+    * `NotConnected` - Attempted to use a method that requires a connection to a database file
+    * `DiscordLevelingSystemError` - Argument "fetch" was the wrong type or used an invalid value
+    * `aiosqlite.Error` - Base aiosqlite error. Multiple errors can arise from this if the SQL query was invalid
+
+
+* *await* **switch_connection**(`path`) - Connect to a different leveling system database file
+  * **Parameters**
+    * **path** (`str`) The location of the database file
+  * **Raises**
+    * `DatabaseFileNotFound` - The database file was not found
+
+
+* *static method* **transfer**(`old, new, guild_id`) - Transfer the database records from a database file created from v0.0.1 to a blank database file created using v0.0.2+. If you were already using a v0.0.2+ database file, there's no need to use this method
+  * **Parameters**
+    * **old** (`str`) The path of the v0.0.1 database file
+    * **new** (`str`) The path of the v0.0.2+ database file
+    * **guild_id** (`int`) ID of the guild that was originally used with this library
+  * **Raises**
+    - `ConnectionFailure` - The event loop is already running
+    - `DatabaseFileNotFound` - "old" or "new" database file was not found
+    - `DiscordLevelingSystemError` - One of the databases is missing the "leaderboard" table. A v0.0.2+ database file contains records, or there was an attempt to transfer records from a v0.0.2+ file to another v0.0.2+ file
+
+
+* *await* **wipe_database**(`guild = None, *, intentional = False`) - Delete EVERYTHING from the database. If `guild` is specified, only the information related to that guild will be deleted
+  * **Parameters**
+    * **guild** (`Optional[discord.Guild]`) The guild for which all information that is related to that guild will be deleted. If `None`, everything will be deleted
+    * **intentional** (`bool`) A simple kwarg to try and ensure that this action is indeed what you want to do. Once executed, this cannot be undone
+  * **Raises**
+    * `DatabaseFileNotFound` - The database file was not found
+    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
+    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
+    * `NotConnected` - Attempted to use a method that requires a connection to a database file
+    * `FailSafe` - "intentional" argument for this method was set to `False` in case you called this method by mistake
+
+</details>
+
+## Migrating from v0.0.1 to v0.0.2+
+<details>
+    <summary>Click to show details</summary>
+
+This library was not originally designed with the use of multiple servers in mind, so all the data you might have currently (your database file was created in `v0.0.1`) should be from a single server. With `v0.0.2`, the structure of the database file was changed to accommodate this fix. That means if you are currently using a `v0.0.1` database file and update to `v0.0.2+`, a vast majority of the library will be broken. To avoid this, you need to transfer all your `v0.0.1` database file records to a `v0.0.2+` database file. This can be done using the `transfer` method.
+
+* Associated static method
+  * `DiscordLevelingSystem.transfer(old: str, new: str, guild_id: int)`
+
+### Parameters
+* `old` (`str`) The path of the `v0.0.1` database file
+* `new` (`str`) The path of the `v0.0.2+` database file (a brand new file from using `DiscordLevelingSystem.create_database_file(path: str)`)
+* `guild_id` (`int`) ID of the guild that was originally used with this library
+
+<div align="left"><sub>EXAMPLE</sub></div>
+
+```py
+from discordLevelingSystem import DiscordLevelingSystem
+
+old = r'C:\Users\Defxult\Documents\DiscordLevelingSystem.db'
+new = r'C:\Users\Defxult\Desktop\DiscordLevelingSystem.db'
+
+DiscordLevelingSystem.transfer(old, new, guild_id=850809412011950121)
+```
+
+</details>
+
+## Inserting your own leveling system information
+<details>
+    <summary>Click to show details</summary>
+
+Insert the records from your leveling system into this one. A lot of leveling system tutorials out there use json files to store information. Although it might work, it is insufficient because json files are not made to act as a database. Using a database file has many benefits over a json file. If you previously watched a tutorial for your leveling system and would like to import your records over to use with this library, you can do so with the below method.
+
+* Associated static method
+  * `await DiscordLevelingSystem.insert(bot: Union[Bot, AutoShardedBot], guild_id: int, users: Dict[int, int], using: str, overwrite=False, show_results=True)`
+
+### Parameters
+- `bot` (`Union[discord.ext.commands.Bot, discord.ext.commands.AutoShardedBot]`) Your bot instance variable
+
+- `guild_id` (`int`) ID of the guild that you used your leveling system with
+
+- `users` (`Dict[int, int]`) This is the information that will be added to the database. The keys are user ID's, and the values are the users total XP or level. Note: This library only uses levels 0-100 and XP 0-1899250. If any number in this dict are over the levels/XP threshold, it is implicitly set back to this libraries maximum value
+
+- `using` (`str`) What structure your leveling system used. Options: "xp" or "levels". Some leveling systems give users only XP and they are ranked up based on that XP value. Others use a combination of levels and XP. If all the values in the `users` dict are based on XP, set this to "xp". If they are based on a users level, set this to "levels"
+
+- `overwrite` (`bool`) If a user you've specified in the `users` dict already has a record in the database, overwrite their current record with the one your inserting
+
+- `show_results` (`bool`) Print the results for how many of the `users` were successfully added to the database file. If any are unsuccessful, their ID along with the value you provided will also be shown
+
+> NOTE: If the users you've provided in the `users` dict is not currently in the guild (`guild_id`), their information will not be inserted. If you'd like, you can manually add those records with method `DiscordLevelingSystem.add_record()`, but that is discouraged because it is better to discard information that is no longer in use (the user is no longer in the guild)
+
+<div align="left"><sub>EXAMPLE</sub></div>
+
+```py
+# leveling_system.json
+[
+  {
+      "5748392849348934" : {
+          "xp" : 373,
+          "level" : 4
+      }
+  },
+  {
+      "89283659820948923" : {
+          "xp" : 23,
+          "level" : 1
+      }
+  }
+]
+
+
+# bot.py
+import json
+from discord.ext import commands
+from discordLevelingSystem import DiscordLevelingSystem
+
+bot = commands.Bot(...)
+
+lvl = DiscordLevelingSystem(...)
+lvl.connect_to_database_file(...)
+
+def json_to_dict() -> dict:
+    with open('leveling_system.json') as fp:
+        data = json.load(fp)
+        formatted: Dict[int, int] = ... # format the data so all keys and values are associated with the user ID and level
+        
+        """
+        In the end, the formatted dict should look like so:
+        
+        formatted = {
+            5748392849348934 : 4,
+            89283659820948923 : 1
+        }
+        """
+        return formatted
+
+@bot.command()
+async def insert(ctx):
+    await lvl.insert(ctx.bot, guild_id=12345678901234, users=json_to_dict(), using='levels')
+
+bot.run(...)
+```
+
+</details>
```

### Comparing `discordLevelingSystem-1.2.0/README.md` & `discordLevelingSystem-1.2.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,837 +1,861 @@
-A library to implement a leveling system into a discord bot. One of the most popular discord bots out there is MEE6 and it's leveling system. This library provides ways to easily implement one for yourself. It uses SQLite (aiosqlite) to locally query things such as their XP, rank, and level. Various amounts of other methods and classes are also provided so you can access or remove contents from the database file.
-
-<!-- ## Installing
-You can install the latest [PyPI version](https://pypi.org/project/discordLevelingSystem/) of the library by doing:
-
-`$ pip install discordLevelingSystem`
-
-Or the development version:
-
-`$ pip install git+https://github.com/Defxult/discordLevelingSystem` -->
-
----
-
-## Showcase
-![showcase](https://cdn.discordapp.com/attachments/655186216060321816/835010159092039680/leveling_showcase.gif)
-
----
-## How to import
-```py
-from discordLevelingSystem import DiscordLevelingSystem, LevelUpAnnouncement, RoleAward
-```
-
----
-## Intents
-[Intents](https://discordpy.readthedocs.io/en/stable/intents.html) are required for proper functionality
-```py
-bot = commands.Bot(..., intents=discord.Intents(messages=True, guilds=True, members=True))
-```
----
-
-
-## DiscordLevelingSystem
-```class DiscordLevelingSystem(rate=1, per=60.0, awards=None, **kwargs)```
-
----
-### Parameters of the DiscordLevelingSystem constructor
-* `rate` (`int`) The amount of messages each member can send before the cooldown triggers
-* `per` (`float`) The amount of seconds each member has to wait before gaining more XP, aka the cooldown
-* `awards` (`Optional[Dict[int, List[RoleAward]]]`) The role given to a member when they reach a `RoleAward` level requirement
----
-### Kwargs of the DiscordLevelingSystem constructor
-| Name | Type | Default Value | Info
-|------|------|---------------|-----
-| `no_xp_roles` | `Sequence[int]` | `None` | A sequence of role ID's. Any member with any of those roles will not gain XP when sending messages
-| `no_xp_channels` | `Sequence[int]` | `None` | A sequence of text channel ID's. Any member sending messages in any of those text channels will not gain XP
-| `announce_level_up` | `bool` | `True` | If `True`, level up messages will be sent when a member levels up
-| `stack_awards` | `bool` | `True` | If this is `True`, when the member levels up the assigned role award will be applied. If `False`, the previous role award will be removed and the level up assigned role will also be applied
-| `level_up_announcement` | `Union[LevelUpAnnouncement, Sequence[LevelUpAnnouncement]]` | `LevelUpAnnouncement()` | The message that is sent when someone levels up. If this is a sequence of `LevelUpAnnouncement`, one is selected at random
-|`bot` | ` Union[AutoShardedBot, Bot]` | `None` | Your bot instance variable. Used only if you'd like to use the `on_dls_level_up` event
-
----
-### Attributes
-* `no_xp_roles`
-* `no_xp_channels`
-* `announce_level_up`
-* `stack_awards`
-* `level_up_announcement`
-* `bot`
-* `rate` (`int`) Read only property from the constructor
-* `per` (`float`) Read only property from the constructor
-* `database_file_path` (`str`) Read only property
-* `active` (`bool`) Enable/disable the leveling system. If `False`, nobody can gain XP when sending messages unless this is set back to `True`
-
-> NOTE: All attributes can be set during initialization
----
-## Initial Setup
-When setting up the leveling system, a database file needs to be created in order for the library to function. 
-* Associated static method
-  * `DiscordLevelingSystem.create_database_file(path: str)`
-
-The above static method is used to create the database file for you in the path you specify. This method only needs to be called once. Example:
-```py
-DiscordLevelingSystem.create_database_file(r'C:\Users\Defxult\Documents')
-```
-Once created, there is no need to ever run that method again unless you want to create a new database file from scratch. Now that you have the database file, you can use the leveling system.
-
----
-## Connecting to the Database
-* Associated method
-  * `DiscordLevelingSystem.connect_to_database_file(path: str)`
-
-Since the database file has already been created, all you need to do is connect to it. 
-> NOTE: When connecting to the database file, the event loop must not be running
-<div align="left"><sub>EXAMPLE</sub></div>
-
-```py
-from discord.ext import commands
-from discordLevelingSystem import DiscordLevelingSystem
-
-bot = commands.Bot(...)
-lvl = DiscordLevelingSystem()
-lvl.connect_to_database_file(r'C:\Users\Defxult\Documents\DiscordLevelingSystem.db')
-
-bot.run(...)
-```
----
-
-## RoleAward
-```class RoleAward(role_id: int, level_requirement: int, role_name=None)```
-
-You can assign roles to the system so when someone levels up to a certain level, they are given that role. `RoleAward` is how that is accomplished.
-
----
-### Parameters of the RoleAward constructor
-* `role_id` (`int`) ID of the role that is to be awarded.
-* `level_requirement` (`int`) What level is required for a member to be awarded the role.
-* `role_name` (`Optional[str]`) A name you can set for the award. Nothing is done with this value, it is used for visual identification purposes only.
----
-### Attributes
-* `role_id`
-* `level_requirement`
-* `role_name`
-* `mention` (`str`) The discord role mention string
-
-When creating role awards, all role IDs and level requirements must be unique. Level requirements must also be in ascending order. It is also possible to assign different role awards for different guilds. If you don't want any role awards, set the `awards` parameter to `None`. When setting `awards`, it accepts a `dict` where the keys are guild IDs and the values are a `list` of `RoleAward`
-<div align="left"><sub>EXAMPLE</sub></div>
-
-```py
-from discordLevelingSystem import DiscordLevelingSystem, RoleAward
-
-johns_server = 587937522043060224
-janes_server = 850809412011950121
-
-my_awards = {
-    johns_server : [
-        RoleAward(role_id=831672678586777601, level_requirement=1, role_name='Rookie'),
-        RoleAward(role_id=831672730583171073, level_requirement=2, role_name='Associate'),
-        RoleAward(role_id=831672814419050526, level_requirement=3, role_name='Legend')
-    ],
-    janes_server : [
-        RoleAward(role_id=851400453904400385, level_requirement=1, role_name='Silver'),
-        RoleAward(role_id=851379776111116329, level_requirement=2, role_name='Gold'),
-        RoleAward(role_id=851959077071880202, level_requirement=3, role_name='Diamond')
-    ]
-}
-
-lvl = DiscordLevelingSystem(..., awards=my_awards)
-```
----
-
-## LevelUpAnnouncement
-```class LevelUpAnnouncement(message=default_message, level_up_channel_ids=None, allowed_mentions=default_mentions, tts=False, delete_after=None)```
-
-Level up announcements are for when you want to implement your own level up messages. It provides access to who leveled up, their rank, level and much more. It also uses some of discord.py's kwargs from it's `Messageable.send` such as `allowed_mentions`, `tts`, and `delete_after` to give you more control over the sent message.
-
----
-### Parameters of the LevelUpAnnouncement constructor
-
-* `message` (`Union[str, discord.Embed]`) The message that is sent when someone levels up. Defaults to `"<mention>, you are now **level <level>!**"`
-
-* `level_up_channel_ids` (`Optional[Sequence[int]]`) The text channel IDs where all level up messages will be sent for each server. If `None`, the level up message will be sent in the channel where they sent the message (example below).
-
-* `allowed_mentions` (`discord.AllowedMentions`) Used to determine who can be pinged in the level up message. Defaults to `discord.AllowedMentions(everyone=False, users=True, roles=False, replied_user=False)`
-
-* `tts` (`bool`) When the level up message is sent, have discord read the level up message aloud.
-
-* `delete_after` (`Optional[float]`) Delete the level up message after an x amount of seconds.
-
-### Class Attributes
-The `LevelUpAnnouncement` class provides a set of markdown attributes for you to use so you can access certain information in a level up message.
-
-* `LevelUpAnnouncement.TOTAL_XP` The members current total XP amount
-* `LevelUpAnnouncement.LEVEL` The members current level
-* `LevelUpAnnouncement.RANK` The members current rank
-
-The below markdown attributes takes the information from a `discord.Member` object so you can access member information in the level up message.
-
-* `LevelUpAnnouncement.Member.avatar_url`
-* `LevelUpAnnouncement.Member.banner_url`
-* `LevelUpAnnouncement.Member.created_at`
-* `LevelUpAnnouncement.Member.default_avatar_url`
-* `LevelUpAnnouncement.Member.discriminator`
-* `LevelUpAnnouncement.Member.display_avatar_url`
-* `LevelUpAnnouncement.Member.display_name`
-* `LevelUpAnnouncement.Member.id`
-* `LevelUpAnnouncement.Member.joined_at`
-* `LevelUpAnnouncement.Member.mention`
-* `LevelUpAnnouncement.Member.name`
-* `LevelUpAnnouncement.Member.nick`
-* `LevelUpAnnouncement.Member.Guild.icon_url`
-* `LevelUpAnnouncement.Member.Guild.id`
-* `LevelUpAnnouncement.Member.Guild.name`
-
-<div align="left"><sub>EXAMPLE</sub></div>
-
-```py
-from discordLevelingSystem import DiscordLevelingSystem, LevelUpAnnouncement
-
-embed = discord.Embed()
-embed.set_author(name=LevelUpAnnouncement.Member.name, icon_url=LevelUpAnnouncement.Member.avatar_url)
-embed.description = f'Congrats {LevelUpAnnouncement.Member.mention}! You are now level {LevelUpAnnouncement.LEVEL} 😎'
-
-announcement = LevelUpAnnouncement(embed)
-
-lvl = DiscordLevelingSystem(..., level_up_announcement=announcement)
-
-# NOTE: You can have multiple level up announcements by setting the parameter to a sequence of LevelUpAnnouncement
-lvl = DiscordLevelingSystem(..., level_up_announcement=[announcement_1, announcement_2, ...])
-```
-When it comes to `level_up_channel_ids`, you can set a designated channel for each server. If you don't set a level up channel ID for a specific server, the level up message will be sent in the channel where the member leveled up. You don't have to specify a level up channel ID for each server unless you'd like to.
-```py
-johns_bot_commands = 489374746737648734 # text channel ID from server A
-janes_levelup_channel = 58498304930493094 # text channel ID from server B
-
-announcement = LevelUpAnnouncement(..., level_up_channel_ids=[johns_bot_commands, janes_levelup_channel])
-lvl = DiscordLevelingSystem(..., level_up_announcement=announcement)
-```
----
-## Handling XP
-Method `award_xp` is how members gain XP. This method is placed inside the `on_message` event of your bot. Members will gain XP if they send a message and if they're *not* on cooldown. Spamming messages will not give them XP.
-> NOTE: Members cannot gain XP in DM's
-* Associated methods
-  * `await DiscordLevelingSystem.add_xp(member: Member, amount: int)`
-  * `await DiscordLevelingSystem.remove_xp(member: Member, amount: int)`
-  * `await DiscordLevelingSystem.set_level(member: Member, level: int)`
-  * `await DiscordLevelingSystem.award_xp(*, amount=[15, 25], message: Message, refresh_name=True, **kwargs)`
-
-
-### Parameters for award_xp
-* `amount` (`Union[int, Sequence[int]]`) The amount of XP to award to the member per message. Must be from 1-25. Can be a sequence with a minimum and maximum length of two. If `amount` is a sequence of two integers, it will randomly pick a number in between those numbers including the numbers provided.
-* `message` (`discord.Message`) A discord message object
-* `refresh_name` (`bool`) Everytime the member sends a message, check if their name still matches the name in the database. If it doesn't match, update the database to match their current name. It is suggested to leave this as `True` so the database can always have the most up-to-date record.
-
-### Kwargs for award_xp
-* `bonus` (`DiscordLevelingSystem.Bonus`) Used to set the roles that will be awarded bonus XP.
-  * `class Bonus(role_ids: Sequence[int], bonus_amount: int, multiply: bool)`
-  * **Parameters of the DiscordLevelingSystem.Bonus constructor**
-    * `role_ids` (`Sequence[int]`) The role(s) a member must have to be able to get bonus XP. They only need to have one of these roles to get the bonus
-    * `bonus_amount` (`int`) Amount of extra XP to be awarded
-    * `multiply` (`bool`) If set to `True`, this will operate on a x2, x3 basis. Meaning if you have the awarded XP amount set to 10 and you want the bonus XP role to be awarded 20, it must be set to 2, not 10. If `False`, it operates purely on the given value. Meaning if you have the awarded XP set to 10 and you want the bonus XP role to be awarded 20, it must be set to 10.
-
-<div align="left"><sub>EXAMPLE</sub></div>
-
-```py
-lvl = DiscordLevelingSystem(...)
-
-nitro_booster = 851379776111116329
-associate_role = 851400453904400385
-
-@bot.event
-async def on_message(message):
-    await lvl.award_xp(amount=[15, 25], message=message, bonus=DiscordLevelingSystem.Bonus([nitro_booster, associate_role], 20, multiply=False))
-```
----
-
-## MemberData
-Accessing the raw information inside the database file can look a bit messy if you don't know exactly what you're looking at. To make things easier, this library comes with the `MemberData` class. A class which returns information about a specific member in the database.
-
-* Associated methods
-  * `await DiscordLevelingSystem.get_data_for(member: Member) -> MemberData`
-  * `await DiscordLevelingSystem.each_member_data(guild: Guild, sort_by=None, limit=None) -> List[MemberData]`
-
-### Attributes
-* `id_number` (`int`) The members ID
-* `name` (`str`) The members name
-* `level` (`int`) The members level
-* `xp` (`int`) The members xp
-* `total_xp` (`int`) The members total xp
-* `rank` (`Optional[int]`) The members rank
-* `mention` (`str`) The discord member mention string
-
-### Methods
-* `MemberData.to_dict() -> dict`
-
-<div align="left"><sub>EXAMPLE</sub></div>
-
-```py
-lvl = DiscordLevelingSystem(...)
-
-@bot.command()
-async def rank(ctx):
-    data = await lvl.get_data_for(ctx.author)
-    await ctx.send(f'You are level {data.level} and your rank is {data.rank}')
-
-@bot.command()
-async def leaderboard(ctx):
-    data = await lvl.each_member_data(ctx.guild, sort_by='rank')
-    # show the leaderboard whichever way you'd like
-```
----
-## Events
-You can set an event to be called when a member levels up. Using the event is considered as an enhanced `LevelUpAnnouncement` because it provides more capabilities rather than simply sending a message with only text/an embed. The `on_dls_level_up` event takes three parameters:
-* `member` (`discord.Member`) The member that leveled up
-* `message` (`discord.Message`) The message that triggered the level up
-* `data` (`MemberData`) The database information for that member
-
-```py
-bot = commands.Bot(...)
-lvl = DiscordLevelingSystem(..., bot=bot) # your bot instance variable is needed
-
-@bot.event
-async def on_dls_level_up(member: discord.Member, message: discord.Message, data: MemberData):
-    # You can do a lot more here compared to LevelUpAnnouncement
-    # - create a level up image and send it with discord.File
-    # - call additional functions that you may need
-    # - access to all attributes/methods that are available within discord.Member and discord.Message
-```
-> NOTE: `LevelUpAnnouncement` and `on_dls_level_up` are not the same. Level up messages are sent by default by the library. If you'd like to only use `on_dls_level_up`, you need to disable level up announcements (`lvl.announce_level_up = False`)
-
----
-## Full Example
-With all classes and core methods introduced, here is a basic implementation of this library.
-```py
-from discord.ext import commands
-from discordLevelingSystem import DiscordLevelingSystem, RoleAward, LevelUpAnnouncement
-
-bot = commands.Bot(...)
-
-main_guild_id = 850809412011950121
-
-my_awards = {
-    main_guild_id : [
-        RoleAward(role_id=831672678586777601, level_requirement=1, role_name='Rookie'),
-        RoleAward(role_id=831672730583171073, level_requirement=2, role_name='Associate'),
-        RoleAward(role_id=831672814419050526, level_requirement=3, role_name='Legend')
-    ]
-}
-
-announcement = LevelUpAnnouncement(f'{LevelUpAnnouncement.Member.mention} just leveled up to level {LevelUpAnnouncement.LEVEL} 😎')
-
-# DiscordLevelingSystem.create_database_file(r'C:\Users\Defxult\Documents') database file already created
-lvl = DiscordLevelingSystem(awards=my_awards, level_up_announcement=announcement)
-lvl.connect_to_database_file(r'C:\Users\Defxult\Documents\DiscordLevelingSystem.db')
-
-@bot.event
-async def on_message(message):
-    await lvl.award_xp(amount=15, message=message)
-
-bot.run(...)
-```
----
-
-## All methods for DiscordLevelingSystem
-<details>
-    <summary>Click to show all methods</summary>
-
-* *await* **add_record**(`guild_id, member_id, member_name, level`) - Manually add a record to the database. If the record already exists (the `guild_id` and `member_id` was found), only the level will be updated. If there were no records that matched those values, all provided information will be added
-  * **Parameters**
-    * **guild_id** (`int`) The guild ID to register
-    * **member_id** (`int`) The member ID to register
-    * **member_name** (`str`) The member name to register
-    * **level** (`int`) The member level to register. Must be from 0-100
-  * **Raises**
-    * `DiscordLevelingSystemError` - The value given from a parameter was not of the correct type or "level" was not 0-100
-
-
-* *await* **add_xp**(`member, amount`) - Give XP to a member. This also changes their level so it matches the associated XP
-  * **Parameters**
-    * **member** (`discord.Member`) The member to give XP to
-    * **amount** (`int`) Amount of XP to give to the member
-  * **Raises**
-    * `DatabaseFileNotFound` - The database file was not found
-    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
-    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
-    * `NotConnected` - Attempted to use a method that requires a connection to a database file
-    * `DiscordLevelingSystemError` - Parameter "amount" was less than or equal to zero. The minimum value is 1 
-
-
-* *await* **award_xp**(`*, amount = [15, 25], message, refresh_name = True, **kwargs`) - Give XP to the member that sent a message
-  * **Parameters**
-    * **amount** (`Union[int, Sequence[int]]`)
-    * **message** (`discord.Message`) A message object
-    * **refresh_name** (`bool`) Everytime the member sends a message, check if their name still matches the name in the database. If it doesn't match, update the database to match their current name. It is suggested to leave this as `True` so the database can always have the most up-to-date record
-  * **Kwargs**
-    * **bonus** (`DiscordLevelingSystem.Bonus`) Set the bonus values. Read the `DiscordLevelingSystem.Bonus` doc string for more details (defaults to `None`)
-  * **Raises**
-    * `DatabaseFileNotFound` - The database file was not found
-    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
-    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
-    * `NotConnected` - Attempted to use a method that requires a connection to a database file
-
-
-* **backup_database_file**(`path, with_timestamp = False`) - Create a copy of the database file to the specified path. If a copy of the backup file is already in the specified path it will be overwritten
-  * **Parameters**
-    * **path** (`str`) The path to copy the database file to
-    * **with_timestamp** (`bool`) Creates a unique file name that has the date and time of when the backup file was created. This is useful when you want multiple backup files
-  * **Raises**
-    * `DiscordLevelingSystemError` - Path doesn't exist or points to another file
-    * `NotConnected` - Attempted to use a method that requires a connection to a database file
-
-
-* *await* **change_cooldown**(`rate, per`) - Update the cooldown rate
-  * **Parameters**
-    * **rate** (`int`) The amount of messages each member can send before the cooldown triggers
-    * **per** (`float`) The amount of seconds each member has to wait before gaining more XP, aka the cooldown
-  * **Raises**
-    * `DatabaseFileNotFound` - The database file was not found
-    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
-    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
-    * `NotConnected` - Attempted to use a method that requires a connection to a database file
-    * `DiscordLevelingSystemError` - The rate or per value was not greater than zero
-
-
-* *await* **clean_database**(`guild`) - Removes the data for members that are no longer in the guild, thus reducing the database file size. It is recommended to have this method in a background loop in order to keep the database file free of records that are no longer in use
-  * **Parameters**
-    * **guild** (`discord.Guild`) The guild records to clean
-  * **Returns**
-    * (`Optional[int]`) The amount of records that were removed from the database
-  * **Raises**
-    * `DatabaseFileNotFound` - The database file was not found
-    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
-    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
-    * `NotConnected` - Attempted to use a method that requires a connection to a database file
-
-
-* **connect_to_database_file**(`path`) - Connect to the existing database file in the specified path
-  * **Parameters**
-    * **path** (`str`) The location of the database file
-  * **Raises**
-    * `ConnectionFailure` - Attempted to connect to the database file when the event loop is already running
-    * `DatabaseFileNotFound` - The database file was not found
-
-
-* *static method* **create_database_file**(`path = None`) - Create the database file and implement the SQL data for the database
-  * **Parameters**
-    * **path** (`Optional[str]`) The location to create the database file. If `None`, the file is created in the current working directory
-  * **Raises**
-    * `ConnectionFailure` - Attempted to create the database file when the event loop is already running
-    * `DiscordLevelingSystemError` - The path does not exist or the path points to a file instead of a directory
-
-
-* *await* **each_member_data**(`guild, sort_by = None, limit = None`) - Return each member in the database as a `MemberData` object for easy access to their XP, level, etc. You can sort the data with `sort_by` with the below values
-  * **Parameters**
-    * **guild** (`discord.Guild`) A guild object
-    * **sort_by** (`Optional[str]`) Return each member sorted by: "name", "level", "xp", "rank". If `None`, it will return in the order they were added to the database
-    * **limit** (`Optional[int]`) Restrict the amount of records returned to the specified amount
-  * **Returns**
-    * `List[MemberData]`
-  * **Raises**
-    * `DatabaseFileNotFound` - The database file was not found
-    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
-    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
-    * `NotConnected` - Attempted to use a method that requires a connection to a database file
-    * `DiscordLevelingSystemError` - The value of `sort_by` was not recognized or `guild` was not of type `discord.Guild`
-
-
-* *await* **export_as_json**(`path, guild`) - Export a json file that represents the database to the path specified
-  * **Parameters**
-    * **path** (`str`) Path to copy the json file to
-    * **guild** (`discord.Guild`) The guild for which the data should be extracted from. If `None`, all guild information will be extracted from the database
-  * **Raises**
-    * `DatabaseFileNotFound` - The database file was not found
-    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
-    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
-    * `NotConnected` - Attempted to use a method that requires a connection to a database file
-    * `DiscordLevelingSystemError` - The path does not exist or does not point to a directory
-
-
-* **get_awards**(`guild = None`) - Get all `RoleAward`'s or only the `RoleAward`'s assigned to the specified guild
-  * **Parameters**
-    * **guild** (`Optional[Union[discord.Guild, int]]`) A guild object or a guild ID
-  * **Returns**
-    * (`Union[Dict[int, List[RoleAward]], List[RoleAward]]`) If `guild` is `None`, this return the awards `dict` that was set in constructor. If `guild` is specified, it returns a List[`RoleAward`] that matches the specified guild ID. Can also return `None` if awards were never set or if the awards for the specified guild was not found
-
-
-* *await* **get_data_for**(`member`) - Get the `MemberData` object that represents the specified member
-  * **Parameters**
-    * **member** (`discord.Member`) The member to get the data for
-  * **Returns**
-    * (`MemberData`) Can be `None` if the member isn't in the database
-  * **Raises**
-    * `DatabaseFileNotFound` - The database file was not found
-    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
-    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
-    * `NotConnected` - Attempted to use a method that requires a connection to a database file
-
-
-* *await* **get_level_for**(`member`) - Get the level for the specified member
-  * **Parameters**
-    * **member** (`discord.Member`) Member to get the level for
-  * **Returns**
-    * (`int`) Can be `None` if the member isn't in the database
-  * **Raises**
-    * `DatabaseFileNotFound` - The database file was not found
-    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
-    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
-    * `NotConnected` - Attempted to use a method that requires a connection to a database file
-
-
-* *await* **get_rank_for**(`member`) - Get the rank for the specified member
-  * **Parameters**
-    * **member** (`discord.Member`) Member to get the rank for
-  * **Returns**
-    * (`int`) Can be `None` if the member isn't ranked yet
-  * **Raises**
-    * `DatabaseFileNotFound` - The database file was not found
-    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
-    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
-    * `NotConnected` - Attempted to use a method that requires a connection to a database file
-
-
-* *await* **get_record_count**(`guild = None`) - Get the amount of members that are registered in the database. If `guild` is set to `None`, ALL members in the database will be counted
-  * **Parameters**
-    * **guild** (`Optional[discord.Guild]`) The guild for which to count the amount of records
-  * **Returns**
-    * (`int`)
-  * **Raises**
-    * `DatabaseFileNotFound` - The database file was not found
-    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
-    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
-    * `NotConnected` - Attempted to use a method that requires a connection to a database file
-
-
-* *await* **get_total_xp_for**(`member`) - Get the total XP for the specified member
-  * **Parameters**
-    * **member** (`discord.Member`) Member to get the total XP for
-  * **Returns**
-    * (`int`) Can be `None` if the member isn't in the database
-  * **Raises**
-    * `DatabaseFileNotFound` - The database file was not found
-    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
-    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
-    * `NotConnected` - Attempted to use a method that requires a connection to a database file
-
-
-* *await* **get_xp_for**(`member`) - Get the XP for the specified member
-  * **Parameters**
-    * **member** (`discord.Member`) Member to get the XP for
-  * **Returns**
-    * (`int`) Can be `None` if the member isn't in the database
-  * **Raises**
-    * `DatabaseFileNotFound` - The database file was not found
-    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
-    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
-    * `NotConnected` - Attempted to use a method that requires a connection to a database file
-
-
-* *static method* **get_xp_for_level**(`level`) - Returns the total amount of XP needed for the specified level. Levels go from 0-100
-  * **Parameters**
-    * **level** (`int`) The level XP information to retrieve
-  * **Returns**
-    * (`int`)
-  * **Raises**
-    * `DiscordLevelingSystemError` - The level specified does not exist
-
-
-* *await* **insert**(`bot, guild_id, users, using, overwrite = False, show_results = True`) - Insert the records from your own leveling system into the library. A lot of leveling system tutorials out there use json files to store information. Although it might work, it is insufficient because json files are not made to act as a database. Using an actual database file has many benefits over a json file
-  * **Parameters**
-    * **bot** (`Union[discord.ext.commands.Bot, discord.ext.commands.AutoShardedBot]`) Your bot instance variable
-    * **guild_id** (`int`) ID of the guild that you used your leveling system with
-    * **users** (`Dict[int, int]`) This is the information that will be added to the database. The keys are user ID's, and the values are the users total XP or level. Note: This library only uses levels 0-100 and XP 0-1899250. If any number in this dict are over the levels/XP threshold, it is implicitly set back to this libraries maximum value
-    * **using** (`str`) What structure your leveling system used. Options: "xp" or "levels". Some leveling systems give users only XP and they are ranked up based on that XP value. Others use a combination of levels and XP. If all the values in the `users` dict are based on XP, set this to "xp". If they are based on a users level, set this to "levels"
-    * **overwrite** (`bool`) If a user you've specified in the `users` dict already has a record in the database, overwrite their current record with the one your inserting
-    * **show_results** (`bool`) Print the results for how many of the `users` were successfully added to the database file. If any are unsuccessful, their ID along with the value you provided will also be shown
-  * **Raises**
-      * `DiscordLevelingSystemError` - The value given from a parameter was not of the correct type. The `users` dict was empty. Or your bot is not in the guild associated with `guild_id`       
-
-
-* *await* **is_in_database**(`member, guild = None`) - A quick check to see if a member is in the database. This is not guild specific although it can be if `guild` is specified
-  * **Parameters**
-    * **member** (`Union[discord.Member, int]`) The member to check for. Can be the member object or that members ID
-    * **guild** (`Optional[discord.Guild]`) The guild to check if the member is registered in
-  * **Returns**
-    * (`bool`)
-  * **Raises**
-    * `DatabaseFileNotFound` - The database file was not found
-    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
-    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
-    * `NotConnected` - Attempted to use a method that requires a connection to a database file
-    * `DiscordLevelingSystemError` - Parameter `member` was not of type `discord.Member` or `int`
-
-
-* *static method* **levels_and_xp**( ) -  Get the raw `dict` representation for the amount of levels/XP in the system. The keys in the `dict` returned is each level, and the values are the amount of XP needed to be awarded that level
-  * **Returns**
-    * (`Dict[str, int]`)
-
-
-* *await* **next_level**(`member`) - Get the next level for the specified member
-  * **Parameters**
-    * **member** (`discord.Member`) Member to get the next level for
-  * **Returns**
-    * (`int`) If the member is currently max level (100), it will return 100. This can also return `None` if the member is not in the database
-  * **Raises**
-    * `DatabaseFileNotFound` - The database file was not found
-    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
-    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
-    * `NotConnected` - Attempted to use a method that requires a connection to a database file
-
-
-* *await* **next_level_up**(`member`) - Get the amount of XP needed for the specified member to level up
-  * **Parameters**
-    * **member** (`discord.Member`) Member to get the amount of XP needed for a level up
-  * **Returns**
-    * (`int`) Returns 0 if the member is currently at max level. Can return `None` if the member is not in the database.
-  * **Raises**
-    * `DatabaseFileNotFound` - The database file was not found
-    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
-    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
-    * `NotConnected` - Attempted to use a method that requires a connection to a database file
-
-
-* *await* **raw_database_contents**(`guild = None`) - Returns everything in the database. Can specify which guild information will be extracted
-  * **Parameters**
-    * **guild** (`Optional[discord.Guild]`) The guild to extract the raw database contents from. If `None`, information about all guilds will be extracted
-  * **Returns**
-    * `List[Tuple[int, int, str, int, int, int]]` The tuples inside the list represents each row of the database:
-      * Index 0 is the guild ID
-      * Index 1 is their ID
-      * Index 2 is their name
-      * Index 3 is their level
-      * Index 4 is their XP
-      * Index 5 is their total xp
-      * Can be an empty list if nothing is in the database
-  * **Raises**
-    * `DatabaseFileNotFound` - The database file was not found
-    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
-    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
-    * `NotConnected` - Attempted to use a method that requires a connection to a database file
-
-
-* *await* **refresh_names**(`guild`) - Update names inside the database. This does not add anything new. It simply verifies if the name in the database matches their current name, and if they don't match, update the database name
-  * **Parameters**
-    * **guild** (`discord.Guild`) A guild object
-  * **Returns**
-    * `(Optional[int])` The amount of records in the database that were updated
-  * **Raises**
-    * `DatabaseFileNotFound` - The database file was not found
-    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
-    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
-    * `NotConnected` - Attempted to use a method that requires a connection to a database file
-
-
-* *await* **remove_from_database**(`member, guild = None`) - Remove a member from the database. This is not guild specific although it can be if `guild` is specified
-  * **Parameters**
-    * **member** (`Union[discord.Member, int]`) The member to remove. Can be the member object or that members ID
-    * **guild** (`Optional[discord.Guild]`) If this parameter is given, it will remove the record of the specified member only from the specified guild record. If `None`, it will remove all records no matter the guild
-  * **Returns**
-    * (`Optional[bool]`) Returns `True` if the member was successfully removed from the database. `False` if the member was not in the database so there was nothing to remove
-  * **Raises**
-      * `DatabaseFileNotFound` - The database file was not found
-      * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
-      * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
-      * `DiscordLevelingSystemError` - Parameter `member` was not of type `discord.Member` or `int`
-      * `NotConnected` - Attempted to use a method that requires a connection to a database file
-
-
-* *await* **remove_xp**(`member, amount`) - Remove XP from a member. This also changes their level so it matches the associated XP
-  * **Parameters**
-      * **member** (`discord.Member`) The member to remove XP from
-      * **amount** (`int`) Amount of XP to remove from the member
-  * **Raises**
-    * `DatabaseFileNotFound` - The database file was not found
-    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
-    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
-    * `NotConnected` - Attempted to use a method that requires a connection to a database file
-    * `DiscordLevelingSystemError` - Parameter "amount" was less than or equal to zero. The minimum value is 1
-
-
-* *await* **reset_everyone**(`guild, *, intentional = False`) - Sets EVERYONES XP, total XP, and level to zero in the database. Can specify which guild to reset
-  * **Parameters**
-      * **guild** (`Union[discord.Guild, None]`) The guild for which everyone will be reset. If this is set to `None`, everyone in the entire database will be reset
-      * **intentional** (`bool`) A simple kwarg to try and ensure that this action is indeed what you want to do. Once executed, this cannot be undone
-  * **Raises**
-    * `DatabaseFileNotFound` - The database file was not found
-    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
-    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
-    * `NotConnected` - Attempted to use a method that requires a connection to a database file
-    * `FailSafe` - "intentional" argument for this method was set to `False` in case you called this method by mistake
-
-
-* *await* **reset_member**(`member`) - Sets the members XP, total XP, and level to zero
-  * **Parameters**
-    * **member** (`discord.Member`) The member to reset
-  * **Raises**
-    * `DatabaseFileNotFound` The database file was not found
-    * `LeaderboardNotFound` Table "leaderboard" in the database file is missing
-    * `ImproperLeaderboard` Leaderboard table was altered. Components changed or deleted
-    * `NotConnected` Attempted to use a method that requires a connection to a database file
-
-
-* *await* **set_level**(`member, level`) - Sets the level for the member. This also changes their total XP so it matches the associated level
-  * **Parameters**
-    * **member** (`discord.Member`) The member who's level will be set
-    * **level** (`int`) Level to set. Must be from 0-100     
-  * **Raises**
-    * `DatabaseFileNotFound` - The database file was not found
-    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
-    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
-    * `NotConnected` - Attempted to use a method that requires a connection to a database file
-    * `DiscordLevelingSystemError` - Parameter "level" was not from 0-100
-
-
-* *await* **sql_query_get**(`sql, parameters = None, fetch = 'ALL'`) - Query and return something from the database using SQL. The following columns are apart of the "leaderboard" table: guild_id, member_id, member_name, member_level, member_xp, member_total_xp
-  * **Parameters**
-    * **sql** (`str`) SQL string used to query the database
-    * **parameters** (`Optional[Tuple[Union[str ,int]]]`) The parameters used for the database query
-    * **fetch** (`Union[str, int]`) The amount of rows you would like back from the query. Options: 'ALL', 'ONE', or an integer value that is greater than zero
-  * **Returns**
-    * (`Union[List[tuple], tuple]`)
-      * Using `fetch='ALL'` returns `List[tuple]`
-      * Using `fetch='ONE'` returns `tuple`
-      * Using `fetch=4` returns `List[tuple]` with only four values
-      * Can also return an empty list if the query was valid but got nothing from it
-  * **Raises**
-    * `DatabaseFileNotFound` - The database file was not found
-    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
-    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
-    * `NotConnected` - Attempted to use a method that requires a connection to a database file
-    * `DiscordLevelingSystemError` - Argument "fetch" was the wrong type or used an invalid value
-    * `aiosqlite.Error` - Base aiosqlite error. Multiple errors can arise from this if the SQL query was invalid
-
-
-* *await* **switch_connection**(`path`) - Connect to a different leveling system database file
-  * **Parameters**
-    * **path** (`str`) The location of the database file
-  * **Raises**
-    * `DatabaseFileNotFound` - The database file was not found
-
-
-* *static method* **transfer**(`old, new, guild_id`) - Transfer the database records from a database file created from v0.0.1 to a blank database file created using v0.0.2+. If you were already using a v0.0.2+ database file, there's no need to use this method
-  * **Parameters**
-    * **old** (`str`) The path of the v0.0.1 database file
-    * **new** (`str`) The path of the v0.0.2+ database file
-    * **guild_id** (`int`) ID of the guild that was originally used with this library
-  * **Raises**
-    - `ConnectionFailure` - The event loop is already running
-    - `DatabaseFileNotFound` - "old" or "new" database file was not found
-    - `DiscordLevelingSystemError` - One of the databases is missing the "leaderboard" table. A v0.0.2+ database file contains records, or there was an attempt to transfer records from a v0.0.2+ file to another v0.0.2+ file
-
-
-* *await* **wipe_database**(`guild = None, *, intentional = False`) - Delete EVERYTHING from the database. If `guild` is specified, only the information related to that guild will be deleted
-  * **Parameters**
-    * **guild** (`Optional[discord.Guild]`) The guild for which all information that is related to that guild will be deleted. If `None`, everything will be deleted
-    * **intentional** (`bool`) A simple kwarg to try and ensure that this action is indeed what you want to do. Once executed, this cannot be undone
-  * **Raises**
-    * `DatabaseFileNotFound` - The database file was not found
-    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
-    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
-    * `NotConnected` - Attempted to use a method that requires a connection to a database file
-    * `FailSafe` - "intentional" argument for this method was set to `False` in case you called this method by mistake
-
-</details>
-
-## Migrating from v0.0.1 to v0.0.2+
-<details>
-    <summary>Click to show details</summary>
-
-This library was not originally designed with the use of multiple servers in mind, so all the data you might have currently (your database file was created in `v0.0.1`) should be from a single server. With `v0.0.2`, the structure of the database file was changed to accommodate this fix. That means if you are currently using a `v0.0.1` database file and update to `v0.0.2+`, a vast majority of the library will be broken. To avoid this, you need to transfer all your `v0.0.1` database file records to a `v0.0.2+` database file. This can be done using the `transfer` method.
-
-* Associated static method
-  * `DiscordLevelingSystem.transfer(old: str, new: str, guild_id: int)`
-
-### Parameters
-* `old` (`str`) The path of the `v0.0.1` database file
-* `new` (`str`) The path of the `v0.0.2+` database file (a brand new file from using `DiscordLevelingSystem.create_database_file(path: str)`)
-* `guild_id` (`int`) ID of the guild that was originally used with this library
-
-<div align="left"><sub>EXAMPLE</sub></div>
-
-```py
-from discordLevelingSystem import DiscordLevelingSystem
-
-old = r'C:\Users\Defxult\Documents\DiscordLevelingSystem.db'
-new = r'C:\Users\Defxult\Desktop\DiscordLevelingSystem.db'
-
-DiscordLevelingSystem.transfer(old, new, guild_id=850809412011950121)
-```
-
-</details>
-
-## Inserting your own leveling system information
-<details>
-    <summary>Click to show details</summary>
-
-Insert the records from your leveling system into this one. A lot of leveling system tutorials out there use json files to store information. Although it might work, it is insufficient because json files are not made to act as a database. Using a database file has many benefits over a json file. If you previously watched a tutorial for your leveling system and would like to import your records over to use with this library, you can do so with the below method.
-
-* Associated static method
-  * `await DiscordLevelingSystem.insert(bot: Union[Bot, AutoShardedBot], guild_id: int, users: Dict[int, int], using: str, overwrite=False, show_results=True)`
-
-### Parameters
-- `bot` (`Union[discord.ext.commands.Bot, discord.ext.commands.AutoShardedBot]`) Your bot instance variable
-
-- `guild_id` (`int`) ID of the guild that you used your leveling system with
-
-- `users` (`Dict[int, int]`) This is the information that will be added to the database. The keys are user ID's, and the values are the users total XP or level. Note: This library only uses levels 0-100 and XP 0-1899250. If any number in this dict are over the levels/XP threshold, it is implicitly set back to this libraries maximum value
-
-- `using` (`str`) What structure your leveling system used. Options: "xp" or "levels". Some leveling systems give users only XP and they are ranked up based on that XP value. Others use a combination of levels and XP. If all the values in the `users` dict are based on XP, set this to "xp". If they are based on a users level, set this to "levels"
-
-- `overwrite` (`bool`) If a user you've specified in the `users` dict already has a record in the database, overwrite their current record with the one your inserting
-
-- `show_results` (`bool`) Print the results for how many of the `users` were successfully added to the database file. If any are unsuccessful, their ID along with the value you provided will also be shown
-
-> NOTE: If the users you've provided in the `users` dict is not currently in the guild (`guild_id`), their information will not be inserted. If you'd like, you can manually add those records with method `DiscordLevelingSystem.add_record()`, but that is discouraged because it is better to discard information that is no longer in use (the user is no longer in the guild)
-
-<div align="left"><sub>EXAMPLE</sub></div>
-
-```py
-# leveling_system.json
-[
-  {
-      "5748392849348934" : {
-          "xp" : 373,
-          "level" : 4
-      }
-  },
-  {
-      "89283659820948923" : {
-          "xp" : 23,
-          "level" : 1
-      }
-  }
-]
-
-
-# bot.py
-import json
-from discord.ext import commands
-from discordLevelingSystem import DiscordLevelingSystem
-
-bot = commands.Bot(...)
-
-lvl = DiscordLevelingSystem(...)
-lvl.connect_to_database_file(...)
-
-def json_to_dict() -> dict:
-    with open('leveling_system.json') as fp:
-        data = json.load(fp)
-        formatted: Dict[int, int] = ... # format the data so all keys and values are associated with the user ID and level
-        
-        """
-        In the end, the formatted dict should look like so:
-        
-        formatted = {
-            5748392849348934 : 4,
-            89283659820948923 : 1
-        }
-        """
-        return formatted
-
-@bot.command()
-async def insert(ctx):
-    await lvl.insert(ctx.bot, guild_id=12345678901234, users=json_to_dict(), using='levels')
-
-bot.run(...)
-```
-
-</details>
+Metadata-Version: 2.1
+Name: discordLevelingSystem
+Version: 1.2.1
+Summary: A library to implement a leveling system into a discord bot. Contains features such as XP, level, ranks, and role awards.
+Author: Defxult#8269
+License: MIT
+Project-URL: Homepage, https://github.com/Defxult/discordLevelingSystem
+Project-URL: Changelog, https://github.com/Defxult/discordLevelingSystem/blob/main/CHANGELOG.md
+Keywords: database,discord,discord bot,discord.py,discord py,discord level,discord leveling,discord leveling system,level,levels,leveling,level up,level system,mee6,rank,ranking,role award,xp
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+A library to implement a leveling system into a discord bot. One of the most popular discord bots out there is MEE6 and it's leveling system. This library provides ways to easily implement one for yourself. It uses SQLite ([aiosqlite](https://pypi.org/project/aiosqlite/)) to locally query things such as their XP, rank, and level. Various amounts of other methods and classes are also provided so you can access or remove contents from the database file.
+
+[![Downloads](https://pepy.tech/badge/discordlevelingsystem)](https://pepy.tech/project/discordlevelingsystem)
+[![Downloads](https://pepy.tech/badge/discordlevelingsystem/month)](https://pepy.tech/project/discordlevelingsystem)
+![python_version](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10-blue)
+
+## Installing
+You can install the latest [PyPI version](https://pypi.org/project/discordLevelingSystem/) of the library by doing:
+
+`$ pip install discordLevelingSystem`
+
+Or the development version:
+
+`$ pip install git+https://github.com/Defxult/discordLevelingSystem`
+
+---
+
+## Showcase
+![showcase](https://cdn.discordapp.com/attachments/655186216060321816/835010159092039680/leveling_showcase.gif)
+
+---
+## How to import
+```py
+from discordLevelingSystem import DiscordLevelingSystem, LevelUpAnnouncement, RoleAward
+```
+
+---
+## Intents
+[Intents](https://discordpy.readthedocs.io/en/stable/intents.html) are required for proper functionality
+```py
+bot = commands.Bot(..., intents=discord.Intents(messages=True, guilds=True, members=True))
+```
+---
+
+
+## DiscordLevelingSystem
+```class DiscordLevelingSystem(rate=1, per=60.0, awards=None, **kwargs)```
+
+---
+### Parameters of the DiscordLevelingSystem constructor
+* `rate` (`int`) The amount of messages each member can send before the cooldown triggers
+* `per` (`float`) The amount of seconds each member has to wait before gaining more XP, aka the cooldown
+* `awards` (`Optional[Dict[int, List[RoleAward]]]`) The role given to a member when they reach a `RoleAward` level requirement
+---
+### Kwargs of the DiscordLevelingSystem constructor
+| Name | Type | Default Value | Info
+|------|------|---------------|-----
+| `no_xp_roles` | `Sequence[int]` | `None` | A sequence of role ID's. Any member with any of those roles will not gain XP when sending messages
+| `no_xp_channels` | `Sequence[int]` | `None` | A sequence of text channel ID's. Any member sending messages in any of those text channels will not gain XP
+| `announce_level_up` | `bool` | `True` | If `True`, level up messages will be sent when a member levels up
+| `stack_awards` | `bool` | `True` | If this is `True`, when the member levels up the assigned role award will be applied. If `False`, the previous role award will be removed and the level up assigned role will also be applied
+| `level_up_announcement` | `Union[LevelUpAnnouncement, Sequence[LevelUpAnnouncement]]` | `LevelUpAnnouncement()` | The message that is sent when someone levels up. If this is a sequence of `LevelUpAnnouncement`, one is selected at random
+|`bot` | ` Union[AutoShardedBot, Bot]` | `None` | Your bot instance variable. Used only if you'd like to use the `on_dls_level_up` event
+
+---
+### Attributes
+* `no_xp_roles`
+* `no_xp_channels`
+* `announce_level_up`
+* `stack_awards`
+* `level_up_announcement`
+* `bot`
+* `rate` (`int`) Read only property from the constructor
+* `per` (`float`) Read only property from the constructor
+* `database_file_path` (`str`) Read only property
+* `active` (`bool`) Enable/disable the leveling system. If `False`, nobody can gain XP when sending messages unless this is set back to `True`
+
+> NOTE: All attributes can be set during initialization
+---
+## Initial Setup
+When setting up the leveling system, a database file needs to be created in order for the library to function. 
+* Associated static method
+  * `DiscordLevelingSystem.create_database_file(path: str)`
+
+The above static method is used to create the database file for you in the path you specify. This method only needs to be called once. Example:
+```py
+DiscordLevelingSystem.create_database_file(r'C:\Users\Defxult\Documents')
+```
+Once created, there is no need to ever run that method again unless you want to create a new database file from scratch. Now that you have the database file, you can use the leveling system.
+
+---
+## Connecting to the Database
+* Associated method
+  * `DiscordLevelingSystem.connect_to_database_file(path: str)`
+
+Since the database file has already been created, all you need to do is connect to it. 
+> NOTE: When connecting to the database file, the event loop must not be running
+<div align="left"><sub>EXAMPLE</sub></div>
+
+```py
+from discord.ext import commands
+from discordLevelingSystem import DiscordLevelingSystem
+
+bot = commands.Bot(...)
+lvl = DiscordLevelingSystem()
+lvl.connect_to_database_file(r'C:\Users\Defxult\Documents\DiscordLevelingSystem.db')
+
+bot.run(...)
+```
+---
+
+## RoleAward
+```class RoleAward(role_id: int, level_requirement: int, role_name=None)```
+
+You can assign roles to the system so when someone levels up to a certain level, they are given that role. `RoleAward` is how that is accomplished.
+
+---
+### Parameters of the RoleAward constructor
+* `role_id` (`int`) ID of the role that is to be awarded.
+* `level_requirement` (`int`) What level is required for a member to be awarded the role.
+* `role_name` (`Optional[str]`) A name you can set for the award. Nothing is done with this value, it is used for visual identification purposes only.
+---
+### Attributes
+* `role_id`
+* `level_requirement`
+* `role_name`
+* `mention` (`str`) The discord role mention string
+
+When creating role awards, all role IDs and level requirements must be unique. Level requirements must also be in ascending order. It is also possible to assign different role awards for different guilds. If you don't want any role awards, set the `awards` parameter to `None`. When setting `awards`, it accepts a `dict` where the keys are guild IDs and the values are a `list` of `RoleAward`
+<div align="left"><sub>EXAMPLE</sub></div>
+
+```py
+from discordLevelingSystem import DiscordLevelingSystem, RoleAward
+
+johns_server = 587937522043060224
+janes_server = 850809412011950121
+
+my_awards = {
+    johns_server : [
+        RoleAward(role_id=831672678586777601, level_requirement=1, role_name='Rookie'),
+        RoleAward(role_id=831672730583171073, level_requirement=2, role_name='Associate'),
+        RoleAward(role_id=831672814419050526, level_requirement=3, role_name='Legend')
+    ],
+    janes_server : [
+        RoleAward(role_id=851400453904400385, level_requirement=1, role_name='Silver'),
+        RoleAward(role_id=851379776111116329, level_requirement=2, role_name='Gold'),
+        RoleAward(role_id=851959077071880202, level_requirement=3, role_name='Diamond')
+    ]
+}
+
+lvl = DiscordLevelingSystem(..., awards=my_awards)
+```
+---
+
+## LevelUpAnnouncement
+```class LevelUpAnnouncement(message=default_message, level_up_channel_ids=None, allowed_mentions=default_mentions, tts=False, delete_after=None)```
+
+Level up announcements are for when you want to implement your own level up messages. It provides access to who leveled up, their rank, level and much more. It also uses some of discord.py's kwargs from it's `Messageable.send` such as `allowed_mentions`, `tts`, and `delete_after` to give you more control over the sent message.
+
+---
+### Parameters of the LevelUpAnnouncement constructor
+
+* `message` (`Union[str, discord.Embed]`) The message that is sent when someone levels up. Defaults to `"<mention>, you are now **level <level>!**"`
+
+* `level_up_channel_ids` (`Optional[Sequence[int]]`) The text channel IDs where all level up messages will be sent for each server. If `None`, the level up message will be sent in the channel where they sent the message (example below).
+
+* `allowed_mentions` (`discord.AllowedMentions`) Used to determine who can be pinged in the level up message. Defaults to `discord.AllowedMentions(everyone=False, users=True, roles=False, replied_user=False)`
+
+* `tts` (`bool`) When the level up message is sent, have discord read the level up message aloud.
+
+* `delete_after` (`Optional[float]`) Delete the level up message after an x amount of seconds.
+
+### Class Attributes
+The `LevelUpAnnouncement` class provides a set of markdown attributes for you to use so you can access certain information in a level up message.
+
+* `LevelUpAnnouncement.TOTAL_XP` The members current total XP amount
+* `LevelUpAnnouncement.LEVEL` The members current level
+* `LevelUpAnnouncement.RANK` The members current rank
+
+The below markdown attributes takes the information from a `discord.Member` object so you can access member information in the level up message.
+
+* `LevelUpAnnouncement.Member.avatar_url`
+* `LevelUpAnnouncement.Member.banner_url`
+* `LevelUpAnnouncement.Member.created_at`
+* `LevelUpAnnouncement.Member.default_avatar_url`
+* `LevelUpAnnouncement.Member.discriminator`
+* `LevelUpAnnouncement.Member.display_avatar_url`
+* `LevelUpAnnouncement.Member.display_name`
+* `LevelUpAnnouncement.Member.id`
+* `LevelUpAnnouncement.Member.joined_at`
+* `LevelUpAnnouncement.Member.mention`
+* `LevelUpAnnouncement.Member.name`
+* `LevelUpAnnouncement.Member.nick`
+* `LevelUpAnnouncement.Member.Guild.icon_url`
+* `LevelUpAnnouncement.Member.Guild.id`
+* `LevelUpAnnouncement.Member.Guild.name`
+
+<div align="left"><sub>EXAMPLE</sub></div>
+
+```py
+from discordLevelingSystem import DiscordLevelingSystem, LevelUpAnnouncement
+
+embed = discord.Embed()
+embed.set_author(name=LevelUpAnnouncement.Member.name, icon_url=LevelUpAnnouncement.Member.avatar_url)
+embed.description = f'Congrats {LevelUpAnnouncement.Member.mention}! You are now level {LevelUpAnnouncement.LEVEL} 😎'
+
+announcement = LevelUpAnnouncement(embed)
+
+lvl = DiscordLevelingSystem(..., level_up_announcement=announcement)
+
+# NOTE: You can have multiple level up announcements by setting the parameter to a sequence of LevelUpAnnouncement
+lvl = DiscordLevelingSystem(..., level_up_announcement=[announcement_1, announcement_2, ...])
+```
+When it comes to `level_up_channel_ids`, you can set a designated channel for each server. If you don't set a level up channel ID for a specific server, the level up message will be sent in the channel where the member leveled up. You don't have to specify a level up channel ID for each server unless you'd like to.
+```py
+johns_bot_commands = 489374746737648734 # text channel ID from server A
+janes_levelup_channel = 58498304930493094 # text channel ID from server B
+
+announcement = LevelUpAnnouncement(..., level_up_channel_ids=[johns_bot_commands, janes_levelup_channel])
+lvl = DiscordLevelingSystem(..., level_up_announcement=announcement)
+```
+---
+## Handling XP
+Method `award_xp` is how members gain XP. This method is placed inside the `on_message` event of your bot. Members will gain XP if they send a message and if they're *not* on cooldown. Spamming messages will not give them XP.
+> NOTE: Members cannot gain XP in DM's
+* Associated methods
+  * `await DiscordLevelingSystem.add_xp(member: Member, amount: int)`
+  * `await DiscordLevelingSystem.remove_xp(member: Member, amount: int)`
+  * `await DiscordLevelingSystem.set_level(member: Member, level: int)`
+  * `await DiscordLevelingSystem.award_xp(*, amount=[15, 25], message: Message, refresh_name=True, **kwargs)`
+
+
+### Parameters for award_xp
+* `amount` (`Union[int, Sequence[int]]`) The amount of XP to award to the member per message. Must be from 1-25. Can be a sequence with a minimum and maximum length of two. If `amount` is a sequence of two integers, it will randomly pick a number in between those numbers including the numbers provided.
+* `message` (`discord.Message`) A discord message object
+* `refresh_name` (`bool`) Everytime the member sends a message, check if their name still matches the name in the database. If it doesn't match, update the database to match their current name. It is suggested to leave this as `True` so the database can always have the most up-to-date record.
+
+### Kwargs for award_xp
+* `bonus` (`DiscordLevelingSystem.Bonus`) Used to set the roles that will be awarded bonus XP.
+  * `class Bonus(role_ids: Sequence[int], bonus_amount: int, multiply: bool)`
+  * **Parameters of the DiscordLevelingSystem.Bonus constructor**
+    * `role_ids` (`Sequence[int]`) The role(s) a member must have to be able to get bonus XP. They only need to have one of these roles to get the bonus
+    * `bonus_amount` (`int`) Amount of extra XP to be awarded
+    * `multiply` (`bool`) If set to `True`, this will operate on a x2, x3 basis. Meaning if you have the awarded XP amount set to 10 and you want the bonus XP role to be awarded 20, it must be set to 2, not 10. If `False`, it operates purely on the given value. Meaning if you have the awarded XP set to 10 and you want the bonus XP role to be awarded 20, it must be set to 10.
+
+<div align="left"><sub>EXAMPLE</sub></div>
+
+```py
+lvl = DiscordLevelingSystem(...)
+
+nitro_booster = 851379776111116329
+associate_role = 851400453904400385
+
+@bot.event
+async def on_message(message):
+    await lvl.award_xp(amount=[15, 25], message=message, bonus=DiscordLevelingSystem.Bonus([nitro_booster, associate_role], 20, multiply=False))
+```
+---
+
+## MemberData
+Accessing the raw information inside the database file can look a bit messy if you don't know exactly what you're looking at. To make things easier, this library comes with the `MemberData` class. A class which returns information about a specific member in the database.
+
+* Associated methods
+  * `await DiscordLevelingSystem.get_data_for(member: Member) -> MemberData`
+  * `await DiscordLevelingSystem.each_member_data(guild: Guild, sort_by=None, limit=None) -> List[MemberData]`
+
+### Attributes
+* `id_number` (`int`) The members ID
+* `name` (`str`) The members name
+* `level` (`int`) The members level
+* `xp` (`int`) The members xp
+* `total_xp` (`int`) The members total xp
+* `rank` (`Optional[int]`) The members rank
+* `mention` (`str`) The discord member mention string
+
+### Methods
+* `MemberData.to_dict() -> dict`
+
+<div align="left"><sub>EXAMPLE</sub></div>
+
+```py
+lvl = DiscordLevelingSystem(...)
+
+@bot.command()
+async def rank(ctx):
+    data = await lvl.get_data_for(ctx.author)
+    await ctx.send(f'You are level {data.level} and your rank is {data.rank}')
+
+@bot.command()
+async def leaderboard(ctx):
+    data = await lvl.each_member_data(ctx.guild, sort_by='rank')
+    # show the leaderboard whichever way you'd like
+```
+---
+## Events
+You can set an event to be called when a member levels up. Using the event is considered as an enhanced `LevelUpAnnouncement` because it provides more capabilities rather than simply sending a message with only text/an embed. The `on_dls_level_up` event takes three parameters:
+* `member` (`discord.Member`) The member that leveled up
+* `message` (`discord.Message`) The message that triggered the level up
+* `data` (`MemberData`) The database information for that member
+
+```py
+bot = commands.Bot(...)
+lvl = DiscordLevelingSystem(..., bot=bot) # your bot instance variable is needed
+
+@bot.event
+async def on_dls_level_up(member: discord.Member, message: discord.Message, data: MemberData):
+    # You can do a lot more here compared to LevelUpAnnouncement
+    # - create a level up image and send it with discord.File
+    # - call additional functions that you may need
+    # - access to all attributes/methods that are available within discord.Member and discord.Message
+```
+> NOTE: `LevelUpAnnouncement` and `on_dls_level_up` are not the same. Level up messages are sent by default by the library. If you'd like to only use `on_dls_level_up`, you need to disable level up announcements (`lvl.announce_level_up = False`)
+
+---
+## Full Example
+With all classes and core methods introduced, here is a basic implementation of this library.
+```py
+from discord.ext import commands
+from discordLevelingSystem import DiscordLevelingSystem, RoleAward, LevelUpAnnouncement
+
+bot = commands.Bot(...)
+
+main_guild_id = 850809412011950121
+
+my_awards = {
+    main_guild_id : [
+        RoleAward(role_id=831672678586777601, level_requirement=1, role_name='Rookie'),
+        RoleAward(role_id=831672730583171073, level_requirement=2, role_name='Associate'),
+        RoleAward(role_id=831672814419050526, level_requirement=3, role_name='Legend')
+    ]
+}
+
+announcement = LevelUpAnnouncement(f'{LevelUpAnnouncement.Member.mention} just leveled up to level {LevelUpAnnouncement.LEVEL} 😎')
+
+# DiscordLevelingSystem.create_database_file(r'C:\Users\Defxult\Documents') database file already created
+lvl = DiscordLevelingSystem(awards=my_awards, level_up_announcement=announcement)
+lvl.connect_to_database_file(r'C:\Users\Defxult\Documents\DiscordLevelingSystem.db')
+
+@bot.event
+async def on_message(message):
+    await lvl.award_xp(amount=15, message=message)
+
+bot.run(...)
+```
+---
+
+## All methods for DiscordLevelingSystem
+<details>
+    <summary>Click to show all methods</summary>
+
+* *await* **add_record**(`guild_id, member_id, member_name, level`) - Manually add a record to the database. If the record already exists (the `guild_id` and `member_id` was found), only the level will be updated. If there were no records that matched those values, all provided information will be added
+  * **Parameters**
+    * **guild_id** (`int`) The guild ID to register
+    * **member_id** (`int`) The member ID to register
+    * **member_name** (`str`) The member name to register
+    * **level** (`int`) The member level to register. Must be from 0-100
+  * **Raises**
+    * `DiscordLevelingSystemError` - The value given from a parameter was not of the correct type or "level" was not 0-100
+
+
+* *await* **add_xp**(`member, amount`) - Give XP to a member. This also changes their level so it matches the associated XP
+  * **Parameters**
+    * **member** (`discord.Member`) The member to give XP to
+    * **amount** (`int`) Amount of XP to give to the member
+  * **Raises**
+    * `DatabaseFileNotFound` - The database file was not found
+    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
+    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
+    * `NotConnected` - Attempted to use a method that requires a connection to a database file
+    * `DiscordLevelingSystemError` - Parameter "amount" was less than or equal to zero. The minimum value is 1 
+
+
+* *await* **award_xp**(`*, amount = [15, 25], message, refresh_name = True, **kwargs`) - Give XP to the member that sent a message
+  * **Parameters**
+    * **amount** (`Union[int, Sequence[int]]`)
+    * **message** (`discord.Message`) A message object
+    * **refresh_name** (`bool`) Everytime the member sends a message, check if their name still matches the name in the database. If it doesn't match, update the database to match their current name. It is suggested to leave this as `True` so the database can always have the most up-to-date record
+  * **Kwargs**
+    * **bonus** (`DiscordLevelingSystem.Bonus`) Set the bonus values. Read the `DiscordLevelingSystem.Bonus` doc string for more details (defaults to `None`)
+  * **Raises**
+    * `DatabaseFileNotFound` - The database file was not found
+    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
+    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
+    * `NotConnected` - Attempted to use a method that requires a connection to a database file
+
+
+* **backup_database_file**(`path, with_timestamp = False`) - Create a copy of the database file to the specified path. If a copy of the backup file is already in the specified path it will be overwritten
+  * **Parameters**
+    * **path** (`str`) The path to copy the database file to
+    * **with_timestamp** (`bool`) Creates a unique file name that has the date and time of when the backup file was created. This is useful when you want multiple backup files
+  * **Raises**
+    * `DiscordLevelingSystemError` - Path doesn't exist or points to another file
+    * `NotConnected` - Attempted to use a method that requires a connection to a database file
+
+
+* *await* **change_cooldown**(`rate, per`) - Update the cooldown rate
+  * **Parameters**
+    * **rate** (`int`) The amount of messages each member can send before the cooldown triggers
+    * **per** (`float`) The amount of seconds each member has to wait before gaining more XP, aka the cooldown
+  * **Raises**
+    * `DatabaseFileNotFound` - The database file was not found
+    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
+    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
+    * `NotConnected` - Attempted to use a method that requires a connection to a database file
+    * `DiscordLevelingSystemError` - The rate or per value was not greater than zero
+
+
+* *await* **clean_database**(`guild`) - Removes the data for members that are no longer in the guild, thus reducing the database file size. It is recommended to have this method in a background loop in order to keep the database file free of records that are no longer in use
+  * **Parameters**
+    * **guild** (`discord.Guild`) The guild records to clean
+  * **Returns**
+    * (`Optional[int]`) The amount of records that were removed from the database
+  * **Raises**
+    * `DatabaseFileNotFound` - The database file was not found
+    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
+    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
+    * `NotConnected` - Attempted to use a method that requires a connection to a database file
+
+
+* **connect_to_database_file**(`path`) - Connect to the existing database file in the specified path
+  * **Parameters**
+    * **path** (`str`) The location of the database file
+  * **Raises**
+    * `ConnectionFailure` - Attempted to connect to the database file when the event loop is already running
+    * `DatabaseFileNotFound` - The database file was not found
+
+
+* *static method* **create_database_file**(`path = None`) - Create the database file and implement the SQL data for the database
+  * **Parameters**
+    * **path** (`Optional[str]`) The location to create the database file. If `None`, the file is created in the current working directory
+  * **Raises**
+    * `ConnectionFailure` - Attempted to create the database file when the event loop is already running
+    * `DiscordLevelingSystemError` - The path does not exist or the path points to a file instead of a directory
+
+
+* *await* **each_member_data**(`guild, sort_by = None, limit = None`) - Return each member in the database as a `MemberData` object for easy access to their XP, level, etc. You can sort the data with `sort_by` with the below values
+  * **Parameters**
+    * **guild** (`discord.Guild`) A guild object
+    * **sort_by** (`Optional[str]`) Return each member sorted by: "name", "level", "xp", "rank". If `None`, it will return in the order they were added to the database
+    * **limit** (`Optional[int]`) Restrict the amount of records returned to the specified amount
+  * **Returns**
+    * `List[MemberData]`
+  * **Raises**
+    * `DatabaseFileNotFound` - The database file was not found
+    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
+    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
+    * `NotConnected` - Attempted to use a method that requires a connection to a database file
+    * `DiscordLevelingSystemError` - The value of `sort_by` was not recognized or `guild` was not of type `discord.Guild`
+
+
+* *await* **export_as_json**(`path, guild`) - Export a json file that represents the database to the path specified
+  * **Parameters**
+    * **path** (`str`) Path to copy the json file to
+    * **guild** (`discord.Guild`) The guild for which the data should be extracted from. If `None`, all guild information will be extracted from the database
+  * **Raises**
+    * `DatabaseFileNotFound` - The database file was not found
+    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
+    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
+    * `NotConnected` - Attempted to use a method that requires a connection to a database file
+    * `DiscordLevelingSystemError` - The path does not exist or does not point to a directory
+
+
+* **get_awards**(`guild = None`) - Get all `RoleAward`'s or only the `RoleAward`'s assigned to the specified guild
+  * **Parameters**
+    * **guild** (`Optional[Union[discord.Guild, int]]`) A guild object or a guild ID
+  * **Returns**
+    * (`Union[Dict[int, List[RoleAward]], List[RoleAward]]`) If `guild` is `None`, this return the awards `dict` that was set in constructor. If `guild` is specified, it returns a List[`RoleAward`] that matches the specified guild ID. Can also return `None` if awards were never set or if the awards for the specified guild was not found
+
+
+* *await* **get_data_for**(`member`) - Get the `MemberData` object that represents the specified member
+  * **Parameters**
+    * **member** (`discord.Member`) The member to get the data for
+  * **Returns**
+    * (`MemberData`) Can be `None` if the member isn't in the database
+  * **Raises**
+    * `DatabaseFileNotFound` - The database file was not found
+    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
+    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
+    * `NotConnected` - Attempted to use a method that requires a connection to a database file
+
+
+* *await* **get_level_for**(`member`) - Get the level for the specified member
+  * **Parameters**
+    * **member** (`discord.Member`) Member to get the level for
+  * **Returns**
+    * (`int`) Can be `None` if the member isn't in the database
+  * **Raises**
+    * `DatabaseFileNotFound` - The database file was not found
+    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
+    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
+    * `NotConnected` - Attempted to use a method that requires a connection to a database file
+
+
+* *await* **get_rank_for**(`member`) - Get the rank for the specified member
+  * **Parameters**
+    * **member** (`discord.Member`) Member to get the rank for
+  * **Returns**
+    * (`int`) Can be `None` if the member isn't ranked yet
+  * **Raises**
+    * `DatabaseFileNotFound` - The database file was not found
+    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
+    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
+    * `NotConnected` - Attempted to use a method that requires a connection to a database file
+
+
+* *await* **get_record_count**(`guild = None`) - Get the amount of members that are registered in the database. If `guild` is set to `None`, ALL members in the database will be counted
+  * **Parameters**
+    * **guild** (`Optional[discord.Guild]`) The guild for which to count the amount of records
+  * **Returns**
+    * (`int`)
+  * **Raises**
+    * `DatabaseFileNotFound` - The database file was not found
+    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
+    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
+    * `NotConnected` - Attempted to use a method that requires a connection to a database file
+
+
+* *await* **get_total_xp_for**(`member`) - Get the total XP for the specified member
+  * **Parameters**
+    * **member** (`discord.Member`) Member to get the total XP for
+  * **Returns**
+    * (`int`) Can be `None` if the member isn't in the database
+  * **Raises**
+    * `DatabaseFileNotFound` - The database file was not found
+    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
+    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
+    * `NotConnected` - Attempted to use a method that requires a connection to a database file
+
+
+* *await* **get_xp_for**(`member`) - Get the XP for the specified member
+  * **Parameters**
+    * **member** (`discord.Member`) Member to get the XP for
+  * **Returns**
+    * (`int`) Can be `None` if the member isn't in the database
+  * **Raises**
+    * `DatabaseFileNotFound` - The database file was not found
+    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
+    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
+    * `NotConnected` - Attempted to use a method that requires a connection to a database file
+
+
+* *static method* **get_xp_for_level**(`level`) - Returns the total amount of XP needed for the specified level. Levels go from 0-100
+  * **Parameters**
+    * **level** (`int`) The level XP information to retrieve
+  * **Returns**
+    * (`int`)
+  * **Raises**
+    * `DiscordLevelingSystemError` - The level specified does not exist
+
+
+* *await* **insert**(`bot, guild_id, users, using, overwrite = False, show_results = True`) - Insert the records from your own leveling system into the library. A lot of leveling system tutorials out there use json files to store information. Although it might work, it is insufficient because json files are not made to act as a database. Using an actual database file has many benefits over a json file
+  * **Parameters**
+    * **bot** (`Union[discord.ext.commands.Bot, discord.ext.commands.AutoShardedBot]`) Your bot instance variable
+    * **guild_id** (`int`) ID of the guild that you used your leveling system with
+    * **users** (`Dict[int, int]`) This is the information that will be added to the database. The keys are user ID's, and the values are the users total XP or level. Note: This library only uses levels 0-100 and XP 0-1899250. If any number in this dict are over the levels/XP threshold, it is implicitly set back to this libraries maximum value
+    * **using** (`str`) What structure your leveling system used. Options: "xp" or "levels". Some leveling systems give users only XP and they are ranked up based on that XP value. Others use a combination of levels and XP. If all the values in the `users` dict are based on XP, set this to "xp". If they are based on a users level, set this to "levels"
+    * **overwrite** (`bool`) If a user you've specified in the `users` dict already has a record in the database, overwrite their current record with the one your inserting
+    * **show_results** (`bool`) Print the results for how many of the `users` were successfully added to the database file. If any are unsuccessful, their ID along with the value you provided will also be shown
+  * **Raises**
+      * `DiscordLevelingSystemError` - The value given from a parameter was not of the correct type. The `users` dict was empty. Or your bot is not in the guild associated with `guild_id`       
+
+
+* *await* **is_in_database**(`member, guild = None`) - A quick check to see if a member is in the database. This is not guild specific although it can be if `guild` is specified
+  * **Parameters**
+    * **member** (`Union[discord.Member, int]`) The member to check for. Can be the member object or that members ID
+    * **guild** (`Optional[discord.Guild]`) The guild to check if the member is registered in
+  * **Returns**
+    * (`bool`)
+  * **Raises**
+    * `DatabaseFileNotFound` - The database file was not found
+    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
+    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
+    * `NotConnected` - Attempted to use a method that requires a connection to a database file
+    * `DiscordLevelingSystemError` - Parameter `member` was not of type `discord.Member` or `int`
+
+
+* *static method* **levels_and_xp**( ) -  Get the raw `dict` representation for the amount of levels/XP in the system. The keys in the `dict` returned is each level, and the values are the amount of XP needed to be awarded that level
+  * **Returns**
+    * (`Dict[str, int]`)
+
+
+* *await* **next_level**(`member`) - Get the next level for the specified member
+  * **Parameters**
+    * **member** (`discord.Member`) Member to get the next level for
+  * **Returns**
+    * (`int`) If the member is currently max level (100), it will return 100. This can also return `None` if the member is not in the database
+  * **Raises**
+    * `DatabaseFileNotFound` - The database file was not found
+    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
+    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
+    * `NotConnected` - Attempted to use a method that requires a connection to a database file
+
+
+* *await* **next_level_up**(`member`) - Get the amount of XP needed for the specified member to level up
+  * **Parameters**
+    * **member** (`discord.Member`) Member to get the amount of XP needed for a level up
+  * **Returns**
+    * (`int`) Returns 0 if the member is currently at max level. Can return `None` if the member is not in the database.
+  * **Raises**
+    * `DatabaseFileNotFound` - The database file was not found
+    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
+    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
+    * `NotConnected` - Attempted to use a method that requires a connection to a database file
+
+
+* *await* **raw_database_contents**(`guild = None`) - Returns everything in the database. Can specify which guild information will be extracted
+  * **Parameters**
+    * **guild** (`Optional[discord.Guild]`) The guild to extract the raw database contents from. If `None`, information about all guilds will be extracted
+  * **Returns**
+    * `List[Tuple[int, int, str, int, int, int]]` The tuples inside the list represents each row of the database:
+      * Index 0 is the guild ID
+      * Index 1 is their ID
+      * Index 2 is their name
+      * Index 3 is their level
+      * Index 4 is their XP
+      * Index 5 is their total xp
+      * Can be an empty list if nothing is in the database
+  * **Raises**
+    * `DatabaseFileNotFound` - The database file was not found
+    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
+    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
+    * `NotConnected` - Attempted to use a method that requires a connection to a database file
+
+
+* *await* **refresh_names**(`guild`) - Update names inside the database. This does not add anything new. It simply verifies if the name in the database matches their current name, and if they don't match, update the database name
+  * **Parameters**
+    * **guild** (`discord.Guild`) A guild object
+  * **Returns**
+    * `(Optional[int])` The amount of records in the database that were updated
+  * **Raises**
+    * `DatabaseFileNotFound` - The database file was not found
+    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
+    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
+    * `NotConnected` - Attempted to use a method that requires a connection to a database file
+
+
+* *await* **remove_from_database**(`member, guild = None`) - Remove a member from the database. This is not guild specific although it can be if `guild` is specified
+  * **Parameters**
+    * **member** (`Union[discord.Member, int]`) The member to remove. Can be the member object or that members ID
+    * **guild** (`Optional[discord.Guild]`) If this parameter is given, it will remove the record of the specified member only from the specified guild record. If `None`, it will remove all records no matter the guild
+  * **Returns**
+    * (`Optional[bool]`) Returns `True` if the member was successfully removed from the database. `False` if the member was not in the database so there was nothing to remove
+  * **Raises**
+      * `DatabaseFileNotFound` - The database file was not found
+      * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
+      * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
+      * `DiscordLevelingSystemError` - Parameter `member` was not of type `discord.Member` or `int`
+      * `NotConnected` - Attempted to use a method that requires a connection to a database file
+
+
+* *await* **remove_xp**(`member, amount`) - Remove XP from a member. This also changes their level so it matches the associated XP
+  * **Parameters**
+      * **member** (`discord.Member`) The member to remove XP from
+      * **amount** (`int`) Amount of XP to remove from the member
+  * **Raises**
+    * `DatabaseFileNotFound` - The database file was not found
+    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
+    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
+    * `NotConnected` - Attempted to use a method that requires a connection to a database file
+    * `DiscordLevelingSystemError` - Parameter "amount" was less than or equal to zero. The minimum value is 1
+
+
+* *await* **reset_everyone**(`guild, *, intentional = False`) - Sets EVERYONES XP, total XP, and level to zero in the database. Can specify which guild to reset
+  * **Parameters**
+      * **guild** (`Union[discord.Guild, None]`) The guild for which everyone will be reset. If this is set to `None`, everyone in the entire database will be reset
+      * **intentional** (`bool`) A simple kwarg to try and ensure that this action is indeed what you want to do. Once executed, this cannot be undone
+  * **Raises**
+    * `DatabaseFileNotFound` - The database file was not found
+    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
+    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
+    * `NotConnected` - Attempted to use a method that requires a connection to a database file
+    * `FailSafe` - "intentional" argument for this method was set to `False` in case you called this method by mistake
+
+
+* *await* **reset_member**(`member`) - Sets the members XP, total XP, and level to zero
+  * **Parameters**
+    * **member** (`discord.Member`) The member to reset
+  * **Raises**
+    * `DatabaseFileNotFound` The database file was not found
+    * `LeaderboardNotFound` Table "leaderboard" in the database file is missing
+    * `ImproperLeaderboard` Leaderboard table was altered. Components changed or deleted
+    * `NotConnected` Attempted to use a method that requires a connection to a database file
+
+
+* *await* **set_level**(`member, level`) - Sets the level for the member. This also changes their total XP so it matches the associated level
+  * **Parameters**
+    * **member** (`discord.Member`) The member who's level will be set
+    * **level** (`int`) Level to set. Must be from 0-100     
+  * **Raises**
+    * `DatabaseFileNotFound` - The database file was not found
+    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
+    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
+    * `NotConnected` - Attempted to use a method that requires a connection to a database file
+    * `DiscordLevelingSystemError` - Parameter "level" was not from 0-100
+
+
+* *await* **sql_query_get**(`sql, parameters = None, fetch = 'ALL'`) - Query and return something from the database using SQL. The following columns are apart of the "leaderboard" table: guild_id, member_id, member_name, member_level, member_xp, member_total_xp
+  * **Parameters**
+    * **sql** (`str`) SQL string used to query the database
+    * **parameters** (`Optional[Tuple[Union[str ,int]]]`) The parameters used for the database query
+    * **fetch** (`Union[str, int]`) The amount of rows you would like back from the query. Options: 'ALL', 'ONE', or an integer value that is greater than zero
+  * **Returns**
+    * (`Union[List[tuple], tuple]`)
+      * Using `fetch='ALL'` returns `List[tuple]`
+      * Using `fetch='ONE'` returns `tuple`
+      * Using `fetch=4` returns `List[tuple]` with only four values
+      * Can also return an empty list if the query was valid but got nothing from it
+  * **Raises**
+    * `DatabaseFileNotFound` - The database file was not found
+    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
+    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
+    * `NotConnected` - Attempted to use a method that requires a connection to a database file
+    * `DiscordLevelingSystemError` - Argument "fetch" was the wrong type or used an invalid value
+    * `aiosqlite.Error` - Base aiosqlite error. Multiple errors can arise from this if the SQL query was invalid
+
+
+* *await* **switch_connection**(`path`) - Connect to a different leveling system database file
+  * **Parameters**
+    * **path** (`str`) The location of the database file
+  * **Raises**
+    * `DatabaseFileNotFound` - The database file was not found
+
+
+* *static method* **transfer**(`old, new, guild_id`) - Transfer the database records from a database file created from v0.0.1 to a blank database file created using v0.0.2+. If you were already using a v0.0.2+ database file, there's no need to use this method
+  * **Parameters**
+    * **old** (`str`) The path of the v0.0.1 database file
+    * **new** (`str`) The path of the v0.0.2+ database file
+    * **guild_id** (`int`) ID of the guild that was originally used with this library
+  * **Raises**
+    - `ConnectionFailure` - The event loop is already running
+    - `DatabaseFileNotFound` - "old" or "new" database file was not found
+    - `DiscordLevelingSystemError` - One of the databases is missing the "leaderboard" table. A v0.0.2+ database file contains records, or there was an attempt to transfer records from a v0.0.2+ file to another v0.0.2+ file
+
+
+* *await* **wipe_database**(`guild = None, *, intentional = False`) - Delete EVERYTHING from the database. If `guild` is specified, only the information related to that guild will be deleted
+  * **Parameters**
+    * **guild** (`Optional[discord.Guild]`) The guild for which all information that is related to that guild will be deleted. If `None`, everything will be deleted
+    * **intentional** (`bool`) A simple kwarg to try and ensure that this action is indeed what you want to do. Once executed, this cannot be undone
+  * **Raises**
+    * `DatabaseFileNotFound` - The database file was not found
+    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
+    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
+    * `NotConnected` - Attempted to use a method that requires a connection to a database file
+    * `FailSafe` - "intentional" argument for this method was set to `False` in case you called this method by mistake
+
+</details>
+
+## Migrating from v0.0.1 to v0.0.2+
+<details>
+    <summary>Click to show details</summary>
+
+This library was not originally designed with the use of multiple servers in mind, so all the data you might have currently (your database file was created in `v0.0.1`) should be from a single server. With `v0.0.2`, the structure of the database file was changed to accommodate this fix. That means if you are currently using a `v0.0.1` database file and update to `v0.0.2+`, a vast majority of the library will be broken. To avoid this, you need to transfer all your `v0.0.1` database file records to a `v0.0.2+` database file. This can be done using the `transfer` method.
+
+* Associated static method
+  * `DiscordLevelingSystem.transfer(old: str, new: str, guild_id: int)`
+
+### Parameters
+* `old` (`str`) The path of the `v0.0.1` database file
+* `new` (`str`) The path of the `v0.0.2+` database file (a brand new file from using `DiscordLevelingSystem.create_database_file(path: str)`)
+* `guild_id` (`int`) ID of the guild that was originally used with this library
+
+<div align="left"><sub>EXAMPLE</sub></div>
+
+```py
+from discordLevelingSystem import DiscordLevelingSystem
+
+old = r'C:\Users\Defxult\Documents\DiscordLevelingSystem.db'
+new = r'C:\Users\Defxult\Desktop\DiscordLevelingSystem.db'
+
+DiscordLevelingSystem.transfer(old, new, guild_id=850809412011950121)
+```
+
+</details>
+
+## Inserting your own leveling system information
+<details>
+    <summary>Click to show details</summary>
+
+Insert the records from your leveling system into this one. A lot of leveling system tutorials out there use json files to store information. Although it might work, it is insufficient because json files are not made to act as a database. Using a database file has many benefits over a json file. If you previously watched a tutorial for your leveling system and would like to import your records over to use with this library, you can do so with the below method.
+
+* Associated static method
+  * `await DiscordLevelingSystem.insert(bot: Union[Bot, AutoShardedBot], guild_id: int, users: Dict[int, int], using: str, overwrite=False, show_results=True)`
+
+### Parameters
+- `bot` (`Union[discord.ext.commands.Bot, discord.ext.commands.AutoShardedBot]`) Your bot instance variable
+
+- `guild_id` (`int`) ID of the guild that you used your leveling system with
+
+- `users` (`Dict[int, int]`) This is the information that will be added to the database. The keys are user ID's, and the values are the users total XP or level. Note: This library only uses levels 0-100 and XP 0-1899250. If any number in this dict are over the levels/XP threshold, it is implicitly set back to this libraries maximum value
+
+- `using` (`str`) What structure your leveling system used. Options: "xp" or "levels". Some leveling systems give users only XP and they are ranked up based on that XP value. Others use a combination of levels and XP. If all the values in the `users` dict are based on XP, set this to "xp". If they are based on a users level, set this to "levels"
+
+- `overwrite` (`bool`) If a user you've specified in the `users` dict already has a record in the database, overwrite their current record with the one your inserting
+
+- `show_results` (`bool`) Print the results for how many of the `users` were successfully added to the database file. If any are unsuccessful, their ID along with the value you provided will also be shown
+
+> NOTE: If the users you've provided in the `users` dict is not currently in the guild (`guild_id`), their information will not be inserted. If you'd like, you can manually add those records with method `DiscordLevelingSystem.add_record()`, but that is discouraged because it is better to discard information that is no longer in use (the user is no longer in the guild)
+
+<div align="left"><sub>EXAMPLE</sub></div>
+
+```py
+# leveling_system.json
+[
+  {
+      "5748392849348934" : {
+          "xp" : 373,
+          "level" : 4
+      }
+  },
+  {
+      "89283659820948923" : {
+          "xp" : 23,
+          "level" : 1
+      }
+  }
+]
+
+
+# bot.py
+import json
+from discord.ext import commands
+from discordLevelingSystem import DiscordLevelingSystem
+
+bot = commands.Bot(...)
+
+lvl = DiscordLevelingSystem(...)
+lvl.connect_to_database_file(...)
+
+def json_to_dict() -> dict:
+    with open('leveling_system.json') as fp:
+        data = json.load(fp)
+        formatted: Dict[int, int] = ... # format the data so all keys and values are associated with the user ID and level
+        
+        """
+        In the end, the formatted dict should look like so:
+        
+        formatted = {
+            5748392849348934 : 4,
+            89283659820948923 : 1
+        }
+        """
+        return formatted
+
+@bot.command()
+async def insert(ctx):
+    await lvl.insert(ctx.bot, guild_id=12345678901234, users=json_to_dict(), using='levels')
+
+bot.run(...)
+```
+
+</details>
```

### Comparing `discordLevelingSystem-1.2.0/discordLevelingSystem/__init__.py` & `discordLevelingSystem-1.2.1/discordLevelingSystem/__init__.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-"""
-Discord Leveling System
-~~~~~~~~~~~~~~~~~~~~~~~
-
-A library to implement a leveling system into a discord bot. Contains features such as XP, level, ranks, and role awards.
-
-:copyright: (c) 2021-present Defxult#8269
-:license: MIT
-
-"""
-
-from .announcement import LevelUpAnnouncement
-from .leveling_system import DiscordLevelingSystem
-from .member_data import MemberData
-from .role_awards import RoleAward
-
-__source__ = 'https://github.com/Defxult/discordLevelingSystem'
-__all__ = (
-    'LevelUpAnnouncement',
-    'DiscordLevelingSystem',
-    'MemberData',
-    'RoleAward'
-)
+"""
+Discord Leveling System
+~~~~~~~~~~~~~~~~~~~~~~~
+
+A library to implement a leveling system into a discord bot. Contains features such as XP, level, ranks, and role awards.
+
+:copyright: (c) 2021-present Defxult#8269
+:license: MIT
+
+"""
+
+from .announcement import LevelUpAnnouncement
+from .leveling_system import DiscordLevelingSystem
+from .member_data import MemberData
+from .role_awards import RoleAward
+
+__source__ = 'https://github.com/Defxult/discordLevelingSystem'
+__all__ = (
+    'LevelUpAnnouncement',
+    'DiscordLevelingSystem',
+    'MemberData',
+    'RoleAward'
+)
```

### Comparing `discordLevelingSystem-1.2.0/discordLevelingSystem/decorators.py` & `discordLevelingSystem-1.2.1/discordLevelingSystem/decorators.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,107 +1,107 @@
-"""
-MIT License
-
-Copyright (c) 2021-present Defxult#8269
-
-Permission is hereby granted, free of charge, to any person obtaining a
-copy of this software and associated documentation files (the "Software"),
-to deal in the Software without restriction, including without limitation
-the rights to use, copy, modify, merge, publish, distribute, sublicense,
-and/or sell copies of the Software, and to permit persons to whom the
-Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in
-all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS
-OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER 
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING 
-FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER 
-DEALINGS IN THE SOFTWARE.
-"""
-
-import os
-from functools import wraps
-
-import aiosqlite
-
-from .errors import DatabaseFileNotFound, ImproperLeaderboard, LeaderboardNotFound, NotConnected
-
-
-def _return_self(args: list):
-    """Return the class instance"""
-    return args[0]
-
-def db_file_exists(func):
-    """Ensure the database file exists before performing any operations"""
-    @wraps(func)
-    async def wrapper(*args, **kwargs):
-        instance = _return_self(args) # type: ignore
-        if not any([instance._database_file_path, instance._connection]):
-            raise DatabaseFileNotFound('The database file was not found. Did you forget to connect to it first using "DiscordLevelingSystem.connect_to_database_file()"?')
-        
-        def path_exists() -> bool:
-            """This is only to check if the path is :class:`None`. If it is, it raises a `TypeError`, and the traceback the user sees doesn't make any sense. This produces a cleaner
-            traceback, and if the path does exist, return `True`"""
-            nonlocal instance
-            try:
-                existence = os.path.exists(instance._database_file_path)
-            except TypeError:
-                raise NotConnected
-            else:
-                return existence
-
-        # if it gets this far, that means :meth:`DiscordLevelingSystem.connect_to_file()` was ran, the connection
-        # object was set, the file path was stored, and that file does end in ".db". This checks it again because
-        # this check applies to various other methods that need to verify that the file exists. Using :meth:`DiscordLevelingSystem.connect_to_file()`
-        # has its own check just like this, and that method will only be called to setup the initial connection
-        if path_exists():
-            if os.path.isfile(instance._database_file_path) and instance._database_file_path.endswith('.db'):
-                return await func(*args, **kwargs)
-            else:
-                raise DatabaseFileNotFound('A file ending with ".db" was not found')
-        else:
-            raise DatabaseFileNotFound(f'The file {instance._database_file_path!r} does not exist')
-    return wrapper
-
-def leaderboard_exists(func):
-    """Ensures the "leaderboard" table exists in the "DiscordLevelingSystem.db" file"""
-    @wraps(func)
-    async def wrapper(*args, **kwargs):
-        instance = _return_self(args) # type: ignore
-        try:
-            async with instance._connection.execute('SELECT * FROM leaderboard'):
-                pass
-        except aiosqlite.OperationalError:
-            raise LeaderboardNotFound
-        else:
-            return await func(*args, **kwargs)
-    return wrapper
-
-def verify_leaderboard_integrity(func):
-    """Ensures the values of the leaderboard table are the values needed in order to operate on said table
-    
-        .. changes::
-            v0.0.2
-                Added pragma for guild_id
-    """
-    @wraps(func)
-    async def wrapper(*args, **kwargs):
-        PRAGMA_LAYOUT = [
-            (0, 'guild_id', 'INT', 1, None, 0),
-            (1, 'member_id', 'INT', 1, None, 0),
-            (2, 'member_name', 'TEXT', 1, None, 0),
-            (3, 'member_level', 'INT', 1, None, 0),
-            (4, 'member_xp', 'INT', 1, None, 0),
-            (5, 'member_total_xp', 'INT', 1, None, 0)
-        ]
-        instance = _return_self(args) # type: ignore
-        async with instance._connection.execute('PRAGMA table_info(leaderboard)') as cursor:
-            current_layout = await cursor.fetchall()
-            if current_layout == PRAGMA_LAYOUT:
-                return await func(*args, **kwargs)
-            else:
-                raise ImproperLeaderboard
-    return wrapper
+"""
+MIT License
+
+Copyright (c) 2021-present Defxult#8269
+
+Permission is hereby granted, free of charge, to any person obtaining a
+copy of this software and associated documentation files (the "Software"),
+to deal in the Software without restriction, including without limitation
+the rights to use, copy, modify, merge, publish, distribute, sublicense,
+and/or sell copies of the Software, and to permit persons to whom the
+Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in
+all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS
+OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER 
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING 
+FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER 
+DEALINGS IN THE SOFTWARE.
+"""
+
+import os
+from functools import wraps
+
+import aiosqlite
+
+from .errors import DatabaseFileNotFound, ImproperLeaderboard, LeaderboardNotFound, NotConnected
+
+
+def _return_self(args: list):
+    """Return the class instance"""
+    return args[0]
+
+def db_file_exists(func):
+    """Ensure the database file exists before performing any operations"""
+    @wraps(func)
+    async def wrapper(*args, **kwargs):
+        instance = _return_self(args) # type: ignore
+        if not any([instance._database_file_path, instance._connection]):
+            raise DatabaseFileNotFound('The database file was not found. Did you forget to connect to it first using "DiscordLevelingSystem.connect_to_database_file()"?')
+        
+        def path_exists() -> bool:
+            """This is only to check if the path is :class:`None`. If it is, it raises a `TypeError`, and the traceback the user sees doesn't make any sense. This produces a cleaner
+            traceback, and if the path does exist, return `True`"""
+            nonlocal instance
+            try:
+                existence = os.path.exists(instance._database_file_path)
+            except TypeError:
+                raise NotConnected
+            else:
+                return existence
+
+        # if it gets this far, that means :meth:`DiscordLevelingSystem.connect_to_file()` was ran, the connection
+        # object was set, the file path was stored, and that file does end in ".db". This checks it again because
+        # this check applies to various other methods that need to verify that the file exists. Using :meth:`DiscordLevelingSystem.connect_to_file()`
+        # has its own check just like this, and that method will only be called to setup the initial connection
+        if path_exists():
+            if os.path.isfile(instance._database_file_path) and instance._database_file_path.endswith('.db'):
+                return await func(*args, **kwargs)
+            else:
+                raise DatabaseFileNotFound('A file ending with ".db" was not found')
+        else:
+            raise DatabaseFileNotFound(f'The file {instance._database_file_path!r} does not exist')
+    return wrapper
+
+def leaderboard_exists(func):
+    """Ensures the "leaderboard" table exists in the "DiscordLevelingSystem.db" file"""
+    @wraps(func)
+    async def wrapper(*args, **kwargs):
+        instance = _return_self(args) # type: ignore
+        try:
+            async with instance._connection.execute('SELECT * FROM leaderboard'):
+                pass
+        except aiosqlite.OperationalError:
+            raise LeaderboardNotFound
+        else:
+            return await func(*args, **kwargs)
+    return wrapper
+
+def verify_leaderboard_integrity(func):
+    """Ensures the values of the leaderboard table are the values needed in order to operate on said table
+    
+        .. changes::
+            v0.0.2
+                Added pragma for guild_id
+    """
+    @wraps(func)
+    async def wrapper(*args, **kwargs):
+        PRAGMA_LAYOUT = [
+            (0, 'guild_id', 'INT', 1, None, 0),
+            (1, 'member_id', 'INT', 1, None, 0),
+            (2, 'member_name', 'TEXT', 1, None, 0),
+            (3, 'member_level', 'INT', 1, None, 0),
+            (4, 'member_xp', 'INT', 1, None, 0),
+            (5, 'member_total_xp', 'INT', 1, None, 0)
+        ]
+        instance = _return_self(args) # type: ignore
+        async with instance._connection.execute('PRAGMA table_info(leaderboard)') as cursor:
+            current_layout = await cursor.fetchall()
+            if current_layout == PRAGMA_LAYOUT:
+                return await func(*args, **kwargs)
+            else:
+                raise ImproperLeaderboard
+    return wrapper
```

### Comparing `discordLevelingSystem-1.2.0/discordLevelingSystem/errors.py` & `discordLevelingSystem-1.2.1/discordLevelingSystem/errors.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,69 +1,69 @@
-"""
-MIT License
-
-Copyright (c) 2021-present Defxult#8269
-
-Permission is hereby granted, free of charge, to any person obtaining a
-copy of this software and associated documentation files (the "Software"),
-to deal in the Software without restriction, including without limitation
-the rights to use, copy, modify, merge, publish, distribute, sublicense,
-and/or sell copies of the Software, and to permit persons to whom the
-Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in
-all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS
-OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER 
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING 
-FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER 
-DEALINGS IN THE SOFTWARE.
-"""
-
-class DiscordLevelingSystemError(Exception):
-    """Base exception for :class:`DiscordLevelingSystem`"""
-    def __init__(self, message: str):
-        super().__init__(message)
-
-class RoleAwardError(DiscordLevelingSystemError):
-    """Base exception for :class:`RoleAward`"""
-    def __init__(self, message: str):
-        super().__init__(message)
-
-class ConnectionFailure(DiscordLevelingSystemError):
-    """Attempted to connect to the database file when the event loop is already running"""
-    def __init__(self):
-        super().__init__('Cannot connect to database file because the event loop is already running')
-
-class NotConnected(DiscordLevelingSystemError):
-    """Attempted to use a method that requires a connection to a database file"""
-    def __init__(self):
-        super().__init__('You attempted to use a method that requires a database connection. Did you forget to connect to the database file first using "DiscordLevelingSystem.connect_to_database_file()"?')
-
-class DatabaseFileNotFound(DiscordLevelingSystemError):
-    """The database file was not found"""
-    def __init__(self, message):
-        super().__init__(message)
-
-class ImproperRoleAwardOrder(RoleAwardError):
-    """When setting the awards :class:`dict` in the :class:`DiscordLevelingSystem` constructor, :attr:`RoleAward.level_requirement` was not greater than the last level"""
-    def __init__(self, message):
-        super().__init__(message)
-
-class ImproperLeaderboard(DiscordLevelingSystemError):
-    """Raised when the leaderboard table in the database file does not have the correct settings"""
-    def __init__(self):
-        super().__init__('It seems like the leaderboard table was altered. Components changed or deleted')
-
-class LeaderboardNotFound(DiscordLevelingSystemError):
-    """When accessing the "DiscordLevelingSystem.db" file, the table "leaderboard" was not found inside that file"""
-    def __init__(self):
-        super().__init__('When accessing the "DiscordLevelingSystem.db" file, the table "leaderboard" was not found inside that file. Use DiscordLevelingSystem.create_database_file() to create the file')
-
-class FailSafe(DiscordLevelingSystemError):
-    """Raised when the expected value for a method that can cause massive unwanted results, such as :meth:`DiscordLevelingSystem.wipe_database()`, was set to `False`"""
-    def __init__(self):
-        super().__init__('Failsafe condition raised due to default argument. "intentional" was set to False')
+"""
+MIT License
+
+Copyright (c) 2021-present Defxult#8269
+
+Permission is hereby granted, free of charge, to any person obtaining a
+copy of this software and associated documentation files (the "Software"),
+to deal in the Software without restriction, including without limitation
+the rights to use, copy, modify, merge, publish, distribute, sublicense,
+and/or sell copies of the Software, and to permit persons to whom the
+Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in
+all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS
+OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER 
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING 
+FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER 
+DEALINGS IN THE SOFTWARE.
+"""
+
+class DiscordLevelingSystemError(Exception):
+    """Base exception for :class:`DiscordLevelingSystem`"""
+    def __init__(self, message: str):
+        super().__init__(message)
+
+class RoleAwardError(DiscordLevelingSystemError):
+    """Base exception for :class:`RoleAward`"""
+    def __init__(self, message: str):
+        super().__init__(message)
+
+class ConnectionFailure(DiscordLevelingSystemError):
+    """Attempted to connect to the database file when the event loop is already running"""
+    def __init__(self):
+        super().__init__('Cannot connect to database file because the event loop is already running')
+
+class NotConnected(DiscordLevelingSystemError):
+    """Attempted to use a method that requires a connection to a database file"""
+    def __init__(self):
+        super().__init__('You attempted to use a method that requires a database connection. Did you forget to connect to the database file first using "DiscordLevelingSystem.connect_to_database_file()"?')
+
+class DatabaseFileNotFound(DiscordLevelingSystemError):
+    """The database file was not found"""
+    def __init__(self, message):
+        super().__init__(message)
+
+class ImproperRoleAwardOrder(RoleAwardError):
+    """When setting the awards :class:`dict` in the :class:`DiscordLevelingSystem` constructor, :attr:`RoleAward.level_requirement` was not greater than the last level"""
+    def __init__(self, message):
+        super().__init__(message)
+
+class ImproperLeaderboard(DiscordLevelingSystemError):
+    """Raised when the leaderboard table in the database file does not have the correct settings"""
+    def __init__(self):
+        super().__init__('It seems like the leaderboard table was altered. Components changed or deleted')
+
+class LeaderboardNotFound(DiscordLevelingSystemError):
+    """When accessing the "DiscordLevelingSystem.db" file, the table "leaderboard" was not found inside that file"""
+    def __init__(self):
+        super().__init__('When accessing the "DiscordLevelingSystem.db" file, the table "leaderboard" was not found inside that file. Use DiscordLevelingSystem.create_database_file() to create the file')
+
+class FailSafe(DiscordLevelingSystemError):
+    """Raised when the expected value for a method that can cause massive unwanted results, such as :meth:`DiscordLevelingSystem.wipe_database()`, was set to `False`"""
+    def __init__(self):
+        super().__init__('Failsafe condition raised due to default argument. "intentional" was set to False')
```

### Comparing `discordLevelingSystem-1.2.0/discordLevelingSystem/leveling_system.py` & `discordLevelingSystem-1.2.1/discordLevelingSystem/leveling_system.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,1971 +1,1971 @@
-"""
-MIT License
-
-Copyright (c) 2021-present Defxult#8269
-
-Permission is hereby granted, free of charge, to any person obtaining a
-copy of this software and associated documentation files (the "Software"),
-to deal in the Software without restriction, including without limitation
-the rights to use, copy, modify, merge, publish, distribute, sublicense,
-and/or sell copies of the Software, and to permit persons to whom the
-Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in
-all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS
-OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER 
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING 
-FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER 
-DEALINGS IN THE SOFTWARE.
-"""
-
-import asyncio
-import collections
-import json
-import os
-import random
-import shutil
-from collections.abc import Sequence
-from datetime import datetime
-from inspect import cleandoc
-from typing import Dict, List, Literal, NamedTuple, Optional, overload, Tuple, Union
-
-import aiosqlite
-from discord import Guild, Member, Message, MessageType, Role
-from discord.ext.commands import AutoShardedBot, Bot, BucketType, CooldownMapping
-
-from .announcement import LevelUpAnnouncement
-from .decorators import db_file_exists, leaderboard_exists, verify_leaderboard_integrity
-from .errors import *
-from .levels_xp_needed import *
-from .member_data import MemberData
-from .role_awards import RoleAward
-
-
-class DiscordLevelingSystem:
-    """A local discord.py leveling system powered by SQLite
-
-    Parameters
-    ----------
-    rate: :class:`int`
-        The amount of messages each member can send before the cooldown triggers
-
-    per: :class:`float`
-        The amount of seconds each member has to wait before gaining more XP, aka the cooldown
-    
-    awards: Optional[Dict[:class:`int`, List[:class:`RoleAward`]]]
-        The role given to a member when they reach a :class:`RoleAward` level requirement
-
-    Kwargs
-    ------
-    no_xp_roles: Sequence[:class:`int`]
-        A sequence of role ID's. Any member with any of those roles will not gain XP when sending messages (defaults to :class:`None`)
-    
-    no_xp_channels: Sequence[:class:`int`]
-        A sequence of text channel ID's. Any member sending messages in any of those text channels will not gain XP (defaults to :class:`None`)
-    
-    announce_level_up: :class:`bool`
-        If `True`, level up messages will be sent when a member levels up (defaults to `True`)
-
-    stack_awards: :class:`bool`
-        If this is `True`, when the member levels up the assigned role award will be applied. If `False`, the previous role award will be removed
-        and the level up assigned role will also be applied (defaults to `True`)
-
-    level_up_announcement: Union[:class:`LevelUpAnnouncement`, Sequence[:class:`LevelUpAnnouncement`]]
-        The message that is sent when someone levels up. If this is a list of :class:`LevelUpAnnouncement`, one is selected at random (defaults to :class:`LevelUpAnnouncement()`)
-    
-    bot: Union[:class:`discord.ext.commands.AutoShardedBot`, :class:`discord.ext.commands.Bot`]
-        Your bot instance variable. Used only if you'd like to use the `on_dls_level_up` event (defaults to :class:`None`)
-    
-    Attributes
-    ----------
-    - `no_xp_roles`
-    - `no_xp_channels`
-    - `announce_level_up`
-    - `stack_awards`
-    - `level_up_announcement`
-    - `active`
-    - `bot`
-    - `rate` (property)
-    - `per` (property)
-    - `database_file_path` (property)
-    """
-    
-    _QUERY_NEW_MEMBER = """
-        INSERT INTO leaderboard
-        VALUES (?, ?, ?, ?, ?, ?)
-    """
-
-    def __init__(self, rate: int=1, per: float=60.0, awards: Optional[Dict[int, List[RoleAward]]]=None, **kwargs):
-        if rate <= 0 or per <= 0:   raise DiscordLevelingSystemError('Invalid rate or per. Values must be greater than zero')
-        self.__rate = rate
-        self.__per = per
-
-        RoleAward._check(awards)
-        self._awards = awards
-
-        self.no_xp_roles: Optional[Sequence[int]] = kwargs.get('no_xp_roles')
-        self.no_xp_channels: Optional[Sequence[int]] = kwargs.get('no_xp_channels')
-        self.announce_level_up: bool = kwargs.get('announce_level_up', True)
-        self.stack_awards: bool = kwargs.get('stack_awards', True)
-        self.level_up_announcement: Union[LevelUpAnnouncement, Sequence[LevelUpAnnouncement]] = kwargs.get('level_up_announcement', LevelUpAnnouncement())
-
-        self._connection: Optional[aiosqlite.Connection] = None
-        self._cursor: Optional[aiosqlite.Cursor] = None
-        
-        self._cooldown = CooldownMapping.from_cooldown(rate, per, BucketType.member)
-        self._loop = asyncio.get_event_loop()
-        self._database_file_path: Optional[str] = None
-
-        # v0.0.2
-        self._message_author: Optional[Member] = None
-
-        # v1.0.0
-        self.active = True
-
-        # v1.0.2
-        self.bot: Optional[Union[AutoShardedBot, Bot]] = kwargs.get('bot')
-    
-    @property
-    def rate(self) -> int:
-        """
-        Returns
-        -------
-        :class:`int`: The amount of messages each member can send before the cooldown triggers
-
-            .. added:: v0.0.2
-        """
-        return self.__rate
-    
-    @property
-    def per(self) -> float:
-        """
-        Returns
-        -------
-        :class:`float`: The amount of seconds each member has to wait before gaining more XP, aka the cooldown
-            
-            .. added:: v0.0.2
-        """
-        return self.__per
-    
-    @property
-    def database_file_path(self) -> Optional[str]:
-        """
-        Returns
-        -------
-        Optional[:class:`str`]: The path of the current database file. Could be :class:`None` if the database connection was never set
-
-            .. added:: v1.0.2
-        """
-        return self._database_file_path
-
-    class Bonus:
-        """Set the roles that gives x amount of extra XP to the member. This is to be used with kwarg "bonus" in the :meth:`award_xp` method
-
-        Note
-        ----
-        Having :param:`multiply` as `True` and :param:`bonus_amount` be greater than 3 is not allowed. If :param:`multiply` is `True`, :param:`bonus_amount` needs to be less than or equal to 3.
-        It should also be noted that if :param:`multiply` is `False`, it doesn't matter what :param:`bonus_amount` you use but if the total amount (awarded XP + the bonus) is greater than 75, the
-        value is implicitly changed back to 75. The maximum amount of XP a member can earn through sending messages is 75.
-
-        Parameters
-        ----------
-        role_ids: Sequence[:class:`int`]
-            The roles a member must have to be able to get bonus XP. They only need to have one of these roles to get the bonus
-
-        bonus_amount: :class:`int`
-            Amount of extra XP to be awarded
-
-        multiply: :class:`bool`
-            If set to `True`, this will operate on a x2, x3 basis. Meaning if you have the awarded XP set to 10 and you want the bonus XP role to be awarded 20, it must be set to 2,
-            not 10. If `False`, it operates purely on the given value. Meaning if you have the awarded XP set to 10 and you want the bonus XP role to be awarded 20, it must be set to 10
-        
-        Attributes
-        ----------
-        - `role_ids`
-        - `bonus_amount`
-        - `multiply`
-
-        Example
-        -------
-        ```
-        lvl = DiscordLevelingSystem(...)
-
-        nitro_booster = 851379776111116329
-        associate_role = 851400453904400385
-
-        @bot.event
-        async def on_message(message):
-            await lvl.award_xp(amount=[15, 25], message=message, bonus=DiscordLevelingSystem.Bonus([nitro_booster, associate_role], 20, multiply=False))
-        ```
-
-            .. added:: v0.0.2
-        """
-        __slots__ = ('role_ids', 'bonus_amount', 'multiply')
-
-        def __repr__(self):
-            return f'<Bonus role_ids={self.role_ids} bonus_amount={self.bonus_amount} multiply={self.multiply}>'
-
-        def __init__(self, role_ids: Sequence[int], bonus_amount: int, multiply: bool):
-            if len(role_ids) >= 1:
-                self.role_ids = role_ids
-                self.bonus_amount = bonus_amount
-                self.multiply = multiply
-
-                if multiply and bonus_amount > 3:
-                    raise DiscordLevelingSystemError('Parameter "bonus_amount" cannot be greater than 3 when parameter "multiply" is True')
-                
-            else:
-                raise DiscordLevelingSystemError('When setting the role_ids for bonus XP, the role ID sequence cannot be empty')
-
-    @staticmethod
-    def levels_and_xp() -> Dict[str, int]:
-        """|static method|
-        
-        Get the raw :class:`dict` representation for the amount of levels/XP in the system. The keys in the :class:`dict` returned is each level, and the values are the amount of XP needed to be
-        awarded that level
-        
-        Returns
-        -------
-        Dict[:class:`str`, :class:`int`]
-
-            .. added:: v1.1.0
-        """
-        return LEVELS_AND_XP.copy()
-    
-    @staticmethod
-    def get_xp_for_level(level: int) -> int:
-        """|static method|
-        
-        Returns the total amount of XP needed for the specified level. Levels go from 0-100
-
-        Parameters
-        ----------
-        level: :class:`int`
-            The level XP information to retrieve
-
-        Returns
-        -------
-        :class:`int`
-
-        Raises
-        ------
-        - `DiscordLevelingSystemError`: The level specified does not exist
-
-            .. added:: v1.1.0
-        """
-        try:
-            return LEVELS_AND_XP[str(level)]
-        except KeyError:
-            raise DiscordLevelingSystemError(f'Levels only go from 0-100, {level} is not a valid level')
-    
-    @staticmethod
-    def create_database_file(path: Optional[str]=None) -> None:
-        """|static method|
-        
-        Create the database file and implement the SQL data for the database
-        
-        Parameters
-        ----------
-        path: Optional[:class:`str`]
-            The location to create the database file. If `None`, the file is created in the current working directory
-        
-        Raises
-        ------
-        - `ConnectionFailure`: Attempted to create the database file when the event loop is already running
-        - `DiscordLevelingSystemError`: The path does not exist or the path points to a file instead of a directory
-        
-            .. changes::
-                v0.0.2
-                    Added guild_id for database file creation
-        """
-        path = os.getcwd() if path is None else path
-        if os.path.exists(path) and os.path.isdir(path):
-            database_file = os.path.join(path, 'DiscordLevelingSystem.db')
-            with open(database_file, mode='w'):
-                try:
-                    loop = asyncio.get_event_loop()
-
-                    # create a temporary connection and build the leaderboard table
-                    connection: aiosqlite.Connection = loop.run_until_complete(aiosqlite.connect(database_file))
-                    query = """
-                        CREATE TABLE leaderboard (
-                            guild_id INT NOT NULL,
-                            member_id INT NOT NULL,
-                            member_name TEXT NOT NULL,
-                            member_level INT NOT NULL,
-                            member_xp INT NOT NULL,
-                            member_total_xp INT NOT NULL
-                        );
-                    """
-                    loop.run_until_complete(connection.execute(query))
-                    loop.run_until_complete(connection.commit())
-                except RuntimeError:
-                    raise ConnectionFailure
-        else:
-            raise DiscordLevelingSystemError(f'The path {path!r} does not exist or that path directs to a file when it is suppose to path to a directory')
-    
-    def backup_database_file(self, path: str, with_timestamp: bool=False) -> None:
-        """Create a copy of the database file to the specified path. If a copy of the backup file is already in the specified path it will be overwritten
-        
-        Parameters
-        ----------
-        path: :class:`str`
-            The path to copy the database file to
-
-        with_timestamp: :class:`bool`
-            (optional) Creates a unique file name that has the date and time of when the backup file was created. This is useful when you want multiple backup files (defaults to `False`)
-        
-        Raises
-        ------
-        - `DiscordLevelingSystemError`: Path doesn't exist or points to another file
-        - `NotConnected`: Attempted to use a method that requires a connection to a database file
-        """
-        # the decorator @db_file_exists should be used here because if :attr:`_database_file_path` is :class:`None`, it will raise TypeError, which is exactly what Exception `NotConnected` is made for
-        # and is handled inside that decorator. But to repurpose the entire function to support functions that are not coroutines is unnecessary. A simple check is all thats needed for this
-        if not self._database_file_path:
-            raise NotConnected
-            
-        if os.path.exists(path) and os.path.isdir(path):
-            if not with_timestamp:
-                database_file = os.path.join(path, 'DiscordLevelingSystem__backup.db')
-                shutil.copyfile(src=self._database_file_path, dst=database_file)
-            else:
-                dt = datetime.now()
-                dt_str = dt.strftime('%Y_%b_%d__%I_%M_%S_%p__%f')
-                database_file = os.path.join(path, 'DiscordLevelingSystem__backup(%s).db' % dt_str)
-                shutil.copyfile(src=self._database_file_path, dst=database_file)
-        else:
-            raise DiscordLevelingSystemError(f'When attempting to backup the database file, the path "{path}" does not exist or points to another file')
-    
-    def connect_to_database_file(self, path: str) -> None:
-        """Connect to the existing database file in the specified path
-        
-        Parameters
-        ----------
-        path: :class:`str`
-            The location of the database file
-        
-        Raises
-        ------
-        - `ConnectionFailure`: Attempted to connect to the database file when the event loop is already running
-        - `DatabaseFileNotFound`: The database file was not found
-        """
-        if all([os.path.exists(path), os.path.isfile(path), path.endswith('.db')]):
-            try:
-                self._connection = self._loop.run_until_complete(aiosqlite.connect(path))
-                self._cursor = self._loop.run_until_complete(self._connection.cursor())
-                self._database_file_path = path
-            except RuntimeError:
-                raise ConnectionFailure
-        else:
-            raise DatabaseFileNotFound(f'The database file in path {path!r} was not found')
-
-    async def switch_connection(self, path: str) -> None:
-        """|coro|
-        
-        Connect to a different leveling system database file
-
-        Parameters
-        ----------
-        path: :class:`str`
-            The location of the database file
-
-        Raises
-        ------
-        - `DatabaseFileNotFound`: The database file was not found
-
-            .. added:: v1.0.2
-        """
-        if all([os.path.exists(path), os.path.isfile(path), path.endswith('.db')]):
-            if self._database_file_path == path:
-                return
-            
-            # close the current connection before making a new one
-            if self._connection is not None:
-                await self._connection.close()
-
-            self._connection = await aiosqlite.connect(path)
-            self._cursor = await self._connection.cursor()
-            self._database_file_path = path
-        else:
-            raise DatabaseFileNotFound(f'The database file in path {path!r} was not found')
-    
-    def _determine_no_xp(self, message: Message) -> bool:
-        """Check if the channel the member is sending messages in is a no XP channel. This also checks if any of the roles they have is a no XP role
-        
-            .. changes::
-                v0.0.2
-                    Complete overhaul to support multi-guild leveling 
-        """
-        has_no_xp_role = False
-        in_no_xp_channel = False
-        
-        if self.no_xp_channels:
-            if message.channel.id in self.no_xp_channels:
-                in_no_xp_channel = True
-        
-        # if :var:`in_no_xp_channel` is already `True`, there's no need to execute the no xp role check
-        if in_no_xp_channel:
-            return True
-
-        if self.no_xp_roles:
-            all_member_role_ids = [role.id for role in message.author.roles] # type: ignore / will always be :class:`discord.Member` because all DM messages are ignored by the lib
-            for no_xp_role_id in self.no_xp_roles:
-                if no_xp_role_id in all_member_role_ids:
-                    has_no_xp_role = True
-                    break
-
-        return any([has_no_xp_role, in_no_xp_channel])        
-    
-    async def _update_record(self, member: Union[Member, int], level: int, xp: int, total_xp: int, guild_id: int, name: Optional[str]=None, **kwargs) -> None:
-        maybe_new_record = kwargs.get('maybe_new_record', False)
-        if maybe_new_record and not name:
-            raise Exception('kwarg "name" needs to be set when adding a new record')
-        
-        # :meth:`DiscordLevelingSystem.is_in_database` parameter "guild" expects a :class:`discord.Guild` object. We don't necessarily *need* an actual :class:`discord.Guild`
-        # object because that method really only needs the ID to operate on the correct guild. Since this method has no :class:`discord.Guild` object, just make a false guild
-        # object so :meth:`DiscordLevelingSystem.is_in_database` will work as intended
-        FakeGuild = collections.namedtuple('FakeGuild', 'id')
-        if await self.is_in_database(member, guild=FakeGuild(id=guild_id)): # type: ignore / it's a fake guild, so yes, it's not compatible with :class:`discord.Guild` that the method is looking for
-            await self._cursor.execute('UPDATE leaderboard SET member_level = ?, member_xp = ?, member_total_xp = ? WHERE member_id = ? AND guild_id = ?', (level, xp, total_xp, member.id if isinstance(member, Member) else member, guild_id)) # type: ignore
-        else:
-            await self._cursor.execute(DiscordLevelingSystem._QUERY_NEW_MEMBER, (guild_id, member.id if isinstance(member, Member) else member, name, level, xp, total_xp)) # type: ignore
-        await self._connection.commit() # type: ignore
-    
-    @staticmethod
-    def _get_transfer(path: str, loop: asyncio.AbstractEventLoop) -> NamedTuple:
-        """|static method| Connect to the target database file in the specified path and return a named tuple of the connection and cursor
-        
-            .. added:: v0.0.2
-        """
-        if all([os.path.exists(path), os.path.isfile(path), path.endswith('.db')]):
-            try:
-                connection = loop.run_until_complete(aiosqlite.connect(path))
-                cursor = loop.run_until_complete(connection.cursor())
-                Transfer = collections.namedtuple('Transfer', ['connection', 'cursor'])
-                return Transfer(connection=connection, cursor=cursor)
-            except RuntimeError:
-                raise ConnectionFailure
-        else:
-            raise DatabaseFileNotFound(f'The database file in path {path!r} was not found')
-    
-    @staticmethod
-    async def _execute_transfer(db_from: 'Transfer', db_to: 'Transfer', guild_id: int) -> None: # type: ignore
-        """|coro static method| Copy the contents from the old database file (v0.0.1), to the new database file (v0.0.2+)
-        
-            .. added:: v0.0.2
-        """
-        try:
-            from_result = await db_from.connection.execute_fetchall('SELECT * FROM leaderboard')
-        except aiosqlite.OperationalError:
-            raise DiscordLevelingSystemError('One of the databases is missing the "leaderboard" table when attempting to transfer')
-        else:
-            OLD_PRAGMA_LAYOUT = [
-                (0, 'member_id', 'INT', 0, None, 1),
-                (1, 'member_name', 'TEXT', 1, None, 0),
-                (2, 'member_level', 'INT', 1, None, 0),
-                (3, 'member_xp', 'INT', 1, None, 0),
-                (4, 'member_total_xp', 'INT', 1, None, 0)
-            ]
-            NEW_PRAGMA_LAYOUT = [
-                (0, 'guild_id', 'INT', 1, None, 0),
-                (1, 'member_id', 'INT', 1, None, 0),
-                (2, 'member_name', 'TEXT', 1, None, 0),
-                (3, 'member_level', 'INT', 1, None, 0),
-                (4, 'member_xp', 'INT', 1, None, 0),
-                (5, 'member_total_xp', 'INT', 1, None, 0)
-            ]
-            old_pragma_check = await db_from.connection.execute_fetchall('PRAGMA table_info(leaderboard)')
-            new_pragma_check = await db_to.connection.execute_fetchall('PRAGMA table_info(leaderboard)')
-            if all([old_pragma_check == OLD_PRAGMA_LAYOUT, new_pragma_check == NEW_PRAGMA_LAYOUT]):
-                # ensure the database file that the data will be transferred to is blank, if so, copy the contents to the new database file
-                await db_to.cursor.execute('SELECT COUNT(*) FROM leaderboard')
-                count_result = await db_to.cursor.fetchone()
-                if count_result[0] == 0:
-                    to_execute = []
-                    for data in from_result:
-                        to_execute.append((guild_id, data[0], data[1], data[2], data[3], data[4]))
-                    else:
-                        await db_to.cursor.executemany(DiscordLevelingSystem._QUERY_NEW_MEMBER, to_execute)
-                        await db_to.connection.commit()
-                        print('Transfer complete')
-                else:
-                    raise DiscordLevelingSystemError('When transferring the data to the new database file (created file using v0.0.2+), that database file must contain no records')
-            else:
-                raise DiscordLevelingSystemError('The "transfer" method is only to be used with transferring the data from the database file from version 0.0.1. If you were already using a database file from version 0.0.2+, there is no need to use this method')
-    
-    @staticmethod
-    def transfer(old: str, new: str, guild_id: int) -> None:
-        """|static method|
-        
-        Transfer the database records from a database file created from v0.0.1 to a blank database file created using v0.0.2+. If you were already using a v0.0.2+
-        database file, there's no need to use this method
-
-        See the following link about transfers: https://github.com/Defxult/discordLevelingSystem#migrating-from-v001-to-v002
-        
-        Parameters
-        ----------
-        old: :class:`str`
-            The path of the v0.0.1 database file
-        
-        new: :class:`str`
-            The path of the v0.0.2+ database file
-        
-        guild_id: :class:`int`
-            ID of the guild that was originally used with this library
-        
-        Raises
-        ------
-        - `ConnectionFailure`: The event loop is already running
-        - `DatabaseFileNotFound`: "old" or "new" database file was not found
-        - `DiscordLevelingSystemError`: One of the databases is missing the "leaderboard" table. A v0.0.2+ database file contains records, or there was an attempt to transfer records from a v0.0.2+ file to another v0.0.2+ file
-        
-            .. added:: v0.0.2
-        """
-        loop = asyncio.get_event_loop()
-        transfer_from = DiscordLevelingSystem._get_transfer(old, loop)
-        transfer_to = DiscordLevelingSystem._get_transfer(new, loop)
-        loop.run_until_complete(DiscordLevelingSystem._execute_transfer(transfer_from, transfer_to, guild_id))
-    
-    @db_file_exists
-    @leaderboard_exists
-    @verify_leaderboard_integrity
-    async def add_record(self, guild_id: int, member_id: int, member_name: str, level: int) -> None:
-        """|coro|
-        
-        Manually add a record to the database. If the record already exists (the :param:`guild_id` and :param:`member_id` was found), only the level will be updated. If there were no records that matched
-        those values, all provided information will be added
-
-        Parameters
-        ----------
-        guild_id: :class:`int`
-            The guild ID to register
-        
-        member_id: :class:`int`
-            The member ID to register
-        
-        member_name: :class:`str`
-            The member name to register
-        
-        level: :class:`int`
-            The member level to register. Must be from 0-100
-        
-        Raises
-        ------
-        - `DiscordLevelingSystemError`: The value given from a parameter was not of the correct type or "level" was not 0-100
-
-            .. added:: v1.0.1
-        """
-        if all([isinstance(guild_id, int), isinstance(member_id, int), isinstance(level, int)]):
-            if not (0 <= level <= 100):
-                raise DiscordLevelingSystemError('Parameter "level" must be from 0-100')
-            await self._update_record(member=member_id, level=level, xp=0, total_xp=LEVELS_AND_XP[str(level)], guild_id=guild_id, name=str(member_name), maybe_new_record=True)
-        else:
-            raise DiscordLevelingSystemError('All parameters that expect an int were not of type int')
-    
-    @overload
-    async def insert(self, bot: AutoShardedBot, guild_id: int, users: Dict[int, int], using: Literal['xp', 'levels'], overwrite: bool=False, show_results: bool=True) -> None:
-        ...
-    
-    @overload
-    async def insert(self, bot: Bot, guild_id: int, users: Dict[int, int], using: Literal['xp', 'levels'], overwrite: bool=False, show_results: bool=True) -> None:
-        ...
-
-    @db_file_exists
-    @leaderboard_exists
-    @verify_leaderboard_integrity
-    async def insert(self, bot: Union[Bot, AutoShardedBot], guild_id: int, users: Dict[int, int], using: Literal['xp', 'levels'], overwrite: bool=False, show_results: bool=True) -> None:
-        """|coro|
-        
-        Insert the records from your own leveling system into the library. A lot of leveling system tutorials out there use json files to store information. Although it might work, it is
-        insufficient because json files are not made to act as a database. Using a database file has many benefits over a json file
-        
-        If you already have records in the database file and you want to insert your records on top of the records that already exist, it is suggested to backup that
-        file using :meth:`DiscordLevelingSystem.backup_database_file()` first. If you don't have any records in your DiscordLevelingSystem database file, then there's no need to create a backup 
-
-        Parameters
-        ----------
-        bot: Union[:class:`discord.ext.commands.Bot`, :class:`discord.ext.commands.AutoShardedBot`]
-            Your bot instance variable
-        
-        guild_id: :class:`int`
-            ID of the guild that you used your leveling system with
-        
-        users: Dict[:class:`int`, :class:`int`]
-            This is the information that will be added to the database. The keys are user ID's, and the values are the users total XP or level.
-            Note: This library only uses levels 0-100 and XP 0-1899250. If any number in this dict are over the levels/XP threshold, it is implicitly set back to this libraries maximum value
-
-        using: :class:`str`
-            What structure your leveling system used. Options: "xp" or "levels". Some leveling systems give users only XP and they are ranked up based on that XP value. Others use a combination of levels and XP. If all the values
-            in the :param:`users` dict are based on XP, set this to "xp". If they are based on a users level, set this to "levels"
-        
-        overwrite: :class:`bool`
-            (optional) If a user you've specified in the :param:`users` dict already has a record in the database, overwrite their current record with the one your inserting (defaults to `False`)
-        
-        show_results: :class:`bool`
-            (optional) Print the results for how many of the :param:`users` were successfully added to the database file. If any are unsuccessful, their ID along with the value you provided will also be shown (defaults to `True`)
-        
-        Raises
-        ------
-        - `DiscordLevelingSystemError`: The value given from a parameter was not of the correct type. The :param:`users` dict was empty. Or your bot is not in the guild associated with :param:`guild_id`
-            
-            .. added:: v1.0.1
-        """
-        # Perform the necessary checks to ensure the proper values will be added to the database
-        if not isinstance(guild_id, int):
-            raise DiscordLevelingSystemError(f'Parameter "guild_id" expected int, got {guild_id.__class__.__name__}')
-        if not users:
-            raise DiscordLevelingSystemError('The "users" dict cannot be empty')
-        for k, v in users.items():
-            if not isinstance(k, int) or not isinstance(v, int):
-                raise DiscordLevelingSystemError('All keys and values in the "users" dict must be of type int')
-        
-        guild = bot.get_guild(guild_id)
-        if guild:
-            using = using.lower() # type: ignore
-            successfully_added: List[Member] = []
-            skipped_users = []
-            registered_users = []
-            SkippedUser = collections.namedtuple('SkippedUser', ['id', 'value'])
-            RegisteredUser = collections.namedtuple('RegisteredUser', ['id', 'name', 'value'])
-            for user_id, user_level_or_xp in users.items():
-                member = guild.get_member(user_id)
-                if member:
-                    if not overwrite and await self.is_in_database(user_id, guild):
-                        registered_users.append(str(RegisteredUser(id=user_id, name=str(member), value=user_level_or_xp)))
-                        continue
-                    else:
-                        if using == 'levels':
-                            level = user_level_or_xp
-                            if level < 0: level = 0
-                            elif level > MAX_LEVEL: level = MAX_LEVEL
-                            await self.set_level(member, level)
-                            successfully_added.append(member)
-                        
-                        elif using == 'xp':
-                            xp = user_level_or_xp
-                            if xp < 0: xp = 0
-                            elif xp > LEVELS_AND_XP[str(MAX_LEVEL)]: xp = LEVELS_AND_XP[str(MAX_LEVEL)]
-                            await self.set_level(member, _find_level(xp))
-                            successfully_added.append(member)
-                        
-                        else:
-                            raise DiscordLevelingSystemError(f'Parameter "using" expected "levels" or "xp", got {using!r}')
-                else:
-                    skipped_users.append(str(SkippedUser(id=user_id, value=user_level_or_xp)))
-            else:
-                if show_results:
-                    stats = cleandoc(f"""
-                        ----------------------------------------
-                        Discord Leveling System - Insert Results
-                        ----------------------------------------
-                        {len(successfully_added)} out of {len(users)} users were successfully added to the database file
-                    """)
-                    if successfully_added:
-                        MemberDataStringRepr = str
-                        data: List[MemberDataStringRepr] = [str(await self.get_data_for(stored_member)) for stored_member in successfully_added]
-                        joined_data = '\n'.join(data)
-                        stats += f'\n\nThe below {len(successfully_added)} user(s) are now apart of the Discord Leveling System and are represented as a MemberData object\n{joined_data}'
-                    
-                    if skipped_users:
-                        joined_skipped = '\n'.join(skipped_users)
-                        stats += f'\n\nThe below {len(skipped_users)} user(s) were skipped because they are not currently in guild {guild_id}\n{joined_skipped}'
-                    
-                    if registered_users:
-                        joined_registered = '\n'.join(registered_users)
-                        stats += f'\n\nThe below {len(registered_users)} user(s) were skipped because they already have a record in the database and the "overwrite" kwarg was set to False\n{joined_registered}'
-                    
-                    print(stats)
-        else:
-            raise DiscordLevelingSystemError(f'Your bot is not in guild {guild_id}')
-    
-    @overload
-    def get_awards(self, guild: Optional[Guild]=None) -> Optional[Dict[int, List[RoleAward]]]:
-        ...
-    
-    @overload
-    def get_awards(self, guild: Optional[Guild]=None) -> Optional[List[RoleAward]]:
-        ...
-    
-    @overload
-    def get_awards(self, guild: Optional[int]=None) -> Optional[Dict[int, List[RoleAward]]]:
-        ...
-    
-    @overload
-    def get_awards(self, guild: Optional[int]=None) -> Optional[List[RoleAward]]:
-        ...
-    
-    def get_awards(self, guild: Optional[Union[Guild, int]]=None) -> Optional[Union[Dict[int, List[RoleAward]], List[RoleAward]]]:
-        """Get all :class:`RoleAward`'s or only the :class:`RoleAward`'s assigned to the specified guild
-
-        Parameters
-        ----------
-        guild: Optional[Union[:class:`discord.Guild`, :class:`int`]]
-            A guild object or a guild ID
-        
-        Returns
-        -------
-        Optional[Union[Dict[:class:`int`, List[:class:`RoleAward`]], List[:class:`RoleAward`]]]: If :param:`guild` is :class:`None`, this returns the awards :class:`dict` that was set in constructor. If :param:`guild`
-        is specified, it returns a List[:class:`RoleAward`] that matches the specified guild ID. Can also return :class:`None` if awards were never set or if the awards for the specified guild was not found
-        
-            .. added:: v1.0.0
-        """
-        if self._awards:
-            if guild:
-                try:
-                    guild_id = guild.id if isinstance(guild, Guild) else guild
-                    return self._awards[guild_id].copy()
-                except KeyError:
-                    return None
-            else:
-                return self._awards.copy()
-        else:
-            return None
-    
-    @db_file_exists
-    @leaderboard_exists
-    @verify_leaderboard_integrity
-    async def add_xp(self, member: Member, amount: int) -> None:
-        """|coro|
-        
-        Give XP to a member. This also changes their level so it matches the associated XP
-
-        Parameters
-        ----------
-        member: :class:`discord.Member`
-            The member to give XP to
-        
-        amount: :class:`int`
-            Amount of XP to give to the member
-
-        Raises
-        ------
-        - `DatabaseFileNotFound`: The database file was not found
-        - `LeaderboardNotFound`: Table "leaderboard" in the database file is missing
-        - `ImproperLeaderboard`: Leaderboard table was altered. Components changed or deleted
-        - `NotConnected`: Attempted to use a method that requires a connection to a database file
-        - `DiscordLevelingSystemError`: Parameter "amount" was less than or equal to zero. The minimum value is 1 
-        
-            .. added:: v0.0.2
-        """
-        if amount <= 0:
-            raise DiscordLevelingSystemError('Parameter "amount" was less than or equal to zero. The minimum value is 1')
-        
-        md = await self.get_data_for(member)
-        if md:
-            if md.total_xp >= MAX_XP:
-                return
-            else:
-                new_total_xp = md.total_xp + amount
-                new_total_xp = new_total_xp if new_total_xp <= MAX_XP else MAX_XP
-                maybe_new_level = _find_level(new_total_xp)
-                await self._update_record(member=member, level=maybe_new_level, xp=md.xp, total_xp=new_total_xp, guild_id=member.guild.id, name=str(member), maybe_new_record=True)
-    
-    @db_file_exists
-    @leaderboard_exists
-    @verify_leaderboard_integrity
-    async def remove_xp(self, member: Member, amount: int) -> None:
-        """|coro|
-        
-        Remove XP from a member. This also changes their level so it matches the associated XP
-
-        Parameters
-        ----------
-        member: :class:`discord.Member`
-            The member to remove XP from
-        
-        amount: :class:`int`
-            Amount of XP to remove from the member
-
-        Raises
-        ------
-        - `DatabaseFileNotFound`: The database file was not found
-        - `LeaderboardNotFound`: Table "leaderboard" in the database file is missing
-        - `ImproperLeaderboard`: Leaderboard table was altered. Components changed or deleted
-        - `NotConnected`: Attempted to use a method that requires a connection to a database file
-        - `DiscordLevelingSystemError`: Parameter "amount" was less than or equal to zero. The minimum value is 1 
-        
-            .. added:: v0.0.2
-        """
-        if amount <= 0:
-            raise DiscordLevelingSystemError('Parameter "amount" was less than or equal to zero. The minimum value is 1')
-        
-        md = await self.get_data_for(member)
-        if md:
-            if md.total_xp == 0:
-                return
-            else:
-                new_total_xp = md.total_xp - amount
-                new_total_xp = new_total_xp if new_total_xp >= 1 else 0
-                maybe_new_level = _find_level(new_total_xp)
-                await self._update_record(member=member, level=maybe_new_level, xp=md.xp, total_xp=new_total_xp, guild_id=member.guild.id)
-    
-    @db_file_exists
-    @leaderboard_exists
-    @verify_leaderboard_integrity
-    async def set_level(self, member: Member, level: int) -> None:
-        """|coro|
-        
-        Sets the level for the member. This also changes their total XP so it matches the associated level
-        
-        Parameters
-        ----------
-        member: :class:`discord.Member`
-            The member who's level will be set
-        
-        level: :class:`int`
-            Level to set. Must be from 0-100
-                
-        Raises
-        ------
-        - `DatabaseFileNotFound`: The database file was not found
-        - `LeaderboardNotFound`: Table "leaderboard" in the database file is missing
-        - `ImproperLeaderboard`: Leaderboard table was altered. Components changed or deleted
-        - `NotConnected`: Attempted to use a method that requires a connection to a database file
-        - `DiscordLevelingSystemError`: Parameter "level" was not from 0-100
-        
-            .. added:: v0.0.2
-        """
-        if 0 <= level <= 100:
-            await self._update_record(member=member, level=level, xp=0, total_xp=LEVELS_AND_XP[str(level)], guild_id=member.guild.id, name=str(member), maybe_new_record=True)
-        else:
-            raise DiscordLevelingSystemError('Parameter "level" must be from 0-100')
-    
-    @db_file_exists
-    @leaderboard_exists
-    @verify_leaderboard_integrity
-    async def change_cooldown(self, rate: int, per: float) -> None:
-        """|coro|
-        
-        Update the cooldown rate
-        
-        Parameters
-        ----------
-        rate: :class:`int`
-            The amount of messages each member can send before the cooldown triggers
-
-        per: :class:`float`
-            The amount of seconds each member has to wait before gaining more XP, aka the cooldown
-
-        Raises
-        ------
-        - `DatabaseFileNotFound`: The database file was not found
-        - `LeaderboardNotFound`: Table "leaderboard" in the database file is missing
-        - `ImproperLeaderboard`: Leaderboard table was altered. Components changed or deleted
-        - `NotConnected`: Attempted to use a method that requires a connection to a database file
-        - `DiscordLevelingSystemError`: The rate or per value was not greater than zero
-        """
-        if rate <= 0 or per <= 0:   raise DiscordLevelingSystemError('Invalid rate or per. Values must be greater than zero')
-        self._cooldown = CooldownMapping.from_cooldown(rate, per, BucketType.member)
-        self.__rate = rate
-        self.__per = per
-
-    @db_file_exists
-    @leaderboard_exists
-    @verify_leaderboard_integrity
-    async def refresh_names(self, guild: Guild) -> int:
-        """|coro|
-        
-        Update names inside the database. This does not add anything new. It simply verifies if the name in the database matches their current name, and if they don't match, update
-        the database name
-        
-        Parameters
-        ----------
-        guild: :class:`discord.Guild`
-            A guild object
-        
-        Returns
-        -------
-        :class:`int`: The amount of records in the database that were updated
-
-        Raises
-        ------
-        - `DatabaseFileNotFound`: The database file was not found
-        - `LeaderboardNotFound`: Table "leaderboard" in the database file is missing
-        - `ImproperLeaderboard`: Leaderboard table was altered. Components changed or deleted
-        - `NotConnected`: Attempted to use a method that requires a connection to a database file
-        """
-        async with self._connection.execute('SELECT member_id, member_name FROM leaderboard WHERE guild_id = ?', (guild.id,)) as cursor: # type: ignore
-            result = await cursor.fetchall()
-            names_updated = 0
-            if result:
-                database_ids = [db[0] for db in result]
-                database_names = [db[1] for db in result]
-                to_execute = []
-                for db_id, db_name in zip(database_ids, database_names):
-                    member = guild.get_member(db_id)
-                    if member:
-                        if str(member) != db_name:
-                            to_execute.append((str(member), db_id, guild.id))
-                            names_updated += 1
-                else: 
-                    await cursor.executemany('UPDATE leaderboard SET member_name = ? WHERE member_id = ? AND guild_id = ?', to_execute)
-                    await self._connection.commit() # type: ignore
-
-            return names_updated
-    
-    @db_file_exists
-    @leaderboard_exists
-    @verify_leaderboard_integrity
-    async def wipe_database(self, guild: Optional[Guild]=None, *, intentional: bool=False) -> None:
-        """|coro|
-        
-        Delete EVERYTHING from the database. If :param:`guild` is specified, only the information related to that guild will be deleted
-
-        Parameters
-        ----------
-        guild: Optional[:class:`discord.Guild`]
-            The guild for which all information that is related to that guild will be deleted. If :class:`None`, everything will be deleted
-
-        intentional: :class:`bool`
-            A simple kwarg to try and ensure that this action is indeed what you want to do. Once executed, this cannot be undone
-
-        Raises
-        ------
-        - `DatabaseFileNotFound`: The database file was not found
-        - `LeaderboardNotFound`: Table "leaderboard" in the database file is missing
-        - `ImproperLeaderboard`: Leaderboard table was altered. Components changed or deleted
-        - `NotConnected`: Attempted to use a method that requires a connection to a database file
-        - `FailSafe`: "intentional" argument for this method was set to `False` in case you called this method by mistake
-        
-            .. changes::
-                v1.0.0
-                    Added :param:`guild`
-        """
-        if intentional:
-            if guild:   await self._cursor.execute('DELETE FROM leaderboard WHERE guild_id = ?', (guild.id,)) # type: ignore
-            else:       await self._cursor.execute('DELETE FROM leaderboard') # type: ignore
-            await self._connection.commit() # type: ignore
-        else:
-            raise FailSafe
-    
-    @db_file_exists
-    @leaderboard_exists
-    @verify_leaderboard_integrity
-    async def clean_database(self, guild: Guild) -> int:
-        """|coro|
-        
-        Removes the data for members that are no longer in the guild, thus reducing the database file size. It is recommended to have this method in a background loop
-        in order to keep the database file free of records that are no longer in use
-
-        Parameters
-        ----------
-        guild: :class:`discord.Guild`
-            The guild records to clean
-        
-        Returns
-        -------
-        :class:`int`: The amount of records that were removed from the database
-        
-        Raises
-        ------
-        - `DatabaseFileNotFound`: The database file was not found
-        - `LeaderboardNotFound`: Table "leaderboard" in the database file is missing
-        - `ImproperLeaderboard`: Leaderboard table was altered. Components changed or deleted
-        - `NotConnected`: Attempted to use a method that requires a connection to a database file
-        
-            .. changes::
-                v0.0.2
-                    Replaced :param:`all_members` with :param:`guild`
-        """
-        result = await self._connection.execute_fetchall('SELECT member_id FROM leaderboard WHERE guild_id = ?', (guild.id,)) # type: ignore
-        all_ids = [i[0] for i in result]
-        to_execute = []
-        records_removed = 0
-
-        for id_ in all_ids:
-            if guild.get_member(id_):
-                continue
-            else:
-                to_execute.append((id_, guild.id))
-                records_removed += 1
-        else:
-            if records_removed:
-                await self._cursor.executemany('DELETE FROM leaderboard WHERE member_id = ? AND guild_id = ?', to_execute) # type: ignore
-                await self._connection.commit() # type: ignore
-            return records_removed
-    
-    @db_file_exists
-    @leaderboard_exists
-    @verify_leaderboard_integrity
-    async def reset_member(self, member: Member) -> None:
-        """|coro|
-        
-        Sets the members XP, total XP, and level to zero
-        
-        Parameters
-        ----------
-        member: :class:`discord.Member`
-            The member to reset
-        
-        Raises
-        ------
-        - `DatabaseFileNotFound`: The database file was not found
-        - `LeaderboardNotFound`: Table "leaderboard" in the database file is missing
-        - `ImproperLeaderboard`: Leaderboard table was altered. Components changed or deleted
-        - `NotConnected`: Attempted to use a method that requires a connection to a database file
-        """
-        await self._cursor.execute('UPDATE leaderboard SET member_level = 0, member_xp = 0, member_total_xp = 0 WHERE member_id = ? AND guild_id = ?', (member.id, member.guild.id)) # type: ignore
-        await self._connection.commit() # type: ignore
-    
-    @overload
-    async def reset_everyone(self, guild: Guild, *, intentional: bool=False) -> None:
-        ...
-    
-    @overload
-    async def reset_everyone(self, guild: None, *, intentional: bool=False) -> None:
-        ...
-    
-    @db_file_exists
-    @leaderboard_exists
-    @verify_leaderboard_integrity
-    async def reset_everyone(self, guild: Union[Guild, None], *, intentional: bool=False) -> None:
-        """|coro|
-        
-        Sets EVERYONES XP, total XP, and level to zero in the database. Can specify which guild to reset
-
-        Parameters
-        ----------
-        guild: Union[:class:`discord.Guild`, :class:`None`]
-            The guild for which everyone will be reset. If this is set to :class:`None`, everyone in the entire database will be reset
-        
-        intentional: :class:`bool`
-            A simple kwarg to try and ensure that this action is indeed what you want to do. Once executed, this cannot be undone
-
-        Raises
-        ------
-        - `DatabaseFileNotFound`: The database file was not found
-        - `LeaderboardNotFound`: Table "leaderboard" in the database file is missing
-        - `ImproperLeaderboard`: Leaderboard table was altered. Components changed or deleted
-        - `NotConnected`: Attempted to use a method that requires a connection to a database file
-        - `FailSafe`: "intentional" argument for this method was set to `False` in case you called this method by mistake
-        
-            .. changes::
-                v0.0.2
-                    Added :param:`guild`
-        """
-        if intentional:
-            if guild: await self._cursor.execute('UPDATE leaderboard SET member_level = 0, member_xp = 0, member_total_xp = 0 WHERE guild_id = ?', (guild.id,)) # type: ignore
-            else:     await self._cursor.execute('UPDATE leaderboard SET member_level = 0, member_xp = 0, member_total_xp = 0') # type: ignore
-            await self._connection.commit() # type: ignore
-        else:
-            raise FailSafe
-    
-    @overload
-    async def export_as_json(self, path: str, guild: Guild) -> None:
-        ...
-    
-    @overload
-    async def export_as_json(self, path: str, guild: None) -> None:
-        ...
-    
-    @db_file_exists
-    @leaderboard_exists
-    @verify_leaderboard_integrity
-    async def export_as_json(self, path: str, guild: Union[Guild, None]) -> None:
-        """|coro|
-        
-        Export a json file that represents the database to the path specified
-        
-        Parameters
-        ----------
-        path: :class:`str`
-            Path to copy the json file to
-        
-        guild: Union[:class:`discord.Guild`, :class:`None`]
-            The guild for which the data should be extracted from. If :class:`None`, all guild information will be extracted from the database
-        
-        Raises
-        ------
-        - `DatabaseFileNotFound`: The database file was not found
-        - `LeaderboardNotFound`: Table "leaderboard" in the database file is missing
-        - `ImproperLeaderboard`: Leaderboard table was altered. Components changed or deleted
-        - `NotConnected`: Attempted to use a method that requires a connection to a database file
-        - `DiscordLevelingSystemError`: The path does not exist or does not point to a directory
-        
-            .. changes::
-                v0.0.2
-                    Added :param:`guild`. Now supports a specific guild to export
-                    Improved overall json format (easier to read)
-        """
-        if os.path.exists(path) and os.path.isdir(path):
-            path = os.path.join(path, 'discord_leveling_system.json')
-            container = []
-            if guild:
-                data = await self._connection.execute_fetchall('SELECT member_id, member_name, member_level, member_xp, member_total_xp FROM leaderboard WHERE guild_id = ?', (guild.id,)) # type: ignore
-                levels = {}
-                for m_id, m_name, m_lvl, m_xp, m_total_xp in data:
-                    levels = {
-                        'id' : m_id,
-                        'name' : m_name,
-                        'level' : m_lvl,
-                        'xp' : m_xp,
-                        'total_xp' : m_total_xp
-                    }
-                    container.append(levels.copy())
-                else:
-                    with open(path, mode='w') as fp:
-                        json.dump(container, fp, indent=4)
-            
-            else:
-                data = await self._connection.execute_fetchall('SELECT * FROM leaderboard') # type: ignore
-                for info in data:
-                    guild_id = info[0]
-                    member_id = info[1]
-                    member_name = info[2]
-                    member_level = info[3]
-                    member_xp = info[4]
-                    member_total_xp = info[5]
-                    levels = {
-                        'guild_id' : guild_id,
-                        'member_id' : member_id,
-                        'name' : member_name,
-                        'level' : member_level,
-                        'xp' : member_xp,
-                        'total_xp' : member_total_xp
-                    }
-                    container.append(levels.copy())
-                else:
-                    with open(path, mode='w') as fp:
-                        json.dump(container, fp, indent=4)
-        else:
-            raise DiscordLevelingSystemError(f'The path {path!r} does not exist or does not point to a directory')
-
-    @db_file_exists
-    @leaderboard_exists
-    @verify_leaderboard_integrity
-    async def raw_database_contents(self, guild: Optional[Guild]=None) -> List[Tuple[int, int, str, int, int, int]]:
-        """|coro|
-        
-        Returns everything in the database. Can specify which guild information will be extracted
-
-        Parameters
-        ----------
-        guild: Optional[:class:`discord.Guild`]
-            The guild to extract the raw database contents from. If :class:`None`, information about all guilds will be extracted
-        
-        Returns
-        -------
-        List[Tuple[:class:`int`, :class:`int`, :class:`str`, :class:`int`, :class:`int`, :class:`int`]]: The tuples inside the list represents each row of the database:
-        
-        - Index 0 is the guild ID
-        - Index 1 is their ID
-        - Index 2 is their name
-        - Index 3 is their level
-        - Index 4 is their XP
-        - Index 5 is their total xp
-        
-        Can be an empty list if nothing is in the database
-        
-        Raises
-        ------
-        - `DatabaseFileNotFound`: The database file was not found
-        - `LeaderboardNotFound`: Table "leaderboard" in the database file is missing
-        - `ImproperLeaderboard`: Leaderboard table was altered. Components changed or deleted
-        - `NotConnected`: Attempted to use a method that requires a connection to a database file
-        
-            .. changes::
-                v0.0.2
-                    Added :param:`guild`
-        """
-        if guild:   return await self._connection.execute_fetchall('SELECT * FROM leaderboard WHERE guild_id = ?', (guild.id,)) # type: ignore
-        else:       return await self._connection.execute_fetchall('SELECT * FROM leaderboard') # type: ignore
-    
-    @overload
-    async def remove_from_database(self, member: Member, guild: Optional[Guild]=None) -> bool:
-        ...
-    
-    @overload
-    async def remove_from_database(self, member: int, guild: Optional[Guild]=None) -> bool:
-        ...
-
-    @db_file_exists
-    @leaderboard_exists
-    @verify_leaderboard_integrity
-    async def remove_from_database(self, member: Union[Member, int], guild: Optional[Guild]=None) -> bool:
-        """|coro|
-        
-        Remove a member from the database. This is not guild specific although it can be if :param:`guild` is specified
-
-        Parameters
-        ----------
-        member: Union[:class:`discord.Member`, :class:`int`]
-            The member to remove. Can be the member object or that members ID
-
-        guild: Optional[:class:`discord.Guild`]
-            If this parameter is given, it will remove the record of the specified member only from the specified guild record. If :class:`None`, it will remove
-            all records no matter the guild
-        
-        Returns
-        -------
-        :class:`bool`: Returns `True` if the member was successfully removed from the database. `False` if the member was not in the database so there was nothing to remove
-
-        Raises
-        ------
-        - `DatabaseFileNotFound`: The database file was not found
-        - `LeaderboardNotFound`: Table "leaderboard" in the database file is missing
-        - `ImproperLeaderboard`: Leaderboard table was altered. Components changed or deleted
-        - `DiscordLevelingSystemError`: Parameter :param:`member` was not of type :class:`discord.Member` or :class:`int`
-        - `NotConnected`: Attempted to use a method that requires a connection to a database file
-        
-            .. changes::
-                v1.0.0
-                    Added :param:`guild`
-        """
-        if isinstance(member, (Member, int)):
-            member_id = member.id if isinstance(member, Member) else member
-            removable = await self.is_in_database(member_id, guild=guild if guild else None)
-            if removable:
-                query = 'DELETE FROM leaderboard WHERE member_id = ? AND guild_id = ?' if guild else 'DELETE FROM leaderboard WHERE member_id = ?'
-                params = (member_id, guild.id) if guild else (member_id,)
-                
-                await self._cursor.execute(query, params) # type: ignore
-                await self._connection.commit() # type: ignore
-            return removable
-        else:
-            raise DiscordLevelingSystemError(f'Parameter "member" expected discord.Member or int, got {member.__class__.__name__}')
-    
-    @overload
-    async def is_in_database(self, member: Member, guild: Optional[Guild]=None) -> bool:
-        ...
-    
-    @overload
-    async def is_in_database(self, member: int, guild: Optional[Guild]=None) -> bool:
-        ...
-
-    @db_file_exists
-    @leaderboard_exists
-    @verify_leaderboard_integrity
-    async def is_in_database(self, member: Union[Member, int], guild: Optional[Guild]=None) -> bool:
-        """|coro|
-        
-        A quick check to see if a member is in the database. This is not guild specific although it can be if :param:`guild` is specified
-
-        Parameters
-        ----------
-        member: Union[:class:`discord.Member`, :class:`int`]
-            The member to check for. Can be the member object or that members ID
-        
-        guild: Optional[:class:`discord.Guild`]
-            The guild to check if the member is registered in
-        
-        Returns
-        -------
-        :class:`bool`
-
-        Raises
-        ------
-        - `DatabaseFileNotFound`: The database file was not found
-        - `LeaderboardNotFound`: Table "leaderboard" in the database file is missing
-        - `ImproperLeaderboard`: Leaderboard table was altered. Components changed or deleted
-        - `NotConnected`: Attempted to use a method that requires a connection to a database file
-        - `DiscordLevelingSystemError`: Parameter :param:`member` was not of type :class:`discord.Member` or :class:`int`
-        
-            .. changes::
-                v1.0.0
-                    Added :param:`guild`
-        """
-        if not isinstance(member, (Member, int)): raise DiscordLevelingSystemError(f'Parameter "member" expected discord.Member or int, got {member.__class__.__name__}')
-        arg = member.id if isinstance(member, Member) else member
-        query = 'SELECT * FROM leaderboard WHERE member_id = ? AND guild_id = ?' if guild else 'SELECT * FROM leaderboard WHERE member_id = ?'
-        params = (arg, guild.id) if guild else (arg,)
-        
-        async with self._connection.execute(query, params) as cursor: # type: ignore
-            result = await cursor.fetchone()
-            if result: return True
-            else: return False
-        
-    @db_file_exists
-    @leaderboard_exists
-    @verify_leaderboard_integrity
-    async def get_record_count(self, guild: Optional[Guild]=None) -> int:
-        """|coro|
-        
-        Get the amount of members that are registered in the database. If :param:`guild` is set to :class:`None`, all members in the database will be counted
-
-        Parameters
-        ----------
-        guild: Optional[:class:`discord.Guild`]
-            The guild for which to count the amount of records
-
-        Returns
-        -------
-        :class:`int`
-
-        Raises
-        ------
-        - `DatabaseFileNotFound`: The database file was not found
-        - `LeaderboardNotFound`: Table "leaderboard" in the database file is missing
-        - `ImproperLeaderboard`: Leaderboard table was altered. Components changed or deleted
-        - `NotConnected`: Attempted to use a method that requires a connection to a database file
-        
-            .. changes::
-                v0.0.2
-                    Added :param:`guild`
-        """
-        if guild:   await self._cursor.execute('SELECT COUNT(*) from leaderboard WHERE guild_id = ?', (guild.id,)) # type: ignore
-        else:       await self._cursor.execute('SELECT COUNT(*) from leaderboard') # type: ignore
-        
-        result = await self._cursor.fetchone() # type: ignore
-        if result: return result[0]
-        else: return 0
-    
-    @db_file_exists
-    @leaderboard_exists
-    @verify_leaderboard_integrity
-    async def next_level_up(self, member: Member) -> Optional[int]:
-        """|coro|
-        
-        Get the amount of XP needed for the specified member to level up
-        
-        Parameters
-        ----------
-        member: :class:`discord.Member`
-            Member to get the amount of XP needed for a level up
-        
-        Returns
-        -------
-        Optional[:class:`int`]: Returns 0 if the member is currently at max level. Can return :class:`None` if the member is not in the database.
-
-        Raises
-        ------
-        - `DatabaseFileNotFound`: The database file was not found
-        - `LeaderboardNotFound`: Table "leaderboard" in the database file is missing
-        - `ImproperLeaderboard`: Leaderboard table was altered. Components changed or deleted
-        - `NotConnected`: Attempted to use a method that requires a connection to a database file
-        """
-        data = await self.get_data_for(member)
-        if not data:
-            return None
-        if data.level == 100:
-            return 0
-        else:
-            details = _next_level_details(data.level)
-            return details.xp_needed - data.xp # type: ignore / attr exists
-    
-    @db_file_exists
-    @leaderboard_exists
-    @verify_leaderboard_integrity
-    async def next_level(self, member: Member) -> Optional[int]:
-        """|coro|
-        
-        Get the next level for the specified member
-        
-        Parameters
-        ----------
-        member: :class:`discord.Member`
-            Member to get the next level for
-        
-        Returns
-        -------
-        Optional[:class:`int`]: If the member is currently max level (100), it will return 100. This can also return :class:`None` if the member is not in the database
-
-        Raises
-        ------
-        - `DatabaseFileNotFound`: The database file was not found
-        - `LeaderboardNotFound`: Table "leaderboard" in the database file is missing
-        - `ImproperLeaderboard`: Leaderboard table was altered. Components changed or deleted
-        - `NotConnected`: Attempted to use a method that requires a connection to a database file
-        
-            .. added:: v1.1.0
-        """
-        data = await self.get_data_for(member)
-        if not data:
-            return None
-        else:
-            next_level = data.level + 1
-            return MAX_LEVEL if next_level > MAX_LEVEL else next_level
-    
-    @db_file_exists
-    @leaderboard_exists
-    @verify_leaderboard_integrity
-    async def get_xp_for(self, member: Member) -> Optional[int]:
-        """|coro|
-        
-        Get the XP for the specified member
-        
-        Parameters
-        ----------
-        member: :class:`discord.Member`
-            Member to get the XP for
-        
-        Returns
-        -------
-        Optional[:class:`int`]: Can be :class:`None` if the member isn't in the database
-
-        Raises
-        ------
-        - `DatabaseFileNotFound`: The database file was not found
-        - `LeaderboardNotFound`: Table "leaderboard" in the database file is missing
-        - `ImproperLeaderboard`: Leaderboard table was altered. Components changed or deleted
-        - `NotConnected`: Attempted to use a method that requires a connection to a database file
-        """
-        md = await self.get_data_for(member)
-        if md: return md.xp
-        else: return None
-    
-    @db_file_exists
-    @leaderboard_exists
-    @verify_leaderboard_integrity
-    async def get_total_xp_for(self, member: Member) -> Optional[int]:
-        """|coro|
-        
-        Get the total XP for the specified member
-        
-        Parameters
-        ----------
-        member: :class:`discord.Member`
-            Member to get the total XP for
-        
-        Returns
-        -------
-        Optional[:class:`int`]: Can be :class:`None` if the member isn't in the database
-
-        Raises
-        ------
-        - `DatabaseFileNotFound`: The database file was not found
-        - `LeaderboardNotFound`: Table "leaderboard" in the database file is missing
-        - `ImproperLeaderboard`: Leaderboard table was altered. Components changed or deleted
-        - `NotConnected`: Attempted to use a method that requires a connection to a database file
-        """
-        md = await self.get_data_for(member)
-        if md: return md.total_xp
-        else: return None
-    
-    @db_file_exists
-    @leaderboard_exists
-    @verify_leaderboard_integrity
-    async def get_level_for(self, member: Member) -> Optional[int]:
-        """|coro|
-        
-        Get the level for the specified member
-        
-        Parameters
-        ----------
-        member: :class:`discord.Member`
-            Member to get the level for
-        
-        Returns
-        -------
-        Optional[:class:`int`]: Can be :class:`None` if the member isn't in the database
-
-        Raises
-        ------
-        - `DatabaseFileNotFound`: The database file was not found
-        - `LeaderboardNotFound`: Table "leaderboard" in the database file is missing
-        - `ImproperLeaderboard`: Leaderboard table was altered. Components changed or deleted
-        - `NotConnected`: Attempted to use a method that requires a connection to a database file
-        """
-        md = await self.get_data_for(member)
-        if md: return md.level
-        else: return None
-    
-    @db_file_exists
-    @leaderboard_exists
-    @verify_leaderboard_integrity
-    async def get_data_for(self, member: Member) -> Optional[MemberData]:
-        """|coro|
-        
-        Get the :class:`MemberData` object that represents the specified member
-        
-        Parameters
-        ----------
-        member: :class:`discord.Member`
-            The member to get the data for
-        
-        Returns
-        -------
-        Optional[:class:`MemberData`]: Can return :class:`None` if the member was not found in the database
-
-        Raises
-        ------
-        - `DatabaseFileNotFound`: The database file was not found
-        - `LeaderboardNotFound`: Table "leaderboard" in the database file is missing
-        - `ImproperLeaderboard`: Leaderboard table was altered. Components changed or deleted
-        - `NotConnected`: Attempted to use a method that requires a connection to a database file
-        """
-        async with self._connection.execute('SELECT * FROM leaderboard WHERE member_id = ? AND guild_id = ?', (member.id, member.guild.id)) as cursor: # type: ignore
-            result = await cursor.fetchone()
-            if result:
-                m_id = result[1]
-                m_name = result[2]
-                m_level = result[3]
-                m_xp = result[4]
-                m_total_xp = result[5]
-                m_rank = await self.get_rank_for(member)
-                return MemberData(m_id, m_name, m_level, m_xp, m_total_xp, m_rank)
-            else:
-                return None
-    
-    @db_file_exists
-    @leaderboard_exists
-    @verify_leaderboard_integrity
-    async def each_member_data(self, guild: Guild, sort_by: Optional[Literal['name', 'level', 'xp', 'rank']]=None, limit: Optional[int]=None) -> List[MemberData]:
-        """|coro|
-        
-        Return each member in the database as a :class:`MemberData` object for easy access to their XP, level, etc.
-
-        Parameters
-        ----------
-        guild: :class:`discord.Guild`
-            A guild object
-        
-        sort_by: Optional[:class:`str`]
-            Return each member data sorted by: "name", "level", "xp", "rank", or :class:`None`. If :class:`None`, it will return in the order they were added to the database
-        
-        limit: Optional[:class:`int`]
-            Restrict the amount of records returned to the specified amount
-        
-        Returns
-        -------
-        List[:class:`MemberData`]
-
-        Raises
-        ------
-        - `DatabaseFileNotFound`: The database file was not found
-        - `LeaderboardNotFound`: Table "leaderboard" in the database file is missing
-        - `ImproperLeaderboard`: Leaderboard table was altered. Components changed or deleted
-        - `NotConnected`: Attempted to use a method that requires a connection to a database file
-        - `DiscordLevelingSystemError`: The value of :param:`sort_by` was not recognized or :param:`guild` was not of type :class:`discord.Guild`
-
-            .. changes::
-                v1.1.0
-                    Added :param:`limit`
-        """
-        if not isinstance(guild, Guild):
-            raise DiscordLevelingSystemError(f'Parameter "guild" expected discord.Guild got {guild.__class__.__name__}')
-        else:
-            # NOTE: there's no need to worry about this method returning :class:`None` because as soon as someone sends a message they are added to the database
-
-            async def result_to_memberdata(query_result) -> List[MemberData]:
-                """Convert the query result into a :class:`list` of :class:`MemberData` objects"""
-                data = []
-                for m_id, m_name, m_level, m_xp, m_total_xp in query_result:
-                    rank = None
-                    member = guild.get_member(m_id)
-                    if member:
-                        rank = await self.get_rank_for(member) # if the member is None (no longer in guild), rank will be None. This is intentional
-                    data.append(MemberData(m_id, m_name, m_level, m_xp, m_total_xp, rank))
-                return data if limit is None else data[:limit]
-
-            if not sort_by:
-                result = await self._connection.execute_fetchall('SELECT member_id, member_name, member_level, member_xp, member_total_xp FROM leaderboard WHERE guild_id = ?', (guild.id,)) # type: ignore
-                return await result_to_memberdata(result)
-            else:
-                sort_by = sort_by.lower() # type: ignore
-                if sort_by in ('name', 'level', 'xp', 'rank'):
-                    if sort_by == 'name':
-                        result = await self._connection.execute_fetchall('SELECT member_id, member_name, member_level, member_xp, member_total_xp FROM leaderboard WHERE guild_id = ? ORDER BY member_name COLLATE NOCASE', (guild.id,)) # type: ignore
-                        return await result_to_memberdata(result)
-                    
-                    elif sort_by == 'level':
-                        result = await self._connection.execute_fetchall('SELECT member_id, member_name, member_level, member_xp, member_total_xp FROM leaderboard WHERE guild_id = ? ORDER BY member_level DESC', (guild.id,)) # type: ignore
-                        return await result_to_memberdata(result)
-                    
-                    elif sort_by == 'xp':
-                        result = await self._connection.execute_fetchall('SELECT member_id, member_name, member_level, member_xp, member_total_xp FROM leaderboard WHERE guild_id = ? ORDER BY member_total_xp DESC', (guild.id,)) # type: ignore
-                        return await result_to_memberdata(result)
-
-                    elif sort_by == 'rank':
-                        def convert(md: MemberData) -> MemberData:
-                            """Set the rank to an :class:`int` value of 0 because it is not possible to sort a list of :class:`int` that has :class:`None` values"""
-                            if md.rank is None:
-                                md.rank = 0
-                            return md
-                        
-                        result = await self._connection.execute_fetchall('SELECT member_id, member_name, member_level, member_xp, member_total_xp FROM leaderboard WHERE guild_id = ?', (guild.id,)) # type: ignore
-                        all_data: List[MemberData] = await result_to_memberdata(result)
-                        
-                        converted = [convert(md) for md in all_data] # convert the data so it can be sorted properly
-                        sorted_converted = sorted(converted, key=lambda md: md.rank) # type: ignore
-
-                        no_rank = [md for md in sorted_converted if md.rank == 0]
-                        with_rank = [md for md in sorted_converted if md.rank != 0]
-                        pre_final = with_rank + no_rank
-    
-                        def zero_to_none(md: MemberData) -> MemberData:
-                            """If they're not in the guild anymore, I don't want their rank to be presented as zero because that implies they are still in the guild, but just has
-                            a rank of zero. Setting it back to :class:`None` makes it more readable and draws further implication that they're no longer in the guild
-                            """
-                            if md.rank == 0:
-                                md.rank = None
-                            return md
-                        
-                        final = [zero_to_none(md) for md in pre_final]
-                        return final
-                else:
-                    raise DiscordLevelingSystemError(f'Parameter "sort_by" expected "name", "level", "xp", or "rank", {sort_by!r} was not recognized')
-    
-    @db_file_exists
-    @leaderboard_exists
-    @verify_leaderboard_integrity
-    async def get_rank_for(self, member: Member) -> Optional[int]:
-        """|coro|
-        
-        Get the rank for the specified member
-        
-        Parameters
-        ----------
-        member: :class:`discord.Member`
-            Member to get the rank for
-        
-        Returns
-        -------
-        Optional[:class:`int`]: Can be :class:`None` if the member isn't ranked yet
-
-        Raises
-        ------
-        - `DatabaseFileNotFound`: The database file was not found
-        - `LeaderboardNotFound`: Table "leaderboard" in the database file is missing
-        - `ImproperLeaderboard`: Leaderboard table was altered. Components changed or deleted
-        - `NotConnected`: Attempted to use a method that requires a connection to a database file
-        """
-        result = await self._connection.execute_fetchall('SELECT member_id FROM leaderboard WHERE guild_id = ? ORDER BY member_total_xp DESC', (member.guild.id,)) # type: ignore
-        all_ids = [m_id[0] for m_id in result]
-        try:
-            rank = all_ids.index(member.id) + 1
-            return rank
-        except ValueError:
-            return None
-    
-    @db_file_exists
-    @leaderboard_exists
-    @verify_leaderboard_integrity
-    async def sql_query_get(self, sql: str, parameters: Optional[Tuple[Union[str, int]]]=None, fetch: Union[str, int]='ALL') -> Union[List[tuple], tuple]:
-        """|coro|
-        
-        Query and return something from the database using SQL. The following columns are apart of the "leaderboard" table:
-
-        - guild_id
-        - member_id
-        - member_name
-        - member_level
-        - member_xp
-        - member_total_xp
-
-        Parameters
-        ----------
-        sql: :class:`str`
-            SQL string used to query the database
-        
-        parameters: Optional[Tuple[Union[:class:`str`, :class:`int`]]]
-            The parameters used for the database query
-        
-        fetch: Union[:class:`str`, :class:`int`]
-            The amount of rows you would like back from the query. Options: 'ALL', 'ONE', or an integer value that is greater than zero
-        
-        Returns
-        -------
-        Union[List[:class:`tuple`], :class:`tuple`]:
-
-        - Using `fetch='ALL'` returns List[:class:`tuple`]
-        - Using `fetch='ONE'` returns :class:`tuple`
-        - Using `fetch=4` returns List[:class:`tuple`] with only four values
-        
-        Can also return an empty list if the query was valid but got nothing from it
-        
-        Raises
-        ------
-        - `DatabaseFileNotFound`: The database file was not found
-        - `LeaderboardNotFound`: Table "leaderboard" in the database file is missing
-        - `ImproperLeaderboard`: Leaderboard table was altered. Components changed or deleted
-        - `NotConnected`: Attempted to use a method that requires a connection to a database file
-        - `DiscordLevelingSystemError`: Argument "fetch" was the wrong type or used an invalid value
-        - `aiosqlite.Error`: Base aiosqlite error. Multiple errors can arise from this if the SQL query was invalid
-        """
-        if isinstance(fetch, str):
-            fetch = fetch.upper()
-            if fetch in ('ALL', 'ONE'):
-                async with self._connection.execute(sql, parameters) as cursor: # type: ignore
-                    if fetch == 'ALL':
-                        return await cursor.fetchall() # type: ignore
-                    elif fetch == 'ONE':
-                        return await cursor.fetchone() # type: ignore
-            else:
-                raise DiscordLevelingSystemError(f'Fetch {fetch!r} not recognized')
-        elif isinstance(fetch, int):
-            if fetch > 0:
-                async with self._connection.execute(sql, parameters) as cursor: # type: ignore
-                    return await cursor.fetchmany(fetch) # type: ignore
-            else:
-                raise DiscordLevelingSystemError('Argument "fetch" must be greater than zero')
-        else:
-            raise DiscordLevelingSystemError(f'Argument "fetch" needs to be str or int, got {fetch.__class__.__name__}')
-    
-    def _get_last_award(self, current_award: RoleAward, guild_awards: List[RoleAward]) -> RoleAward:
-        """Get the last :class:`RoleAward` that was given to the member. Returns the current :class:`RoleAward` if the last award is the current one
-        
-            .. changes::
-                v0.0.2
-                    Added :param:`guild_awards`
-        """
-        current_award_idx = guild_awards.index(current_award)
-        last_award_idx = guild_awards.index(current_award) - 1
-        if last_award_idx < 0:
-            last_award_idx = current_award_idx
-
-        if last_award_idx == current_award_idx:
-            return current_award
-        else:
-            return guild_awards[last_award_idx]
-    
-    async def _refresh_name(self, message: Message) -> None:
-        """|coro| If the members current database name doesn't match the name that's on discord, update the name in the database
-
-            .. NOTE
-                This is called AFTER we update or insert a new member into the database from :meth:`award_xp`, so :meth:`fetchone` will always return something
-        """
-        async with self._connection.execute('SELECT member_name FROM leaderboard WHERE member_id = ? AND guild_id = ?', (message.author.id, message.author.guild.id)) as cursor: # type: ignore
-            data = await cursor.fetchone()
-            database_name = data[0] # type: ignore / will always have a value because as *soon* as a member sends a message, the database is updated to contain a value to fetch
-            if database_name != str(message.author):
-                await cursor.execute('UPDATE leaderboard SET member_name = ? WHERE member_id = ? AND guild_id = ?', (str(message.author), message.author.id, message.author.guild.id)) # type: ignore
-                await self._connection.commit() # type: ignore
-    
-    async def _handle_level_up(self, message: Message, md: MemberData, leveled_up: bool) -> None:
-        """|coro| Gives/removes roles from members that leveled up and met the :class:`RoleAward` requirement. This also sends the level up message
-        
-            .. changes::
-                v0.0.2
-                    Added handling for level up messages that are embeds
-                    Added handling for random selections of level up messages
-                    Added :param:`md`
-                    Added :param:`leveled_up`
-                    Added if check for :param:`leveled_up`
-                    Added :func:`send_announcement`
-                    Removed raising of exception (AwardedRoleNotFound) to support multi-guild leveling
-                    Removed raising of exception (LevelUpChannelNotFound) to support multi-guild level up channel IDs
-                v1.0.2
-                    Added handling for event `on_dls_level_up`
-        """
-        if leveled_up:
-            member: Member = message.author # type: ignore / `.author` will be :class:`discord.Member` (lib doesn't work in DMs)
-            
-            def role_exists(award: RoleAward) -> Optional[Role]:
-                """Check to ensure the role associated with the :class:`RoleAward` still exists in the guild. If it does, it returns that discord role object for use"""
-                return message.guild.get_role(award.role_id) # type: ignore / `.guild` will always be :class:`discord.Guild`
-            
-            async def send_announcement(announcement_message, channel, send_kwargs):
-                """|coro| Send the level up message
-
-                    .. added:: v0.0.2
-                """
-                if isinstance(announcement_message, str):
-                    await channel.send(announcement_message, **send_kwargs)
-                else:
-                    await channel.send(embed=announcement_message, **send_kwargs)
-            
-            # send the level up message
-            if self.announce_level_up:
-                
-                # set the values for the level up announcement
-                lua: LevelUpAnnouncement = random.choice(self.level_up_announcement) if isinstance(self.level_up_announcement, Sequence) else self.level_up_announcement
-                lua._total_xp = md.total_xp
-                lua._level = md.level
-                lua._rank = md.rank
-                announcement_message = lua._parse_message(lua.message, self._message_author) # type: ignore
-
-                if lua.level_up_channel_ids:
-                    channel_found = False
-                    for channel_id in lua.level_up_channel_ids:
-                        channel = message.guild.get_channel(channel_id) # type: ignore / `.guild` will always be :class:`discord.Guild`
-                        if channel:
-                            channel_found = True
-                            break
-                    
-                    if channel_found:
-                        await send_announcement(announcement_message, channel, lua._send_kwargs) # type: ignore / this will not execute if channel not found
-                    else:
-                        await send_announcement(announcement_message, message.channel, lua._send_kwargs)
-                else:
-                    await send_announcement(announcement_message, message.channel, lua._send_kwargs)
-            
-            # check if there is a role award for the new level, if so, apply it
-            if self._awards:
-                try:
-                    # get the list of RoleAwards that match the guild ID
-                    guild_role_awards: List[RoleAward] = self._awards[message.guild.id] # type: ignore / `.guild` will always be :class:`discord.Guild`
-                except KeyError:
-                    return
-                else:
-                    # get the role award that matches the level up
-                    role_award = [ra for ra in guild_role_awards if ra.level_requirement == md.level]
-                    if role_award:
-                        role_award = role_award[0]
-                        if self.stack_awards:
-                            role_obj: Optional[Role] = role_exists(award=role_award)
-                            if role_obj:
-                                await member.add_roles(role_obj)
-                            else:
-                                return
-                        else:
-                            last_award: RoleAward = self._get_last_award(role_award, guild_role_awards)
-                            role_to_remove: Optional[Role] = role_exists(award=last_award)
-                            role_to_add: Optional[Role] = role_exists(award=role_award)
-                            
-                            # Note: Don't use an exception here because of multi-guild support
-                            if not role_to_remove or not role_to_add:
-                                return
-
-                            if last_award == role_award:
-                                await member.add_roles(role_to_add)
-                            else:
-                                await member.add_roles(role_to_add)
-                                await member.remove_roles(role_to_remove)
-            
-            if self.bot is not None:
-                self.bot.dispatch('dls_level_up', member, message, md)
-    
-    def _handle_amount_param(self, arg: Union[int, Sequence[int]]) -> None:
-        """Simple check to ensure the proper types are being used for parameter "amount" in method :meth:`DiscordLevelingSystem.award_xp()`
-        
-            .. changes::
-                v0.0.2
-                    Added check to ensure the first value is larger than the next
-                    Added check to ensure the each value is unique
-                    Changed the value range from 1-100 to 1-25
-                v1.1.0
-                    Changed from list to Sequence
-        """
-        if isinstance(arg, (int, Sequence)):
-            if isinstance(arg, int):
-                # ensures the values are from 1-25
-                if arg <= 0 or arg > 25:
-                    raise DiscordLevelingSystemError('Parameter "amount" can only be a value from 1-25')
-            else:
-                # ensures there are only 2 values in the sequence
-                if len(arg) != 2:
-                    raise DiscordLevelingSystemError('Parameter "amount" sequence must only have two values')
-                
-                # ensures all values in the sequence are of type int
-                for item in arg:
-                    if not isinstance(item, int):
-                        raise DiscordLevelingSystemError('Parameter "amount" sequence, all values must be of type int')
-                
-                # ensures all values in the sequence are >= 1 and <= 25
-                for item in arg:
-                    if item <= 0 or item > 25:
-                        raise DiscordLevelingSystemError('Parameter "amount" sequence, all values can only be from 1-25')
-                
-                # ensures each value is unique
-                if arg[0] == arg[1]:
-                    raise DiscordLevelingSystemError('Parameter "amount" sequence expects both values to be unique')
-                
-                # ensures the first value is larger than the next
-                if arg[1] < arg[0]:
-                    raise DiscordLevelingSystemError('Parameter "amount" sequence expected value 1 to be larger than value 2')
-        else:
-            raise DiscordLevelingSystemError(f'Parameter "amount" expected int or Sequence, got {arg.__class__.__name__}')
-    
-    @overload
-    async def award_xp(self, *, amount: int, message: Message, refresh_name: bool=True, **kwargs) -> None:
-        ...
-    
-    @overload
-    async def award_xp(self, *, amount: Sequence[int]=[15, 25], message: Message, refresh_name: bool=True, **kwargs) -> None:
-        ...
-    
-    @db_file_exists
-    @leaderboard_exists
-    @verify_leaderboard_integrity
-    async def award_xp(self, *, amount: Union[int, Sequence[int]]=[15, 25], message: Message, refresh_name: bool=True, **kwargs) -> None:
-        """|coro|
-        
-        Give XP to the member that sent a message
-
-        Parameters
-        ----------
-        amount: Union[:class:`int`, Sequence[:class:`int`]]
-            The amount of XP to award to the member per message. Must be from 1-25. Can be a sequence with a minimum and maximum length of two. If :param:`amount` is a sequence of two integers, it will randomly
-            pick a number in between those numbers including the numbers provided
-        
-        message: :class:`discord.Message`
-            A message object
-        
-        refresh_name: :class:`bool`
-            Everytime the member sends a message, check if their name still matches the name in the database. If it doesn't match, update the database to match their current name. It is
-            suggested to leave this as `True` so the database can always have the most up-to-date record
-
-        Kwargs
-        ------
-        bonus: :class:`DiscordLevelingSystem.Bonus`
-            Set the bonus values. Read the :class:`DiscordLevelingSystem.Bonus` doc string for more details (defaults to :class:`None`)
-        
-        Raises
-        ------
-        - `DatabaseFileNotFound`: The database file was not found
-        - `LeaderboardNotFound`: Table "leaderboard" in the database file is missing
-        - `ImproperLeaderboard`: Leaderboard table was altered. Components changed or deleted
-        - `NotConnected`: Attempted to use a method that requires a connection to a database file
-        
-            .. changes::
-                v0.0.2
-                    Added handling for bonus xp (kwarg "bonus")
-                    Added initialization for :attr:`_message_author`
-                    Replaced query with class attr
-                    Moved the detection of a level up from :meth:`_handle_level_up` to here
-        """
-        if any([message.guild is None, self._determine_no_xp(message), message.author.bot, message.type != MessageType.default, self.active is False]):
-            return
-        else:
-            self._handle_amount_param(arg=amount)
-            if isinstance(amount, Sequence):
-                amount = random.randint(amount[0], amount[1])
-            
-            # bonus XP
-            bonus: Optional[DiscordLevelingSystem.Bonus] = kwargs.get('bonus')
-            if bonus:
-                for role_id in bonus.role_ids:
-                    role: Optional[Role] = message.guild.get_role(role_id) # type: ignore
-                    if role in message.author.roles: # type: ignore / This lib cannot operate with :class:`discord.User` (DM's). It will always be :class:`discord.Member`
-                        if bonus.multiply:
-                            amount *= bonus.bonus_amount
-                        else:
-                            amount += bonus.bonus_amount
-                        
-                        if amount > 75:
-                            amount = 75
-                        break
-            
-            bucket = self._cooldown.get_bucket(message)
-            on_cooldown = bucket.update_rate_limit() # type: ignore
-
-            if not on_cooldown:
-                member = message.author
-                self._message_author = member # type: ignore
-                async with self._connection.execute('SELECT * FROM leaderboard WHERE member_id = ? AND guild_id = ?', (member.id, member.guild.id)) as cursor: # type: ignore
-                    record = await cursor.fetchone()
-                    member_level_up = False
-                    if record:
-                        # update the database with the new amount
-                        query = """
-                            UPDATE leaderboard
-                            SET member_xp = member_xp + ?, member_total_xp = member_total_xp + ?
-                            WHERE member_id = ? AND guild_id = ?
-                        """
-                        await cursor.execute(query, (amount, amount, member.id, member.guild.id)) # type: ignore
-                        await self._connection.commit() # type: ignore
-
-                        # get the updated member data (level is not updated yet)
-                        md = await self.get_data_for(member) # type: ignore
-
-                        next_details = _next_level_details(md.level) # type: ignore
-                        if md.xp >= next_details.xp_needed and md.level < next_details.level: # type: ignore
-                            # update the database with the new level and reset the current XP count
-                            await cursor.execute('UPDATE leaderboard SET member_level = ?, member_xp = ? WHERE member_id = ? AND guild_id = ?', (next_details.level, 0, member.id, member.guild.id)) # type: ignore
-                            await self._connection.commit() # type: ignore
-                            member_level_up = True
-
-                        md = await self.get_data_for(member) # type: ignore
-                        await self._handle_level_up(message, md, leveled_up=member_level_up) # type: ignore
-
-                    else:
-                        await cursor.execute(DiscordLevelingSystem._QUERY_NEW_MEMBER, (member.guild.id, member.id, str(member), 0, amount, amount)) # type: ignore
-                        await self._connection.commit() # type: ignore
-
-                    if refresh_name:
-                        await self._refresh_name(message)
+"""
+MIT License
+
+Copyright (c) 2021-present Defxult#8269
+
+Permission is hereby granted, free of charge, to any person obtaining a
+copy of this software and associated documentation files (the "Software"),
+to deal in the Software without restriction, including without limitation
+the rights to use, copy, modify, merge, publish, distribute, sublicense,
+and/or sell copies of the Software, and to permit persons to whom the
+Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in
+all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS
+OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER 
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING 
+FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER 
+DEALINGS IN THE SOFTWARE.
+"""
+
+import asyncio
+import collections
+import json
+import os
+import random
+import shutil
+from collections.abc import Sequence
+from datetime import datetime
+from inspect import cleandoc
+from typing import Dict, List, Literal, NamedTuple, Optional, overload, Tuple, Union
+
+import aiosqlite
+from discord import Guild, Member, Message, MessageType, Role
+from discord.ext.commands import AutoShardedBot, Bot, BucketType, CooldownMapping
+
+from .announcement import LevelUpAnnouncement
+from .decorators import db_file_exists, leaderboard_exists, verify_leaderboard_integrity
+from .errors import *
+from .levels_xp_needed import *
+from .member_data import MemberData
+from .role_awards import RoleAward
+
+
+class DiscordLevelingSystem:
+    """A local discord.py leveling system powered by SQLite
+
+    Parameters
+    ----------
+    rate: :class:`int`
+        The amount of messages each member can send before the cooldown triggers
+
+    per: :class:`float`
+        The amount of seconds each member has to wait before gaining more XP, aka the cooldown
+    
+    awards: Optional[Dict[:class:`int`, List[:class:`RoleAward`]]]
+        The role given to a member when they reach a :class:`RoleAward` level requirement
+
+    Kwargs
+    ------
+    no_xp_roles: Sequence[:class:`int`]
+        A sequence of role ID's. Any member with any of those roles will not gain XP when sending messages (defaults to :class:`None`)
+    
+    no_xp_channels: Sequence[:class:`int`]
+        A sequence of text channel ID's. Any member sending messages in any of those text channels will not gain XP (defaults to :class:`None`)
+    
+    announce_level_up: :class:`bool`
+        If `True`, level up messages will be sent when a member levels up (defaults to `True`)
+
+    stack_awards: :class:`bool`
+        If this is `True`, when the member levels up the assigned role award will be applied. If `False`, the previous role award will be removed
+        and the level up assigned role will also be applied (defaults to `True`)
+
+    level_up_announcement: Union[:class:`LevelUpAnnouncement`, Sequence[:class:`LevelUpAnnouncement`]]
+        The message that is sent when someone levels up. If this is a list of :class:`LevelUpAnnouncement`, one is selected at random (defaults to :class:`LevelUpAnnouncement()`)
+    
+    bot: Union[:class:`discord.ext.commands.AutoShardedBot`, :class:`discord.ext.commands.Bot`]
+        Your bot instance variable. Used only if you'd like to use the `on_dls_level_up` event (defaults to :class:`None`)
+    
+    Attributes
+    ----------
+    - `no_xp_roles`
+    - `no_xp_channels`
+    - `announce_level_up`
+    - `stack_awards`
+    - `level_up_announcement`
+    - `active`
+    - `bot`
+    - `rate` (property)
+    - `per` (property)
+    - `database_file_path` (property)
+    """
+    
+    _QUERY_NEW_MEMBER = """
+        INSERT INTO leaderboard
+        VALUES (?, ?, ?, ?, ?, ?)
+    """
+
+    def __init__(self, rate: int=1, per: float=60.0, awards: Optional[Dict[int, List[RoleAward]]]=None, **kwargs):
+        if rate <= 0 or per <= 0:   raise DiscordLevelingSystemError('Invalid rate or per. Values must be greater than zero')
+        self.__rate = rate
+        self.__per = per
+
+        RoleAward._check(awards)
+        self._awards = awards
+
+        self.no_xp_roles: Optional[Sequence[int]] = kwargs.get('no_xp_roles')
+        self.no_xp_channels: Optional[Sequence[int]] = kwargs.get('no_xp_channels')
+        self.announce_level_up: bool = kwargs.get('announce_level_up', True)
+        self.stack_awards: bool = kwargs.get('stack_awards', True)
+        self.level_up_announcement: Union[LevelUpAnnouncement, Sequence[LevelUpAnnouncement]] = kwargs.get('level_up_announcement', LevelUpAnnouncement())
+
+        self._connection: Optional[aiosqlite.Connection] = None
+        self._cursor: Optional[aiosqlite.Cursor] = None
+        
+        self._cooldown = CooldownMapping.from_cooldown(rate, per, BucketType.member)
+        self._loop = asyncio.get_event_loop()
+        self._database_file_path: Optional[str] = None
+
+        # v0.0.2
+        self._message_author: Optional[Member] = None
+
+        # v1.0.0
+        self.active = True
+
+        # v1.0.2
+        self.bot: Optional[Union[AutoShardedBot, Bot]] = kwargs.get('bot')
+    
+    @property
+    def rate(self) -> int:
+        """
+        Returns
+        -------
+        :class:`int`: The amount of messages each member can send before the cooldown triggers
+
+            .. added:: v0.0.2
+        """
+        return self.__rate
+    
+    @property
+    def per(self) -> float:
+        """
+        Returns
+        -------
+        :class:`float`: The amount of seconds each member has to wait before gaining more XP, aka the cooldown
+            
+            .. added:: v0.0.2
+        """
+        return self.__per
+    
+    @property
+    def database_file_path(self) -> Optional[str]:
+        """
+        Returns
+        -------
+        Optional[:class:`str`]: The path of the current database file. Could be :class:`None` if the database connection was never set
+
+            .. added:: v1.0.2
+        """
+        return self._database_file_path
+
+    class Bonus:
+        """Set the roles that gives x amount of extra XP to the member. This is to be used with kwarg "bonus" in the :meth:`award_xp` method
+
+        Note
+        ----
+        Having :param:`multiply` as `True` and :param:`bonus_amount` be greater than 3 is not allowed. If :param:`multiply` is `True`, :param:`bonus_amount` needs to be less than or equal to 3.
+        It should also be noted that if :param:`multiply` is `False`, it doesn't matter what :param:`bonus_amount` you use but if the total amount (awarded XP + the bonus) is greater than 75, the
+        value is implicitly changed back to 75. The maximum amount of XP a member can earn through sending messages is 75.
+
+        Parameters
+        ----------
+        role_ids: Sequence[:class:`int`]
+            The roles a member must have to be able to get bonus XP. They only need to have one of these roles to get the bonus
+
+        bonus_amount: :class:`int`
+            Amount of extra XP to be awarded
+
+        multiply: :class:`bool`
+            If set to `True`, this will operate on a x2, x3 basis. Meaning if you have the awarded XP set to 10 and you want the bonus XP role to be awarded 20, it must be set to 2,
+            not 10. If `False`, it operates purely on the given value. Meaning if you have the awarded XP set to 10 and you want the bonus XP role to be awarded 20, it must be set to 10
+        
+        Attributes
+        ----------
+        - `role_ids`
+        - `bonus_amount`
+        - `multiply`
+
+        Example
+        -------
+        ```
+        lvl = DiscordLevelingSystem(...)
+
+        nitro_booster = 851379776111116329
+        associate_role = 851400453904400385
+
+        @bot.event
+        async def on_message(message):
+            await lvl.award_xp(amount=[15, 25], message=message, bonus=DiscordLevelingSystem.Bonus([nitro_booster, associate_role], 20, multiply=False))
+        ```
+
+            .. added:: v0.0.2
+        """
+        __slots__ = ('role_ids', 'bonus_amount', 'multiply')
+
+        def __repr__(self):
+            return f'<Bonus role_ids={self.role_ids} bonus_amount={self.bonus_amount} multiply={self.multiply}>'
+
+        def __init__(self, role_ids: Sequence[int], bonus_amount: int, multiply: bool):
+            if len(role_ids) >= 1:
+                self.role_ids = role_ids
+                self.bonus_amount = bonus_amount
+                self.multiply = multiply
+
+                if multiply and bonus_amount > 3:
+                    raise DiscordLevelingSystemError('Parameter "bonus_amount" cannot be greater than 3 when parameter "multiply" is True')
+                
+            else:
+                raise DiscordLevelingSystemError('When setting the role_ids for bonus XP, the role ID sequence cannot be empty')
+
+    @staticmethod
+    def levels_and_xp() -> Dict[str, int]:
+        """|static method|
+        
+        Get the raw :class:`dict` representation for the amount of levels/XP in the system. The keys in the :class:`dict` returned is each level, and the values are the amount of XP needed to be
+        awarded that level
+        
+        Returns
+        -------
+        Dict[:class:`str`, :class:`int`]
+
+            .. added:: v1.1.0
+        """
+        return LEVELS_AND_XP.copy()
+    
+    @staticmethod
+    def get_xp_for_level(level: int) -> int:
+        """|static method|
+        
+        Returns the total amount of XP needed for the specified level. Levels go from 0-100
+
+        Parameters
+        ----------
+        level: :class:`int`
+            The level XP information to retrieve
+
+        Returns
+        -------
+        :class:`int`
+
+        Raises
+        ------
+        - `DiscordLevelingSystemError`: The level specified does not exist
+
+            .. added:: v1.1.0
+        """
+        try:
+            return LEVELS_AND_XP[str(level)]
+        except KeyError:
+            raise DiscordLevelingSystemError(f'Levels only go from 0-100, {level} is not a valid level')
+    
+    @staticmethod
+    def create_database_file(path: Optional[str]=None) -> None:
+        """|static method|
+        
+        Create the database file and implement the SQL data for the database
+        
+        Parameters
+        ----------
+        path: Optional[:class:`str`]
+            The location to create the database file. If `None`, the file is created in the current working directory
+        
+        Raises
+        ------
+        - `ConnectionFailure`: Attempted to create the database file when the event loop is already running
+        - `DiscordLevelingSystemError`: The path does not exist or the path points to a file instead of a directory
+        
+            .. changes::
+                v0.0.2
+                    Added guild_id for database file creation
+        """
+        path = os.getcwd() if path is None else path
+        if os.path.exists(path) and os.path.isdir(path):
+            database_file = os.path.join(path, 'DiscordLevelingSystem.db')
+            with open(database_file, mode='w'):
+                try:
+                    loop = asyncio.get_event_loop()
+
+                    # create a temporary connection and build the leaderboard table
+                    connection: aiosqlite.Connection = loop.run_until_complete(aiosqlite.connect(database_file))
+                    query = """
+                        CREATE TABLE leaderboard (
+                            guild_id INT NOT NULL,
+                            member_id INT NOT NULL,
+                            member_name TEXT NOT NULL,
+                            member_level INT NOT NULL,
+                            member_xp INT NOT NULL,
+                            member_total_xp INT NOT NULL
+                        );
+                    """
+                    loop.run_until_complete(connection.execute(query))
+                    loop.run_until_complete(connection.commit())
+                except RuntimeError:
+                    raise ConnectionFailure
+        else:
+            raise DiscordLevelingSystemError(f'The path {path!r} does not exist or that path directs to a file when it is suppose to path to a directory')
+    
+    def backup_database_file(self, path: str, with_timestamp: bool=False) -> None:
+        """Create a copy of the database file to the specified path. If a copy of the backup file is already in the specified path it will be overwritten
+        
+        Parameters
+        ----------
+        path: :class:`str`
+            The path to copy the database file to
+
+        with_timestamp: :class:`bool`
+            (optional) Creates a unique file name that has the date and time of when the backup file was created. This is useful when you want multiple backup files (defaults to `False`)
+        
+        Raises
+        ------
+        - `DiscordLevelingSystemError`: Path doesn't exist or points to another file
+        - `NotConnected`: Attempted to use a method that requires a connection to a database file
+        """
+        # the decorator @db_file_exists should be used here because if :attr:`_database_file_path` is :class:`None`, it will raise TypeError, which is exactly what Exception `NotConnected` is made for
+        # and is handled inside that decorator. But to repurpose the entire function to support functions that are not coroutines is unnecessary. A simple check is all thats needed for this
+        if not self._database_file_path:
+            raise NotConnected
+            
+        if os.path.exists(path) and os.path.isdir(path):
+            if not with_timestamp:
+                database_file = os.path.join(path, 'DiscordLevelingSystem__backup.db')
+                shutil.copyfile(src=self._database_file_path, dst=database_file)
+            else:
+                dt = datetime.now()
+                dt_str = dt.strftime('%Y_%b_%d__%I_%M_%S_%p__%f')
+                database_file = os.path.join(path, 'DiscordLevelingSystem__backup(%s).db' % dt_str)
+                shutil.copyfile(src=self._database_file_path, dst=database_file)
+        else:
+            raise DiscordLevelingSystemError(f'When attempting to backup the database file, the path "{path}" does not exist or points to another file')
+    
+    def connect_to_database_file(self, path: str) -> None:
+        """Connect to the existing database file in the specified path
+        
+        Parameters
+        ----------
+        path: :class:`str`
+            The location of the database file
+        
+        Raises
+        ------
+        - `ConnectionFailure`: Attempted to connect to the database file when the event loop is already running
+        - `DatabaseFileNotFound`: The database file was not found
+        """
+        if all([os.path.exists(path), os.path.isfile(path), path.endswith('.db')]):
+            try:
+                self._connection = self._loop.run_until_complete(aiosqlite.connect(path))
+                self._cursor = self._loop.run_until_complete(self._connection.cursor())
+                self._database_file_path = path
+            except RuntimeError:
+                raise ConnectionFailure
+        else:
+            raise DatabaseFileNotFound(f'The database file in path {path!r} was not found')
+
+    async def switch_connection(self, path: str) -> None:
+        """|coro|
+        
+        Connect to a different leveling system database file
+
+        Parameters
+        ----------
+        path: :class:`str`
+            The location of the database file
+
+        Raises
+        ------
+        - `DatabaseFileNotFound`: The database file was not found
+
+            .. added:: v1.0.2
+        """
+        if all([os.path.exists(path), os.path.isfile(path), path.endswith('.db')]):
+            if self._database_file_path == path:
+                return
+            
+            # close the current connection before making a new one
+            if self._connection is not None:
+                await self._connection.close()
+
+            self._connection = await aiosqlite.connect(path)
+            self._cursor = await self._connection.cursor()
+            self._database_file_path = path
+        else:
+            raise DatabaseFileNotFound(f'The database file in path {path!r} was not found')
+    
+    def _determine_no_xp(self, message: Message) -> bool:
+        """Check if the channel the member is sending messages in is a no XP channel. This also checks if any of the roles they have is a no XP role
+        
+            .. changes::
+                v0.0.2
+                    Complete overhaul to support multi-guild leveling 
+        """
+        has_no_xp_role = False
+        in_no_xp_channel = False
+        
+        if self.no_xp_channels:
+            if message.channel.id in self.no_xp_channels:
+                in_no_xp_channel = True
+        
+        # if :var:`in_no_xp_channel` is already `True`, there's no need to execute the no xp role check
+        if in_no_xp_channel:
+            return True
+
+        if self.no_xp_roles:
+            all_member_role_ids = [role.id for role in message.author.roles] # type: ignore / will always be :class:`discord.Member` because all DM messages are ignored by the lib
+            for no_xp_role_id in self.no_xp_roles:
+                if no_xp_role_id in all_member_role_ids:
+                    has_no_xp_role = True
+                    break
+
+        return any([has_no_xp_role, in_no_xp_channel])        
+    
+    async def _update_record(self, member: Union[Member, int], level: int, xp: int, total_xp: int, guild_id: int, name: Optional[str]=None, **kwargs) -> None:
+        maybe_new_record = kwargs.get('maybe_new_record', False)
+        if maybe_new_record and not name:
+            raise Exception('kwarg "name" needs to be set when adding a new record')
+        
+        # :meth:`DiscordLevelingSystem.is_in_database` parameter "guild" expects a :class:`discord.Guild` object. We don't necessarily *need* an actual :class:`discord.Guild`
+        # object because that method really only needs the ID to operate on the correct guild. Since this method has no :class:`discord.Guild` object, just make a false guild
+        # object so :meth:`DiscordLevelingSystem.is_in_database` will work as intended
+        FakeGuild = collections.namedtuple('FakeGuild', 'id')
+        if await self.is_in_database(member, guild=FakeGuild(id=guild_id)): # type: ignore / it's a fake guild, so yes, it's not compatible with :class:`discord.Guild` that the method is looking for
+            await self._cursor.execute('UPDATE leaderboard SET member_level = ?, member_xp = ?, member_total_xp = ? WHERE member_id = ? AND guild_id = ?', (level, xp, total_xp, member.id if isinstance(member, Member) else member, guild_id)) # type: ignore
+        else:
+            await self._cursor.execute(DiscordLevelingSystem._QUERY_NEW_MEMBER, (guild_id, member.id if isinstance(member, Member) else member, name, level, xp, total_xp)) # type: ignore
+        await self._connection.commit() # type: ignore
+    
+    @staticmethod
+    def _get_transfer(path: str, loop: asyncio.AbstractEventLoop) -> NamedTuple:
+        """|static method| Connect to the target database file in the specified path and return a named tuple of the connection and cursor
+        
+            .. added:: v0.0.2
+        """
+        if all([os.path.exists(path), os.path.isfile(path), path.endswith('.db')]):
+            try:
+                connection = loop.run_until_complete(aiosqlite.connect(path))
+                cursor = loop.run_until_complete(connection.cursor())
+                Transfer = collections.namedtuple('Transfer', ['connection', 'cursor'])
+                return Transfer(connection=connection, cursor=cursor)
+            except RuntimeError:
+                raise ConnectionFailure
+        else:
+            raise DatabaseFileNotFound(f'The database file in path {path!r} was not found')
+    
+    @staticmethod
+    async def _execute_transfer(db_from: 'Transfer', db_to: 'Transfer', guild_id: int) -> None: # type: ignore
+        """|coro static method| Copy the contents from the old database file (v0.0.1), to the new database file (v0.0.2+)
+        
+            .. added:: v0.0.2
+        """
+        try:
+            from_result = await db_from.connection.execute_fetchall('SELECT * FROM leaderboard')
+        except aiosqlite.OperationalError:
+            raise DiscordLevelingSystemError('One of the databases is missing the "leaderboard" table when attempting to transfer')
+        else:
+            OLD_PRAGMA_LAYOUT = [
+                (0, 'member_id', 'INT', 0, None, 1),
+                (1, 'member_name', 'TEXT', 1, None, 0),
+                (2, 'member_level', 'INT', 1, None, 0),
+                (3, 'member_xp', 'INT', 1, None, 0),
+                (4, 'member_total_xp', 'INT', 1, None, 0)
+            ]
+            NEW_PRAGMA_LAYOUT = [
+                (0, 'guild_id', 'INT', 1, None, 0),
+                (1, 'member_id', 'INT', 1, None, 0),
+                (2, 'member_name', 'TEXT', 1, None, 0),
+                (3, 'member_level', 'INT', 1, None, 0),
+                (4, 'member_xp', 'INT', 1, None, 0),
+                (5, 'member_total_xp', 'INT', 1, None, 0)
+            ]
+            old_pragma_check = await db_from.connection.execute_fetchall('PRAGMA table_info(leaderboard)')
+            new_pragma_check = await db_to.connection.execute_fetchall('PRAGMA table_info(leaderboard)')
+            if all([old_pragma_check == OLD_PRAGMA_LAYOUT, new_pragma_check == NEW_PRAGMA_LAYOUT]):
+                # ensure the database file that the data will be transferred to is blank, if so, copy the contents to the new database file
+                await db_to.cursor.execute('SELECT COUNT(*) FROM leaderboard')
+                count_result = await db_to.cursor.fetchone()
+                if count_result[0] == 0:
+                    to_execute = []
+                    for data in from_result:
+                        to_execute.append((guild_id, data[0], data[1], data[2], data[3], data[4]))
+                    else:
+                        await db_to.cursor.executemany(DiscordLevelingSystem._QUERY_NEW_MEMBER, to_execute)
+                        await db_to.connection.commit()
+                        print('Transfer complete')
+                else:
+                    raise DiscordLevelingSystemError('When transferring the data to the new database file (created file using v0.0.2+), that database file must contain no records')
+            else:
+                raise DiscordLevelingSystemError('The "transfer" method is only to be used with transferring the data from the database file from version 0.0.1. If you were already using a database file from version 0.0.2+, there is no need to use this method')
+    
+    @staticmethod
+    def transfer(old: str, new: str, guild_id: int) -> None:
+        """|static method|
+        
+        Transfer the database records from a database file created from v0.0.1 to a blank database file created using v0.0.2+. If you were already using a v0.0.2+
+        database file, there's no need to use this method
+
+        See the following link about transfers: https://github.com/Defxult/discordLevelingSystem#migrating-from-v001-to-v002
+        
+        Parameters
+        ----------
+        old: :class:`str`
+            The path of the v0.0.1 database file
+        
+        new: :class:`str`
+            The path of the v0.0.2+ database file
+        
+        guild_id: :class:`int`
+            ID of the guild that was originally used with this library
+        
+        Raises
+        ------
+        - `ConnectionFailure`: The event loop is already running
+        - `DatabaseFileNotFound`: "old" or "new" database file was not found
+        - `DiscordLevelingSystemError`: One of the databases is missing the "leaderboard" table. A v0.0.2+ database file contains records, or there was an attempt to transfer records from a v0.0.2+ file to another v0.0.2+ file
+        
+            .. added:: v0.0.2
+        """
+        loop = asyncio.get_event_loop()
+        transfer_from = DiscordLevelingSystem._get_transfer(old, loop)
+        transfer_to = DiscordLevelingSystem._get_transfer(new, loop)
+        loop.run_until_complete(DiscordLevelingSystem._execute_transfer(transfer_from, transfer_to, guild_id))
+    
+    @db_file_exists
+    @leaderboard_exists
+    @verify_leaderboard_integrity
+    async def add_record(self, guild_id: int, member_id: int, member_name: str, level: int) -> None:
+        """|coro|
+        
+        Manually add a record to the database. If the record already exists (the :param:`guild_id` and :param:`member_id` was found), only the level will be updated. If there were no records that matched
+        those values, all provided information will be added
+
+        Parameters
+        ----------
+        guild_id: :class:`int`
+            The guild ID to register
+        
+        member_id: :class:`int`
+            The member ID to register
+        
+        member_name: :class:`str`
+            The member name to register
+        
+        level: :class:`int`
+            The member level to register. Must be from 0-100
+        
+        Raises
+        ------
+        - `DiscordLevelingSystemError`: The value given from a parameter was not of the correct type or "level" was not 0-100
+
+            .. added:: v1.0.1
+        """
+        if all([isinstance(guild_id, int), isinstance(member_id, int), isinstance(level, int)]):
+            if not (0 <= level <= 100):
+                raise DiscordLevelingSystemError('Parameter "level" must be from 0-100')
+            await self._update_record(member=member_id, level=level, xp=0, total_xp=LEVELS_AND_XP[str(level)], guild_id=guild_id, name=str(member_name), maybe_new_record=True)
+        else:
+            raise DiscordLevelingSystemError('All parameters that expect an int were not of type int')
+    
+    @overload
+    async def insert(self, bot: AutoShardedBot, guild_id: int, users: Dict[int, int], using: Literal['xp', 'levels'], overwrite: bool=False, show_results: bool=True) -> None:
+        ...
+    
+    @overload
+    async def insert(self, bot: Bot, guild_id: int, users: Dict[int, int], using: Literal['xp', 'levels'], overwrite: bool=False, show_results: bool=True) -> None:
+        ...
+
+    @db_file_exists
+    @leaderboard_exists
+    @verify_leaderboard_integrity
+    async def insert(self, bot: Union[Bot, AutoShardedBot], guild_id: int, users: Dict[int, int], using: Literal['xp', 'levels'], overwrite: bool=False, show_results: bool=True) -> None:
+        """|coro|
+        
+        Insert the records from your own leveling system into the library. A lot of leveling system tutorials out there use json files to store information. Although it might work, it is
+        insufficient because json files are not made to act as a database. Using a database file has many benefits over a json file
+        
+        If you already have records in the database file and you want to insert your records on top of the records that already exist, it is suggested to backup that
+        file using :meth:`DiscordLevelingSystem.backup_database_file()` first. If you don't have any records in your DiscordLevelingSystem database file, then there's no need to create a backup 
+
+        Parameters
+        ----------
+        bot: Union[:class:`discord.ext.commands.Bot`, :class:`discord.ext.commands.AutoShardedBot`]
+            Your bot instance variable
+        
+        guild_id: :class:`int`
+            ID of the guild that you used your leveling system with
+        
+        users: Dict[:class:`int`, :class:`int`]
+            This is the information that will be added to the database. The keys are user ID's, and the values are the users total XP or level.
+            Note: This library only uses levels 0-100 and XP 0-1899250. If any number in this dict are over the levels/XP threshold, it is implicitly set back to this libraries maximum value
+
+        using: :class:`str`
+            What structure your leveling system used. Options: "xp" or "levels". Some leveling systems give users only XP and they are ranked up based on that XP value. Others use a combination of levels and XP. If all the values
+            in the :param:`users` dict are based on XP, set this to "xp". If they are based on a users level, set this to "levels"
+        
+        overwrite: :class:`bool`
+            (optional) If a user you've specified in the :param:`users` dict already has a record in the database, overwrite their current record with the one your inserting (defaults to `False`)
+        
+        show_results: :class:`bool`
+            (optional) Print the results for how many of the :param:`users` were successfully added to the database file. If any are unsuccessful, their ID along with the value you provided will also be shown (defaults to `True`)
+        
+        Raises
+        ------
+        - `DiscordLevelingSystemError`: The value given from a parameter was not of the correct type. The :param:`users` dict was empty. Or your bot is not in the guild associated with :param:`guild_id`
+            
+            .. added:: v1.0.1
+        """
+        # Perform the necessary checks to ensure the proper values will be added to the database
+        if not isinstance(guild_id, int):
+            raise DiscordLevelingSystemError(f'Parameter "guild_id" expected int, got {guild_id.__class__.__name__}')
+        if not users:
+            raise DiscordLevelingSystemError('The "users" dict cannot be empty')
+        for k, v in users.items():
+            if not isinstance(k, int) or not isinstance(v, int):
+                raise DiscordLevelingSystemError('All keys and values in the "users" dict must be of type int')
+        
+        guild = bot.get_guild(guild_id)
+        if guild:
+            using = using.lower() # type: ignore
+            successfully_added: List[Member] = []
+            skipped_users = []
+            registered_users = []
+            SkippedUser = collections.namedtuple('SkippedUser', ['id', 'value'])
+            RegisteredUser = collections.namedtuple('RegisteredUser', ['id', 'name', 'value'])
+            for user_id, user_level_or_xp in users.items():
+                member = guild.get_member(user_id)
+                if member:
+                    if not overwrite and await self.is_in_database(user_id, guild):
+                        registered_users.append(str(RegisteredUser(id=user_id, name=str(member), value=user_level_or_xp)))
+                        continue
+                    else:
+                        if using == 'levels':
+                            level = user_level_or_xp
+                            if level < 0: level = 0
+                            elif level > MAX_LEVEL: level = MAX_LEVEL
+                            await self.set_level(member, level)
+                            successfully_added.append(member)
+                        
+                        elif using == 'xp':
+                            xp = user_level_or_xp
+                            if xp < 0: xp = 0
+                            elif xp > LEVELS_AND_XP[str(MAX_LEVEL)]: xp = LEVELS_AND_XP[str(MAX_LEVEL)]
+                            await self.set_level(member, _find_level(xp))
+                            successfully_added.append(member)
+                        
+                        else:
+                            raise DiscordLevelingSystemError(f'Parameter "using" expected "levels" or "xp", got {using!r}')
+                else:
+                    skipped_users.append(str(SkippedUser(id=user_id, value=user_level_or_xp)))
+            else:
+                if show_results:
+                    stats = cleandoc(f"""
+                        ----------------------------------------
+                        Discord Leveling System - Insert Results
+                        ----------------------------------------
+                        {len(successfully_added)} out of {len(users)} users were successfully added to the database file
+                    """)
+                    if successfully_added:
+                        MemberDataStringRepr = str
+                        data: List[MemberDataStringRepr] = [str(await self.get_data_for(stored_member)) for stored_member in successfully_added]
+                        joined_data = '\n'.join(data)
+                        stats += f'\n\nThe below {len(successfully_added)} user(s) are now apart of the Discord Leveling System and are represented as a MemberData object\n{joined_data}'
+                    
+                    if skipped_users:
+                        joined_skipped = '\n'.join(skipped_users)
+                        stats += f'\n\nThe below {len(skipped_users)} user(s) were skipped because they are not currently in guild {guild_id}\n{joined_skipped}'
+                    
+                    if registered_users:
+                        joined_registered = '\n'.join(registered_users)
+                        stats += f'\n\nThe below {len(registered_users)} user(s) were skipped because they already have a record in the database and the "overwrite" kwarg was set to False\n{joined_registered}'
+                    
+                    print(stats)
+        else:
+            raise DiscordLevelingSystemError(f'Your bot is not in guild {guild_id}')
+    
+    @overload
+    def get_awards(self, guild: Optional[Guild]=None) -> Optional[Dict[int, List[RoleAward]]]:
+        ...
+    
+    @overload
+    def get_awards(self, guild: Optional[Guild]=None) -> Optional[List[RoleAward]]:
+        ...
+    
+    @overload
+    def get_awards(self, guild: Optional[int]=None) -> Optional[Dict[int, List[RoleAward]]]:
+        ...
+    
+    @overload
+    def get_awards(self, guild: Optional[int]=None) -> Optional[List[RoleAward]]:
+        ...
+    
+    def get_awards(self, guild: Optional[Union[Guild, int]]=None) -> Optional[Union[Dict[int, List[RoleAward]], List[RoleAward]]]:
+        """Get all :class:`RoleAward`'s or only the :class:`RoleAward`'s assigned to the specified guild
+
+        Parameters
+        ----------
+        guild: Optional[Union[:class:`discord.Guild`, :class:`int`]]
+            A guild object or a guild ID
+        
+        Returns
+        -------
+        Optional[Union[Dict[:class:`int`, List[:class:`RoleAward`]], List[:class:`RoleAward`]]]: If :param:`guild` is :class:`None`, this returns the awards :class:`dict` that was set in constructor. If :param:`guild`
+        is specified, it returns a List[:class:`RoleAward`] that matches the specified guild ID. Can also return :class:`None` if awards were never set or if the awards for the specified guild was not found
+        
+            .. added:: v1.0.0
+        """
+        if self._awards:
+            if guild:
+                try:
+                    guild_id = guild.id if isinstance(guild, Guild) else guild
+                    return self._awards[guild_id].copy()
+                except KeyError:
+                    return None
+            else:
+                return self._awards.copy()
+        else:
+            return None
+    
+    @db_file_exists
+    @leaderboard_exists
+    @verify_leaderboard_integrity
+    async def add_xp(self, member: Member, amount: int) -> None:
+        """|coro|
+        
+        Give XP to a member. This also changes their level so it matches the associated XP
+
+        Parameters
+        ----------
+        member: :class:`discord.Member`
+            The member to give XP to
+        
+        amount: :class:`int`
+            Amount of XP to give to the member
+
+        Raises
+        ------
+        - `DatabaseFileNotFound`: The database file was not found
+        - `LeaderboardNotFound`: Table "leaderboard" in the database file is missing
+        - `ImproperLeaderboard`: Leaderboard table was altered. Components changed or deleted
+        - `NotConnected`: Attempted to use a method that requires a connection to a database file
+        - `DiscordLevelingSystemError`: Parameter "amount" was less than or equal to zero. The minimum value is 1 
+        
+            .. added:: v0.0.2
+        """
+        if amount <= 0:
+            raise DiscordLevelingSystemError('Parameter "amount" was less than or equal to zero. The minimum value is 1')
+        
+        md = await self.get_data_for(member)
+        if md:
+            if md.total_xp >= MAX_XP:
+                return
+            else:
+                new_total_xp = md.total_xp + amount
+                new_total_xp = new_total_xp if new_total_xp <= MAX_XP else MAX_XP
+                maybe_new_level = _find_level(new_total_xp)
+                await self._update_record(member=member, level=maybe_new_level, xp=md.xp, total_xp=new_total_xp, guild_id=member.guild.id, name=str(member), maybe_new_record=True)
+    
+    @db_file_exists
+    @leaderboard_exists
+    @verify_leaderboard_integrity
+    async def remove_xp(self, member: Member, amount: int) -> None:
+        """|coro|
+        
+        Remove XP from a member. This also changes their level so it matches the associated XP
+
+        Parameters
+        ----------
+        member: :class:`discord.Member`
+            The member to remove XP from
+        
+        amount: :class:`int`
+            Amount of XP to remove from the member
+
+        Raises
+        ------
+        - `DatabaseFileNotFound`: The database file was not found
+        - `LeaderboardNotFound`: Table "leaderboard" in the database file is missing
+        - `ImproperLeaderboard`: Leaderboard table was altered. Components changed or deleted
+        - `NotConnected`: Attempted to use a method that requires a connection to a database file
+        - `DiscordLevelingSystemError`: Parameter "amount" was less than or equal to zero. The minimum value is 1 
+        
+            .. added:: v0.0.2
+        """
+        if amount <= 0:
+            raise DiscordLevelingSystemError('Parameter "amount" was less than or equal to zero. The minimum value is 1')
+        
+        md = await self.get_data_for(member)
+        if md:
+            if md.total_xp == 0:
+                return
+            else:
+                new_total_xp = md.total_xp - amount
+                new_total_xp = new_total_xp if new_total_xp >= 1 else 0
+                maybe_new_level = _find_level(new_total_xp)
+                await self._update_record(member=member, level=maybe_new_level, xp=md.xp, total_xp=new_total_xp, guild_id=member.guild.id)
+    
+    @db_file_exists
+    @leaderboard_exists
+    @verify_leaderboard_integrity
+    async def set_level(self, member: Member, level: int) -> None:
+        """|coro|
+        
+        Sets the level for the member. This also changes their total XP so it matches the associated level
+        
+        Parameters
+        ----------
+        member: :class:`discord.Member`
+            The member who's level will be set
+        
+        level: :class:`int`
+            Level to set. Must be from 0-100
+                
+        Raises
+        ------
+        - `DatabaseFileNotFound`: The database file was not found
+        - `LeaderboardNotFound`: Table "leaderboard" in the database file is missing
+        - `ImproperLeaderboard`: Leaderboard table was altered. Components changed or deleted
+        - `NotConnected`: Attempted to use a method that requires a connection to a database file
+        - `DiscordLevelingSystemError`: Parameter "level" was not from 0-100
+        
+            .. added:: v0.0.2
+        """
+        if 0 <= level <= 100:
+            await self._update_record(member=member, level=level, xp=0, total_xp=LEVELS_AND_XP[str(level)], guild_id=member.guild.id, name=str(member), maybe_new_record=True)
+        else:
+            raise DiscordLevelingSystemError('Parameter "level" must be from 0-100')
+    
+    @db_file_exists
+    @leaderboard_exists
+    @verify_leaderboard_integrity
+    async def change_cooldown(self, rate: int, per: float) -> None:
+        """|coro|
+        
+        Update the cooldown rate
+        
+        Parameters
+        ----------
+        rate: :class:`int`
+            The amount of messages each member can send before the cooldown triggers
+
+        per: :class:`float`
+            The amount of seconds each member has to wait before gaining more XP, aka the cooldown
+
+        Raises
+        ------
+        - `DatabaseFileNotFound`: The database file was not found
+        - `LeaderboardNotFound`: Table "leaderboard" in the database file is missing
+        - `ImproperLeaderboard`: Leaderboard table was altered. Components changed or deleted
+        - `NotConnected`: Attempted to use a method that requires a connection to a database file
+        - `DiscordLevelingSystemError`: The rate or per value was not greater than zero
+        """
+        if rate <= 0 or per <= 0:   raise DiscordLevelingSystemError('Invalid rate or per. Values must be greater than zero')
+        self._cooldown = CooldownMapping.from_cooldown(rate, per, BucketType.member)
+        self.__rate = rate
+        self.__per = per
+
+    @db_file_exists
+    @leaderboard_exists
+    @verify_leaderboard_integrity
+    async def refresh_names(self, guild: Guild) -> int:
+        """|coro|
+        
+        Update names inside the database. This does not add anything new. It simply verifies if the name in the database matches their current name, and if they don't match, update
+        the database name
+        
+        Parameters
+        ----------
+        guild: :class:`discord.Guild`
+            A guild object
+        
+        Returns
+        -------
+        :class:`int`: The amount of records in the database that were updated
+
+        Raises
+        ------
+        - `DatabaseFileNotFound`: The database file was not found
+        - `LeaderboardNotFound`: Table "leaderboard" in the database file is missing
+        - `ImproperLeaderboard`: Leaderboard table was altered. Components changed or deleted
+        - `NotConnected`: Attempted to use a method that requires a connection to a database file
+        """
+        async with self._connection.execute('SELECT member_id, member_name FROM leaderboard WHERE guild_id = ?', (guild.id,)) as cursor: # type: ignore
+            result = await cursor.fetchall()
+            names_updated = 0
+            if result:
+                database_ids = [db[0] for db in result]
+                database_names = [db[1] for db in result]
+                to_execute = []
+                for db_id, db_name in zip(database_ids, database_names):
+                    member = guild.get_member(db_id)
+                    if member:
+                        if str(member) != db_name:
+                            to_execute.append((str(member), db_id, guild.id))
+                            names_updated += 1
+                else: 
+                    await cursor.executemany('UPDATE leaderboard SET member_name = ? WHERE member_id = ? AND guild_id = ?', to_execute)
+                    await self._connection.commit() # type: ignore
+
+            return names_updated
+    
+    @db_file_exists
+    @leaderboard_exists
+    @verify_leaderboard_integrity
+    async def wipe_database(self, guild: Optional[Guild]=None, *, intentional: bool=False) -> None:
+        """|coro|
+        
+        Delete EVERYTHING from the database. If :param:`guild` is specified, only the information related to that guild will be deleted
+
+        Parameters
+        ----------
+        guild: Optional[:class:`discord.Guild`]
+            The guild for which all information that is related to that guild will be deleted. If :class:`None`, everything will be deleted
+
+        intentional: :class:`bool`
+            A simple kwarg to try and ensure that this action is indeed what you want to do. Once executed, this cannot be undone
+
+        Raises
+        ------
+        - `DatabaseFileNotFound`: The database file was not found
+        - `LeaderboardNotFound`: Table "leaderboard" in the database file is missing
+        - `ImproperLeaderboard`: Leaderboard table was altered. Components changed or deleted
+        - `NotConnected`: Attempted to use a method that requires a connection to a database file
+        - `FailSafe`: "intentional" argument for this method was set to `False` in case you called this method by mistake
+        
+            .. changes::
+                v1.0.0
+                    Added :param:`guild`
+        """
+        if intentional:
+            if guild:   await self._cursor.execute('DELETE FROM leaderboard WHERE guild_id = ?', (guild.id,)) # type: ignore
+            else:       await self._cursor.execute('DELETE FROM leaderboard') # type: ignore
+            await self._connection.commit() # type: ignore
+        else:
+            raise FailSafe
+    
+    @db_file_exists
+    @leaderboard_exists
+    @verify_leaderboard_integrity
+    async def clean_database(self, guild: Guild) -> int:
+        """|coro|
+        
+        Removes the data for members that are no longer in the guild, thus reducing the database file size. It is recommended to have this method in a background loop
+        in order to keep the database file free of records that are no longer in use
+
+        Parameters
+        ----------
+        guild: :class:`discord.Guild`
+            The guild records to clean
+        
+        Returns
+        -------
+        :class:`int`: The amount of records that were removed from the database
+        
+        Raises
+        ------
+        - `DatabaseFileNotFound`: The database file was not found
+        - `LeaderboardNotFound`: Table "leaderboard" in the database file is missing
+        - `ImproperLeaderboard`: Leaderboard table was altered. Components changed or deleted
+        - `NotConnected`: Attempted to use a method that requires a connection to a database file
+        
+            .. changes::
+                v0.0.2
+                    Replaced :param:`all_members` with :param:`guild`
+        """
+        result = await self._connection.execute_fetchall('SELECT member_id FROM leaderboard WHERE guild_id = ?', (guild.id,)) # type: ignore
+        all_ids = [i[0] for i in result]
+        to_execute = []
+        records_removed = 0
+
+        for id_ in all_ids:
+            if guild.get_member(id_):
+                continue
+            else:
+                to_execute.append((id_, guild.id))
+                records_removed += 1
+        else:
+            if records_removed:
+                await self._cursor.executemany('DELETE FROM leaderboard WHERE member_id = ? AND guild_id = ?', to_execute) # type: ignore
+                await self._connection.commit() # type: ignore
+            return records_removed
+    
+    @db_file_exists
+    @leaderboard_exists
+    @verify_leaderboard_integrity
+    async def reset_member(self, member: Member) -> None:
+        """|coro|
+        
+        Sets the members XP, total XP, and level to zero
+        
+        Parameters
+        ----------
+        member: :class:`discord.Member`
+            The member to reset
+        
+        Raises
+        ------
+        - `DatabaseFileNotFound`: The database file was not found
+        - `LeaderboardNotFound`: Table "leaderboard" in the database file is missing
+        - `ImproperLeaderboard`: Leaderboard table was altered. Components changed or deleted
+        - `NotConnected`: Attempted to use a method that requires a connection to a database file
+        """
+        await self._cursor.execute('UPDATE leaderboard SET member_level = 0, member_xp = 0, member_total_xp = 0 WHERE member_id = ? AND guild_id = ?', (member.id, member.guild.id)) # type: ignore
+        await self._connection.commit() # type: ignore
+    
+    @overload
+    async def reset_everyone(self, guild: Guild, *, intentional: bool=False) -> None:
+        ...
+    
+    @overload
+    async def reset_everyone(self, guild: None, *, intentional: bool=False) -> None:
+        ...
+    
+    @db_file_exists
+    @leaderboard_exists
+    @verify_leaderboard_integrity
+    async def reset_everyone(self, guild: Union[Guild, None], *, intentional: bool=False) -> None:
+        """|coro|
+        
+        Sets EVERYONES XP, total XP, and level to zero in the database. Can specify which guild to reset
+
+        Parameters
+        ----------
+        guild: Union[:class:`discord.Guild`, :class:`None`]
+            The guild for which everyone will be reset. If this is set to :class:`None`, everyone in the entire database will be reset
+        
+        intentional: :class:`bool`
+            A simple kwarg to try and ensure that this action is indeed what you want to do. Once executed, this cannot be undone
+
+        Raises
+        ------
+        - `DatabaseFileNotFound`: The database file was not found
+        - `LeaderboardNotFound`: Table "leaderboard" in the database file is missing
+        - `ImproperLeaderboard`: Leaderboard table was altered. Components changed or deleted
+        - `NotConnected`: Attempted to use a method that requires a connection to a database file
+        - `FailSafe`: "intentional" argument for this method was set to `False` in case you called this method by mistake
+        
+            .. changes::
+                v0.0.2
+                    Added :param:`guild`
+        """
+        if intentional:
+            if guild: await self._cursor.execute('UPDATE leaderboard SET member_level = 0, member_xp = 0, member_total_xp = 0 WHERE guild_id = ?', (guild.id,)) # type: ignore
+            else:     await self._cursor.execute('UPDATE leaderboard SET member_level = 0, member_xp = 0, member_total_xp = 0') # type: ignore
+            await self._connection.commit() # type: ignore
+        else:
+            raise FailSafe
+    
+    @overload
+    async def export_as_json(self, path: str, guild: Guild) -> None:
+        ...
+    
+    @overload
+    async def export_as_json(self, path: str, guild: None) -> None:
+        ...
+    
+    @db_file_exists
+    @leaderboard_exists
+    @verify_leaderboard_integrity
+    async def export_as_json(self, path: str, guild: Union[Guild, None]) -> None:
+        """|coro|
+        
+        Export a json file that represents the database to the path specified
+        
+        Parameters
+        ----------
+        path: :class:`str`
+            Path to copy the json file to
+        
+        guild: Union[:class:`discord.Guild`, :class:`None`]
+            The guild for which the data should be extracted from. If :class:`None`, all guild information will be extracted from the database
+        
+        Raises
+        ------
+        - `DatabaseFileNotFound`: The database file was not found
+        - `LeaderboardNotFound`: Table "leaderboard" in the database file is missing
+        - `ImproperLeaderboard`: Leaderboard table was altered. Components changed or deleted
+        - `NotConnected`: Attempted to use a method that requires a connection to a database file
+        - `DiscordLevelingSystemError`: The path does not exist or does not point to a directory
+        
+            .. changes::
+                v0.0.2
+                    Added :param:`guild`. Now supports a specific guild to export
+                    Improved overall json format (easier to read)
+        """
+        if os.path.exists(path) and os.path.isdir(path):
+            path = os.path.join(path, 'discord_leveling_system.json')
+            container = []
+            if guild:
+                data = await self._connection.execute_fetchall('SELECT member_id, member_name, member_level, member_xp, member_total_xp FROM leaderboard WHERE guild_id = ?', (guild.id,)) # type: ignore
+                levels = {}
+                for m_id, m_name, m_lvl, m_xp, m_total_xp in data:
+                    levels = {
+                        'id' : m_id,
+                        'name' : m_name,
+                        'level' : m_lvl,
+                        'xp' : m_xp,
+                        'total_xp' : m_total_xp
+                    }
+                    container.append(levels.copy())
+                else:
+                    with open(path, mode='w') as fp:
+                        json.dump(container, fp, indent=4)
+            
+            else:
+                data = await self._connection.execute_fetchall('SELECT * FROM leaderboard') # type: ignore
+                for info in data:
+                    guild_id = info[0]
+                    member_id = info[1]
+                    member_name = info[2]
+                    member_level = info[3]
+                    member_xp = info[4]
+                    member_total_xp = info[5]
+                    levels = {
+                        'guild_id' : guild_id,
+                        'member_id' : member_id,
+                        'name' : member_name,
+                        'level' : member_level,
+                        'xp' : member_xp,
+                        'total_xp' : member_total_xp
+                    }
+                    container.append(levels.copy())
+                else:
+                    with open(path, mode='w') as fp:
+                        json.dump(container, fp, indent=4)
+        else:
+            raise DiscordLevelingSystemError(f'The path {path!r} does not exist or does not point to a directory')
+
+    @db_file_exists
+    @leaderboard_exists
+    @verify_leaderboard_integrity
+    async def raw_database_contents(self, guild: Optional[Guild]=None) -> List[Tuple[int, int, str, int, int, int]]:
+        """|coro|
+        
+        Returns everything in the database. Can specify which guild information will be extracted
+
+        Parameters
+        ----------
+        guild: Optional[:class:`discord.Guild`]
+            The guild to extract the raw database contents from. If :class:`None`, information about all guilds will be extracted
+        
+        Returns
+        -------
+        List[Tuple[:class:`int`, :class:`int`, :class:`str`, :class:`int`, :class:`int`, :class:`int`]]: The tuples inside the list represents each row of the database:
+        
+        - Index 0 is the guild ID
+        - Index 1 is their ID
+        - Index 2 is their name
+        - Index 3 is their level
+        - Index 4 is their XP
+        - Index 5 is their total xp
+        
+        Can be an empty list if nothing is in the database
+        
+        Raises
+        ------
+        - `DatabaseFileNotFound`: The database file was not found
+        - `LeaderboardNotFound`: Table "leaderboard" in the database file is missing
+        - `ImproperLeaderboard`: Leaderboard table was altered. Components changed or deleted
+        - `NotConnected`: Attempted to use a method that requires a connection to a database file
+        
+            .. changes::
+                v0.0.2
+                    Added :param:`guild`
+        """
+        if guild:   return await self._connection.execute_fetchall('SELECT * FROM leaderboard WHERE guild_id = ?', (guild.id,)) # type: ignore
+        else:       return await self._connection.execute_fetchall('SELECT * FROM leaderboard') # type: ignore
+    
+    @overload
+    async def remove_from_database(self, member: Member, guild: Optional[Guild]=None) -> bool:
+        ...
+    
+    @overload
+    async def remove_from_database(self, member: int, guild: Optional[Guild]=None) -> bool:
+        ...
+
+    @db_file_exists
+    @leaderboard_exists
+    @verify_leaderboard_integrity
+    async def remove_from_database(self, member: Union[Member, int], guild: Optional[Guild]=None) -> bool:
+        """|coro|
+        
+        Remove a member from the database. This is not guild specific although it can be if :param:`guild` is specified
+
+        Parameters
+        ----------
+        member: Union[:class:`discord.Member`, :class:`int`]
+            The member to remove. Can be the member object or that members ID
+
+        guild: Optional[:class:`discord.Guild`]
+            If this parameter is given, it will remove the record of the specified member only from the specified guild record. If :class:`None`, it will remove
+            all records no matter the guild
+        
+        Returns
+        -------
+        :class:`bool`: Returns `True` if the member was successfully removed from the database. `False` if the member was not in the database so there was nothing to remove
+
+        Raises
+        ------
+        - `DatabaseFileNotFound`: The database file was not found
+        - `LeaderboardNotFound`: Table "leaderboard" in the database file is missing
+        - `ImproperLeaderboard`: Leaderboard table was altered. Components changed or deleted
+        - `DiscordLevelingSystemError`: Parameter :param:`member` was not of type :class:`discord.Member` or :class:`int`
+        - `NotConnected`: Attempted to use a method that requires a connection to a database file
+        
+            .. changes::
+                v1.0.0
+                    Added :param:`guild`
+        """
+        if isinstance(member, (Member, int)):
+            member_id = member.id if isinstance(member, Member) else member
+            removable = await self.is_in_database(member_id, guild=guild if guild else None)
+            if removable:
+                query = 'DELETE FROM leaderboard WHERE member_id = ? AND guild_id = ?' if guild else 'DELETE FROM leaderboard WHERE member_id = ?'
+                params = (member_id, guild.id) if guild else (member_id,)
+                
+                await self._cursor.execute(query, params) # type: ignore
+                await self._connection.commit() # type: ignore
+            return removable
+        else:
+            raise DiscordLevelingSystemError(f'Parameter "member" expected discord.Member or int, got {member.__class__.__name__}')
+    
+    @overload
+    async def is_in_database(self, member: Member, guild: Optional[Guild]=None) -> bool:
+        ...
+    
+    @overload
+    async def is_in_database(self, member: int, guild: Optional[Guild]=None) -> bool:
+        ...
+
+    @db_file_exists
+    @leaderboard_exists
+    @verify_leaderboard_integrity
+    async def is_in_database(self, member: Union[Member, int], guild: Optional[Guild]=None) -> bool:
+        """|coro|
+        
+        A quick check to see if a member is in the database. This is not guild specific although it can be if :param:`guild` is specified
+
+        Parameters
+        ----------
+        member: Union[:class:`discord.Member`, :class:`int`]
+            The member to check for. Can be the member object or that members ID
+        
+        guild: Optional[:class:`discord.Guild`]
+            The guild to check if the member is registered in
+        
+        Returns
+        -------
+        :class:`bool`
+
+        Raises
+        ------
+        - `DatabaseFileNotFound`: The database file was not found
+        - `LeaderboardNotFound`: Table "leaderboard" in the database file is missing
+        - `ImproperLeaderboard`: Leaderboard table was altered. Components changed or deleted
+        - `NotConnected`: Attempted to use a method that requires a connection to a database file
+        - `DiscordLevelingSystemError`: Parameter :param:`member` was not of type :class:`discord.Member` or :class:`int`
+        
+            .. changes::
+                v1.0.0
+                    Added :param:`guild`
+        """
+        if not isinstance(member, (Member, int)): raise DiscordLevelingSystemError(f'Parameter "member" expected discord.Member or int, got {member.__class__.__name__}')
+        arg = member.id if isinstance(member, Member) else member
+        query = 'SELECT * FROM leaderboard WHERE member_id = ? AND guild_id = ?' if guild else 'SELECT * FROM leaderboard WHERE member_id = ?'
+        params = (arg, guild.id) if guild else (arg,)
+        
+        async with self._connection.execute(query, params) as cursor: # type: ignore
+            result = await cursor.fetchone()
+            if result: return True
+            else: return False
+        
+    @db_file_exists
+    @leaderboard_exists
+    @verify_leaderboard_integrity
+    async def get_record_count(self, guild: Optional[Guild]=None) -> int:
+        """|coro|
+        
+        Get the amount of members that are registered in the database. If :param:`guild` is set to :class:`None`, all members in the database will be counted
+
+        Parameters
+        ----------
+        guild: Optional[:class:`discord.Guild`]
+            The guild for which to count the amount of records
+
+        Returns
+        -------
+        :class:`int`
+
+        Raises
+        ------
+        - `DatabaseFileNotFound`: The database file was not found
+        - `LeaderboardNotFound`: Table "leaderboard" in the database file is missing
+        - `ImproperLeaderboard`: Leaderboard table was altered. Components changed or deleted
+        - `NotConnected`: Attempted to use a method that requires a connection to a database file
+        
+            .. changes::
+                v0.0.2
+                    Added :param:`guild`
+        """
+        if guild:   await self._cursor.execute('SELECT COUNT(*) from leaderboard WHERE guild_id = ?', (guild.id,)) # type: ignore
+        else:       await self._cursor.execute('SELECT COUNT(*) from leaderboard') # type: ignore
+        
+        result = await self._cursor.fetchone() # type: ignore
+        if result: return result[0]
+        else: return 0
+    
+    @db_file_exists
+    @leaderboard_exists
+    @verify_leaderboard_integrity
+    async def next_level_up(self, member: Member) -> Optional[int]:
+        """|coro|
+        
+        Get the amount of XP needed for the specified member to level up
+        
+        Parameters
+        ----------
+        member: :class:`discord.Member`
+            Member to get the amount of XP needed for a level up
+        
+        Returns
+        -------
+        Optional[:class:`int`]: Returns 0 if the member is currently at max level. Can return :class:`None` if the member is not in the database.
+
+        Raises
+        ------
+        - `DatabaseFileNotFound`: The database file was not found
+        - `LeaderboardNotFound`: Table "leaderboard" in the database file is missing
+        - `ImproperLeaderboard`: Leaderboard table was altered. Components changed or deleted
+        - `NotConnected`: Attempted to use a method that requires a connection to a database file
+        """
+        data = await self.get_data_for(member)
+        if not data:
+            return None
+        if data.level == 100:
+            return 0
+        else:
+            details = _next_level_details(data.level)
+            return details.xp_needed - data.xp # type: ignore / attr exists
+    
+    @db_file_exists
+    @leaderboard_exists
+    @verify_leaderboard_integrity
+    async def next_level(self, member: Member) -> Optional[int]:
+        """|coro|
+        
+        Get the next level for the specified member
+        
+        Parameters
+        ----------
+        member: :class:`discord.Member`
+            Member to get the next level for
+        
+        Returns
+        -------
+        Optional[:class:`int`]: If the member is currently max level (100), it will return 100. This can also return :class:`None` if the member is not in the database
+
+        Raises
+        ------
+        - `DatabaseFileNotFound`: The database file was not found
+        - `LeaderboardNotFound`: Table "leaderboard" in the database file is missing
+        - `ImproperLeaderboard`: Leaderboard table was altered. Components changed or deleted
+        - `NotConnected`: Attempted to use a method that requires a connection to a database file
+        
+            .. added:: v1.1.0
+        """
+        data = await self.get_data_for(member)
+        if not data:
+            return None
+        else:
+            next_level = data.level + 1
+            return MAX_LEVEL if next_level > MAX_LEVEL else next_level
+    
+    @db_file_exists
+    @leaderboard_exists
+    @verify_leaderboard_integrity
+    async def get_xp_for(self, member: Member) -> Optional[int]:
+        """|coro|
+        
+        Get the XP for the specified member
+        
+        Parameters
+        ----------
+        member: :class:`discord.Member`
+            Member to get the XP for
+        
+        Returns
+        -------
+        Optional[:class:`int`]: Can be :class:`None` if the member isn't in the database
+
+        Raises
+        ------
+        - `DatabaseFileNotFound`: The database file was not found
+        - `LeaderboardNotFound`: Table "leaderboard" in the database file is missing
+        - `ImproperLeaderboard`: Leaderboard table was altered. Components changed or deleted
+        - `NotConnected`: Attempted to use a method that requires a connection to a database file
+        """
+        md = await self.get_data_for(member)
+        if md: return md.xp
+        else: return None
+    
+    @db_file_exists
+    @leaderboard_exists
+    @verify_leaderboard_integrity
+    async def get_total_xp_for(self, member: Member) -> Optional[int]:
+        """|coro|
+        
+        Get the total XP for the specified member
+        
+        Parameters
+        ----------
+        member: :class:`discord.Member`
+            Member to get the total XP for
+        
+        Returns
+        -------
+        Optional[:class:`int`]: Can be :class:`None` if the member isn't in the database
+
+        Raises
+        ------
+        - `DatabaseFileNotFound`: The database file was not found
+        - `LeaderboardNotFound`: Table "leaderboard" in the database file is missing
+        - `ImproperLeaderboard`: Leaderboard table was altered. Components changed or deleted
+        - `NotConnected`: Attempted to use a method that requires a connection to a database file
+        """
+        md = await self.get_data_for(member)
+        if md: return md.total_xp
+        else: return None
+    
+    @db_file_exists
+    @leaderboard_exists
+    @verify_leaderboard_integrity
+    async def get_level_for(self, member: Member) -> Optional[int]:
+        """|coro|
+        
+        Get the level for the specified member
+        
+        Parameters
+        ----------
+        member: :class:`discord.Member`
+            Member to get the level for
+        
+        Returns
+        -------
+        Optional[:class:`int`]: Can be :class:`None` if the member isn't in the database
+
+        Raises
+        ------
+        - `DatabaseFileNotFound`: The database file was not found
+        - `LeaderboardNotFound`: Table "leaderboard" in the database file is missing
+        - `ImproperLeaderboard`: Leaderboard table was altered. Components changed or deleted
+        - `NotConnected`: Attempted to use a method that requires a connection to a database file
+        """
+        md = await self.get_data_for(member)
+        if md: return md.level
+        else: return None
+    
+    @db_file_exists
+    @leaderboard_exists
+    @verify_leaderboard_integrity
+    async def get_data_for(self, member: Member) -> Optional[MemberData]:
+        """|coro|
+        
+        Get the :class:`MemberData` object that represents the specified member
+        
+        Parameters
+        ----------
+        member: :class:`discord.Member`
+            The member to get the data for
+        
+        Returns
+        -------
+        Optional[:class:`MemberData`]: Can return :class:`None` if the member was not found in the database
+
+        Raises
+        ------
+        - `DatabaseFileNotFound`: The database file was not found
+        - `LeaderboardNotFound`: Table "leaderboard" in the database file is missing
+        - `ImproperLeaderboard`: Leaderboard table was altered. Components changed or deleted
+        - `NotConnected`: Attempted to use a method that requires a connection to a database file
+        """
+        async with self._connection.execute('SELECT * FROM leaderboard WHERE member_id = ? AND guild_id = ?', (member.id, member.guild.id)) as cursor: # type: ignore
+            result = await cursor.fetchone()
+            if result:
+                m_id = result[1]
+                m_name = result[2]
+                m_level = result[3]
+                m_xp = result[4]
+                m_total_xp = result[5]
+                m_rank = await self.get_rank_for(member)
+                return MemberData(m_id, m_name, m_level, m_xp, m_total_xp, m_rank)
+            else:
+                return None
+    
+    @db_file_exists
+    @leaderboard_exists
+    @verify_leaderboard_integrity
+    async def each_member_data(self, guild: Guild, sort_by: Optional[Literal['name', 'level', 'xp', 'rank']]=None, limit: Optional[int]=None) -> List[MemberData]:
+        """|coro|
+        
+        Return each member in the database as a :class:`MemberData` object for easy access to their XP, level, etc.
+
+        Parameters
+        ----------
+        guild: :class:`discord.Guild`
+            A guild object
+        
+        sort_by: Optional[:class:`str`]
+            Return each member data sorted by: "name", "level", "xp", "rank", or :class:`None`. If :class:`None`, it will return in the order they were added to the database
+        
+        limit: Optional[:class:`int`]
+            Restrict the amount of records returned to the specified amount
+        
+        Returns
+        -------
+        List[:class:`MemberData`]
+
+        Raises
+        ------
+        - `DatabaseFileNotFound`: The database file was not found
+        - `LeaderboardNotFound`: Table "leaderboard" in the database file is missing
+        - `ImproperLeaderboard`: Leaderboard table was altered. Components changed or deleted
+        - `NotConnected`: Attempted to use a method that requires a connection to a database file
+        - `DiscordLevelingSystemError`: The value of :param:`sort_by` was not recognized or :param:`guild` was not of type :class:`discord.Guild`
+
+            .. changes::
+                v1.1.0
+                    Added :param:`limit`
+        """
+        if not isinstance(guild, Guild):
+            raise DiscordLevelingSystemError(f'Parameter "guild" expected discord.Guild got {guild.__class__.__name__}')
+        else:
+            # NOTE: there's no need to worry about this method returning :class:`None` because as soon as someone sends a message they are added to the database
+
+            async def result_to_memberdata(query_result) -> List[MemberData]:
+                """Convert the query result into a :class:`list` of :class:`MemberData` objects"""
+                data = []
+                for m_id, m_name, m_level, m_xp, m_total_xp in query_result:
+                    rank = None
+                    member = guild.get_member(m_id)
+                    if member:
+                        rank = await self.get_rank_for(member) # if the member is None (no longer in guild), rank will be None. This is intentional
+                    data.append(MemberData(m_id, m_name, m_level, m_xp, m_total_xp, rank))
+                return data if limit is None else data[:limit]
+
+            if not sort_by:
+                result = await self._connection.execute_fetchall('SELECT member_id, member_name, member_level, member_xp, member_total_xp FROM leaderboard WHERE guild_id = ?', (guild.id,)) # type: ignore
+                return await result_to_memberdata(result)
+            else:
+                sort_by = sort_by.lower() # type: ignore
+                if sort_by in ('name', 'level', 'xp', 'rank'):
+                    if sort_by == 'name':
+                        result = await self._connection.execute_fetchall('SELECT member_id, member_name, member_level, member_xp, member_total_xp FROM leaderboard WHERE guild_id = ? ORDER BY member_name COLLATE NOCASE', (guild.id,)) # type: ignore
+                        return await result_to_memberdata(result)
+                    
+                    elif sort_by == 'level':
+                        result = await self._connection.execute_fetchall('SELECT member_id, member_name, member_level, member_xp, member_total_xp FROM leaderboard WHERE guild_id = ? ORDER BY member_level DESC', (guild.id,)) # type: ignore
+                        return await result_to_memberdata(result)
+                    
+                    elif sort_by == 'xp':
+                        result = await self._connection.execute_fetchall('SELECT member_id, member_name, member_level, member_xp, member_total_xp FROM leaderboard WHERE guild_id = ? ORDER BY member_total_xp DESC', (guild.id,)) # type: ignore
+                        return await result_to_memberdata(result)
+
+                    elif sort_by == 'rank':
+                        def convert(md: MemberData) -> MemberData:
+                            """Set the rank to an :class:`int` value of 0 because it is not possible to sort a list of :class:`int` that has :class:`None` values"""
+                            if md.rank is None:
+                                md.rank = 0
+                            return md
+                        
+                        result = await self._connection.execute_fetchall('SELECT member_id, member_name, member_level, member_xp, member_total_xp FROM leaderboard WHERE guild_id = ?', (guild.id,)) # type: ignore
+                        all_data: List[MemberData] = await result_to_memberdata(result)
+                        
+                        converted = [convert(md) for md in all_data] # convert the data so it can be sorted properly
+                        sorted_converted = sorted(converted, key=lambda md: md.rank) # type: ignore
+
+                        no_rank = [md for md in sorted_converted if md.rank == 0]
+                        with_rank = [md for md in sorted_converted if md.rank != 0]
+                        pre_final = with_rank + no_rank
+    
+                        def zero_to_none(md: MemberData) -> MemberData:
+                            """If they're not in the guild anymore, I don't want their rank to be presented as zero because that implies they are still in the guild, but just has
+                            a rank of zero. Setting it back to :class:`None` makes it more readable and draws further implication that they're no longer in the guild
+                            """
+                            if md.rank == 0:
+                                md.rank = None
+                            return md
+                        
+                        final = [zero_to_none(md) for md in pre_final]
+                        return final
+                else:
+                    raise DiscordLevelingSystemError(f'Parameter "sort_by" expected "name", "level", "xp", or "rank", {sort_by!r} was not recognized')
+    
+    @db_file_exists
+    @leaderboard_exists
+    @verify_leaderboard_integrity
+    async def get_rank_for(self, member: Member) -> Optional[int]:
+        """|coro|
+        
+        Get the rank for the specified member
+        
+        Parameters
+        ----------
+        member: :class:`discord.Member`
+            Member to get the rank for
+        
+        Returns
+        -------
+        Optional[:class:`int`]: Can be :class:`None` if the member isn't ranked yet
+
+        Raises
+        ------
+        - `DatabaseFileNotFound`: The database file was not found
+        - `LeaderboardNotFound`: Table "leaderboard" in the database file is missing
+        - `ImproperLeaderboard`: Leaderboard table was altered. Components changed or deleted
+        - `NotConnected`: Attempted to use a method that requires a connection to a database file
+        """
+        result = await self._connection.execute_fetchall('SELECT member_id FROM leaderboard WHERE guild_id = ? ORDER BY member_total_xp DESC', (member.guild.id,)) # type: ignore
+        all_ids = [m_id[0] for m_id in result]
+        try:
+            rank = all_ids.index(member.id) + 1
+            return rank
+        except ValueError:
+            return None
+    
+    @db_file_exists
+    @leaderboard_exists
+    @verify_leaderboard_integrity
+    async def sql_query_get(self, sql: str, parameters: Optional[Tuple[Union[str, int]]]=None, fetch: Union[str, int]='ALL') -> Union[List[tuple], tuple]:
+        """|coro|
+        
+        Query and return something from the database using SQL. The following columns are apart of the "leaderboard" table:
+
+        - guild_id
+        - member_id
+        - member_name
+        - member_level
+        - member_xp
+        - member_total_xp
+
+        Parameters
+        ----------
+        sql: :class:`str`
+            SQL string used to query the database
+        
+        parameters: Optional[Tuple[Union[:class:`str`, :class:`int`]]]
+            The parameters used for the database query
+        
+        fetch: Union[:class:`str`, :class:`int`]
+            The amount of rows you would like back from the query. Options: 'ALL', 'ONE', or an integer value that is greater than zero
+        
+        Returns
+        -------
+        Union[List[:class:`tuple`], :class:`tuple`]:
+
+        - Using `fetch='ALL'` returns List[:class:`tuple`]
+        - Using `fetch='ONE'` returns :class:`tuple`
+        - Using `fetch=4` returns List[:class:`tuple`] with only four values
+        
+        Can also return an empty list if the query was valid but got nothing from it
+        
+        Raises
+        ------
+        - `DatabaseFileNotFound`: The database file was not found
+        - `LeaderboardNotFound`: Table "leaderboard" in the database file is missing
+        - `ImproperLeaderboard`: Leaderboard table was altered. Components changed or deleted
+        - `NotConnected`: Attempted to use a method that requires a connection to a database file
+        - `DiscordLevelingSystemError`: Argument "fetch" was the wrong type or used an invalid value
+        - `aiosqlite.Error`: Base aiosqlite error. Multiple errors can arise from this if the SQL query was invalid
+        """
+        if isinstance(fetch, str):
+            fetch = fetch.upper()
+            if fetch in ('ALL', 'ONE'):
+                async with self._connection.execute(sql, parameters) as cursor: # type: ignore
+                    if fetch == 'ALL':
+                        return await cursor.fetchall() # type: ignore
+                    elif fetch == 'ONE':
+                        return await cursor.fetchone() # type: ignore
+            else:
+                raise DiscordLevelingSystemError(f'Fetch {fetch!r} not recognized')
+        elif isinstance(fetch, int):
+            if fetch > 0:
+                async with self._connection.execute(sql, parameters) as cursor: # type: ignore
+                    return await cursor.fetchmany(fetch) # type: ignore
+            else:
+                raise DiscordLevelingSystemError('Argument "fetch" must be greater than zero')
+        else:
+            raise DiscordLevelingSystemError(f'Argument "fetch" needs to be str or int, got {fetch.__class__.__name__}')
+    
+    def _get_last_award(self, current_award: RoleAward, guild_awards: List[RoleAward]) -> RoleAward:
+        """Get the last :class:`RoleAward` that was given to the member. Returns the current :class:`RoleAward` if the last award is the current one
+        
+            .. changes::
+                v0.0.2
+                    Added :param:`guild_awards`
+        """
+        current_award_idx = guild_awards.index(current_award)
+        last_award_idx = guild_awards.index(current_award) - 1
+        if last_award_idx < 0:
+            last_award_idx = current_award_idx
+
+        if last_award_idx == current_award_idx:
+            return current_award
+        else:
+            return guild_awards[last_award_idx]
+    
+    async def _refresh_name(self, message: Message) -> None:
+        """|coro| If the members current database name doesn't match the name that's on discord, update the name in the database
+
+            .. NOTE
+                This is called AFTER we update or insert a new member into the database from :meth:`award_xp`, so :meth:`fetchone` will always return something
+        """
+        async with self._connection.execute('SELECT member_name FROM leaderboard WHERE member_id = ? AND guild_id = ?', (message.author.id, message.author.guild.id)) as cursor: # type: ignore
+            data = await cursor.fetchone()
+            database_name = data[0] # type: ignore / will always have a value because as *soon* as a member sends a message, the database is updated to contain a value to fetch
+            if database_name != str(message.author):
+                await cursor.execute('UPDATE leaderboard SET member_name = ? WHERE member_id = ? AND guild_id = ?', (str(message.author), message.author.id, message.author.guild.id)) # type: ignore
+                await self._connection.commit() # type: ignore
+    
+    async def _handle_level_up(self, message: Message, md: MemberData, leveled_up: bool) -> None:
+        """|coro| Gives/removes roles from members that leveled up and met the :class:`RoleAward` requirement. This also sends the level up message
+        
+            .. changes::
+                v0.0.2
+                    Added handling for level up messages that are embeds
+                    Added handling for random selections of level up messages
+                    Added :param:`md`
+                    Added :param:`leveled_up`
+                    Added if check for :param:`leveled_up`
+                    Added :func:`send_announcement`
+                    Removed raising of exception (AwardedRoleNotFound) to support multi-guild leveling
+                    Removed raising of exception (LevelUpChannelNotFound) to support multi-guild level up channel IDs
+                v1.0.2
+                    Added handling for event `on_dls_level_up`
+        """
+        if leveled_up:
+            member: Member = message.author # type: ignore / `.author` will be :class:`discord.Member` (lib doesn't work in DMs)
+            
+            def role_exists(award: RoleAward) -> Optional[Role]:
+                """Check to ensure the role associated with the :class:`RoleAward` still exists in the guild. If it does, it returns that discord role object for use"""
+                return message.guild.get_role(award.role_id) # type: ignore / `.guild` will always be :class:`discord.Guild`
+            
+            async def send_announcement(announcement_message, channel, send_kwargs):
+                """|coro| Send the level up message
+
+                    .. added:: v0.0.2
+                """
+                if isinstance(announcement_message, str):
+                    await channel.send(announcement_message, **send_kwargs)
+                else:
+                    await channel.send(embed=announcement_message, **send_kwargs)
+            
+            # send the level up message
+            if self.announce_level_up:
+                
+                # set the values for the level up announcement
+                lua: LevelUpAnnouncement = random.choice(self.level_up_announcement) if isinstance(self.level_up_announcement, Sequence) else self.level_up_announcement
+                lua._total_xp = md.total_xp
+                lua._level = md.level
+                lua._rank = md.rank
+                announcement_message = lua._parse_message(lua.message, self._message_author) # type: ignore
+
+                if lua.level_up_channel_ids:
+                    channel_found = False
+                    for channel_id in lua.level_up_channel_ids:
+                        channel = message.guild.get_channel(channel_id) # type: ignore / `.guild` will always be :class:`discord.Guild`
+                        if channel:
+                            channel_found = True
+                            break
+                    
+                    if channel_found:
+                        await send_announcement(announcement_message, channel, lua._send_kwargs) # type: ignore / this will not execute if channel not found
+                    else:
+                        await send_announcement(announcement_message, message.channel, lua._send_kwargs)
+                else:
+                    await send_announcement(announcement_message, message.channel, lua._send_kwargs)
+            
+            # check if there is a role award for the new level, if so, apply it
+            if self._awards:
+                try:
+                    # get the list of RoleAwards that match the guild ID
+                    guild_role_awards: List[RoleAward] = self._awards[message.guild.id] # type: ignore / `.guild` will always be :class:`discord.Guild`
+                except KeyError:
+                    return
+                else:
+                    # get the role award that matches the level up
+                    role_award = [ra for ra in guild_role_awards if ra.level_requirement == md.level]
+                    if role_award:
+                        role_award = role_award[0]
+                        if self.stack_awards:
+                            role_obj: Optional[Role] = role_exists(award=role_award)
+                            if role_obj:
+                                await member.add_roles(role_obj)
+                            else:
+                                return
+                        else:
+                            last_award: RoleAward = self._get_last_award(role_award, guild_role_awards)
+                            role_to_remove: Optional[Role] = role_exists(award=last_award)
+                            role_to_add: Optional[Role] = role_exists(award=role_award)
+                            
+                            # Note: Don't use an exception here because of multi-guild support
+                            if not role_to_remove or not role_to_add:
+                                return
+
+                            if last_award == role_award:
+                                await member.add_roles(role_to_add)
+                            else:
+                                await member.add_roles(role_to_add)
+                                await member.remove_roles(role_to_remove)
+            
+            if self.bot is not None:
+                self.bot.dispatch('dls_level_up', member, message, md)
+    
+    def _handle_amount_param(self, arg: Union[int, Sequence[int]]) -> None:
+        """Simple check to ensure the proper types are being used for parameter "amount" in method :meth:`DiscordLevelingSystem.award_xp()`
+        
+            .. changes::
+                v0.0.2
+                    Added check to ensure the first value is larger than the next
+                    Added check to ensure the each value is unique
+                    Changed the value range from 1-100 to 1-25
+                v1.1.0
+                    Changed from list to Sequence
+        """
+        if isinstance(arg, (int, Sequence)):
+            if isinstance(arg, int):
+                # ensures the values are from 1-25
+                if arg <= 0 or arg > 25:
+                    raise DiscordLevelingSystemError('Parameter "amount" can only be a value from 1-25')
+            else:
+                # ensures there are only 2 values in the sequence
+                if len(arg) != 2:
+                    raise DiscordLevelingSystemError('Parameter "amount" sequence must only have two values')
+                
+                # ensures all values in the sequence are of type int
+                for item in arg:
+                    if not isinstance(item, int):
+                        raise DiscordLevelingSystemError('Parameter "amount" sequence, all values must be of type int')
+                
+                # ensures all values in the sequence are >= 1 and <= 25
+                for item in arg:
+                    if item <= 0 or item > 25:
+                        raise DiscordLevelingSystemError('Parameter "amount" sequence, all values can only be from 1-25')
+                
+                # ensures each value is unique
+                if arg[0] == arg[1]:
+                    raise DiscordLevelingSystemError('Parameter "amount" sequence expects both values to be unique')
+                
+                # ensures the first value is larger than the next
+                if arg[1] < arg[0]:
+                    raise DiscordLevelingSystemError('Parameter "amount" sequence expected value 1 to be larger than value 2')
+        else:
+            raise DiscordLevelingSystemError(f'Parameter "amount" expected int or Sequence, got {arg.__class__.__name__}')
+    
+    @overload
+    async def award_xp(self, *, amount: int, message: Message, refresh_name: bool=True, **kwargs) -> None:
+        ...
+    
+    @overload
+    async def award_xp(self, *, amount: Sequence[int]=[15, 25], message: Message, refresh_name: bool=True, **kwargs) -> None:
+        ...
+    
+    @db_file_exists
+    @leaderboard_exists
+    @verify_leaderboard_integrity
+    async def award_xp(self, *, amount: Union[int, Sequence[int]]=[15, 25], message: Message, refresh_name: bool=True, **kwargs) -> None:
+        """|coro|
+        
+        Give XP to the member that sent a message
+
+        Parameters
+        ----------
+        amount: Union[:class:`int`, Sequence[:class:`int`]]
+            The amount of XP to award to the member per message. Must be from 1-25. Can be a sequence with a minimum and maximum length of two. If :param:`amount` is a sequence of two integers, it will randomly
+            pick a number in between those numbers including the numbers provided
+        
+        message: :class:`discord.Message`
+            A message object
+        
+        refresh_name: :class:`bool`
+            Everytime the member sends a message, check if their name still matches the name in the database. If it doesn't match, update the database to match their current name. It is
+            suggested to leave this as `True` so the database can always have the most up-to-date record
+
+        Kwargs
+        ------
+        bonus: :class:`DiscordLevelingSystem.Bonus`
+            Set the bonus values. Read the :class:`DiscordLevelingSystem.Bonus` doc string for more details (defaults to :class:`None`)
+        
+        Raises
+        ------
+        - `DatabaseFileNotFound`: The database file was not found
+        - `LeaderboardNotFound`: Table "leaderboard" in the database file is missing
+        - `ImproperLeaderboard`: Leaderboard table was altered. Components changed or deleted
+        - `NotConnected`: Attempted to use a method that requires a connection to a database file
+        
+            .. changes::
+                v0.0.2
+                    Added handling for bonus xp (kwarg "bonus")
+                    Added initialization for :attr:`_message_author`
+                    Replaced query with class attr
+                    Moved the detection of a level up from :meth:`_handle_level_up` to here
+        """
+        if any([message.guild is None, self._determine_no_xp(message), message.author.bot, message.type != MessageType.default, self.active is False]):
+            return
+        else:
+            self._handle_amount_param(arg=amount)
+            if isinstance(amount, Sequence):
+                amount = random.randint(amount[0], amount[1])
+            
+            # bonus XP
+            bonus: Optional[DiscordLevelingSystem.Bonus] = kwargs.get('bonus')
+            if bonus:
+                for role_id in bonus.role_ids:
+                    role: Optional[Role] = message.guild.get_role(role_id) # type: ignore
+                    if role in message.author.roles: # type: ignore / This lib cannot operate with :class:`discord.User` (DM's). It will always be :class:`discord.Member`
+                        if bonus.multiply:
+                            amount *= bonus.bonus_amount
+                        else:
+                            amount += bonus.bonus_amount
+                        
+                        if amount > 75: # type: ignore
+                            amount = 75
+                        break
+            
+            bucket = self._cooldown.get_bucket(message)
+            on_cooldown = bucket.update_rate_limit() # type: ignore
+
+            if not on_cooldown:
+                member = message.author
+                self._message_author = member # type: ignore
+                async with self._connection.execute('SELECT * FROM leaderboard WHERE member_id = ? AND guild_id = ?', (member.id, member.guild.id)) as cursor: # type: ignore
+                    record = await cursor.fetchone()
+                    member_level_up = False
+                    if record:
+                        # update the database with the new amount
+                        query = """
+                            UPDATE leaderboard
+                            SET member_xp = member_xp + ?, member_total_xp = member_total_xp + ?
+                            WHERE member_id = ? AND guild_id = ?
+                        """
+                        await cursor.execute(query, (amount, amount, member.id, member.guild.id)) # type: ignore
+                        await self._connection.commit() # type: ignore
+
+                        # get the updated member data (level is not updated yet)
+                        md = await self.get_data_for(member) # type: ignore
+
+                        next_details = _next_level_details(md.level) # type: ignore
+                        if md.xp >= next_details.xp_needed and md.level < next_details.level: # type: ignore
+                            # update the database with the new level and reset the current XP count
+                            await cursor.execute('UPDATE leaderboard SET member_level = ?, member_xp = ? WHERE member_id = ? AND guild_id = ?', (next_details.level, 0, member.id, member.guild.id)) # type: ignore
+                            await self._connection.commit() # type: ignore
+                            member_level_up = True
+
+                        md = await self.get_data_for(member) # type: ignore
+                        await self._handle_level_up(message, md, leveled_up=member_level_up) # type: ignore
+
+                    else:
+                        await cursor.execute(DiscordLevelingSystem._QUERY_NEW_MEMBER, (member.guild.id, member.id, str(member), 0, amount, amount)) # type: ignore
+                        await self._connection.commit() # type: ignore
+
+                    if refresh_name:
+                        await self._refresh_name(message)
```

### Comparing `discordLevelingSystem-1.2.0/discordLevelingSystem/member_data.py` & `discordLevelingSystem-1.2.1/discordLevelingSystem/member_data.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,77 +1,77 @@
-"""
-MIT License
-
-Copyright (c) 2021-present Defxult#8269
-
-Permission is hereby granted, free of charge, to any person obtaining a
-copy of this software and associated documentation files (the "Software"),
-to deal in the Software without restriction, including without limitation
-the rights to use, copy, modify, merge, publish, distribute, sublicense,
-and/or sell copies of the Software, and to permit persons to whom the
-Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in
-all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS
-OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER 
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING 
-FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER 
-DEALINGS IN THE SOFTWARE.
-"""
-
-from typing import Dict, Optional, Union
-
-class MemberData:
-    """Represents a members record from the database converted to an object where each value from their record can be easily accessed. Used in coordination with :class:`DiscordLevelingSystem`
-
-    Attributes
-    ----------
-    id_number: :class:`int`
-        The members ID
-        
-    name: :class:`str`
-        The members name
-
-    level: :class:`int`
-        The members level
-        
-    xp: :class:`int`
-        The members xp
-
-    total_xp: :class:`int`
-        The members total xp
-
-    rank: Optional[:class:`int`]
-        The members rank. Can be `None` if the member is not ranked yet
-    
-    mention: :class:`str`
-        The discord member mention string
-    """
-
-    __slots__ = ('id_number', 'name', 'level', 'xp', 'total_xp', 'rank', 'mention')
-
-    def __init__(self, id_number: int, name: str, level: int, xp: int, total_xp: int, rank: Optional[int]):
-        self.id_number = id_number
-        self.name = name
-        self.level = level
-        self.xp = xp
-        self.total_xp = total_xp
-        self.rank = rank
-        self.mention = f'<@{id_number}>'
-    
-    def __repr__(self):
-        return f'<MemberData id_number={self.id_number} name={self.name!r} level={self.level} xp={self.xp} total_xp={self.total_xp} rank={self.rank}>'
-    
-    def to_dict(self) -> Dict[str, Union[int, str]]:
-        """Return the :class:`dict` representation of the :class:`MemberData` object
-
-        Returns
-        -------
-        Dict[:class:`str`, Union[:class:`int`, :class:`str`]]
-
-            .. added:: v1.0.1
-        """
-        return {key : getattr(self, key) for key in self.__class__.__slots__}
+"""
+MIT License
+
+Copyright (c) 2021-present Defxult#8269
+
+Permission is hereby granted, free of charge, to any person obtaining a
+copy of this software and associated documentation files (the "Software"),
+to deal in the Software without restriction, including without limitation
+the rights to use, copy, modify, merge, publish, distribute, sublicense,
+and/or sell copies of the Software, and to permit persons to whom the
+Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in
+all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS
+OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER 
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING 
+FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER 
+DEALINGS IN THE SOFTWARE.
+"""
+
+from typing import Dict, Optional, Union
+
+class MemberData:
+    """Represents a members record from the database converted to an object where each value from their record can be easily accessed. Used in coordination with :class:`DiscordLevelingSystem`
+
+    Attributes
+    ----------
+    id_number: :class:`int`
+        The members ID
+        
+    name: :class:`str`
+        The members name
+
+    level: :class:`int`
+        The members level
+        
+    xp: :class:`int`
+        The members xp
+
+    total_xp: :class:`int`
+        The members total xp
+
+    rank: Optional[:class:`int`]
+        The members rank. Can be `None` if the member is not ranked yet
+    
+    mention: :class:`str`
+        The discord member mention string
+    """
+
+    __slots__ = ('id_number', 'name', 'level', 'xp', 'total_xp', 'rank', 'mention')
+
+    def __init__(self, id_number: int, name: str, level: int, xp: int, total_xp: int, rank: Optional[int]):
+        self.id_number = id_number
+        self.name = name
+        self.level = level
+        self.xp = xp
+        self.total_xp = total_xp
+        self.rank = rank
+        self.mention = f'<@{id_number}>'
+    
+    def __repr__(self):
+        return f'<MemberData id_number={self.id_number} name={self.name!r} level={self.level} xp={self.xp} total_xp={self.total_xp} rank={self.rank}>'
+    
+    def to_dict(self) -> Dict[str, Union[int, str]]:
+        """Return the :class:`dict` representation of the :class:`MemberData` object
+
+        Returns
+        -------
+        Dict[:class:`str`, Union[:class:`int`, :class:`str`]]
+
+            .. added:: v1.0.1
+        """
+        return {key : getattr(self, key) for key in self.__class__.__slots__}
```

### Comparing `discordLevelingSystem-1.2.0/discordLevelingSystem/role_awards.py` & `discordLevelingSystem-1.2.1/discordLevelingSystem/role_awards.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,139 +1,139 @@
-"""
-MIT License
-
-Copyright (c) 2021-present Defxult#8269
-
-Permission is hereby granted, free of charge, to any person obtaining a
-copy of this software and associated documentation files (the "Software"),
-to deal in the Software without restriction, including without limitation
-the rights to use, copy, modify, merge, publish, distribute, sublicense,
-and/or sell copies of the Software, and to permit persons to whom the
-Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in
-all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS
-OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER 
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING 
-FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER 
-DEALINGS IN THE SOFTWARE.
-"""
-
-from __future__ import annotations
-
-from collections import Counter
-from typing import Dict, List, Optional, Union
-
-from .errors import ImproperRoleAwardOrder, RoleAwardError
-
-
-class RoleAward:
-    """Represents the role that will be awarded to the member upon meeting the XP requirement
-
-    Parameters
-    ----------
-    role_id: :class:`int`
-        ID of the role that is to be awarded
-    
-    level_requirement: :class:`int`
-        What level is required for a member to be awarded the role
-    
-    role_name: Optional[:class:`str`]
-        A name you can set for the award. Nothing is done with this value, it is used for visual identification purposes only
-    
-    Attributes
-    ----------
-    - `role_id`
-    - `level_requirement`
-    - `role_name`
-    - `mention`
-    """
-
-    __slots__ = ('role_id', 'level_requirement', 'role_name', 'mention')
-
-    def __init__(self, role_id: int, level_requirement: int, role_name: Optional[str]=None):
-        self.role_id = role_id
-        self.level_requirement = level_requirement
-        
-        # v0.0.2
-        self.role_name = role_name
-        
-        # v1.0.0
-        self.mention = f'<@&{role_id}>'
-
-    def __repr__(self):
-        return f'<RoleAward role_id={self.role_id} level_requirement={self.level_requirement} role_name={self.role_name!r}>'
-    
-    def __eq__(self, value: object):
-        if isinstance(value, RoleAward):
-            return all([self.role_id == value.role_id, self.level_requirement == value.level_requirement])
-        else:
-            return False
-    
-    @staticmethod
-    def _check(awards: Union[Dict[int, List[RoleAward]], None]) -> None:
-        if awards:
-            if not isinstance(awards, (dict, type(None))): raise RoleAwardError(f'"awards" expected dict or None, got {awards.__class__.__name__}')
-
-            # ensure all dict keys and values are of the correct type
-            for key, value in awards.items():
-                if not isinstance(key, int): raise RoleAwardError('When setting the "awards" dict, all keys must be of type int')
-                if not isinstance(value, list): raise RoleAwardError('When setting the "awards" dict, all values must be of type list')
-                if isinstance(value, list) and not all([isinstance(role_award, RoleAward) for role_award in value]): raise RoleAwardError('When setting the "awards" dict, all values in the list must be of type RoleAward')
-            else:
-                RoleAward._guild_id_check(list(awards.keys()))
-                for award in awards.values():
-                    RoleAward._role_id_check(award)
-                    RoleAward._level_req_check(award)
-                    RoleAward._verify_duplicate_awards(award)
-                    RoleAward._verify_awards_integrity(award)
-    
-    @staticmethod
-    def _guild_id_check(guild_ids: List[int]) -> None:
-        """|static method| Ensures all guild IDs are unique
-        
-            .. added:: v0.0.2
-        """
-        counter = Counter(guild_ids)
-        if max(counter.values()) != 1:
-            raise RoleAwardError('When assigning role awards, all guild IDs must be unique')
-
-    @staticmethod
-    def _role_id_check(awards: List[RoleAward]) -> None:
-        """|static method| Ensure all IDs are unique"""
-        role_id_counter = Counter([award.role_id for award in awards])
-        if max(role_id_counter.values()) != 1:
-            raise RoleAwardError("There cannot be duplicate ID numbers when using role awards. All ID's must be unique")
-    
-    @staticmethod
-    def _level_req_check(awards: List[RoleAward]) -> None:
-        """|static method| Ensures all level requirements/level requirements values are unique and greater than zero"""
-        # ensure all level requirements are unique
-        lvl_req_counter = Counter([award.level_requirement for award in awards])
-        if max(lvl_req_counter.values()) != 1:
-            raise RoleAwardError("There cannot be duplicate level requirements when using role awards. All level requirements must be unique")
-        
-        # ensure all level requirement values are greater than zero
-        lvl_reqs = [award.level_requirement for award in awards if award.level_requirement <= 0]
-        if lvl_reqs:
-            raise RoleAwardError('All level requirement values must greater than zero')
-    
-    @staticmethod
-    def _verify_duplicate_awards(awards: List[RoleAward]) -> None:
-        """|static method| Only used in the :class:`DiscordLevelingSystem` constructor. Ensures all :class:`RoleAward` objects submitted are unique"""
-        object_ids = [id(obj) for obj in awards]
-        counter = Counter(object_ids)
-        if max(counter.values()) != 1:
-            raise RoleAwardError('There cannot be duplicate role award objects when setting the "awards"')
-    
-    @staticmethod
-    def _verify_awards_integrity(awards: List[RoleAward]) -> None:
-        """|static method| Only used in the :class:`DiscordLevelingSystem` constructor. Ensures the awards submitted to its constructor are in ascending order according to their level requirement"""
-        previous_level_requirement = 0
-        for award in awards:
-            if award.level_requirement < previous_level_requirement:
-                raise ImproperRoleAwardOrder('When setting "awards", role award level requirements must be in ascending order')
-            previous_level_requirement = award.level_requirement
+"""
+MIT License
+
+Copyright (c) 2021-present Defxult#8269
+
+Permission is hereby granted, free of charge, to any person obtaining a
+copy of this software and associated documentation files (the "Software"),
+to deal in the Software without restriction, including without limitation
+the rights to use, copy, modify, merge, publish, distribute, sublicense,
+and/or sell copies of the Software, and to permit persons to whom the
+Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in
+all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS
+OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER 
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING 
+FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER 
+DEALINGS IN THE SOFTWARE.
+"""
+
+from __future__ import annotations
+
+from collections import Counter
+from typing import Dict, List, Optional, Union
+
+from .errors import ImproperRoleAwardOrder, RoleAwardError
+
+
+class RoleAward:
+    """Represents the role that will be awarded to the member upon meeting the XP requirement
+
+    Parameters
+    ----------
+    role_id: :class:`int`
+        ID of the role that is to be awarded
+    
+    level_requirement: :class:`int`
+        What level is required for a member to be awarded the role
+    
+    role_name: Optional[:class:`str`]
+        A name you can set for the award. Nothing is done with this value, it is used for visual identification purposes only
+    
+    Attributes
+    ----------
+    - `role_id`
+    - `level_requirement`
+    - `role_name`
+    - `mention`
+    """
+
+    __slots__ = ('role_id', 'level_requirement', 'role_name', 'mention')
+
+    def __init__(self, role_id: int, level_requirement: int, role_name: Optional[str]=None):
+        self.role_id = role_id
+        self.level_requirement = level_requirement
+        
+        # v0.0.2
+        self.role_name = role_name
+        
+        # v1.0.0
+        self.mention = f'<@&{role_id}>'
+
+    def __repr__(self):
+        return f'<RoleAward role_id={self.role_id} level_requirement={self.level_requirement} role_name={self.role_name!r}>'
+    
+    def __eq__(self, value: object):
+        if isinstance(value, RoleAward):
+            return all([self.role_id == value.role_id, self.level_requirement == value.level_requirement])
+        else:
+            return False
+    
+    @staticmethod
+    def _check(awards: Union[Dict[int, List[RoleAward]], None]) -> None:
+        if awards:
+            if not isinstance(awards, (dict, type(None))): raise RoleAwardError(f'"awards" expected dict or None, got {awards.__class__.__name__}')
+
+            # ensure all dict keys and values are of the correct type
+            for key, value in awards.items():
+                if not isinstance(key, int): raise RoleAwardError('When setting the "awards" dict, all keys must be of type int')
+                if not isinstance(value, list): raise RoleAwardError('When setting the "awards" dict, all values must be of type list')
+                if isinstance(value, list) and not all([isinstance(role_award, RoleAward) for role_award in value]): raise RoleAwardError('When setting the "awards" dict, all values in the list must be of type RoleAward')
+            else:
+                RoleAward._guild_id_check(list(awards.keys()))
+                for award in awards.values():
+                    RoleAward._role_id_check(award)
+                    RoleAward._level_req_check(award)
+                    RoleAward._verify_duplicate_awards(award)
+                    RoleAward._verify_awards_integrity(award)
+    
+    @staticmethod
+    def _guild_id_check(guild_ids: List[int]) -> None:
+        """|static method| Ensures all guild IDs are unique
+        
+            .. added:: v0.0.2
+        """
+        counter = Counter(guild_ids)
+        if max(counter.values()) != 1:
+            raise RoleAwardError('When assigning role awards, all guild IDs must be unique')
+
+    @staticmethod
+    def _role_id_check(awards: List[RoleAward]) -> None:
+        """|static method| Ensure all IDs are unique"""
+        role_id_counter = Counter([award.role_id for award in awards])
+        if max(role_id_counter.values()) != 1:
+            raise RoleAwardError("There cannot be duplicate ID numbers when using role awards. All ID's must be unique")
+    
+    @staticmethod
+    def _level_req_check(awards: List[RoleAward]) -> None:
+        """|static method| Ensures all level requirements/level requirements values are unique and greater than zero"""
+        # ensure all level requirements are unique
+        lvl_req_counter = Counter([award.level_requirement for award in awards])
+        if max(lvl_req_counter.values()) != 1:
+            raise RoleAwardError("There cannot be duplicate level requirements when using role awards. All level requirements must be unique")
+        
+        # ensure all level requirement values are greater than zero
+        lvl_reqs = [award.level_requirement for award in awards if award.level_requirement <= 0]
+        if lvl_reqs:
+            raise RoleAwardError('All level requirement values must greater than zero')
+    
+    @staticmethod
+    def _verify_duplicate_awards(awards: List[RoleAward]) -> None:
+        """|static method| Only used in the :class:`DiscordLevelingSystem` constructor. Ensures all :class:`RoleAward` objects submitted are unique"""
+        object_ids = [id(obj) for obj in awards]
+        counter = Counter(object_ids)
+        if max(counter.values()) != 1:
+            raise RoleAwardError('There cannot be duplicate role award objects when setting the "awards"')
+    
+    @staticmethod
+    def _verify_awards_integrity(awards: List[RoleAward]) -> None:
+        """|static method| Only used in the :class:`DiscordLevelingSystem` constructor. Ensures the awards submitted to its constructor are in ascending order according to their level requirement"""
+        previous_level_requirement = 0
+        for award in awards:
+            if award.level_requirement < previous_level_requirement:
+                raise ImproperRoleAwardOrder('When setting "awards", role award level requirements must be in ascending order')
+            previous_level_requirement = award.level_requirement
```

### Comparing `discordLevelingSystem-1.2.0/discordLevelingSystem.egg-info/PKG-INFO` & `discordLevelingSystem-1.2.1/discordLevelingSystem.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,856 +1,861 @@
-Metadata-Version: 2.1
-Name: discordLevelingSystem
-Version: 1.2.0
-Summary: A library to implement a leveling system into a discord bot. Contains features such as XP, level, ranks, and role awards.
-Home-page: https://github.com/Defxult/discordLevelingSystem
-Author: Defxult#8269
-License: MIT
-Project-URL: Changelog, https://github.com/Defxult/discordLevelingSystem/blob/main/CHANGELOG.md
-Keywords: database,discord,discord bot,discord.py,discord py,discord level,discord leveling,discord leveling system,level,levels,leveling,level up,level system,mee6,rank,ranking,role award,xp
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-A library to implement a leveling system into a discord bot. One of the most popular discord bots out there is MEE6 and it's leveling system. This library provides ways to easily implement one for yourself. It uses SQLite (aiosqlite) to locally query things such as their XP, rank, and level. Various amounts of other methods and classes are also provided so you can access or remove contents from the database file.
-
-<!-- ## Installing
-You can install the latest [PyPI version](https://pypi.org/project/discordLevelingSystem/) of the library by doing:
-
-`$ pip install discordLevelingSystem`
-
-Or the development version:
-
-`$ pip install git+https://github.com/Defxult/discordLevelingSystem` -->
-
----
-
-## Showcase
-![showcase](https://cdn.discordapp.com/attachments/655186216060321816/835010159092039680/leveling_showcase.gif)
-
----
-## How to import
-```py
-from discordLevelingSystem import DiscordLevelingSystem, LevelUpAnnouncement, RoleAward
-```
-
----
-## Intents
-[Intents](https://discordpy.readthedocs.io/en/stable/intents.html) are required for proper functionality
-```py
-bot = commands.Bot(..., intents=discord.Intents(messages=True, guilds=True, members=True))
-```
----
-
-
-## DiscordLevelingSystem
-```class DiscordLevelingSystem(rate=1, per=60.0, awards=None, **kwargs)```
-
----
-### Parameters of the DiscordLevelingSystem constructor
-* `rate` (`int`) The amount of messages each member can send before the cooldown triggers
-* `per` (`float`) The amount of seconds each member has to wait before gaining more XP, aka the cooldown
-* `awards` (`Optional[Dict[int, List[RoleAward]]]`) The role given to a member when they reach a `RoleAward` level requirement
----
-### Kwargs of the DiscordLevelingSystem constructor
-| Name | Type | Default Value | Info
-|------|------|---------------|-----
-| `no_xp_roles` | `Sequence[int]` | `None` | A sequence of role ID's. Any member with any of those roles will not gain XP when sending messages
-| `no_xp_channels` | `Sequence[int]` | `None` | A sequence of text channel ID's. Any member sending messages in any of those text channels will not gain XP
-| `announce_level_up` | `bool` | `True` | If `True`, level up messages will be sent when a member levels up
-| `stack_awards` | `bool` | `True` | If this is `True`, when the member levels up the assigned role award will be applied. If `False`, the previous role award will be removed and the level up assigned role will also be applied
-| `level_up_announcement` | `Union[LevelUpAnnouncement, Sequence[LevelUpAnnouncement]]` | `LevelUpAnnouncement()` | The message that is sent when someone levels up. If this is a sequence of `LevelUpAnnouncement`, one is selected at random
-|`bot` | ` Union[AutoShardedBot, Bot]` | `None` | Your bot instance variable. Used only if you'd like to use the `on_dls_level_up` event
-
----
-### Attributes
-* `no_xp_roles`
-* `no_xp_channels`
-* `announce_level_up`
-* `stack_awards`
-* `level_up_announcement`
-* `bot`
-* `rate` (`int`) Read only property from the constructor
-* `per` (`float`) Read only property from the constructor
-* `database_file_path` (`str`) Read only property
-* `active` (`bool`) Enable/disable the leveling system. If `False`, nobody can gain XP when sending messages unless this is set back to `True`
-
-> NOTE: All attributes can be set during initialization
----
-## Initial Setup
-When setting up the leveling system, a database file needs to be created in order for the library to function. 
-* Associated static method
-  * `DiscordLevelingSystem.create_database_file(path: str)`
-
-The above static method is used to create the database file for you in the path you specify. This method only needs to be called once. Example:
-```py
-DiscordLevelingSystem.create_database_file(r'C:\Users\Defxult\Documents')
-```
-Once created, there is no need to ever run that method again unless you want to create a new database file from scratch. Now that you have the database file, you can use the leveling system.
-
----
-## Connecting to the Database
-* Associated method
-  * `DiscordLevelingSystem.connect_to_database_file(path: str)`
-
-Since the database file has already been created, all you need to do is connect to it. 
-> NOTE: When connecting to the database file, the event loop must not be running
-<div align="left"><sub>EXAMPLE</sub></div>
-
-```py
-from discord.ext import commands
-from discordLevelingSystem import DiscordLevelingSystem
-
-bot = commands.Bot(...)
-lvl = DiscordLevelingSystem()
-lvl.connect_to_database_file(r'C:\Users\Defxult\Documents\DiscordLevelingSystem.db')
-
-bot.run(...)
-```
----
-
-## RoleAward
-```class RoleAward(role_id: int, level_requirement: int, role_name=None)```
-
-You can assign roles to the system so when someone levels up to a certain level, they are given that role. `RoleAward` is how that is accomplished.
-
----
-### Parameters of the RoleAward constructor
-* `role_id` (`int`) ID of the role that is to be awarded.
-* `level_requirement` (`int`) What level is required for a member to be awarded the role.
-* `role_name` (`Optional[str]`) A name you can set for the award. Nothing is done with this value, it is used for visual identification purposes only.
----
-### Attributes
-* `role_id`
-* `level_requirement`
-* `role_name`
-* `mention` (`str`) The discord role mention string
-
-When creating role awards, all role IDs and level requirements must be unique. Level requirements must also be in ascending order. It is also possible to assign different role awards for different guilds. If you don't want any role awards, set the `awards` parameter to `None`. When setting `awards`, it accepts a `dict` where the keys are guild IDs and the values are a `list` of `RoleAward`
-<div align="left"><sub>EXAMPLE</sub></div>
-
-```py
-from discordLevelingSystem import DiscordLevelingSystem, RoleAward
-
-johns_server = 587937522043060224
-janes_server = 850809412011950121
-
-my_awards = {
-    johns_server : [
-        RoleAward(role_id=831672678586777601, level_requirement=1, role_name='Rookie'),
-        RoleAward(role_id=831672730583171073, level_requirement=2, role_name='Associate'),
-        RoleAward(role_id=831672814419050526, level_requirement=3, role_name='Legend')
-    ],
-    janes_server : [
-        RoleAward(role_id=851400453904400385, level_requirement=1, role_name='Silver'),
-        RoleAward(role_id=851379776111116329, level_requirement=2, role_name='Gold'),
-        RoleAward(role_id=851959077071880202, level_requirement=3, role_name='Diamond')
-    ]
-}
-
-lvl = DiscordLevelingSystem(..., awards=my_awards)
-```
----
-
-## LevelUpAnnouncement
-```class LevelUpAnnouncement(message=default_message, level_up_channel_ids=None, allowed_mentions=default_mentions, tts=False, delete_after=None)```
-
-Level up announcements are for when you want to implement your own level up messages. It provides access to who leveled up, their rank, level and much more. It also uses some of discord.py's kwargs from it's `Messageable.send` such as `allowed_mentions`, `tts`, and `delete_after` to give you more control over the sent message.
-
----
-### Parameters of the LevelUpAnnouncement constructor
-
-* `message` (`Union[str, discord.Embed]`) The message that is sent when someone levels up. Defaults to `"<mention>, you are now **level <level>!**"`
-
-* `level_up_channel_ids` (`Optional[Sequence[int]]`) The text channel IDs where all level up messages will be sent for each server. If `None`, the level up message will be sent in the channel where they sent the message (example below).
-
-* `allowed_mentions` (`discord.AllowedMentions`) Used to determine who can be pinged in the level up message. Defaults to `discord.AllowedMentions(everyone=False, users=True, roles=False, replied_user=False)`
-
-* `tts` (`bool`) When the level up message is sent, have discord read the level up message aloud.
-
-* `delete_after` (`Optional[float]`) Delete the level up message after an x amount of seconds.
-
-### Class Attributes
-The `LevelUpAnnouncement` class provides a set of markdown attributes for you to use so you can access certain information in a level up message.
-
-* `LevelUpAnnouncement.TOTAL_XP` The members current total XP amount
-* `LevelUpAnnouncement.LEVEL` The members current level
-* `LevelUpAnnouncement.RANK` The members current rank
-
-The below markdown attributes takes the information from a `discord.Member` object so you can access member information in the level up message.
-
-* `LevelUpAnnouncement.Member.avatar_url`
-* `LevelUpAnnouncement.Member.banner_url`
-* `LevelUpAnnouncement.Member.created_at`
-* `LevelUpAnnouncement.Member.default_avatar_url`
-* `LevelUpAnnouncement.Member.discriminator`
-* `LevelUpAnnouncement.Member.display_avatar_url`
-* `LevelUpAnnouncement.Member.display_name`
-* `LevelUpAnnouncement.Member.id`
-* `LevelUpAnnouncement.Member.joined_at`
-* `LevelUpAnnouncement.Member.mention`
-* `LevelUpAnnouncement.Member.name`
-* `LevelUpAnnouncement.Member.nick`
-* `LevelUpAnnouncement.Member.Guild.icon_url`
-* `LevelUpAnnouncement.Member.Guild.id`
-* `LevelUpAnnouncement.Member.Guild.name`
-
-<div align="left"><sub>EXAMPLE</sub></div>
-
-```py
-from discordLevelingSystem import DiscordLevelingSystem, LevelUpAnnouncement
-
-embed = discord.Embed()
-embed.set_author(name=LevelUpAnnouncement.Member.name, icon_url=LevelUpAnnouncement.Member.avatar_url)
-embed.description = f'Congrats {LevelUpAnnouncement.Member.mention}! You are now level {LevelUpAnnouncement.LEVEL} 😎'
-
-announcement = LevelUpAnnouncement(embed)
-
-lvl = DiscordLevelingSystem(..., level_up_announcement=announcement)
-
-# NOTE: You can have multiple level up announcements by setting the parameter to a sequence of LevelUpAnnouncement
-lvl = DiscordLevelingSystem(..., level_up_announcement=[announcement_1, announcement_2, ...])
-```
-When it comes to `level_up_channel_ids`, you can set a designated channel for each server. If you don't set a level up channel ID for a specific server, the level up message will be sent in the channel where the member leveled up. You don't have to specify a level up channel ID for each server unless you'd like to.
-```py
-johns_bot_commands = 489374746737648734 # text channel ID from server A
-janes_levelup_channel = 58498304930493094 # text channel ID from server B
-
-announcement = LevelUpAnnouncement(..., level_up_channel_ids=[johns_bot_commands, janes_levelup_channel])
-lvl = DiscordLevelingSystem(..., level_up_announcement=announcement)
-```
----
-## Handling XP
-Method `award_xp` is how members gain XP. This method is placed inside the `on_message` event of your bot. Members will gain XP if they send a message and if they're *not* on cooldown. Spamming messages will not give them XP.
-> NOTE: Members cannot gain XP in DM's
-* Associated methods
-  * `await DiscordLevelingSystem.add_xp(member: Member, amount: int)`
-  * `await DiscordLevelingSystem.remove_xp(member: Member, amount: int)`
-  * `await DiscordLevelingSystem.set_level(member: Member, level: int)`
-  * `await DiscordLevelingSystem.award_xp(*, amount=[15, 25], message: Message, refresh_name=True, **kwargs)`
-
-
-### Parameters for award_xp
-* `amount` (`Union[int, Sequence[int]]`) The amount of XP to award to the member per message. Must be from 1-25. Can be a sequence with a minimum and maximum length of two. If `amount` is a sequence of two integers, it will randomly pick a number in between those numbers including the numbers provided.
-* `message` (`discord.Message`) A discord message object
-* `refresh_name` (`bool`) Everytime the member sends a message, check if their name still matches the name in the database. If it doesn't match, update the database to match their current name. It is suggested to leave this as `True` so the database can always have the most up-to-date record.
-
-### Kwargs for award_xp
-* `bonus` (`DiscordLevelingSystem.Bonus`) Used to set the roles that will be awarded bonus XP.
-  * `class Bonus(role_ids: Sequence[int], bonus_amount: int, multiply: bool)`
-  * **Parameters of the DiscordLevelingSystem.Bonus constructor**
-    * `role_ids` (`Sequence[int]`) The role(s) a member must have to be able to get bonus XP. They only need to have one of these roles to get the bonus
-    * `bonus_amount` (`int`) Amount of extra XP to be awarded
-    * `multiply` (`bool`) If set to `True`, this will operate on a x2, x3 basis. Meaning if you have the awarded XP amount set to 10 and you want the bonus XP role to be awarded 20, it must be set to 2, not 10. If `False`, it operates purely on the given value. Meaning if you have the awarded XP set to 10 and you want the bonus XP role to be awarded 20, it must be set to 10.
-
-<div align="left"><sub>EXAMPLE</sub></div>
-
-```py
-lvl = DiscordLevelingSystem(...)
-
-nitro_booster = 851379776111116329
-associate_role = 851400453904400385
-
-@bot.event
-async def on_message(message):
-    await lvl.award_xp(amount=[15, 25], message=message, bonus=DiscordLevelingSystem.Bonus([nitro_booster, associate_role], 20, multiply=False))
-```
----
-
-## MemberData
-Accessing the raw information inside the database file can look a bit messy if you don't know exactly what you're looking at. To make things easier, this library comes with the `MemberData` class. A class which returns information about a specific member in the database.
-
-* Associated methods
-  * `await DiscordLevelingSystem.get_data_for(member: Member) -> MemberData`
-  * `await DiscordLevelingSystem.each_member_data(guild: Guild, sort_by=None, limit=None) -> List[MemberData]`
-
-### Attributes
-* `id_number` (`int`) The members ID
-* `name` (`str`) The members name
-* `level` (`int`) The members level
-* `xp` (`int`) The members xp
-* `total_xp` (`int`) The members total xp
-* `rank` (`Optional[int]`) The members rank
-* `mention` (`str`) The discord member mention string
-
-### Methods
-* `MemberData.to_dict() -> dict`
-
-<div align="left"><sub>EXAMPLE</sub></div>
-
-```py
-lvl = DiscordLevelingSystem(...)
-
-@bot.command()
-async def rank(ctx):
-    data = await lvl.get_data_for(ctx.author)
-    await ctx.send(f'You are level {data.level} and your rank is {data.rank}')
-
-@bot.command()
-async def leaderboard(ctx):
-    data = await lvl.each_member_data(ctx.guild, sort_by='rank')
-    # show the leaderboard whichever way you'd like
-```
----
-## Events
-You can set an event to be called when a member levels up. Using the event is considered as an enhanced `LevelUpAnnouncement` because it provides more capabilities rather than simply sending a message with only text/an embed. The `on_dls_level_up` event takes three parameters:
-* `member` (`discord.Member`) The member that leveled up
-* `message` (`discord.Message`) The message that triggered the level up
-* `data` (`MemberData`) The database information for that member
-
-```py
-bot = commands.Bot(...)
-lvl = DiscordLevelingSystem(..., bot=bot) # your bot instance variable is needed
-
-@bot.event
-async def on_dls_level_up(member: discord.Member, message: discord.Message, data: MemberData):
-    # You can do a lot more here compared to LevelUpAnnouncement
-    # - create a level up image and send it with discord.File
-    # - call additional functions that you may need
-    # - access to all attributes/methods that are available within discord.Member and discord.Message
-```
-> NOTE: `LevelUpAnnouncement` and `on_dls_level_up` are not the same. Level up messages are sent by default by the library. If you'd like to only use `on_dls_level_up`, you need to disable level up announcements (`lvl.announce_level_up = False`)
-
----
-## Full Example
-With all classes and core methods introduced, here is a basic implementation of this library.
-```py
-from discord.ext import commands
-from discordLevelingSystem import DiscordLevelingSystem, RoleAward, LevelUpAnnouncement
-
-bot = commands.Bot(...)
-
-main_guild_id = 850809412011950121
-
-my_awards = {
-    main_guild_id : [
-        RoleAward(role_id=831672678586777601, level_requirement=1, role_name='Rookie'),
-        RoleAward(role_id=831672730583171073, level_requirement=2, role_name='Associate'),
-        RoleAward(role_id=831672814419050526, level_requirement=3, role_name='Legend')
-    ]
-}
-
-announcement = LevelUpAnnouncement(f'{LevelUpAnnouncement.Member.mention} just leveled up to level {LevelUpAnnouncement.LEVEL} 😎')
-
-# DiscordLevelingSystem.create_database_file(r'C:\Users\Defxult\Documents') database file already created
-lvl = DiscordLevelingSystem(awards=my_awards, level_up_announcement=announcement)
-lvl.connect_to_database_file(r'C:\Users\Defxult\Documents\DiscordLevelingSystem.db')
-
-@bot.event
-async def on_message(message):
-    await lvl.award_xp(amount=15, message=message)
-
-bot.run(...)
-```
----
-
-## All methods for DiscordLevelingSystem
-<details>
-    <summary>Click to show all methods</summary>
-
-* *await* **add_record**(`guild_id, member_id, member_name, level`) - Manually add a record to the database. If the record already exists (the `guild_id` and `member_id` was found), only the level will be updated. If there were no records that matched those values, all provided information will be added
-  * **Parameters**
-    * **guild_id** (`int`) The guild ID to register
-    * **member_id** (`int`) The member ID to register
-    * **member_name** (`str`) The member name to register
-    * **level** (`int`) The member level to register. Must be from 0-100
-  * **Raises**
-    * `DiscordLevelingSystemError` - The value given from a parameter was not of the correct type or "level" was not 0-100
-
-
-* *await* **add_xp**(`member, amount`) - Give XP to a member. This also changes their level so it matches the associated XP
-  * **Parameters**
-    * **member** (`discord.Member`) The member to give XP to
-    * **amount** (`int`) Amount of XP to give to the member
-  * **Raises**
-    * `DatabaseFileNotFound` - The database file was not found
-    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
-    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
-    * `NotConnected` - Attempted to use a method that requires a connection to a database file
-    * `DiscordLevelingSystemError` - Parameter "amount" was less than or equal to zero. The minimum value is 1 
-
-
-* *await* **award_xp**(`*, amount = [15, 25], message, refresh_name = True, **kwargs`) - Give XP to the member that sent a message
-  * **Parameters**
-    * **amount** (`Union[int, Sequence[int]]`)
-    * **message** (`discord.Message`) A message object
-    * **refresh_name** (`bool`) Everytime the member sends a message, check if their name still matches the name in the database. If it doesn't match, update the database to match their current name. It is suggested to leave this as `True` so the database can always have the most up-to-date record
-  * **Kwargs**
-    * **bonus** (`DiscordLevelingSystem.Bonus`) Set the bonus values. Read the `DiscordLevelingSystem.Bonus` doc string for more details (defaults to `None`)
-  * **Raises**
-    * `DatabaseFileNotFound` - The database file was not found
-    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
-    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
-    * `NotConnected` - Attempted to use a method that requires a connection to a database file
-
-
-* **backup_database_file**(`path, with_timestamp = False`) - Create a copy of the database file to the specified path. If a copy of the backup file is already in the specified path it will be overwritten
-  * **Parameters**
-    * **path** (`str`) The path to copy the database file to
-    * **with_timestamp** (`bool`) Creates a unique file name that has the date and time of when the backup file was created. This is useful when you want multiple backup files
-  * **Raises**
-    * `DiscordLevelingSystemError` - Path doesn't exist or points to another file
-    * `NotConnected` - Attempted to use a method that requires a connection to a database file
-
-
-* *await* **change_cooldown**(`rate, per`) - Update the cooldown rate
-  * **Parameters**
-    * **rate** (`int`) The amount of messages each member can send before the cooldown triggers
-    * **per** (`float`) The amount of seconds each member has to wait before gaining more XP, aka the cooldown
-  * **Raises**
-    * `DatabaseFileNotFound` - The database file was not found
-    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
-    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
-    * `NotConnected` - Attempted to use a method that requires a connection to a database file
-    * `DiscordLevelingSystemError` - The rate or per value was not greater than zero
-
-
-* *await* **clean_database**(`guild`) - Removes the data for members that are no longer in the guild, thus reducing the database file size. It is recommended to have this method in a background loop in order to keep the database file free of records that are no longer in use
-  * **Parameters**
-    * **guild** (`discord.Guild`) The guild records to clean
-  * **Returns**
-    * (`Optional[int]`) The amount of records that were removed from the database
-  * **Raises**
-    * `DatabaseFileNotFound` - The database file was not found
-    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
-    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
-    * `NotConnected` - Attempted to use a method that requires a connection to a database file
-
-
-* **connect_to_database_file**(`path`) - Connect to the existing database file in the specified path
-  * **Parameters**
-    * **path** (`str`) The location of the database file
-  * **Raises**
-    * `ConnectionFailure` - Attempted to connect to the database file when the event loop is already running
-    * `DatabaseFileNotFound` - The database file was not found
-
-
-* *static method* **create_database_file**(`path = None`) - Create the database file and implement the SQL data for the database
-  * **Parameters**
-    * **path** (`Optional[str]`) The location to create the database file. If `None`, the file is created in the current working directory
-  * **Raises**
-    * `ConnectionFailure` - Attempted to create the database file when the event loop is already running
-    * `DiscordLevelingSystemError` - The path does not exist or the path points to a file instead of a directory
-
-
-* *await* **each_member_data**(`guild, sort_by = None, limit = None`) - Return each member in the database as a `MemberData` object for easy access to their XP, level, etc. You can sort the data with `sort_by` with the below values
-  * **Parameters**
-    * **guild** (`discord.Guild`) A guild object
-    * **sort_by** (`Optional[str]`) Return each member sorted by: "name", "level", "xp", "rank". If `None`, it will return in the order they were added to the database
-    * **limit** (`Optional[int]`) Restrict the amount of records returned to the specified amount
-  * **Returns**
-    * `List[MemberData]`
-  * **Raises**
-    * `DatabaseFileNotFound` - The database file was not found
-    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
-    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
-    * `NotConnected` - Attempted to use a method that requires a connection to a database file
-    * `DiscordLevelingSystemError` - The value of `sort_by` was not recognized or `guild` was not of type `discord.Guild`
-
-
-* *await* **export_as_json**(`path, guild`) - Export a json file that represents the database to the path specified
-  * **Parameters**
-    * **path** (`str`) Path to copy the json file to
-    * **guild** (`discord.Guild`) The guild for which the data should be extracted from. If `None`, all guild information will be extracted from the database
-  * **Raises**
-    * `DatabaseFileNotFound` - The database file was not found
-    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
-    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
-    * `NotConnected` - Attempted to use a method that requires a connection to a database file
-    * `DiscordLevelingSystemError` - The path does not exist or does not point to a directory
-
-
-* **get_awards**(`guild = None`) - Get all `RoleAward`'s or only the `RoleAward`'s assigned to the specified guild
-  * **Parameters**
-    * **guild** (`Optional[Union[discord.Guild, int]]`) A guild object or a guild ID
-  * **Returns**
-    * (`Union[Dict[int, List[RoleAward]], List[RoleAward]]`) If `guild` is `None`, this return the awards `dict` that was set in constructor. If `guild` is specified, it returns a List[`RoleAward`] that matches the specified guild ID. Can also return `None` if awards were never set or if the awards for the specified guild was not found
-
-
-* *await* **get_data_for**(`member`) - Get the `MemberData` object that represents the specified member
-  * **Parameters**
-    * **member** (`discord.Member`) The member to get the data for
-  * **Returns**
-    * (`MemberData`) Can be `None` if the member isn't in the database
-  * **Raises**
-    * `DatabaseFileNotFound` - The database file was not found
-    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
-    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
-    * `NotConnected` - Attempted to use a method that requires a connection to a database file
-
-
-* *await* **get_level_for**(`member`) - Get the level for the specified member
-  * **Parameters**
-    * **member** (`discord.Member`) Member to get the level for
-  * **Returns**
-    * (`int`) Can be `None` if the member isn't in the database
-  * **Raises**
-    * `DatabaseFileNotFound` - The database file was not found
-    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
-    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
-    * `NotConnected` - Attempted to use a method that requires a connection to a database file
-
-
-* *await* **get_rank_for**(`member`) - Get the rank for the specified member
-  * **Parameters**
-    * **member** (`discord.Member`) Member to get the rank for
-  * **Returns**
-    * (`int`) Can be `None` if the member isn't ranked yet
-  * **Raises**
-    * `DatabaseFileNotFound` - The database file was not found
-    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
-    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
-    * `NotConnected` - Attempted to use a method that requires a connection to a database file
-
-
-* *await* **get_record_count**(`guild = None`) - Get the amount of members that are registered in the database. If `guild` is set to `None`, ALL members in the database will be counted
-  * **Parameters**
-    * **guild** (`Optional[discord.Guild]`) The guild for which to count the amount of records
-  * **Returns**
-    * (`int`)
-  * **Raises**
-    * `DatabaseFileNotFound` - The database file was not found
-    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
-    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
-    * `NotConnected` - Attempted to use a method that requires a connection to a database file
-
-
-* *await* **get_total_xp_for**(`member`) - Get the total XP for the specified member
-  * **Parameters**
-    * **member** (`discord.Member`) Member to get the total XP for
-  * **Returns**
-    * (`int`) Can be `None` if the member isn't in the database
-  * **Raises**
-    * `DatabaseFileNotFound` - The database file was not found
-    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
-    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
-    * `NotConnected` - Attempted to use a method that requires a connection to a database file
-
-
-* *await* **get_xp_for**(`member`) - Get the XP for the specified member
-  * **Parameters**
-    * **member** (`discord.Member`) Member to get the XP for
-  * **Returns**
-    * (`int`) Can be `None` if the member isn't in the database
-  * **Raises**
-    * `DatabaseFileNotFound` - The database file was not found
-    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
-    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
-    * `NotConnected` - Attempted to use a method that requires a connection to a database file
-
-
-* *static method* **get_xp_for_level**(`level`) - Returns the total amount of XP needed for the specified level. Levels go from 0-100
-  * **Parameters**
-    * **level** (`int`) The level XP information to retrieve
-  * **Returns**
-    * (`int`)
-  * **Raises**
-    * `DiscordLevelingSystemError` - The level specified does not exist
-
-
-* *await* **insert**(`bot, guild_id, users, using, overwrite = False, show_results = True`) - Insert the records from your own leveling system into the library. A lot of leveling system tutorials out there use json files to store information. Although it might work, it is insufficient because json files are not made to act as a database. Using an actual database file has many benefits over a json file
-  * **Parameters**
-    * **bot** (`Union[discord.ext.commands.Bot, discord.ext.commands.AutoShardedBot]`) Your bot instance variable
-    * **guild_id** (`int`) ID of the guild that you used your leveling system with
-    * **users** (`Dict[int, int]`) This is the information that will be added to the database. The keys are user ID's, and the values are the users total XP or level. Note: This library only uses levels 0-100 and XP 0-1899250. If any number in this dict are over the levels/XP threshold, it is implicitly set back to this libraries maximum value
-    * **using** (`str`) What structure your leveling system used. Options: "xp" or "levels". Some leveling systems give users only XP and they are ranked up based on that XP value. Others use a combination of levels and XP. If all the values in the `users` dict are based on XP, set this to "xp". If they are based on a users level, set this to "levels"
-    * **overwrite** (`bool`) If a user you've specified in the `users` dict already has a record in the database, overwrite their current record with the one your inserting
-    * **show_results** (`bool`) Print the results for how many of the `users` were successfully added to the database file. If any are unsuccessful, their ID along with the value you provided will also be shown
-  * **Raises**
-      * `DiscordLevelingSystemError` - The value given from a parameter was not of the correct type. The `users` dict was empty. Or your bot is not in the guild associated with `guild_id`       
-
-
-* *await* **is_in_database**(`member, guild = None`) - A quick check to see if a member is in the database. This is not guild specific although it can be if `guild` is specified
-  * **Parameters**
-    * **member** (`Union[discord.Member, int]`) The member to check for. Can be the member object or that members ID
-    * **guild** (`Optional[discord.Guild]`) The guild to check if the member is registered in
-  * **Returns**
-    * (`bool`)
-  * **Raises**
-    * `DatabaseFileNotFound` - The database file was not found
-    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
-    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
-    * `NotConnected` - Attempted to use a method that requires a connection to a database file
-    * `DiscordLevelingSystemError` - Parameter `member` was not of type `discord.Member` or `int`
-
-
-* *static method* **levels_and_xp**( ) -  Get the raw `dict` representation for the amount of levels/XP in the system. The keys in the `dict` returned is each level, and the values are the amount of XP needed to be awarded that level
-  * **Returns**
-    * (`Dict[str, int]`)
-
-
-* *await* **next_level**(`member`) - Get the next level for the specified member
-  * **Parameters**
-    * **member** (`discord.Member`) Member to get the next level for
-  * **Returns**
-    * (`int`) If the member is currently max level (100), it will return 100. This can also return `None` if the member is not in the database
-  * **Raises**
-    * `DatabaseFileNotFound` - The database file was not found
-    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
-    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
-    * `NotConnected` - Attempted to use a method that requires a connection to a database file
-
-
-* *await* **next_level_up**(`member`) - Get the amount of XP needed for the specified member to level up
-  * **Parameters**
-    * **member** (`discord.Member`) Member to get the amount of XP needed for a level up
-  * **Returns**
-    * (`int`) Returns 0 if the member is currently at max level. Can return `None` if the member is not in the database.
-  * **Raises**
-    * `DatabaseFileNotFound` - The database file was not found
-    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
-    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
-    * `NotConnected` - Attempted to use a method that requires a connection to a database file
-
-
-* *await* **raw_database_contents**(`guild = None`) - Returns everything in the database. Can specify which guild information will be extracted
-  * **Parameters**
-    * **guild** (`Optional[discord.Guild]`) The guild to extract the raw database contents from. If `None`, information about all guilds will be extracted
-  * **Returns**
-    * `List[Tuple[int, int, str, int, int, int]]` The tuples inside the list represents each row of the database:
-      * Index 0 is the guild ID
-      * Index 1 is their ID
-      * Index 2 is their name
-      * Index 3 is their level
-      * Index 4 is their XP
-      * Index 5 is their total xp
-      * Can be an empty list if nothing is in the database
-  * **Raises**
-    * `DatabaseFileNotFound` - The database file was not found
-    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
-    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
-    * `NotConnected` - Attempted to use a method that requires a connection to a database file
-
-
-* *await* **refresh_names**(`guild`) - Update names inside the database. This does not add anything new. It simply verifies if the name in the database matches their current name, and if they don't match, update the database name
-  * **Parameters**
-    * **guild** (`discord.Guild`) A guild object
-  * **Returns**
-    * `(Optional[int])` The amount of records in the database that were updated
-  * **Raises**
-    * `DatabaseFileNotFound` - The database file was not found
-    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
-    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
-    * `NotConnected` - Attempted to use a method that requires a connection to a database file
-
-
-* *await* **remove_from_database**(`member, guild = None`) - Remove a member from the database. This is not guild specific although it can be if `guild` is specified
-  * **Parameters**
-    * **member** (`Union[discord.Member, int]`) The member to remove. Can be the member object or that members ID
-    * **guild** (`Optional[discord.Guild]`) If this parameter is given, it will remove the record of the specified member only from the specified guild record. If `None`, it will remove all records no matter the guild
-  * **Returns**
-    * (`Optional[bool]`) Returns `True` if the member was successfully removed from the database. `False` if the member was not in the database so there was nothing to remove
-  * **Raises**
-      * `DatabaseFileNotFound` - The database file was not found
-      * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
-      * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
-      * `DiscordLevelingSystemError` - Parameter `member` was not of type `discord.Member` or `int`
-      * `NotConnected` - Attempted to use a method that requires a connection to a database file
-
-
-* *await* **remove_xp**(`member, amount`) - Remove XP from a member. This also changes their level so it matches the associated XP
-  * **Parameters**
-      * **member** (`discord.Member`) The member to remove XP from
-      * **amount** (`int`) Amount of XP to remove from the member
-  * **Raises**
-    * `DatabaseFileNotFound` - The database file was not found
-    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
-    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
-    * `NotConnected` - Attempted to use a method that requires a connection to a database file
-    * `DiscordLevelingSystemError` - Parameter "amount" was less than or equal to zero. The minimum value is 1
-
-
-* *await* **reset_everyone**(`guild, *, intentional = False`) - Sets EVERYONES XP, total XP, and level to zero in the database. Can specify which guild to reset
-  * **Parameters**
-      * **guild** (`Union[discord.Guild, None]`) The guild for which everyone will be reset. If this is set to `None`, everyone in the entire database will be reset
-      * **intentional** (`bool`) A simple kwarg to try and ensure that this action is indeed what you want to do. Once executed, this cannot be undone
-  * **Raises**
-    * `DatabaseFileNotFound` - The database file was not found
-    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
-    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
-    * `NotConnected` - Attempted to use a method that requires a connection to a database file
-    * `FailSafe` - "intentional" argument for this method was set to `False` in case you called this method by mistake
-
-
-* *await* **reset_member**(`member`) - Sets the members XP, total XP, and level to zero
-  * **Parameters**
-    * **member** (`discord.Member`) The member to reset
-  * **Raises**
-    * `DatabaseFileNotFound` The database file was not found
-    * `LeaderboardNotFound` Table "leaderboard" in the database file is missing
-    * `ImproperLeaderboard` Leaderboard table was altered. Components changed or deleted
-    * `NotConnected` Attempted to use a method that requires a connection to a database file
-
-
-* *await* **set_level**(`member, level`) - Sets the level for the member. This also changes their total XP so it matches the associated level
-  * **Parameters**
-    * **member** (`discord.Member`) The member who's level will be set
-    * **level** (`int`) Level to set. Must be from 0-100     
-  * **Raises**
-    * `DatabaseFileNotFound` - The database file was not found
-    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
-    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
-    * `NotConnected` - Attempted to use a method that requires a connection to a database file
-    * `DiscordLevelingSystemError` - Parameter "level" was not from 0-100
-
-
-* *await* **sql_query_get**(`sql, parameters = None, fetch = 'ALL'`) - Query and return something from the database using SQL. The following columns are apart of the "leaderboard" table: guild_id, member_id, member_name, member_level, member_xp, member_total_xp
-  * **Parameters**
-    * **sql** (`str`) SQL string used to query the database
-    * **parameters** (`Optional[Tuple[Union[str ,int]]]`) The parameters used for the database query
-    * **fetch** (`Union[str, int]`) The amount of rows you would like back from the query. Options: 'ALL', 'ONE', or an integer value that is greater than zero
-  * **Returns**
-    * (`Union[List[tuple], tuple]`)
-      * Using `fetch='ALL'` returns `List[tuple]`
-      * Using `fetch='ONE'` returns `tuple`
-      * Using `fetch=4` returns `List[tuple]` with only four values
-      * Can also return an empty list if the query was valid but got nothing from it
-  * **Raises**
-    * `DatabaseFileNotFound` - The database file was not found
-    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
-    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
-    * `NotConnected` - Attempted to use a method that requires a connection to a database file
-    * `DiscordLevelingSystemError` - Argument "fetch" was the wrong type or used an invalid value
-    * `aiosqlite.Error` - Base aiosqlite error. Multiple errors can arise from this if the SQL query was invalid
-
-
-* *await* **switch_connection**(`path`) - Connect to a different leveling system database file
-  * **Parameters**
-    * **path** (`str`) The location of the database file
-  * **Raises**
-    * `DatabaseFileNotFound` - The database file was not found
-
-
-* *static method* **transfer**(`old, new, guild_id`) - Transfer the database records from a database file created from v0.0.1 to a blank database file created using v0.0.2+. If you were already using a v0.0.2+ database file, there's no need to use this method
-  * **Parameters**
-    * **old** (`str`) The path of the v0.0.1 database file
-    * **new** (`str`) The path of the v0.0.2+ database file
-    * **guild_id** (`int`) ID of the guild that was originally used with this library
-  * **Raises**
-    - `ConnectionFailure` - The event loop is already running
-    - `DatabaseFileNotFound` - "old" or "new" database file was not found
-    - `DiscordLevelingSystemError` - One of the databases is missing the "leaderboard" table. A v0.0.2+ database file contains records, or there was an attempt to transfer records from a v0.0.2+ file to another v0.0.2+ file
-
-
-* *await* **wipe_database**(`guild = None, *, intentional = False`) - Delete EVERYTHING from the database. If `guild` is specified, only the information related to that guild will be deleted
-  * **Parameters**
-    * **guild** (`Optional[discord.Guild]`) The guild for which all information that is related to that guild will be deleted. If `None`, everything will be deleted
-    * **intentional** (`bool`) A simple kwarg to try and ensure that this action is indeed what you want to do. Once executed, this cannot be undone
-  * **Raises**
-    * `DatabaseFileNotFound` - The database file was not found
-    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
-    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
-    * `NotConnected` - Attempted to use a method that requires a connection to a database file
-    * `FailSafe` - "intentional" argument for this method was set to `False` in case you called this method by mistake
-
-</details>
-
-## Migrating from v0.0.1 to v0.0.2+
-<details>
-    <summary>Click to show details</summary>
-
-This library was not originally designed with the use of multiple servers in mind, so all the data you might have currently (your database file was created in `v0.0.1`) should be from a single server. With `v0.0.2`, the structure of the database file was changed to accommodate this fix. That means if you are currently using a `v0.0.1` database file and update to `v0.0.2+`, a vast majority of the library will be broken. To avoid this, you need to transfer all your `v0.0.1` database file records to a `v0.0.2+` database file. This can be done using the `transfer` method.
-
-* Associated static method
-  * `DiscordLevelingSystem.transfer(old: str, new: str, guild_id: int)`
-
-### Parameters
-* `old` (`str`) The path of the `v0.0.1` database file
-* `new` (`str`) The path of the `v0.0.2+` database file (a brand new file from using `DiscordLevelingSystem.create_database_file(path: str)`)
-* `guild_id` (`int`) ID of the guild that was originally used with this library
-
-<div align="left"><sub>EXAMPLE</sub></div>
-
-```py
-from discordLevelingSystem import DiscordLevelingSystem
-
-old = r'C:\Users\Defxult\Documents\DiscordLevelingSystem.db'
-new = r'C:\Users\Defxult\Desktop\DiscordLevelingSystem.db'
-
-DiscordLevelingSystem.transfer(old, new, guild_id=850809412011950121)
-```
-
-</details>
-
-## Inserting your own leveling system information
-<details>
-    <summary>Click to show details</summary>
-
-Insert the records from your leveling system into this one. A lot of leveling system tutorials out there use json files to store information. Although it might work, it is insufficient because json files are not made to act as a database. Using a database file has many benefits over a json file. If you previously watched a tutorial for your leveling system and would like to import your records over to use with this library, you can do so with the below method.
-
-* Associated static method
-  * `await DiscordLevelingSystem.insert(bot: Union[Bot, AutoShardedBot], guild_id: int, users: Dict[int, int], using: str, overwrite=False, show_results=True)`
-
-### Parameters
-- `bot` (`Union[discord.ext.commands.Bot, discord.ext.commands.AutoShardedBot]`) Your bot instance variable
-
-- `guild_id` (`int`) ID of the guild that you used your leveling system with
-
-- `users` (`Dict[int, int]`) This is the information that will be added to the database. The keys are user ID's, and the values are the users total XP or level. Note: This library only uses levels 0-100 and XP 0-1899250. If any number in this dict are over the levels/XP threshold, it is implicitly set back to this libraries maximum value
-
-- `using` (`str`) What structure your leveling system used. Options: "xp" or "levels". Some leveling systems give users only XP and they are ranked up based on that XP value. Others use a combination of levels and XP. If all the values in the `users` dict are based on XP, set this to "xp". If they are based on a users level, set this to "levels"
-
-- `overwrite` (`bool`) If a user you've specified in the `users` dict already has a record in the database, overwrite their current record with the one your inserting
-
-- `show_results` (`bool`) Print the results for how many of the `users` were successfully added to the database file. If any are unsuccessful, their ID along with the value you provided will also be shown
-
-> NOTE: If the users you've provided in the `users` dict is not currently in the guild (`guild_id`), their information will not be inserted. If you'd like, you can manually add those records with method `DiscordLevelingSystem.add_record()`, but that is discouraged because it is better to discard information that is no longer in use (the user is no longer in the guild)
-
-<div align="left"><sub>EXAMPLE</sub></div>
-
-```py
-# leveling_system.json
-[
-  {
-      "5748392849348934" : {
-          "xp" : 373,
-          "level" : 4
-      }
-  },
-  {
-      "89283659820948923" : {
-          "xp" : 23,
-          "level" : 1
-      }
-  }
-]
-
-
-# bot.py
-import json
-from discord.ext import commands
-from discordLevelingSystem import DiscordLevelingSystem
-
-bot = commands.Bot(...)
-
-lvl = DiscordLevelingSystem(...)
-lvl.connect_to_database_file(...)
-
-def json_to_dict() -> dict:
-    with open('leveling_system.json') as fp:
-        data = json.load(fp)
-        formatted: Dict[int, int] = ... # format the data so all keys and values are associated with the user ID and level
-        
-        """
-        In the end, the formatted dict should look like so:
-        
-        formatted = {
-            5748392849348934 : 4,
-            89283659820948923 : 1
-        }
-        """
-        return formatted
-
-@bot.command()
-async def insert(ctx):
-    await lvl.insert(ctx.bot, guild_id=12345678901234, users=json_to_dict(), using='levels')
-
-bot.run(...)
-```
-
-</details>
+Metadata-Version: 2.1
+Name: discordLevelingSystem
+Version: 1.2.1
+Summary: A library to implement a leveling system into a discord bot. Contains features such as XP, level, ranks, and role awards.
+Author: Defxult#8269
+License: MIT
+Project-URL: Homepage, https://github.com/Defxult/discordLevelingSystem
+Project-URL: Changelog, https://github.com/Defxult/discordLevelingSystem/blob/main/CHANGELOG.md
+Keywords: database,discord,discord bot,discord.py,discord py,discord level,discord leveling,discord leveling system,level,levels,leveling,level up,level system,mee6,rank,ranking,role award,xp
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+A library to implement a leveling system into a discord bot. One of the most popular discord bots out there is MEE6 and it's leveling system. This library provides ways to easily implement one for yourself. It uses SQLite ([aiosqlite](https://pypi.org/project/aiosqlite/)) to locally query things such as their XP, rank, and level. Various amounts of other methods and classes are also provided so you can access or remove contents from the database file.
+
+[![Downloads](https://pepy.tech/badge/discordlevelingsystem)](https://pepy.tech/project/discordlevelingsystem)
+[![Downloads](https://pepy.tech/badge/discordlevelingsystem/month)](https://pepy.tech/project/discordlevelingsystem)
+![python_version](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10-blue)
+
+## Installing
+You can install the latest [PyPI version](https://pypi.org/project/discordLevelingSystem/) of the library by doing:
+
+`$ pip install discordLevelingSystem`
+
+Or the development version:
+
+`$ pip install git+https://github.com/Defxult/discordLevelingSystem`
+
+---
+
+## Showcase
+![showcase](https://cdn.discordapp.com/attachments/655186216060321816/835010159092039680/leveling_showcase.gif)
+
+---
+## How to import
+```py
+from discordLevelingSystem import DiscordLevelingSystem, LevelUpAnnouncement, RoleAward
+```
+
+---
+## Intents
+[Intents](https://discordpy.readthedocs.io/en/stable/intents.html) are required for proper functionality
+```py
+bot = commands.Bot(..., intents=discord.Intents(messages=True, guilds=True, members=True))
+```
+---
+
+
+## DiscordLevelingSystem
+```class DiscordLevelingSystem(rate=1, per=60.0, awards=None, **kwargs)```
+
+---
+### Parameters of the DiscordLevelingSystem constructor
+* `rate` (`int`) The amount of messages each member can send before the cooldown triggers
+* `per` (`float`) The amount of seconds each member has to wait before gaining more XP, aka the cooldown
+* `awards` (`Optional[Dict[int, List[RoleAward]]]`) The role given to a member when they reach a `RoleAward` level requirement
+---
+### Kwargs of the DiscordLevelingSystem constructor
+| Name | Type | Default Value | Info
+|------|------|---------------|-----
+| `no_xp_roles` | `Sequence[int]` | `None` | A sequence of role ID's. Any member with any of those roles will not gain XP when sending messages
+| `no_xp_channels` | `Sequence[int]` | `None` | A sequence of text channel ID's. Any member sending messages in any of those text channels will not gain XP
+| `announce_level_up` | `bool` | `True` | If `True`, level up messages will be sent when a member levels up
+| `stack_awards` | `bool` | `True` | If this is `True`, when the member levels up the assigned role award will be applied. If `False`, the previous role award will be removed and the level up assigned role will also be applied
+| `level_up_announcement` | `Union[LevelUpAnnouncement, Sequence[LevelUpAnnouncement]]` | `LevelUpAnnouncement()` | The message that is sent when someone levels up. If this is a sequence of `LevelUpAnnouncement`, one is selected at random
+|`bot` | ` Union[AutoShardedBot, Bot]` | `None` | Your bot instance variable. Used only if you'd like to use the `on_dls_level_up` event
+
+---
+### Attributes
+* `no_xp_roles`
+* `no_xp_channels`
+* `announce_level_up`
+* `stack_awards`
+* `level_up_announcement`
+* `bot`
+* `rate` (`int`) Read only property from the constructor
+* `per` (`float`) Read only property from the constructor
+* `database_file_path` (`str`) Read only property
+* `active` (`bool`) Enable/disable the leveling system. If `False`, nobody can gain XP when sending messages unless this is set back to `True`
+
+> NOTE: All attributes can be set during initialization
+---
+## Initial Setup
+When setting up the leveling system, a database file needs to be created in order for the library to function. 
+* Associated static method
+  * `DiscordLevelingSystem.create_database_file(path: str)`
+
+The above static method is used to create the database file for you in the path you specify. This method only needs to be called once. Example:
+```py
+DiscordLevelingSystem.create_database_file(r'C:\Users\Defxult\Documents')
+```
+Once created, there is no need to ever run that method again unless you want to create a new database file from scratch. Now that you have the database file, you can use the leveling system.
+
+---
+## Connecting to the Database
+* Associated method
+  * `DiscordLevelingSystem.connect_to_database_file(path: str)`
+
+Since the database file has already been created, all you need to do is connect to it. 
+> NOTE: When connecting to the database file, the event loop must not be running
+<div align="left"><sub>EXAMPLE</sub></div>
+
+```py
+from discord.ext import commands
+from discordLevelingSystem import DiscordLevelingSystem
+
+bot = commands.Bot(...)
+lvl = DiscordLevelingSystem()
+lvl.connect_to_database_file(r'C:\Users\Defxult\Documents\DiscordLevelingSystem.db')
+
+bot.run(...)
+```
+---
+
+## RoleAward
+```class RoleAward(role_id: int, level_requirement: int, role_name=None)```
+
+You can assign roles to the system so when someone levels up to a certain level, they are given that role. `RoleAward` is how that is accomplished.
+
+---
+### Parameters of the RoleAward constructor
+* `role_id` (`int`) ID of the role that is to be awarded.
+* `level_requirement` (`int`) What level is required for a member to be awarded the role.
+* `role_name` (`Optional[str]`) A name you can set for the award. Nothing is done with this value, it is used for visual identification purposes only.
+---
+### Attributes
+* `role_id`
+* `level_requirement`
+* `role_name`
+* `mention` (`str`) The discord role mention string
+
+When creating role awards, all role IDs and level requirements must be unique. Level requirements must also be in ascending order. It is also possible to assign different role awards for different guilds. If you don't want any role awards, set the `awards` parameter to `None`. When setting `awards`, it accepts a `dict` where the keys are guild IDs and the values are a `list` of `RoleAward`
+<div align="left"><sub>EXAMPLE</sub></div>
+
+```py
+from discordLevelingSystem import DiscordLevelingSystem, RoleAward
+
+johns_server = 587937522043060224
+janes_server = 850809412011950121
+
+my_awards = {
+    johns_server : [
+        RoleAward(role_id=831672678586777601, level_requirement=1, role_name='Rookie'),
+        RoleAward(role_id=831672730583171073, level_requirement=2, role_name='Associate'),
+        RoleAward(role_id=831672814419050526, level_requirement=3, role_name='Legend')
+    ],
+    janes_server : [
+        RoleAward(role_id=851400453904400385, level_requirement=1, role_name='Silver'),
+        RoleAward(role_id=851379776111116329, level_requirement=2, role_name='Gold'),
+        RoleAward(role_id=851959077071880202, level_requirement=3, role_name='Diamond')
+    ]
+}
+
+lvl = DiscordLevelingSystem(..., awards=my_awards)
+```
+---
+
+## LevelUpAnnouncement
+```class LevelUpAnnouncement(message=default_message, level_up_channel_ids=None, allowed_mentions=default_mentions, tts=False, delete_after=None)```
+
+Level up announcements are for when you want to implement your own level up messages. It provides access to who leveled up, their rank, level and much more. It also uses some of discord.py's kwargs from it's `Messageable.send` such as `allowed_mentions`, `tts`, and `delete_after` to give you more control over the sent message.
+
+---
+### Parameters of the LevelUpAnnouncement constructor
+
+* `message` (`Union[str, discord.Embed]`) The message that is sent when someone levels up. Defaults to `"<mention>, you are now **level <level>!**"`
+
+* `level_up_channel_ids` (`Optional[Sequence[int]]`) The text channel IDs where all level up messages will be sent for each server. If `None`, the level up message will be sent in the channel where they sent the message (example below).
+
+* `allowed_mentions` (`discord.AllowedMentions`) Used to determine who can be pinged in the level up message. Defaults to `discord.AllowedMentions(everyone=False, users=True, roles=False, replied_user=False)`
+
+* `tts` (`bool`) When the level up message is sent, have discord read the level up message aloud.
+
+* `delete_after` (`Optional[float]`) Delete the level up message after an x amount of seconds.
+
+### Class Attributes
+The `LevelUpAnnouncement` class provides a set of markdown attributes for you to use so you can access certain information in a level up message.
+
+* `LevelUpAnnouncement.TOTAL_XP` The members current total XP amount
+* `LevelUpAnnouncement.LEVEL` The members current level
+* `LevelUpAnnouncement.RANK` The members current rank
+
+The below markdown attributes takes the information from a `discord.Member` object so you can access member information in the level up message.
+
+* `LevelUpAnnouncement.Member.avatar_url`
+* `LevelUpAnnouncement.Member.banner_url`
+* `LevelUpAnnouncement.Member.created_at`
+* `LevelUpAnnouncement.Member.default_avatar_url`
+* `LevelUpAnnouncement.Member.discriminator`
+* `LevelUpAnnouncement.Member.display_avatar_url`
+* `LevelUpAnnouncement.Member.display_name`
+* `LevelUpAnnouncement.Member.id`
+* `LevelUpAnnouncement.Member.joined_at`
+* `LevelUpAnnouncement.Member.mention`
+* `LevelUpAnnouncement.Member.name`
+* `LevelUpAnnouncement.Member.nick`
+* `LevelUpAnnouncement.Member.Guild.icon_url`
+* `LevelUpAnnouncement.Member.Guild.id`
+* `LevelUpAnnouncement.Member.Guild.name`
+
+<div align="left"><sub>EXAMPLE</sub></div>
+
+```py
+from discordLevelingSystem import DiscordLevelingSystem, LevelUpAnnouncement
+
+embed = discord.Embed()
+embed.set_author(name=LevelUpAnnouncement.Member.name, icon_url=LevelUpAnnouncement.Member.avatar_url)
+embed.description = f'Congrats {LevelUpAnnouncement.Member.mention}! You are now level {LevelUpAnnouncement.LEVEL} 😎'
+
+announcement = LevelUpAnnouncement(embed)
+
+lvl = DiscordLevelingSystem(..., level_up_announcement=announcement)
+
+# NOTE: You can have multiple level up announcements by setting the parameter to a sequence of LevelUpAnnouncement
+lvl = DiscordLevelingSystem(..., level_up_announcement=[announcement_1, announcement_2, ...])
+```
+When it comes to `level_up_channel_ids`, you can set a designated channel for each server. If you don't set a level up channel ID for a specific server, the level up message will be sent in the channel where the member leveled up. You don't have to specify a level up channel ID for each server unless you'd like to.
+```py
+johns_bot_commands = 489374746737648734 # text channel ID from server A
+janes_levelup_channel = 58498304930493094 # text channel ID from server B
+
+announcement = LevelUpAnnouncement(..., level_up_channel_ids=[johns_bot_commands, janes_levelup_channel])
+lvl = DiscordLevelingSystem(..., level_up_announcement=announcement)
+```
+---
+## Handling XP
+Method `award_xp` is how members gain XP. This method is placed inside the `on_message` event of your bot. Members will gain XP if they send a message and if they're *not* on cooldown. Spamming messages will not give them XP.
+> NOTE: Members cannot gain XP in DM's
+* Associated methods
+  * `await DiscordLevelingSystem.add_xp(member: Member, amount: int)`
+  * `await DiscordLevelingSystem.remove_xp(member: Member, amount: int)`
+  * `await DiscordLevelingSystem.set_level(member: Member, level: int)`
+  * `await DiscordLevelingSystem.award_xp(*, amount=[15, 25], message: Message, refresh_name=True, **kwargs)`
+
+
+### Parameters for award_xp
+* `amount` (`Union[int, Sequence[int]]`) The amount of XP to award to the member per message. Must be from 1-25. Can be a sequence with a minimum and maximum length of two. If `amount` is a sequence of two integers, it will randomly pick a number in between those numbers including the numbers provided.
+* `message` (`discord.Message`) A discord message object
+* `refresh_name` (`bool`) Everytime the member sends a message, check if their name still matches the name in the database. If it doesn't match, update the database to match their current name. It is suggested to leave this as `True` so the database can always have the most up-to-date record.
+
+### Kwargs for award_xp
+* `bonus` (`DiscordLevelingSystem.Bonus`) Used to set the roles that will be awarded bonus XP.
+  * `class Bonus(role_ids: Sequence[int], bonus_amount: int, multiply: bool)`
+  * **Parameters of the DiscordLevelingSystem.Bonus constructor**
+    * `role_ids` (`Sequence[int]`) The role(s) a member must have to be able to get bonus XP. They only need to have one of these roles to get the bonus
+    * `bonus_amount` (`int`) Amount of extra XP to be awarded
+    * `multiply` (`bool`) If set to `True`, this will operate on a x2, x3 basis. Meaning if you have the awarded XP amount set to 10 and you want the bonus XP role to be awarded 20, it must be set to 2, not 10. If `False`, it operates purely on the given value. Meaning if you have the awarded XP set to 10 and you want the bonus XP role to be awarded 20, it must be set to 10.
+
+<div align="left"><sub>EXAMPLE</sub></div>
+
+```py
+lvl = DiscordLevelingSystem(...)
+
+nitro_booster = 851379776111116329
+associate_role = 851400453904400385
+
+@bot.event
+async def on_message(message):
+    await lvl.award_xp(amount=[15, 25], message=message, bonus=DiscordLevelingSystem.Bonus([nitro_booster, associate_role], 20, multiply=False))
+```
+---
+
+## MemberData
+Accessing the raw information inside the database file can look a bit messy if you don't know exactly what you're looking at. To make things easier, this library comes with the `MemberData` class. A class which returns information about a specific member in the database.
+
+* Associated methods
+  * `await DiscordLevelingSystem.get_data_for(member: Member) -> MemberData`
+  * `await DiscordLevelingSystem.each_member_data(guild: Guild, sort_by=None, limit=None) -> List[MemberData]`
+
+### Attributes
+* `id_number` (`int`) The members ID
+* `name` (`str`) The members name
+* `level` (`int`) The members level
+* `xp` (`int`) The members xp
+* `total_xp` (`int`) The members total xp
+* `rank` (`Optional[int]`) The members rank
+* `mention` (`str`) The discord member mention string
+
+### Methods
+* `MemberData.to_dict() -> dict`
+
+<div align="left"><sub>EXAMPLE</sub></div>
+
+```py
+lvl = DiscordLevelingSystem(...)
+
+@bot.command()
+async def rank(ctx):
+    data = await lvl.get_data_for(ctx.author)
+    await ctx.send(f'You are level {data.level} and your rank is {data.rank}')
+
+@bot.command()
+async def leaderboard(ctx):
+    data = await lvl.each_member_data(ctx.guild, sort_by='rank')
+    # show the leaderboard whichever way you'd like
+```
+---
+## Events
+You can set an event to be called when a member levels up. Using the event is considered as an enhanced `LevelUpAnnouncement` because it provides more capabilities rather than simply sending a message with only text/an embed. The `on_dls_level_up` event takes three parameters:
+* `member` (`discord.Member`) The member that leveled up
+* `message` (`discord.Message`) The message that triggered the level up
+* `data` (`MemberData`) The database information for that member
+
+```py
+bot = commands.Bot(...)
+lvl = DiscordLevelingSystem(..., bot=bot) # your bot instance variable is needed
+
+@bot.event
+async def on_dls_level_up(member: discord.Member, message: discord.Message, data: MemberData):
+    # You can do a lot more here compared to LevelUpAnnouncement
+    # - create a level up image and send it with discord.File
+    # - call additional functions that you may need
+    # - access to all attributes/methods that are available within discord.Member and discord.Message
+```
+> NOTE: `LevelUpAnnouncement` and `on_dls_level_up` are not the same. Level up messages are sent by default by the library. If you'd like to only use `on_dls_level_up`, you need to disable level up announcements (`lvl.announce_level_up = False`)
+
+---
+## Full Example
+With all classes and core methods introduced, here is a basic implementation of this library.
+```py
+from discord.ext import commands
+from discordLevelingSystem import DiscordLevelingSystem, RoleAward, LevelUpAnnouncement
+
+bot = commands.Bot(...)
+
+main_guild_id = 850809412011950121
+
+my_awards = {
+    main_guild_id : [
+        RoleAward(role_id=831672678586777601, level_requirement=1, role_name='Rookie'),
+        RoleAward(role_id=831672730583171073, level_requirement=2, role_name='Associate'),
+        RoleAward(role_id=831672814419050526, level_requirement=3, role_name='Legend')
+    ]
+}
+
+announcement = LevelUpAnnouncement(f'{LevelUpAnnouncement.Member.mention} just leveled up to level {LevelUpAnnouncement.LEVEL} 😎')
+
+# DiscordLevelingSystem.create_database_file(r'C:\Users\Defxult\Documents') database file already created
+lvl = DiscordLevelingSystem(awards=my_awards, level_up_announcement=announcement)
+lvl.connect_to_database_file(r'C:\Users\Defxult\Documents\DiscordLevelingSystem.db')
+
+@bot.event
+async def on_message(message):
+    await lvl.award_xp(amount=15, message=message)
+
+bot.run(...)
+```
+---
+
+## All methods for DiscordLevelingSystem
+<details>
+    <summary>Click to show all methods</summary>
+
+* *await* **add_record**(`guild_id, member_id, member_name, level`) - Manually add a record to the database. If the record already exists (the `guild_id` and `member_id` was found), only the level will be updated. If there were no records that matched those values, all provided information will be added
+  * **Parameters**
+    * **guild_id** (`int`) The guild ID to register
+    * **member_id** (`int`) The member ID to register
+    * **member_name** (`str`) The member name to register
+    * **level** (`int`) The member level to register. Must be from 0-100
+  * **Raises**
+    * `DiscordLevelingSystemError` - The value given from a parameter was not of the correct type or "level" was not 0-100
+
+
+* *await* **add_xp**(`member, amount`) - Give XP to a member. This also changes their level so it matches the associated XP
+  * **Parameters**
+    * **member** (`discord.Member`) The member to give XP to
+    * **amount** (`int`) Amount of XP to give to the member
+  * **Raises**
+    * `DatabaseFileNotFound` - The database file was not found
+    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
+    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
+    * `NotConnected` - Attempted to use a method that requires a connection to a database file
+    * `DiscordLevelingSystemError` - Parameter "amount" was less than or equal to zero. The minimum value is 1 
+
+
+* *await* **award_xp**(`*, amount = [15, 25], message, refresh_name = True, **kwargs`) - Give XP to the member that sent a message
+  * **Parameters**
+    * **amount** (`Union[int, Sequence[int]]`)
+    * **message** (`discord.Message`) A message object
+    * **refresh_name** (`bool`) Everytime the member sends a message, check if their name still matches the name in the database. If it doesn't match, update the database to match their current name. It is suggested to leave this as `True` so the database can always have the most up-to-date record
+  * **Kwargs**
+    * **bonus** (`DiscordLevelingSystem.Bonus`) Set the bonus values. Read the `DiscordLevelingSystem.Bonus` doc string for more details (defaults to `None`)
+  * **Raises**
+    * `DatabaseFileNotFound` - The database file was not found
+    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
+    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
+    * `NotConnected` - Attempted to use a method that requires a connection to a database file
+
+
+* **backup_database_file**(`path, with_timestamp = False`) - Create a copy of the database file to the specified path. If a copy of the backup file is already in the specified path it will be overwritten
+  * **Parameters**
+    * **path** (`str`) The path to copy the database file to
+    * **with_timestamp** (`bool`) Creates a unique file name that has the date and time of when the backup file was created. This is useful when you want multiple backup files
+  * **Raises**
+    * `DiscordLevelingSystemError` - Path doesn't exist or points to another file
+    * `NotConnected` - Attempted to use a method that requires a connection to a database file
+
+
+* *await* **change_cooldown**(`rate, per`) - Update the cooldown rate
+  * **Parameters**
+    * **rate** (`int`) The amount of messages each member can send before the cooldown triggers
+    * **per** (`float`) The amount of seconds each member has to wait before gaining more XP, aka the cooldown
+  * **Raises**
+    * `DatabaseFileNotFound` - The database file was not found
+    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
+    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
+    * `NotConnected` - Attempted to use a method that requires a connection to a database file
+    * `DiscordLevelingSystemError` - The rate or per value was not greater than zero
+
+
+* *await* **clean_database**(`guild`) - Removes the data for members that are no longer in the guild, thus reducing the database file size. It is recommended to have this method in a background loop in order to keep the database file free of records that are no longer in use
+  * **Parameters**
+    * **guild** (`discord.Guild`) The guild records to clean
+  * **Returns**
+    * (`Optional[int]`) The amount of records that were removed from the database
+  * **Raises**
+    * `DatabaseFileNotFound` - The database file was not found
+    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
+    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
+    * `NotConnected` - Attempted to use a method that requires a connection to a database file
+
+
+* **connect_to_database_file**(`path`) - Connect to the existing database file in the specified path
+  * **Parameters**
+    * **path** (`str`) The location of the database file
+  * **Raises**
+    * `ConnectionFailure` - Attempted to connect to the database file when the event loop is already running
+    * `DatabaseFileNotFound` - The database file was not found
+
+
+* *static method* **create_database_file**(`path = None`) - Create the database file and implement the SQL data for the database
+  * **Parameters**
+    * **path** (`Optional[str]`) The location to create the database file. If `None`, the file is created in the current working directory
+  * **Raises**
+    * `ConnectionFailure` - Attempted to create the database file when the event loop is already running
+    * `DiscordLevelingSystemError` - The path does not exist or the path points to a file instead of a directory
+
+
+* *await* **each_member_data**(`guild, sort_by = None, limit = None`) - Return each member in the database as a `MemberData` object for easy access to their XP, level, etc. You can sort the data with `sort_by` with the below values
+  * **Parameters**
+    * **guild** (`discord.Guild`) A guild object
+    * **sort_by** (`Optional[str]`) Return each member sorted by: "name", "level", "xp", "rank". If `None`, it will return in the order they were added to the database
+    * **limit** (`Optional[int]`) Restrict the amount of records returned to the specified amount
+  * **Returns**
+    * `List[MemberData]`
+  * **Raises**
+    * `DatabaseFileNotFound` - The database file was not found
+    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
+    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
+    * `NotConnected` - Attempted to use a method that requires a connection to a database file
+    * `DiscordLevelingSystemError` - The value of `sort_by` was not recognized or `guild` was not of type `discord.Guild`
+
+
+* *await* **export_as_json**(`path, guild`) - Export a json file that represents the database to the path specified
+  * **Parameters**
+    * **path** (`str`) Path to copy the json file to
+    * **guild** (`discord.Guild`) The guild for which the data should be extracted from. If `None`, all guild information will be extracted from the database
+  * **Raises**
+    * `DatabaseFileNotFound` - The database file was not found
+    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
+    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
+    * `NotConnected` - Attempted to use a method that requires a connection to a database file
+    * `DiscordLevelingSystemError` - The path does not exist or does not point to a directory
+
+
+* **get_awards**(`guild = None`) - Get all `RoleAward`'s or only the `RoleAward`'s assigned to the specified guild
+  * **Parameters**
+    * **guild** (`Optional[Union[discord.Guild, int]]`) A guild object or a guild ID
+  * **Returns**
+    * (`Union[Dict[int, List[RoleAward]], List[RoleAward]]`) If `guild` is `None`, this return the awards `dict` that was set in constructor. If `guild` is specified, it returns a List[`RoleAward`] that matches the specified guild ID. Can also return `None` if awards were never set or if the awards for the specified guild was not found
+
+
+* *await* **get_data_for**(`member`) - Get the `MemberData` object that represents the specified member
+  * **Parameters**
+    * **member** (`discord.Member`) The member to get the data for
+  * **Returns**
+    * (`MemberData`) Can be `None` if the member isn't in the database
+  * **Raises**
+    * `DatabaseFileNotFound` - The database file was not found
+    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
+    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
+    * `NotConnected` - Attempted to use a method that requires a connection to a database file
+
+
+* *await* **get_level_for**(`member`) - Get the level for the specified member
+  * **Parameters**
+    * **member** (`discord.Member`) Member to get the level for
+  * **Returns**
+    * (`int`) Can be `None` if the member isn't in the database
+  * **Raises**
+    * `DatabaseFileNotFound` - The database file was not found
+    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
+    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
+    * `NotConnected` - Attempted to use a method that requires a connection to a database file
+
+
+* *await* **get_rank_for**(`member`) - Get the rank for the specified member
+  * **Parameters**
+    * **member** (`discord.Member`) Member to get the rank for
+  * **Returns**
+    * (`int`) Can be `None` if the member isn't ranked yet
+  * **Raises**
+    * `DatabaseFileNotFound` - The database file was not found
+    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
+    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
+    * `NotConnected` - Attempted to use a method that requires a connection to a database file
+
+
+* *await* **get_record_count**(`guild = None`) - Get the amount of members that are registered in the database. If `guild` is set to `None`, ALL members in the database will be counted
+  * **Parameters**
+    * **guild** (`Optional[discord.Guild]`) The guild for which to count the amount of records
+  * **Returns**
+    * (`int`)
+  * **Raises**
+    * `DatabaseFileNotFound` - The database file was not found
+    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
+    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
+    * `NotConnected` - Attempted to use a method that requires a connection to a database file
+
+
+* *await* **get_total_xp_for**(`member`) - Get the total XP for the specified member
+  * **Parameters**
+    * **member** (`discord.Member`) Member to get the total XP for
+  * **Returns**
+    * (`int`) Can be `None` if the member isn't in the database
+  * **Raises**
+    * `DatabaseFileNotFound` - The database file was not found
+    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
+    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
+    * `NotConnected` - Attempted to use a method that requires a connection to a database file
+
+
+* *await* **get_xp_for**(`member`) - Get the XP for the specified member
+  * **Parameters**
+    * **member** (`discord.Member`) Member to get the XP for
+  * **Returns**
+    * (`int`) Can be `None` if the member isn't in the database
+  * **Raises**
+    * `DatabaseFileNotFound` - The database file was not found
+    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
+    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
+    * `NotConnected` - Attempted to use a method that requires a connection to a database file
+
+
+* *static method* **get_xp_for_level**(`level`) - Returns the total amount of XP needed for the specified level. Levels go from 0-100
+  * **Parameters**
+    * **level** (`int`) The level XP information to retrieve
+  * **Returns**
+    * (`int`)
+  * **Raises**
+    * `DiscordLevelingSystemError` - The level specified does not exist
+
+
+* *await* **insert**(`bot, guild_id, users, using, overwrite = False, show_results = True`) - Insert the records from your own leveling system into the library. A lot of leveling system tutorials out there use json files to store information. Although it might work, it is insufficient because json files are not made to act as a database. Using an actual database file has many benefits over a json file
+  * **Parameters**
+    * **bot** (`Union[discord.ext.commands.Bot, discord.ext.commands.AutoShardedBot]`) Your bot instance variable
+    * **guild_id** (`int`) ID of the guild that you used your leveling system with
+    * **users** (`Dict[int, int]`) This is the information that will be added to the database. The keys are user ID's, and the values are the users total XP or level. Note: This library only uses levels 0-100 and XP 0-1899250. If any number in this dict are over the levels/XP threshold, it is implicitly set back to this libraries maximum value
+    * **using** (`str`) What structure your leveling system used. Options: "xp" or "levels". Some leveling systems give users only XP and they are ranked up based on that XP value. Others use a combination of levels and XP. If all the values in the `users` dict are based on XP, set this to "xp". If they are based on a users level, set this to "levels"
+    * **overwrite** (`bool`) If a user you've specified in the `users` dict already has a record in the database, overwrite their current record with the one your inserting
+    * **show_results** (`bool`) Print the results for how many of the `users` were successfully added to the database file. If any are unsuccessful, their ID along with the value you provided will also be shown
+  * **Raises**
+      * `DiscordLevelingSystemError` - The value given from a parameter was not of the correct type. The `users` dict was empty. Or your bot is not in the guild associated with `guild_id`       
+
+
+* *await* **is_in_database**(`member, guild = None`) - A quick check to see if a member is in the database. This is not guild specific although it can be if `guild` is specified
+  * **Parameters**
+    * **member** (`Union[discord.Member, int]`) The member to check for. Can be the member object or that members ID
+    * **guild** (`Optional[discord.Guild]`) The guild to check if the member is registered in
+  * **Returns**
+    * (`bool`)
+  * **Raises**
+    * `DatabaseFileNotFound` - The database file was not found
+    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
+    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
+    * `NotConnected` - Attempted to use a method that requires a connection to a database file
+    * `DiscordLevelingSystemError` - Parameter `member` was not of type `discord.Member` or `int`
+
+
+* *static method* **levels_and_xp**( ) -  Get the raw `dict` representation for the amount of levels/XP in the system. The keys in the `dict` returned is each level, and the values are the amount of XP needed to be awarded that level
+  * **Returns**
+    * (`Dict[str, int]`)
+
+
+* *await* **next_level**(`member`) - Get the next level for the specified member
+  * **Parameters**
+    * **member** (`discord.Member`) Member to get the next level for
+  * **Returns**
+    * (`int`) If the member is currently max level (100), it will return 100. This can also return `None` if the member is not in the database
+  * **Raises**
+    * `DatabaseFileNotFound` - The database file was not found
+    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
+    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
+    * `NotConnected` - Attempted to use a method that requires a connection to a database file
+
+
+* *await* **next_level_up**(`member`) - Get the amount of XP needed for the specified member to level up
+  * **Parameters**
+    * **member** (`discord.Member`) Member to get the amount of XP needed for a level up
+  * **Returns**
+    * (`int`) Returns 0 if the member is currently at max level. Can return `None` if the member is not in the database.
+  * **Raises**
+    * `DatabaseFileNotFound` - The database file was not found
+    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
+    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
+    * `NotConnected` - Attempted to use a method that requires a connection to a database file
+
+
+* *await* **raw_database_contents**(`guild = None`) - Returns everything in the database. Can specify which guild information will be extracted
+  * **Parameters**
+    * **guild** (`Optional[discord.Guild]`) The guild to extract the raw database contents from. If `None`, information about all guilds will be extracted
+  * **Returns**
+    * `List[Tuple[int, int, str, int, int, int]]` The tuples inside the list represents each row of the database:
+      * Index 0 is the guild ID
+      * Index 1 is their ID
+      * Index 2 is their name
+      * Index 3 is their level
+      * Index 4 is their XP
+      * Index 5 is their total xp
+      * Can be an empty list if nothing is in the database
+  * **Raises**
+    * `DatabaseFileNotFound` - The database file was not found
+    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
+    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
+    * `NotConnected` - Attempted to use a method that requires a connection to a database file
+
+
+* *await* **refresh_names**(`guild`) - Update names inside the database. This does not add anything new. It simply verifies if the name in the database matches their current name, and if they don't match, update the database name
+  * **Parameters**
+    * **guild** (`discord.Guild`) A guild object
+  * **Returns**
+    * `(Optional[int])` The amount of records in the database that were updated
+  * **Raises**
+    * `DatabaseFileNotFound` - The database file was not found
+    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
+    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
+    * `NotConnected` - Attempted to use a method that requires a connection to a database file
+
+
+* *await* **remove_from_database**(`member, guild = None`) - Remove a member from the database. This is not guild specific although it can be if `guild` is specified
+  * **Parameters**
+    * **member** (`Union[discord.Member, int]`) The member to remove. Can be the member object or that members ID
+    * **guild** (`Optional[discord.Guild]`) If this parameter is given, it will remove the record of the specified member only from the specified guild record. If `None`, it will remove all records no matter the guild
+  * **Returns**
+    * (`Optional[bool]`) Returns `True` if the member was successfully removed from the database. `False` if the member was not in the database so there was nothing to remove
+  * **Raises**
+      * `DatabaseFileNotFound` - The database file was not found
+      * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
+      * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
+      * `DiscordLevelingSystemError` - Parameter `member` was not of type `discord.Member` or `int`
+      * `NotConnected` - Attempted to use a method that requires a connection to a database file
+
+
+* *await* **remove_xp**(`member, amount`) - Remove XP from a member. This also changes their level so it matches the associated XP
+  * **Parameters**
+      * **member** (`discord.Member`) The member to remove XP from
+      * **amount** (`int`) Amount of XP to remove from the member
+  * **Raises**
+    * `DatabaseFileNotFound` - The database file was not found
+    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
+    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
+    * `NotConnected` - Attempted to use a method that requires a connection to a database file
+    * `DiscordLevelingSystemError` - Parameter "amount" was less than or equal to zero. The minimum value is 1
+
+
+* *await* **reset_everyone**(`guild, *, intentional = False`) - Sets EVERYONES XP, total XP, and level to zero in the database. Can specify which guild to reset
+  * **Parameters**
+      * **guild** (`Union[discord.Guild, None]`) The guild for which everyone will be reset. If this is set to `None`, everyone in the entire database will be reset
+      * **intentional** (`bool`) A simple kwarg to try and ensure that this action is indeed what you want to do. Once executed, this cannot be undone
+  * **Raises**
+    * `DatabaseFileNotFound` - The database file was not found
+    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
+    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
+    * `NotConnected` - Attempted to use a method that requires a connection to a database file
+    * `FailSafe` - "intentional" argument for this method was set to `False` in case you called this method by mistake
+
+
+* *await* **reset_member**(`member`) - Sets the members XP, total XP, and level to zero
+  * **Parameters**
+    * **member** (`discord.Member`) The member to reset
+  * **Raises**
+    * `DatabaseFileNotFound` The database file was not found
+    * `LeaderboardNotFound` Table "leaderboard" in the database file is missing
+    * `ImproperLeaderboard` Leaderboard table was altered. Components changed or deleted
+    * `NotConnected` Attempted to use a method that requires a connection to a database file
+
+
+* *await* **set_level**(`member, level`) - Sets the level for the member. This also changes their total XP so it matches the associated level
+  * **Parameters**
+    * **member** (`discord.Member`) The member who's level will be set
+    * **level** (`int`) Level to set. Must be from 0-100     
+  * **Raises**
+    * `DatabaseFileNotFound` - The database file was not found
+    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
+    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
+    * `NotConnected` - Attempted to use a method that requires a connection to a database file
+    * `DiscordLevelingSystemError` - Parameter "level" was not from 0-100
+
+
+* *await* **sql_query_get**(`sql, parameters = None, fetch = 'ALL'`) - Query and return something from the database using SQL. The following columns are apart of the "leaderboard" table: guild_id, member_id, member_name, member_level, member_xp, member_total_xp
+  * **Parameters**
+    * **sql** (`str`) SQL string used to query the database
+    * **parameters** (`Optional[Tuple[Union[str ,int]]]`) The parameters used for the database query
+    * **fetch** (`Union[str, int]`) The amount of rows you would like back from the query. Options: 'ALL', 'ONE', or an integer value that is greater than zero
+  * **Returns**
+    * (`Union[List[tuple], tuple]`)
+      * Using `fetch='ALL'` returns `List[tuple]`
+      * Using `fetch='ONE'` returns `tuple`
+      * Using `fetch=4` returns `List[tuple]` with only four values
+      * Can also return an empty list if the query was valid but got nothing from it
+  * **Raises**
+    * `DatabaseFileNotFound` - The database file was not found
+    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
+    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
+    * `NotConnected` - Attempted to use a method that requires a connection to a database file
+    * `DiscordLevelingSystemError` - Argument "fetch" was the wrong type or used an invalid value
+    * `aiosqlite.Error` - Base aiosqlite error. Multiple errors can arise from this if the SQL query was invalid
+
+
+* *await* **switch_connection**(`path`) - Connect to a different leveling system database file
+  * **Parameters**
+    * **path** (`str`) The location of the database file
+  * **Raises**
+    * `DatabaseFileNotFound` - The database file was not found
+
+
+* *static method* **transfer**(`old, new, guild_id`) - Transfer the database records from a database file created from v0.0.1 to a blank database file created using v0.0.2+. If you were already using a v0.0.2+ database file, there's no need to use this method
+  * **Parameters**
+    * **old** (`str`) The path of the v0.0.1 database file
+    * **new** (`str`) The path of the v0.0.2+ database file
+    * **guild_id** (`int`) ID of the guild that was originally used with this library
+  * **Raises**
+    - `ConnectionFailure` - The event loop is already running
+    - `DatabaseFileNotFound` - "old" or "new" database file was not found
+    - `DiscordLevelingSystemError` - One of the databases is missing the "leaderboard" table. A v0.0.2+ database file contains records, or there was an attempt to transfer records from a v0.0.2+ file to another v0.0.2+ file
+
+
+* *await* **wipe_database**(`guild = None, *, intentional = False`) - Delete EVERYTHING from the database. If `guild` is specified, only the information related to that guild will be deleted
+  * **Parameters**
+    * **guild** (`Optional[discord.Guild]`) The guild for which all information that is related to that guild will be deleted. If `None`, everything will be deleted
+    * **intentional** (`bool`) A simple kwarg to try and ensure that this action is indeed what you want to do. Once executed, this cannot be undone
+  * **Raises**
+    * `DatabaseFileNotFound` - The database file was not found
+    * `LeaderboardNotFound` - Table "leaderboard" in the database file is missing
+    * `ImproperLeaderboard` - Leaderboard table was altered. Components changed or deleted
+    * `NotConnected` - Attempted to use a method that requires a connection to a database file
+    * `FailSafe` - "intentional" argument for this method was set to `False` in case you called this method by mistake
+
+</details>
+
+## Migrating from v0.0.1 to v0.0.2+
+<details>
+    <summary>Click to show details</summary>
+
+This library was not originally designed with the use of multiple servers in mind, so all the data you might have currently (your database file was created in `v0.0.1`) should be from a single server. With `v0.0.2`, the structure of the database file was changed to accommodate this fix. That means if you are currently using a `v0.0.1` database file and update to `v0.0.2+`, a vast majority of the library will be broken. To avoid this, you need to transfer all your `v0.0.1` database file records to a `v0.0.2+` database file. This can be done using the `transfer` method.
+
+* Associated static method
+  * `DiscordLevelingSystem.transfer(old: str, new: str, guild_id: int)`
+
+### Parameters
+* `old` (`str`) The path of the `v0.0.1` database file
+* `new` (`str`) The path of the `v0.0.2+` database file (a brand new file from using `DiscordLevelingSystem.create_database_file(path: str)`)
+* `guild_id` (`int`) ID of the guild that was originally used with this library
+
+<div align="left"><sub>EXAMPLE</sub></div>
+
+```py
+from discordLevelingSystem import DiscordLevelingSystem
+
+old = r'C:\Users\Defxult\Documents\DiscordLevelingSystem.db'
+new = r'C:\Users\Defxult\Desktop\DiscordLevelingSystem.db'
+
+DiscordLevelingSystem.transfer(old, new, guild_id=850809412011950121)
+```
+
+</details>
+
+## Inserting your own leveling system information
+<details>
+    <summary>Click to show details</summary>
+
+Insert the records from your leveling system into this one. A lot of leveling system tutorials out there use json files to store information. Although it might work, it is insufficient because json files are not made to act as a database. Using a database file has many benefits over a json file. If you previously watched a tutorial for your leveling system and would like to import your records over to use with this library, you can do so with the below method.
+
+* Associated static method
+  * `await DiscordLevelingSystem.insert(bot: Union[Bot, AutoShardedBot], guild_id: int, users: Dict[int, int], using: str, overwrite=False, show_results=True)`
+
+### Parameters
+- `bot` (`Union[discord.ext.commands.Bot, discord.ext.commands.AutoShardedBot]`) Your bot instance variable
+
+- `guild_id` (`int`) ID of the guild that you used your leveling system with
+
+- `users` (`Dict[int, int]`) This is the information that will be added to the database. The keys are user ID's, and the values are the users total XP or level. Note: This library only uses levels 0-100 and XP 0-1899250. If any number in this dict are over the levels/XP threshold, it is implicitly set back to this libraries maximum value
+
+- `using` (`str`) What structure your leveling system used. Options: "xp" or "levels". Some leveling systems give users only XP and they are ranked up based on that XP value. Others use a combination of levels and XP. If all the values in the `users` dict are based on XP, set this to "xp". If they are based on a users level, set this to "levels"
+
+- `overwrite` (`bool`) If a user you've specified in the `users` dict already has a record in the database, overwrite their current record with the one your inserting
+
+- `show_results` (`bool`) Print the results for how many of the `users` were successfully added to the database file. If any are unsuccessful, their ID along with the value you provided will also be shown
+
+> NOTE: If the users you've provided in the `users` dict is not currently in the guild (`guild_id`), their information will not be inserted. If you'd like, you can manually add those records with method `DiscordLevelingSystem.add_record()`, but that is discouraged because it is better to discard information that is no longer in use (the user is no longer in the guild)
+
+<div align="left"><sub>EXAMPLE</sub></div>
+
+```py
+# leveling_system.json
+[
+  {
+      "5748392849348934" : {
+          "xp" : 373,
+          "level" : 4
+      }
+  },
+  {
+      "89283659820948923" : {
+          "xp" : 23,
+          "level" : 1
+      }
+  }
+]
+
+
+# bot.py
+import json
+from discord.ext import commands
+from discordLevelingSystem import DiscordLevelingSystem
+
+bot = commands.Bot(...)
+
+lvl = DiscordLevelingSystem(...)
+lvl.connect_to_database_file(...)
+
+def json_to_dict() -> dict:
+    with open('leveling_system.json') as fp:
+        data = json.load(fp)
+        formatted: Dict[int, int] = ... # format the data so all keys and values are associated with the user ID and level
+        
+        """
+        In the end, the formatted dict should look like so:
+        
+        formatted = {
+            5748392849348934 : 4,
+            89283659820948923 : 1
+        }
+        """
+        return formatted
+
+@bot.command()
+async def insert(ctx):
+    await lvl.insert(ctx.bot, guild_id=12345678901234, users=json_to_dict(), using='levels')
+
+bot.run(...)
+```
+
+</details>
```

### Comparing `discordLevelingSystem-1.2.0/discordLevelingSystem.egg-info/SOURCES.txt` & `discordLevelingSystem-1.2.1/discordLevelingSystem.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 LICENSE
 README.md
+pyproject.toml
 setup.py
 discordLevelingSystem/__init__.py
 discordLevelingSystem/announcement.py
 discordLevelingSystem/decorators.py
 discordLevelingSystem/errors.py
 discordLevelingSystem/leveling_system.py
 discordLevelingSystem/levels_xp_needed.py
```

