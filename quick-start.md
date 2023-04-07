---
description: Here you can find information to start using our api
coverY: 0
---

# 🏠 Quick Start

## Docs Pages

{% content-ref url="broken-reference" %}
[Broken link](broken-reference)
{% endcontent-ref %}

## Get your bot's token

To use our api you need to use as authorization header your custom bot's token threw our website. To do that, follow the next steps:

{% hint style="danger" %}
**Do not** **share/post** your bot's token with no-one!
{% endhint %}

1. Go to [braxybots](https://braxybots.eu.org) website.
2. Click the "Login" button at the top right of your screen.
3. When you have login in go to your profile by clicking again your name at the right corner of you screen.
4. After that you should find your bot's profile. If you have not any bots submitted, make a new bot application and wait for verification.
5. If you have a bot, click on his profile. You will find this box as the picture and after that click the "Copy" button.
6.

    <figure><img src=".gitbook/assets/Στιγμιότυπο οθόνης 2023-04-02 140913 (1).png" alt="Danger Zone"><figcaption><p>Danger Zone Box</p></figcaption></figure>
7. Then to start trying our api, you need to open the main file of your bot.
8. Once you have opened that, copy the next basic code of posting the server count where you bot has joined.

### On JavaScript language

{% code title="ready.js" overflow="wrap" lineNumbers="true" %}
```javascript
const fetch = require("node-fetch");
const client = new Client({...});

client.on("ready", () => {
    //Your bot's code
    fetch('https://braxybots.eu.org/api/v1/bots/stats', {
        method: "POST",
        body: JSON.stringify({
            serverCount: client.guilds.cache.size,
        }),
        headers: {
            "Content-Type": "application/json",
            Authorization: "YOUR BOT'S TOKEN FOR THE WEBSITE"
        }
    })
    .then(req=>req.json())
    .then(res=>{
        console.log(`Success!`)
    
     })
});
```
{% endcode %}

### On Python language

{% code title="ready.py" overflow="wrap" lineNumbers="true" %}
```python
import discord
import requests
import json

client = discord.Client()

@client.event
async def on_ready():
#Your bot's code
headers = {
"Content-Type": "application/json",
"Authorization": "YOUR BOT'S TOKEN FOR THE WEBSITE"
}
data = {
"serverCount": len(client.guilds)
}
response = requests.post('https://braxybots.eu.org/api/v1/bots/stats', headers=headers, json=data)
if response.ok:
print("Success!")

client.run("YOUR BOT'S DISCORD TOKEN")
```
{% endcode %}

In this way we can get information about your bot such as server, shard and more.\
