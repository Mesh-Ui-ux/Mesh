import os
from telegram import Bot
from dotenv import load_dotenv

load_dotenv()

BOT_TOKEN = os.getenv("BOT_TOKEN")
CHAT_ID = os.getenv("CHAT_ID")

bot = Bot(token=BOT_TOKEN)
bot.send_message(chat_id=CHAT_ID, text="Bot deployed successfully!")

python-telegram-bot==13.15
python-dotenv==1.0.1

BOT_TOKEN=123456789:ABCdefYourBotTokenHere
CHAT_ID=123456789
