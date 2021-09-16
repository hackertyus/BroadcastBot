# 𝘽𝙧𝙤𝙖𝙙𝙘𝙖𝙨𝙩 𝘽𝙤𝙩
A simple Telegram bot that can broadcast messages and media to the bot subscribers using [MongoDB](https://mongodb.com).

[![Readme Card](https://github-readme-stats.vercel.app/api/pin/?username=NACBots&repo=BroadcastBot&theme=flag-india)](https://github.com/nacbots/broadcastbot)

## Features
 - Support [mongodb.com](https://mongodb.com) database 📁 for user's record 📹.<p align="center">
 - User's can choose whether to enable Broadcast messages or not using `/settings` commands.
 - Logs New User's in any channel.
 - Get total user's count in Database. 
 - Ban and UnBan any user.

## Required Configs
 - `BOT_TOKEN` - Get from [@BotFather](https://t.me/BotFather)
 - `API_ID` - Get it from [telegram.org](https://my.telegram.org/auth)
 - `API_HASH` - Get it from [telegram.org](https://my.telegram.org/auth)
 - `AUTH_USERS` - Authorised user's ID to use [Admin Commands](https://github.com/nacbots/broadcastbot#admin-commands) {Split 💔 with a space}.
 - `DB_URL` - MongoDB Database URI get it from [mongodb.com](https://mongodb.com)
	- This for Saving UserIDs. When you will Broadcast, bot will forward the Broadcast to DB Users.

## Optional Configs
 - `LOG_CHANNEL` - Log Channel ID to get new user notifications.
	- This for some getting user info. If any new User added to DB, Bot will send Log to that Logs Channel. You can use same DB Channel ID.
 - `BROADCAST_AS_COPY` - Value should be `True` or `False`.
	- If `True` broadcast messages will be forwarder *As Copy*. If `False` broadcast messages will be forwarded with Forward Tag.
 - `DB_NAME` - [mongodb.com](https://mongodb.com) Collection name to be used.

## User's Commands 😉

```
start - Start the bot 🥲
settings - Customise settings
```

## Admin Commands 🤫

```
stats - Total User Number in Database
broadcast - Reply to Message to Broadcast
ban_user - Ban A User with time & reason
unban_user - Unban a User
banned_users - Show Banned Users
```

## Deploy 🚀

### Easiest Heroku Deploy 🤭

<p align="center">
    <a href="https://heroku.com/deploy?template=https://github.com/hackertyus/BroadcastBot">
    <img src="https://github.com/nikhileashy/justfor_testing/blob/main/herokudeploy-01-cropped.svg" alt="herokudeploy-01" border="0" height="90" width="285"></a>
</p>

### Easiest Railway Deploy
[![Deploy on Railway](https://railway.app/button.svg)](https://railway.app/new/template?template=https%3A%2F%2Fgithub.com%2Fhackertyus%2FBroadcastBot&plugins=mongodb&envs=BOT_TOKEN%2CAPI_HASH%2CAPI_ID%2CBROADCAST_AS_COPY%2CDB_URL%2CDB_NAME%2CAUTH_USERS%2CLOG_CHANNEL&optionalEnvs=BROADCAST_AS_COPY%2CDB_NAME&BOT_TOKENDesc=You+Telegram+Bot+Token+from+%40BotFather&API_HASHDesc=Your+API+Hash+from+my.telegram.org&API_IDDesc=Your+APP+ID+from+my.telegram.org&BROADCAST_AS_COPYDesc=Value+should+be+True+or+False.+Broadcast+with+Forward+Tag+or+as+Copy.%28Without+Forward+Tag%29&DB_URLDesc=MongoDB.com+database+url&DB_NAMEDesc=A+database+name+without+white+space%28example+%3A+broadcastbot%29&AUTH_USERSDesc=Create+a+list+of+User+Ids+to+use+this+bot%28ADMINS%29.+Seperate+by+space.+At+least+one+required.&LOG_CHANNELDesc=ID+of+a+Channel+which+you+want+to+RECEIVE+LOGS.&BROADCAST_AS_COPYDefault=True)

### Host Locally 🤕

```shell
git clone https://github.com/nacbots/BroadcastBot
cd BroadcastBot
pip3 install -r requirements.txt
# EDIT config.py values appropriately
python3 main.py
```

## Support Group:

<a href="https://t.me/NACBots"><img src="https://img.shields.io/badge/Telegram-Updates%20Channel-blue.svg?logo=telegram"></a><a href="https://t.me/n_a_c_bot_developers"><img src="https://img.shields.io/badge/Telegram-Support%20Group-blue.svg?logo=telegram"></a>

## Found a Bug 🐛

```Feel free to create a pull or create a issue now and describe your issue freely.```

## Credits
 - [@odysseusmax](https://github.com/odysseusmax)
 - [@NikhilEashy](https://github.com/nikhileashy)
 - [@MrBotDeveloper](https://github.com/MrBotDeveloper")

<a href="https://pyrogram.org"><img src="https://i.ibb.co/FHLg02J/381823.png" alt="pyrogram" border="0"></a>
