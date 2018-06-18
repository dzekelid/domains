{
  "info": {
    "name": "Flickr Stats Get Photo Domains",
    "_postman_id": "6b883077-6d59-4b91-a618-791eff178d12",
    "description": "Get a list of referring domains for a photo.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Stats",
      "item": [
        {
          "id": "f8934136-8da9-46d3-b3d5-10d184a9584e",
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
              "id": "582ea463-7cd4-4a5a-a28f-c928fc41c4a7"
            }
          ]
        },
        {
          "id": "10fb528c-6d4d-4ab7-aa5c-4c4e34d1b28d",
          "name": "getRestMethodFlickr.stats.getphotodomains",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.stats.getPhotoDomains?api_key=%7B%7D&date=%7B%7D&format=%7B%7D&page=%7B%7D&per_page=%7B%7D&photo_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a list of referring domains for a photo."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9f9696fa-ebf1-453d-9116-3d75396b7bc3"
            }
          ]
        }
      ]
    }
  ]
}