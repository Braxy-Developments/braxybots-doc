---
description: Find information about a bot on the website
coverY: 0
---

# Bot Search

{% swagger method="get" path="/botID" baseUrl="https://braxybots.eu.org/api/v1/bots" summary="" %}
{% swagger-description %}

{% endswagger-description %}

{% swagger-parameter in="path" name="botID" required="true" type="Number" %}
The bot's id you want to search
{% endswagger-parameter %}

{% swagger-response status="200: OK" description="You got your info!" %}
JSON Example:

```json5
{
 "avatar": "https://cdn.discordapp.com/avatars/1003970641747259462/f31f778d339540ade022176d881da9d8.webp",
 "botID": "1003970641747259462",
 "username": "Buster",
 "discrim": "3189",
 "shortDesc": "A Multi-Purpose bot with slash-command support to help you with the management & protect of your server, have fun with your friends and list",
 "dlink": "https://discord.com/api/oauth2/authorize?client_id=1003970641747259462&permissions=8&scope=bot%20applications.commands",
 "privacy": "",
 "prefix": "/help",
 "votes": 2,
 "ownerID": "794563552606289952",
 "coowners": [],
 "tags": [
  "Moderation",
  "Fun",
  "Multi-Purpose",
  "Games",
  "Guard",
  "Anime",
  "Invite",
  "Music",
  "Logging",
  "Web Dashboard",
  "Youtube",
  "Greek",
  "English",
  "Apple Music",
  "24/7",
  "Automod"
 ],
 "longDesc": "👋Hello! My name is Buster! \r\n\r\nHere is some features that I have....\r\n\r\n<h2>🧪Features</h2>\r\n• Advanced Mod Commands to help you with the management & protect of your server!\r\n• Music System to listen to music!\r\n• An Advanced Help Command to help you find the best command to use for your goal!\r\n• Games Command to have fun with your friends by playing them!\r\n• A Dashboard Website to help you with the management of the bot! (Still's On Work)\r\n• A Good Anti-System to help you protect your server/members.\r\n• Logging System.\r\n• Everything is in slash-command to be more easy to use the commands!\r\n• There are available commands to help you find the best information about your fav's streamers and build new Embeds!\r\n• Fun Commands to have fun such as tic-tac-toe & fight system.\r\n• AI Chat Pro System to talk with the bot!\r\n\r\nAnd so much more to discover.....\r\n\r\n<h2>📱Support</h2>\r\n• Our Bot is being host in Virtual Private Server (VPS) with 8gb of ram and an strong core!\r\n• There is available 24/7 Support to help you with the usage of the bot and also to report bugs!\r\n• Our Official Discord Server & Website for help: discord.gg/HmUVvxacDp \r\n\r\n<h2>🧑‍💻Our Team</h2>\r\nWe are a new  small developement team with a success of our bots such as JukeDisc & JukeMod, made with love for you!\r\n• Our Members: H.Dev | Mr.Diesel\r\n• Our Supporters who helped us with the bot: Helper | 𝒯𝒶𝓁𝑜𝓈𝒯𝒽𝑒𝑀𝒾𝓃𝑜𝒶𝓃\r\n\r\nMade with 💗 once again.....\r\n\r\nThis Project is being protected by DMCA Licence.",
 "certificate": "Certified",
 "support": "dsc.gg/braxytm",
 "website": "braxybots.eu.org",
 "serverCount": "123",
 "usersCount": "123"
}
```
{% endswagger-response %}

{% swagger-response status="404: Not Found" description="You entered invalid bot id." %}
```json
{
 "404": "You entered invalid bot id."
}
```
{% endswagger-response %}
{% endswagger %}
