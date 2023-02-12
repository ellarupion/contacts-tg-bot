## Telegram Contacts Bot

This is a simple Telegram bot that allows you to search, add, and edit contacts using a JSON file.


## Requirements

Python 3.6+
python-telegram-bot library
A Telegram bot token
You can install the python-telegram-bot library using pip:

```pip install python-telegram-bot==13.7```


## Getting Started
1.Clone this repository to your local machine or server.

2.Create a new bot on Telegram and obtain your bot token from BotFather.

3. Insert your token in line 83:
```updater = Updater('YOUR_BOT_TOKEN_HERE', use_context=True)```

4. Create a data.JSON file to store your contacts, and populate it with some sample data. An example file is included in the project directory.
```[
  {
    "full_name": "Linus Torvalds",
    "post": "Developer",
    "phones": [
      "123-456-7890",
      "555-555-5555"
    ],
    "comment": "Likes bananas."
  },
  {
    "full_name": "Jony Ive",
    "post": "Designer",
    "phones": [
      "987-654-3210"
    ],
    "comment": "Also likes bananas."
  }
]
```

5. Run the bot using the following command:
```python main.py```

The bot should now be running and listening for incoming messages.

## Usage
To search for a contact, type `/search [query]` or simply `[query]` in the chat. The bot will search for contacts whose full_name, post, phones, or comment fields contain the given query. For example:

```/search Linus```
or
```Linus```

To add a new contact, type `/add [full name];[post];[phone numbers];[comment]` in the chat. The phone numbers should be separated by commas. 

For example:

```/add Michelangelo di Lodovico Buonarroti Simoni;Designer;123-456-7890,555-555-5555;Allergic to bananas.```

To edit a contact, simply reply to the search result message with the new contact information in the same format as when adding a contact.

For example:

```Michelangelo di Lodovico Buonarroti Simoni;Product Manager;123-456-7890,555-555-5555;Likes apples.```

## License
This project is licensed under the MIT License. See the [LICENSE](https://github.com/ellarupion/contacts-tg-bot/blob/main/LICENSE) file for details.
