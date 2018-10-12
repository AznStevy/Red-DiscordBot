# owo - An osu! Discord bot
[<img src="https://discordapp.com/api/guilds/290312423309705218/widget.png?style=shield">](https://discord.gg/aNKde73)

**This code no longer works due to the game's website changing + other small changes, so I've decided to stop updating it. The bot (v3) is currently being rewritten (with better code practices... now that I know, whoops) and will no longer follow the Redbot structure (v2 or v3). Please keep this in mind as you contemplate wasting 3+ hours trying to get this code to work. If you want to see what new stuff v3 might offer, click that fancy button-looking thing above to join the owo dev server. Cheers!**

This is [owo](http://owobot.xyz/), an instance of Red, an open source Discord bot created by [Twentysix](https://github.com/Twentysix26/Red-DiscordBot) and modified by Stevy for the specific purpose of Osu!.

Key Features include:
- User profiles
- Top/Recent plays
- Score tracking
- Map detection and pp calculation
- Screenshot detection
- Standard map recommendations

You can add the bot using this [link](https://discordapp.com/oauth2/authorize?client_id=289066747443675143&scope=bot&permissions=305187840) or join the owo server [here](https://discord.gg/aNKde73).

If you would like to run your own instance of owo because tracking is getting too slow or some other reason, please follow the instructions provided by [Twentysix](https://twentysix26.github.io/Red-Docs/) and others on how to install a Redbot for your system. Then, getting this to work should make more sense. If you're having issues with `leveler.py` and/or `osu.py`, be sure you read up on [my cog repo](https://github.com/AznStevy/Maybe-Useful-Cogs) on how to install those two cogs. Have fun! If you have questions/need help, ask in the [owo! Official](https://discord.gg/aNKde73) server.

Command List:

| Command | Description |
| --- | --- |
| `osu [username1] [username2]... (option)` | Shows osu! Standard profile; options: `-ripple/-official` `-d`|
| `taiko [username1] [username2]... (option)` | Shows taiko profile; options: `-ripple/-official` `-d`|
| `ctb [username1] [username2]... (option)` | Shows ctb profile; options: `-ripple/-official` `-d`|
| `mania [username1] [username2]... (option)` | Shows mania profile; options: `-ripple/-official` `-d`|
| `osutop [username] (options)` | Shows top 5 osu! Standard plays for a certain player; options: `-p [top play number = 1-100]` `-ripple/-official` `-r` `-g`|
| `taikotop [username] (options)` | Shows top 5 taiko plays for a certain player; options: `-p [top play number = 1-100]` `-ripple/-official` `-r` `-g`|
| `ctbtop [username] (options)` | Shows top 5 ctb plays for a certain player; options: `-p [top play number = 1-100]` `-ripple/-official` `-r` `-g`|
| `maniatop [username] (options)` | Shows top 5 mania plays for a certain player; options: `-p [top play number = 1-100]` `-ripple/-official` `-r` `-g`|
| `recent [username] (options)` | Gets the recent play of player according to their default gamemode; options: `[gamemode = osu|taiko|ctb|mania]`|
| --- | --- |
| `osuset` | Shows General Commands for Setting Information in the Module |
| `osuset api [official/ripple]` | Set the default api to use for the server for the commands above |
| `osuset default [0/1/2/3]` | Set a users default gamemode to use for recent command |
| `osuset displaytop [#]` | Set # of best plays being displayed in top command  |
| `osuset key osu [key]` | Set osu api key **Must do this first for anything to work!** You can get one here: https://osu.ppy.sh/p/api|
| `osuset key puush [key]` | Set puush api key. You can get a key here: https://puush.me/|
| `osuset tracking [enable/disable]` | Disable/Enable tracking on server |
| `osuset user [username]` | Links username to discord account |
| --- | --- |
| `osutrack` | Shows General Commands for Player Tracking |
| `overview` | Shows stats of player tracking |
| `osutrack add [username1] [username2]... (options)` | Adds a player to tracking (can edit/don't have to remove first); options: `-m [gamemode = 0123]` `-t [track number = 1-100]` `-r [recent modes = 0123]`\*|
| `osutrack clear` | Removes all players from tracking in the server |
| `osutrack list` | Lists all people tracked in server + modes/# of plays |
| `osutrack remove [username1] [username2]...` | Removes a player from tracking |
| --- | --- |
| `recommend (options)` | Standard map recommendations; options: `any/nomod/(mod combo)` `pp target`|
| --- | --- |
| `options` | Shows Server Toggles (Mostly for passive detection) |
| `options beatmap` | Toggles beatmap url detection |
| `options beatmapgraph` | Toggles beatmap graph |
| `options screenshot` | Toggles screenshot detection |
| `options ssgraph` | Toggles screenshot detection graph |
\* Work in progress (see branch for recent tracking)
