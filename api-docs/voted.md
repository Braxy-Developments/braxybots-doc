---
coverY: 0
---

# Voted

{% swagger method="get" path="/userID" baseUrl="https://braxybots.eu.org/api/v1/bots/check" summary="" %}
{% swagger-description %}

{% endswagger-description %}

{% swagger-parameter in="header" required="true" name="Authorization" %}
The Bot's token from the bot's profile.
{% endswagger-parameter %}

{% swagger-parameter in="path" name="userID" type="Number" required="true" %}
User's ID you want to check.
{% endswagger-parameter %}

{% swagger-response status="200: OK" description="You can check now if a user voted or not." %}

{% endswagger-response %}

{% swagger-response status="401: Unauthorized" description="You entered an invalid bot token." %}

{% endswagger-response %}

{% swagger-response status="403: Forbidden" description="You must enter a bot token." %}

{% endswagger-response %}

{% swagger-response status="404: Not Found" description="You must enter a user id." %}

{% endswagger-response %}
{% endswagger %}
