---
description: You can Hyra's Ranking API to programmatically rank users.
---

# Ranking a user

You can rank a user using the ranking API with ease. The rank API supports ranking any user within your group, and can only rank users which are below the bot account.

### Methods

{% api-method method="post" host="https://ranking.hyra.io" path="/rank" %}
{% api-method-summary %}
Rank User
{% endapi-method-summary %}

{% api-method-description %}
This route will rank a user to the provided roleset. You should send a JSON body \(text/json\)
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-body-parameters %}
{% api-method-parameter name="token" type="string" required=true %}
The token taken from the Hyra Admin
{% endapi-method-parameter %}

{% api-method-parameter name="rankNumber" type="integer" required=true %}
The rank ID of the role in which the user should be ranked to. Taken from group admin - **must be unique**.
{% endapi-method-parameter %}

{% api-method-parameter name="targetId" type="integer" required=true %}
The ID of the user you are trying to rank
{% endapi-method-parameter %}

{% api-method-parameter name="groupId" type="integer" required=true %}
The ID of the group where you are performing the rank
{% endapi-method-parameter %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Success
{% endapi-method-response-example-description %}

```javascript
{
  "Success": true,
  "Message": "Successfully changed rank of user"
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

[![Run in Postman](https://run.pstmn.io/button.svg)](https://app.getpostman.com/run-collection/c7575e83a33bc0fb206b)

