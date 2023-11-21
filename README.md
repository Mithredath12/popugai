# popugai
Popugai telegram bot for Omirzak Islam Advanced programming(python) course final project

This Python code sets up a Telegram bot using the Telebot library. Here's a breakdown:

1. Importing Libraries:
   - import telebot: Imports the Telebot library for working with the Telegram Bot API.
   - import config: Presumably, it imports a configuration file (config.py), which likely contains sensitive information like the bot token.

2. Initializing the Bot:
   - bot = telebot.TeleBot(config.TOKEN): Creates a Telebot instance with the provided bot token from the configuration file.

3. Defining Message Handling:
   - @bot.message_handler(content_types=['text']): Decorator that specifies the following function (lalala) will handle text messages.
   - def lalala(message):: Defines the lalala function, which takes a Telegram message as a parameter.
   - bot.send_message(message.chat.id, message.text): Sends the received text message back to the same chat it came from.

4. Running the Bot:
   - bot.polling(none_stop=True): Initiates the bot's polling mechanism to continuously check for new messages. The none_stop=True ensures the bot keeps running even in case of errors.

In summary, this script creates a simple echo bot that responds to any text message it receives by sending the same message back to the originating chat. The bot runs continuously, polling for new messages.
