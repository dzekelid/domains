{
  "info": {
    "name": "Stripe Get Apple Pay Domains",
    "_postman_id": "d04854bd-5961-4018-b2ff-39110eca4ab1",
    "description": "Get Apple, Pay, Domains",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "apple",
      "item": [
        {
          "id": "cc456b12-160d-45b5-97fb-d3b852e00f70",
          "name": "getApplePayDomains",
          "request": {
            "url": "http://api.stripe.com/v1/apple_pay/domains?domain_name=%7B%7D&ending_before=%7B%7D&expand=%7B%7D&limit=%7B%7D&starting_after=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get Apple, Pay, Domains"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5be82eef-5ce2-4b4d-bf4e-931a7b5c5521"
            }
          ]
        }
      ]
    }
  ]
}