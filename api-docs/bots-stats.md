---
coverY: 0
---

# Bot's Stats

{% swagger method="post" path="/stats" baseUrl="https://braxybots.eu.org/api/v1/bots" summary="" %}
{% swagger-description %}

{% endswagger-description %}

{% swagger-parameter in="header" name="Authorization" required="true" %}
The Bot's token from the bot's profile.
{% endswagger-parameter %}

{% swagger-parameter in="header" name="serverCount" required="true" %}
The bot's server count.
{% endswagger-parameter %}

{% swagger-parameter in="header" name="shardCount" %}
The bot's shard count.
{% endswagger-parameter %}

{% swagger-response status="200: OK" description="You posted your bot's stats!" %}

{% endswagger-response %}

{% swagger-response status="401: Unauthorized" description="You entered an invalid bot token." %}

{% endswagger-response %}

{% swagger-response status="403: Forbidden" description="You must enter a bot token." %}

{% endswagger-response %}

{% swagger-response status="404: Not Found" description="You entered an invalid bot token." %}

{% endswagger-response %}
{% endswagger %}
