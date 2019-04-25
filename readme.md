---
description: Get information about the game and player
---

# GetGameInfo API

{% api-method method="get" host="host" path="/FootBallStrike/GetGameInfo/" %}
{% api-method-summary %}

{% endapi-method-summary %}

{% api-method-description %}
This endpoint allows you to get free cakes.
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
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
    "DisplayName":"xxx1234",
    "PlayerId":”123456”,
    "Currency":"EUR",
    "Balance":”700.00”,
    "MaxBet":”1300.00”,
    "MinBet":”1.00”,
    "Chips":"1,5,25,100,500",
    "MaxPayout":”100000”,
    "DefaultChip":”5”,
    "TableLimit":[
        {
            "BetOption":"Tiger",
            "BetOptionMin":”1.00”,
            "BetOptionMax":”800.00”
        },
        {
            "BetOption":"Crab",
            "BetOptionMin":”1.00”,
            "BetOptionMax":”800.00”
        }
    ]
}
```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=404 %}
{% api-method-response-example-description %}
Could not find a cake matching this query.
{% endapi-method-response-example-description %}

```javascript
{
    "message": "Could not find the page"
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}



