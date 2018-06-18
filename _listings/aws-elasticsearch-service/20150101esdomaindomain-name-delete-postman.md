{
  "info": {
    "name": "Amazon Elasticsearch Service API Delete Elasticsearch Domain",
    "_postman_id": "d0eb0b77-68ae-4591-8330-95a0b1fdf28b",
    "description": "Deletes an Amazon ES domain and all of its data. A domain cannot be recovered after it\n                is deleted. Use the DELETE HTTP method with this operation.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Tags",
      "item": [
        {
          "id": "98327001-8fae-4b9c-9a17-dcfe98d37f97",
          "name": "addTags",
          "request": {
            "url": "http://example.com/api/2015-01-01/tags",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Attaches resource tags to an Amazon ES domain. Use the POST HTTP method\n                with this operation. For more information, see Tagging Amazon ES\n                Domains."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e6ad68ed-b797-4b7a-9783-707d2287d1e5"
            }
          ]
        }
      ]
    },
    {
      "name": "Domains",
      "item": [
        {
          "id": "a0359014-7eaa-4a1e-b097-da2d4fa87ab2",
          "name": "createElasticsearchDomain",
          "request": {
            "url": "http://example.com/api/2015-01-01/es/domain",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new Amazon ES domain. Use the HTTP POST method with this\n                operation. For more information, see Creating Amazon ES Domains."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7e66e6e0-4456-4676-b278-455ab37d6885"
            }
          ]
        },
        {
          "id": "9be210a4-0dd4-4e8e-8b9c-92aefc7bdc0e",
          "name": "deleteElasticsearchDomain",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "api",
                "2015-01-01/es/domain/:domain_name"
              ],
              "variable": [
                {
                  "id": "domain_name",
                  "value": "domain_name",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes an Amazon ES domain and all of its data. A domain cannot be recovered after it\n                is deleted. Use the DELETE HTTP method with this operation."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "08fb3ac5-67bf-4240-b1f4-25f55e23322a"
            }
          ]
        }
      ]
    }
  ]
}