{
  "info": {
    "name": "AWS CloudSearch Describe Domains",
    "_postman_id": "882b7311-ae67-4220-b464-3d6019c8c1cb",
    "description": "Gets information about the search domains owned by this account.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Tags",
      "item": [
        {
          "id": "316d42f4-3afb-45c2-86a7-42a016471a27",
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
              "id": "fba9e554-4d75-4a62-a9cc-1414447befd9"
            }
          ]
        }
      ]
    },
    {
      "name": "Suggesters",
      "item": [
        {
          "id": "9a3198fd-4c78-4785-a19a-88631a7d51d8",
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
              "id": "a0bd2df9-574d-459e-bd31-9aaead64bfe9"
            }
          ]
        },
        {
          "id": "d37fb9a5-5d03-494d-bdda-64109ddc29b0",
          "name": "DefineSuggester",
          "request": {
            "url": "http://example.com/api/?Action=DefineSuggester?DomainName=DomainName&Suggester=Suggester",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Configures a suggester for a domain."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "368c2ab6-7f5f-41b7-82c5-165be4859f8d"
            }
          ]
        },
        {
          "id": "c5b723d8-f34b-44d2-b6f2-601e77fe798a",
          "name": "DeleteSuggester",
          "request": {
            "url": "http://example.com/api/?Action=DeleteSuggester?DomainName=DomainName&SuggesterName=SuggesterName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a suggester."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8f73b180-917d-4e55-8e81-fddbc74c654f"
            }
          ]
        }
      ]
    },
    {
      "name": "Domains",
      "item": [
        {
          "id": "8ddf048a-0a8b-4857-8991-82765e0c478c",
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
              "id": "b143065e-7e8f-487b-8d94-7a9c779354f9"
            }
          ]
        },
        {
          "id": "710a9d8e-0adc-4ecd-8a59-2fe4ebcf7ab8",
          "name": "DeleteDomain",
          "request": {
            "url": "http://example.com/api/?Action=DeleteDomain?DomainName=DomainName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Permanently deletes a search domain and all of its data."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0c5bf949-2c76-4a29-8cdc-676f4c48a5d5"
            }
          ]
        },
        {
          "id": "da0271ec-6bd5-4955-848d-94cc9ac64c9a",
          "name": "DescribeDomains",
          "request": {
            "url": "http://example.com/api/?Action=DescribeDomains?DomainNames.member.N=DomainNames.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets information about the search domains owned by this account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "84f98f14-4a77-426d-8315-d4bdd07d2d24"
            }
          ]
        }
      ]
    },
    {
      "name": "Analysis Scheme",
      "item": [
        {
          "id": "1b6143ab-b863-4246-b307-b10986ec096f",
          "name": "DefineAnalysisScheme",
          "request": {
            "url": "http://example.com/api/?Action=DefineAnalysisScheme?AnalysisScheme=AnalysisScheme&DomainName=DomainName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Configures an analysis scheme that can be applied to a text or text-array field to define language-specific text processing options."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "15e1d1ce-e0e1-4cca-be37-6be08d2d3101"
            }
          ]
        },
        {
          "id": "1e10ab7d-e171-4426-9f9f-e0b535668b73",
          "name": "DeleteAnalysisScheme",
          "request": {
            "url": "http://example.com/api/?Action=DeleteAnalysisScheme?AnalysisSchemeName=AnalysisSchemeName&DomainName=DomainName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes an analysis scheme."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5edcc35d-ccf7-40c7-98d2-085463c944c0"
            }
          ]
        },
        {
          "id": "8bf8e17c-1a83-45a1-ba17-e41e843e4f38",
          "name": "DescribeAnalysisSchemes",
          "request": {
            "url": "http://example.com/api/?Action=DescribeAnalysisSchemes?AnalysisSchemeNames.member.N=AnalysisSchemeNames.member.N&Deployed=Deployed&DomainName=DomainName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets the analysis schemes configured for a domain."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "12a6a69d-b7f8-4ab0-90ea-1608410e8fb5"
            }
          ]
        }
      ]
    },
    {
      "name": "Expressions",
      "item": [
        {
          "id": "e6efbec9-b4bc-46a6-ab12-f541662b0f1e",
          "name": "DefineExpression",
          "request": {
            "url": "http://example.com/api/?Action=DefineExpression?DomainName=DomainName&Expression=Expression",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Configures an Expression  for the search domain."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "28c0fcb4-cac7-4489-8eff-2503a1ff151e"
            }
          ]
        },
        {
          "id": "de0b3cb5-8756-478c-9985-5e6543bede0e",
          "name": "DeleteExpression",
          "request": {
            "url": "http://example.com/api/?Action=DeleteExpression?DomainName=DomainName&ExpressionName=ExpressionName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Removes an \n  Expression\n  from the search domain."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "64d30dc8-ff49-4254-9ccf-1fb87f4dfa10"
            }
          ]
        }
      ]
    },
    {
      "name": "Index Fields",
      "item": [
        {
          "id": "b70d9538-5f2d-44ee-bd5f-c8514b3d79ec",
          "name": "DefineIndexField",
          "request": {
            "url": "http://example.com/api/?Action=DefineIndexField?DomainName=DomainName&IndexField=IndexField",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Configures an ndexField  for the search domain."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "01b7c00b-4d7f-43a9-9b7d-ed925e149c3f"
            }
          ]
        },
        {
          "id": "ed75763f-25c4-4957-ac47-c330b3a55bbe",
          "name": "DeleteIndexField",
          "request": {
            "url": "http://example.com/api/?Action=DeleteIndexField?DomainName=DomainName&IndexFieldName=IndexFieldName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Removes an \n  IndexField\n  from the search domain."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dc4f4677-321a-4995-9fe4-43f960279009"
            }
          ]
        }
      ]
    },
    {
      "name": "Availability Options",
      "item": [
        {
          "id": "5a0f0605-f118-44ef-bb4e-39bd80fee564",
          "name": "DescribeAvailabilityOptions",
          "request": {
            "url": "http://example.com/api/?Action=DescribeAvailabilityOptions?Deployed=Deployed&DomainName=DomainName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets the availability options configured for a domain."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f36fb838-b6e9-4553-8ac9-f5b6d844c2e8"
            }
          ]
        }
      ]
    }
  ]
}