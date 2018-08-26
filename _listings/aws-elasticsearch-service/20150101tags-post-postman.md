{
  "info": {
    "name": "Amazon Elasticsearch Service API Add Tags",
    "_postman_id": "29b66ee9-6896-4eda-9b4b-328d6ef26d82",
    "description": "Attaches resource tags to an Amazon ES domain. Use the POST HTTP method\n                with this operation. For more information, see Tagging Amazon ES\n                Domains.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Tags",
      "item": [
        {
          "id": "523649a9-5bf1-4b92-8e81-3597897e6b95",
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
              "id": "fcd4fa9b-ceb4-4210-b9cc-290993850007"
            }
          ]
        }
      ]
    }
  ]
}