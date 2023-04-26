# ML-discord-bot

This is a Python script for a Discord bot that monitors messages in a server and takes action if it detects inappropriate content. The bot logs all messages containing blocked words, phrases, or terms to a separate log file and reports them to a webhook URL. It also sends a warning message to the user who sent the message, and deletes messages that contain inappropriate content.

The bot loads a list of banned words from the "profanity1.txt" file, a list of functional words from the "functional_words.txt" file, and a list of allowed words from the "allowed_words.txt" file. The bot skips any words that appear in the functional_words or allowed_words list. The bot uses the FuzzyWuzzy library to calculate a similarity score between each word in the message and the banned words list. If the similarity score is greater than 80, the bot logs the message, sends a warning message to the user, and deletes the message. If the message contains the word "tenor" and a banned word, the bot will delete the message and send a warning message to the user.

The script logs its activities to two different log files: "bot.log" for bot-related errors, and "blocked.log" for messages that contain banned words.

## ChatGPT3
In order to analyze the sentence and the image you will need to import your own set of credensials. 
