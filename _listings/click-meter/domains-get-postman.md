{
  "info": {
    "name": "Click Meter Retrieve a list of domains",
    "_postman_id": "cec4b1d2-6582-44d1-9530-b03ff96211a9",
    "description": "Retrieve a list of domains.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Domains",
      "item": [
        {
          "id": "4431f5d6-12a6-4550-8e63-4f47772f2894",
          "name": "getDomains",
          "request": {
            "url": "http://apiv2.clickmeter.com:80/domains?limit=%7B%7D&name=%7B%7D&offset=%7B%7D&type=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve a list of domains."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "060dd4c4-a17e-44fd-bee6-6358206ac298"
            }
          ]
        }
      ]
    }
  ]
}