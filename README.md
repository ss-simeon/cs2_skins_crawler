# cs2_skins_crawler
Monitors CS2 skin marketplaces for good discounts and notifies via Discord webhooks.

# Discord Link to [Skin Alert](https://discord.gg/uMHSyhzMNU)
- For Skin Alert, the program is being ran off my Raspberry Pi

# Current CS2 Marketplaces Monitored
- csfloat
- skinbid

# How to run the program
1. Copy the repo
2. Install the discord.py, requests and pytest module
   - pip install discord
   - pip install requests
   - pip install pytest
3. Create "secret.py" in "src" directory and implement the following inside:
   - skinsWebhook = "https://discord.com/api/webhooks/examplewebhook"
   - stickerWebhook = "https://discord.com/api/webhooks/examplewebhook"
   - updateWebhook = "https://discord.com/api/webhooks/examplewebhook"
   - bot_token = "BotTokenExample"
5. Make sure you're not on Python 3.12 as there's an issue with the requests package, I am currently on Python 3.11.1
6. run python3 src/main.py for main program
   - if you have a bot you can  run "python3 src/DiscordBot.py" - useful for my case as the program is run off a Raspberry Pi, letting me know if program is running (if bot is online)
