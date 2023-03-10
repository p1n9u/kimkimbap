<img src="https://badgen.net/badge/icon/typescript?icon=typescript&label">

# KimKimbap (Discord Music Bot)

> KimKimbap uses template from [Rawon](https://github.com/Clytage/rawon)   
> The only music play version of Rawon `3.2.0`, remove moderation commands.   
> A Discord Music Bot built with TypeScript, discord.js & uses Command Handler from [discordjs.guide](https://discordjs.guide)

## Requirements, Dev Settings

1. Discord Bot Token **[Guide](https://discordjs.guide/preparations/setting-up-a-bot-application.html#creating-your-bot)**  
   1.1. `Token` - This is the only required option for your bot to run. You must provide the token for your Discord bot account.   
   1.2. To create a bot account, go to your [applications page](https://discordapp.com/developers/applications/me) (logging in if prompted), and then follow this [10 second video](https://drive.google.com/file/d/1wZG_TBVfjQfj0CEYaRTzS60D-cbfeeYZ/view).   
   1.3. If you followed it entirely, you should have revealed your token and can now copy it into the config file.
   1.4. Enable 'Message Content Intent' in Discord Developer Portal
2. node `v16.11.0` (nvm install used), `v16.6.0` or higher required   
   2.1. npm `8.0.0`   
   2.2. nvm `0.39.1`
3. Ubuntu 22.04.2 LTS

## 🚀 Installation

```bash
git clone https://github.com/p1n9u/kimkimbap.git

cd kimkimbap

touch .env # copy contents, you can get from original Rawon Repo above link.

npm install
npm run build
npm prune --production
```
After installation finishes follow configuration instructions then run `npm run start` to start the bot.

## 📝 Register Service

### Register 

base path : project root directory kimkimbap
```bash
cd dist
chmod +x index.js
cd ..
sudo systemctl link ~/kimkimbap/kimkimbap.service # pwd conmand
sudo systemctl start kimkimbap
sudo systemctl enable kimkimbap
```
- Add the code below to the top of the `index.js` file.
```jsx
#!/home/(username)/.nvm/versions/node/v16.11.0/bin/node
```

### Display Log
```bash
journalctl -u kimkimbap
# Result
systemd[1]: Started A Discord Music Bot KimKimbap.
...
```

## ⚙️ Configuration

`.env` from Notion Github/disbot (personal notion space)

## 🌎 Locales

- English (en)
