---
description: You can message a user on Roblox through Hyra Ranking
---

# Messaging a user

You can message a user using the ranking API with ease. This supports messaging any user on Roblox, and each successful invocation is counted against the 500 daily quota. 

{% hint style="info" %}
This only works on Hyra Cookie accounts. If you are using a Campfire Managed account please contact our team to request a transfer. 
{% endhint %}

### Methods

{% api-method method="post" host="https://ranking.hyra.io" path="/message" %}
{% api-method-summary %}
Message User
{% endapi-method-summary %}

{% api-method-description %}
This route will send a user a Roblox Message. 
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-body-parameters %}
{% api-method-parameter name="token" type="string" required=true %}
Your Hyra Ranking token
{% endapi-method-parameter %}

{% api-method-parameter name="subject" type="string" required=true %}
The subject of the message
{% endapi-method-parameter %}

{% api-method-parameter name="message" type="string" required=true %}
The contents of the message
{% endapi-method-parameter %}

{% api-method-parameter name="targetId" type="string" required=true %}
The user you wish to message
{% endapi-method-parameter %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```javascript
{
    "Success": true,
    "Message": "Successfully messaged user",
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

