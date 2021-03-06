<img src="https://raw.githubusercontent.com/zekroTJA/DiscordBot/master/.websrc/logo%20-%20title.png" />
<br/>

[![GitHub release](https://img.shields.io/github/release/zekrotja/DiscordBot.svg)](https://github.com/zekroTJA/DiscordBot/releases)&nbsp;
[![GitHub (pre-)release](https://img.shields.io/github/release/zekrotja/DiscordBot/all.svg)](https://github.com/zekroTJA/DiscordBot/releases)&nbsp;
<a href="https://discordapp.com/oauth2/authorize?client_id=272336949841362944&scope=bot&permissions=1882582134">
<img src="https://img.shields.io/badge/currently%20running%20on-1.40.1.0-3cd0d8.svg"></a><br>

-----

If you want to use the code of this project for your own ones, please read **[this](http://s.zekro.de/codepolicy)** before!

So you have some questions or want to join my developer community discord? Take a look! :^)
<br/><a href="http://discord.zekro.de"><img src="https://discordapp.com/api/guilds/307084334198816769/embed.png"/></a>

-----
### Get it!
<a href="https://discordapp.com/oauth2/authorize?client_id=272336949841362944&scope=bot&permissions=1882582134"><img src="https://github.com/zekroTJA/DiscordBot/blob/master/.websrc/add_to_discord.png?raw=true" width="300"/></a>

---
### Donate

Not long ago, I've moved the host of the bot from my Raspberry Pi to a VPS, wich costs around €20 per year. This bot will be still completely free to use, but I would really appreciate it if you could help a a bit to finance the server for the bot :) <3

<a href="https://support.zekro.de"><img src="https://github.com/zekroTJA/DiscordBot/blob/master/.websrc/donate.png" width="300"/></a>

🏆 Goal *(this year payment cicle)*  **`$9 / $24`**

**List of donators**<br>
Sydrus (Patreon)  -  $9

-----
### Features

```
Here are just listed some of the various functions and >64 commands of the bot.
```
**Here you can find a full list of commands:**<br><br>
<a href="https://docs.google.com/spreadsheets/d/1vDsZgn49s6D1OCfyJE0aAixgbMfHb1n6ybHPG8g2Ing/edit?usp=sharing" target="_blank"><img src="https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/1033926355/original/GoogleSheets.png" width="150"/></a><br><br>

- **Fun / Chat commands**
  - `-8ball` - typical 8ball yes/no generator
  - `-cat` - send cute cat pictures (also with a spam function to send them in time periods)
  - `-clear` - typical clear command to clear messages
  - `-joke` - throw a yomama joke :^)
  - `-quote` - quote messages from channels on the guild<br>
  &nbsp;![](https://image.prntscr.com/image/g3-ctAYBSlu1eS9qoFTSSQ.png)
  - `-stups` - nudge someone on the guild
  - `-vote` - create polls<br>
  &nbsp;![](https://image.prntscr.com/image/5_avzZNQRUijY2rUgc1XgQ.png)
  
  
- **Server administration**
  - `-kick` - kick someone from the server
  - `-vkick` - kick someone out of the voice channel, also for a specific time period
  - `-mute` - mute members in text channels
  - `-blacklist` - disallow users to use the bot
  
- **Other functions**
  - `-music` - Music player with many functions
  - `-scpacer` - Create spacer voice channels wich can not be joined
  - `-rand6` - Random operators for rainbow six<br>
  &nbsp;![](https://image.prntscr.com/image/WHZh5l76TKupvWUmoIQBpA.png)

-----
### Installation

Just download the latest version from **[Releases](https://github.com/zekroTJA/DiscordBot/releases)** and save it somewhere on your pc or server.

First start the JAR file with:
```bash
java -jar DiscordBot.jar
```
The bot will create a `SETTINGS.txt` file. Open it and enter your settings.
The most important is to set first the API token you'll get from [this page](https://discordapp.com/developers/applications/me) *(if you just created an bot account there).* Also its realy important to set yout Discord account ID as `BOT_OWNER_ID`! You can get your client id by right-clicking on your name in discord and select `Copy ID` *(for that, you need to enable developer mode in Discord!)*
![img](https://image.prntscr.com/image/Jmf2FssPSdKEb9jNOTra-g.png)
![img](https://image.prntscr.com/image/UrxT_eI7SbqmZIcbQs1QvQ.png)

Then restart the bot with
```bash
java -jar DiscordBot.jar
```

If you are running the bot on a Linux server via SSH, use **[screen](https://wiki.ubuntuusers.de/Screen/)** to run the bot as background process:
```bash
$ sudo screen -L -S zekroBot sudo java -jar DiscordBot.jar
```
*(`-L` generates a logfile `screenlog.0` and `-S zekroBot` set a name to the screen so you can reopen the screen with `sudo screen -r zekroBot`)*

You also can create a bash file like this to start (and restart) the bot:
```bash
# resume running screen (if there is a screen running) to stop it with [STRG] + [C]
sudo screen -r zekroBot
# cd to bot JAR location (enter YOUR path there)
cd Programs/zekroBot
# start the bot in screen
sudo screen -L -S zekroBot sudo java -jar DiscordBot.jar
```

After that, use the guild settings commands to configure the bot for your guild(s)
![img](https://image.prntscr.com/image/VKw6mpxPS8in40ZB4sTOMQ.png)

-----
### Latest Changelogs

**PLEASE LOOK IN <a href="https://github.com/zekroTJA/DiscordBot/releases">RELEASES</a> TO SEE LATEST CHANGE LOGS.**

-----
### Future Intends

**SEE CURRENT TODO-LIST <a href="https://docs.google.com/spreadsheets/d/e/2PACX-1vTPfpbg5fEssYD-X4XaR5ISM_xXrOEoqKnoWO7kUkVVBFARxtf49u4wKfUe0L-tkN2AoNffhebZJ-5R/pubhtml">HERE</a>**

-----
### Used libraries

- <a href="https://github.com/DV8FromTheWorld/JDA">JDA</a>
- <a href="https://github.com/mwanji/toml4j">Toml4j</a>
- <a href="https://github.com/sedmelluq/lavaplayer">lavaplayer</a>
- <a href="https://github.com/koraktor/steam-condenser-java">steam-condenser</a>
- <a href="https://github.com/bertrandmartel/speed-test-lib">JSpeedTest</a>
- <a href="https://github.com/brunocvcunha/jiphy">jiphy</a>

-----
### Mentions
Special thanks to <a href="https://github.com/jagrosh">@jagrosh</a> for helping me with fixing the combatibility bug of lava player on linux system.

Also a special thanks to Sophie, who helped me a lot developing some features of that bot and better performance coding. <3

Another lovely thanks to all of our "Trupp Lätzl"-Discord members and team for testing the bot and using it and also a special lovley thanks to all members on my Dev Discord helping me a lot with new experiences and a lot of helpful hints. :)
