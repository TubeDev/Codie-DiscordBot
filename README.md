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
  <img alt="Info Command" width="300" src="https://github.com/user-attachments/assets/32317ef0-73d5-49a8-8536-e5be4a341b29" />
  <img alt="Info Command" width="300" src="https://github.com/user-attachments/assets/22ece348-b26b-478e-b251-619de4e1dca8" />
  
</p>
