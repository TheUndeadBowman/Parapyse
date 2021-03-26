# Parapyse
A Paradise Bot List API Wrapper in Python.

## Initializing Class

The main class is called Parapyse, you create an object like so:

```py
p = Parapyse(user_id, token)
```

Here, `user_id` is your client id (in discord.py, `client.user.id`) and `token` is your Paradise API token for your bot.

## Class Properties

Properties are in the format `parapyse_object.property`. In the above example, `p` is the Parapyse object. If property names have a comma they are aliases.

`username`- The name of your bot (str).  
`certified`- Whether the bot is certified or not. (bool)  
`owner`- The ID of the owner. (int)  
`additional_owners`- A list of IDs of additional owners. The main owner is not included. Will return an empty list `[]` if there are no additional owners. (list)  
`prefix`- The bot's prefix. (str)  
`short`, `description`- The bot's short description. (str)  
`long`, `long_description`- The bot's long description. (str)  
`votes`- Number of users who voted for the bot. (int)  
`users_voted`- Unique (non-repeated) users who have voted. (list)  
`unique_votes`- Number of unique votes. Same as `len(users_voted)`. (int)  

The following may return None if not applicable.

`vanity_url`- The end of the Vanity URL (for certified bots only) (str, NoneType)  
`server`- The bot's support server. (str, NoneType)  
`website`- The bot's website  
