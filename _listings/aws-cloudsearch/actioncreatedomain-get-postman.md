{
  "info": {
    "name": "AWS CloudSearch Create Domain",
    "_postman_id": "9b07f323-2c55-4a35-83e5-c346c4dcb9b2",
    "description": "Creates a new search domain.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Tags",
      "item": [
        {
          "id": "781c0252-bcec-46cb-b660-87559cd8554f",
          "name": "AddTags",
          "request": {
            "url": "http://example.com/api/?Action=AddTags?Base=Base&InternalException=InternalException&LimitExceededException=LimitExceededException&ValidationException=ValidationException",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Attaches resource tags to an\n Amazon CloudSearch domain."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c999a6d8-2ed7-4440-b381-2b2ebbff9aca"
            }
          ]
        }
      ]
    },
    {
      "name": "Suggesters",
      "item": [
        {
          "id": "4d49de76-70cd-46a0-8ccc-77384fc6cdc1",
          "name": "BuildSuggesters",
          "request": {
            "url": "http://example.com/api/?Action=BuildSuggesters?DomainName=DomainName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Indexes the search suggestions."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e864cc28-402d-4fd8-8ceb-e36011bb15c1"
            }
          ]
        }
      ]
    },
    {
      "name": "Domains",
      "item": [
        {
          "id": "8e2f6316-7c3b-4952-899a-b49916fb2965",
          "name": "CreateDomain",
          "request": {
            "url": "http://example.com/api/?Action=CreateDomain?DomainName=DomainName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new search domain."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5cdeefa6-45a5-4f55-96d4-35003bbc9e57"
            }
          ]
        }
      ]
    }
  ]
}