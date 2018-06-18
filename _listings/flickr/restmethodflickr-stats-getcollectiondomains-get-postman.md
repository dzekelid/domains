{
  "info": {
    "name": "Flickr Stats Get Collection Domains",
    "_postman_id": "8e54c239-66ed-450b-b140-7fea5f183d01",
    "description": "Get a list of referring domains for a collection",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Stats",
      "item": [
        {
          "id": "3ea37878-7e33-4ac5-a5b4-c1e8cede4af9",
          "name": "getRestMethodFlickr.stats.getcollectiondomains",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.stats.getCollectionDomains?api_key=%7B%7D&collection_id=%7B%7D&date=%7B%7D&format=%7B%7D&page=%7B%7D&per_page=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a list of referring domains for a collection"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1222230e-4f7b-4455-8114-b6386f815b65"
            }
          ]
        }
      ]
    }
  ]
}