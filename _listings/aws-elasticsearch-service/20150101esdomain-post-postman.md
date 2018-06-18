{
  "info": {
    "name": "Amazon Elasticsearch Service API Create Elasticsearch Domain",
    "_postman_id": "a2c4a38b-8136-4eea-a7bf-2183dba5a0e4",
    "description": "Creates a new Amazon ES domain. Use the HTTP POST method with this\n                operation. For more information, see Creating Amazon ES Domains.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Tags",
      "item": [
        {
          "id": "b9ad8a34-eede-4587-b8d8-43cf8451ac4e",
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
              "id": "8825d358-1ed8-4257-91ab-3b63b6eaf758"
            }
          ]
        }
      ]
    },
    {
      "name": "Domains",
      "item": [
        {
          "id": "8be9422f-a502-4225-b7d5-b385efa8ed7c",
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
              "id": "50597490-e3a7-448c-b01e-f124ddac6636"
            }
          ]
        }
      ]
    }
  ]
}