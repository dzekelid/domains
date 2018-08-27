{
  "info": {
    "name": "Digital Ocean List all Domains",
    "_postman_id": "ff4de5ed-99fa-4c11-b34c-fd431d2fabb8",
    "description": "To retrieve a list of all of the domains in your account, send a GET request to /v2/domains.\r\n\r\nThe response will be a JSON object with a key called domains.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "List",
      "item": [
        {
          "id": "c0fda52d-6499-4650-963e-7a2d298fbf74",
          "name": "DomainsGet",
          "request": {
            "url": "http://example.com/domains",
            "method": "GET",
            "header": [
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "To retrieve a list of all of the domains in your account, send a GET request to /v2/domains.\r\n\r\nThe response will be a JSON object with a key called domains."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "85a1dc0e-8a0b-4634-87d1-65fa1aa24635"
            }
          ]
        }
      ]
    }
  ]
}