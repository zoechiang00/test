---
description: Player Place Bet
---

# PlaceBet API

{% api-method method="get" host="host" path="/FootBallStrike/PlaceBet/" %}
{% api-method-summary %}
Get Cakes
{% endapi-method-summary %}

{% api-method-description %}
This endpoint allows you to get free cakes.
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="GameCode" type="integer" required=true %}

{% endapi-method-parameter %}

{% api-method-parameter name="ProductType" type="integer" required=true %}

{% endapi-method-parameter %}

{% api-method-parameter name="LiveGameId" type="integer" required=true %}

{% endapi-method-parameter %}

{% api-method-parameter name="GoalBet" type="number" required=true %}

{% endapi-method-parameter %}

{% api-method-parameter name="GoalLeftBet" type="number" required=true %}

{% endapi-method-parameter %}

{% api-method-parameter name="GoalMiddleBet" type="number" required=true %}

{% endapi-method-parameter %}

{% api-method-parameter name="GoalRightBet" type="number" required=true %}

{% endapi-method-parameter %}

{% api-method-parameter name="SaveBet" type="number" required=true %}

{% endapi-method-parameter %}

{% api-method-parameter name="SaveLeftBet" type="number" required=true %}

{% endapi-method-parameter %}

{% api-method-parameter name="SaveMiddleBet" type="number" required=true %}

{% endapi-method-parameter %}

{% api-method-parameter name="SaveRightBet" type="number" required=true %}

{% endapi-method-parameter %}

{% api-method-parameter name="Token" type="string" required=true %}

{% endapi-method-parameter %}
{% endapi-method-path-parameters %}

{% api-method-headers %}
{% api-method-parameter name="Authentication" type="string" required=true %}
Authentication token to track down who is emptying our stocks. 
{% endapi-method-parameter %}
{% endapi-method-headers %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Cake successfully retrieved.
{% endapi-method-response-example-description %}

```javascript
{
    "ErrorCode": "0",
    "RefNo": "T698231687",
    "Balance": ”7426.83”
}

```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=404 %}
{% api-method-response-example-description %}
Could not find a cake matching this query.
{% endapi-method-response-example-description %}

```javascript
{
    "message": "Page not found."
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}



