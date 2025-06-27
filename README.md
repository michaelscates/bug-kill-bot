# 🐛 Bug-Kill Bot

A lightweight Discord bot that listens for GitHub repo links, clones the target repo, runs your tests, and posts the results back into the same Discord channel. Ideal for quick remote debugging when you're away from a full dev setup.

## 🚀 Features

- Trigger test runs by pasting a GitHub repo URL into a designated channel
- Automatically clones the repo and sets up a virtual environment
- Runs your test suite (e.g. with `pytest`)
- Stops on the first error and reports results back to Discord
- Designed to run on a Raspberry Pi or lightweight VPS

## 🧰 Requirements

- Python 3.8+
- `git`
- `pip` / `venv`
- A bot token from Discord
- Discord channel ID where the bot will listen

## 🛠️ Setup

1. Clone this repo to your Raspberry Pi or server:

```bash
git clone https://github.com/your-username/bug-kill-bot.git
cd bug-kill-bot

2. Install dependencies:



pip install -r requirements.txt

3. Create a .env file based on .env.example:



DISCORD_BOT_TOKEN=your_token_here
CHANNEL_ID=your_channel_id_here

4. Run the bot:



python bot.py

🧪 How It Works

You paste a GitHub link (e.g. https://github.com/yourname/my-bugfix-fork) into the bot's channel.

The bot clones the repo into a temporary folder.

It runs run_tests.sh to set up and test the code.

Results are sent back into the Discord channel as a message block.


🧾 License

MIT License – see the LICENSE file for details.


