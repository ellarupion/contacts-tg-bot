**Contacts Bot**
The Contacts Bot is a Telegram bot that allows users to search and add contacts.

**Features**
Search contacts by name, position, phone number, and comment
Add new contacts with name, position, phone number(s), and optional comment
Edit existing contacts
All contacts are stored in a JSON file

**Usage**
To use the Contacts Bot, start by sending the /search command followed by a search query. You can also simply type a search query and the bot will automatically search for it. The bot will return a list of contacts that match your search query, including the contact's name, position, phone number(s), and optional comment.

To add a new contact, use the /add command followed by the contact information in the following format: full name;position;phone number(s);comment (optional). Separate phone numbers with commas.

To edit a contact, simply reply to the search result with the /edit command followed by the updated contact information in the same format as adding a contact. Note that you can only edit one field at a time.

Commands
/search [query]: Search for contacts by name, position, phone number, or comment
/add [contact]: Add a new contact in the format full name;position;phone number(s);comment (optional)
/edit [contact]: Edit an existing contact by replying to a search result with the updated contact information in the format full name;position;phone number(s);comment (optional)
