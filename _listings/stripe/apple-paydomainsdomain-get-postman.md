{
  "info": {
    "name": "Stripe Get Apple Pay Domains Domain",
    "_postman_id": "7a9e9c46-2c82-49b2-8f4b-a1eed05570bf",
    "description": "Get Apple, Pay, Domains, Domain",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "apple",
      "item": [
        {
          "id": "299e88fc-2565-4166-b7cf-6943bc74cf63",
          "name": "getApplePayDomainsDomain",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.stripe.com",
              "path": [
                "v1",
                "apple_pay/domains/:domain"
              ],
              "query": [
                {
                  "key": "expand",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "domain",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get Apple, Pay, Domains, Domain"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8c069191-2f4b-4ffd-a85a-736edbf5d70e"
            }
          ]
        }
      ]
    }
  ]
}