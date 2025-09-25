# 🤖 Codie - Discord Bot

Codie is a fun, multi-functional Discord bot built with the `discord.py` library. It combines playful interactions with practical utilities, backed by a robust and well-structured backend.

This project showcases a wide range of features - from simple commands to advanced systems like user credit management, interactive modals, and developer-only tools.

Codie includes:

- 💬 Both modern slash and prefix command support
- 💸 Mini credit economy system
- 🎲 Fun commands
- ⚙️ Error handling and code reliability
- 🔐 Secure token handling via `dotenv`
- 📋 Logging system for activity tracking and debug purposes
- 🧠 Interactive modals for user input

## ✨ Features

### 🔹 Slash Commands

- `/info`  
Displays your current credit balance.

- `/gamble <bet>`  
Bet your credits. If you win, you double your stake; if you lose, the bet is deducted.

- `/work`  
Solve simple math problems to earn credits, get penalized if you answer wrong.

- `/hello`  
Get a greeting from Codie!

- `/dice`  
Roll the dice and get a random number between 1 and 6.

- `/ping`  
Sends a playful message in chat and a “Pong” in your DMs.

- `/count <x>`  
The bot counts from 1 up to `x` in chat. Includes user cooldowns and limits to prevent spam.

### 🔹 Prefix Commands

- `?status`  
Displays an embedded bot status message.

- `?terminate` (Developer only)  
Securely shuts down the bot with an embedded status message.

- `?add_credit <@user> <amount>` (Developer only)  
Adds the specified amount of credits to a user’s balance. User can be specified either by mentioning them, putting their Discord username or putting their user ID, eg. `?add_credit tube__ 800`

- `?set_credit <@user> <amount>` (Developer only)  
Sets a user’s credit balance to the specified amount. User argument input logic is the same as `?add_credit` command.

**Note:** Developer only commands are only accessible to users whose Discord user IDs have been added to the dev list in the configuration section of the bot's code.

## 🛠️ Tech Highlights

- Slash command integration (`bot.tree`) for modern UX.
- Modal input for interactive work command.
- Logging system with persistent log file (`fancy_stuff.log`).
- Environment variable management with `python-dotenv`.
- Developer-only command restrictions by Discord ID.
- Clean error handling for startup and invalid tokens.
- Easily configurable settings in the bot's configuration section of its code.

## 🖼️ Gallery

<p align="left">
  <img width="300" alt="Info Command" src="https://github.com/user-attachments/assets/c9941a08-961c-4336-af3a-e2eb53e8ce16"/>
  
  <img width="300" alt="Dice Command" src="https://github.com/user-attachments/assets/c9156ed8-87ec-4220-8c51-63175c1755b6"/>
  
  <img width="300" alt="Gamble Command" src="https://github.com/user-attachments/assets/80497fbc-6256-4c58-b483-cd03833ede20"/>
  
  <img width="300" alt="Work Command" src="https://github.com/user-attachments/assets/ef7d8d21-c7c3-4e08-9435-b0c42ef39782"/>
  
  <img width="300" alt="Add credit Command" src="https://github.com/user-attachments/assets/e9a9e92c-1c75-460f-ab41-400555c2cbb2"/>
  
  <img width="300" alt="Terminate Command" src="https://github.com/user-attachments/assets/29737b1e-cdde-4b8f-a6d8-c95553f5cd1c"/>
</p>

## ⚙️ How to Run

### Invite the bot to your server

Go to the [Discord Developer Portal](https://discord.com/developers/applications) and create a new application. In the Bot section, enable intents "Server Members Intent" and "Message Content Intent", then copy the bot token.

In the OAuth2 section, get URL to invite the bot to your server. Be sure to tick the necessary scopes (bot, applications.commands) when generating the URL. Make sure to also give the bot appropriate permissions based on the commands you want to use.
Invite the bot to your server using the generated URL.

### Run the bot

1. Clone the repository:
   ```bash
   git clone https://github.com/TubeDev/Codie-DiscordBot.git
   cd Codie-DiscordBot
   ```

2. Install the required packages:
   ```bash
   pip install -r requirements.txt
   ```

3. Set up your environment variables:  
   - Create a `.env` file in the root directory.
   - Add your Discord bot token:
     ```
     DISCORD_TOKEN=your_token_here
     ```

4. Run the bot:
   ```bash
   python Discord_BOT.py
   ```

After running the main script, the bot should appear online in your Discord server and be ready to use!

---

### 📜 License

This project is licensed under the [**MIT License**](https://opensource.org/licenses/MIT).  
You are free to use, modify, and distribute this project as permitted by the license.

![TubeDev](https://img.shields.io/badge/TubeDev--lime)
![Python](https://img.shields.io/badge/Python--blue?logo=python&logoColor=white)
![MIT](https://img.shields.io/badge/License-MIT-gold)

<p align="left">
  <img width="500" src="https://github.com/user-attachments/assets/f5a0f154-dee7-4653-9451-caa52513573a" alt="logo" />
</p>
