{
  "info": {
    "name": "Rackspace Create domain",
    "_postman_id": "8c53520f-d73e-4f6f-81d7-9c706baeb9e9",
    "description": "NoteThis call returns an asynchronous response, See\nSynchronous and asynchronous responses\nfor more details and examples of the way that asynchronous responses work.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Limits",
      "item": [
        {
          "id": "434b4499-1c7d-4e3d-a56e-cde118aaaab4",
          "name": "list-limits",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "api",
                "v1.0/:account/limits\n"
              ],
              "variable": [
                {
                  "id": "account",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "X-Auth-Token",
                "value": "{}",
                "description": "Arbitrary characterstring generated by theauthentication servicein response to validcredentials",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "This call provides a list of all applicable limits for a specified account.The following examples show the requests and corresponding responses to list\nall limits for the specified account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a4b045e3-a3f9-49d7-bfcb-fda9f2714c1e"
            }
          ]
        },
        {
          "id": "7f192add-8c40-4937-91da-eb907a2eb8e3",
          "name": "show-limits",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "api",
                "v1.0/:account/limits/:type\n"
              ],
              "variable": [
                {
                  "id": "account",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "type",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "X-Auth-Token",
                "value": "{}",
                "description": "Arbitrary characterstring generated by theauthentication servicein response to validcredentials",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "This call provides a list of all applicable limits of a specified type for\nthe specified account.The following examples show the requests and corresponding responses to list\nall applicable limits of a specified type for the specified account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d67b6275-607e-407f-901a-260a587a1694"
            }
          ]
        },
        {
          "id": "d9f93d40-2f2d-42f4-94aa-5846f17cda0c",
          "name": "list-limit-types",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "api",
                "v1.0/:account/limits/types\n"
              ],
              "variable": [
                {
                  "id": "account",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "X-Auth-Token",
                "value": "{}",
                "description": "Arbitrary characterstring generated by theauthentication servicein response to validcredentials",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "This call provides a list of all applicable limit types for a specified account.The following examples show the requests and corresponding responses to list\nall limit types for the specified account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b6dc3103-0f6b-4e14-b07e-1563e2f749df"
            }
          ]
        }
      ]
    },
    {
      "name": "Domains",
      "item": [
        {
          "id": "b51c1c21-d4b7-4e3f-bbd7-fbace2754a8c",
          "name": "list-domains",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "api",
                "v1.0/:account/domains\n"
              ],
              "variable": [
                {
                  "id": "account",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "X-Auth-Token",
                "value": "{}",
                "description": "Arbitrary characterstring generated by theauthentication servicein response to validcredentials",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "These calls provide a list of all DNS domains manageable by a given account.\nThe resulting list is flat, and does not break the domains down hierarchically\nby subdomain. All representative domains are included in the list, even if a\ndomain is conceptually a subdomain of another domain in the list.Note"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ce4d3556-c126-4e3e-b076-88ecb83321af"
            }
          ]
        },
        {
          "id": "99826a9d-d85d-4047-a364-769c2ffe8571",
          "name": "create-domain",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "api",
                "v1.0/:account/domains\n"
              ],
              "variable": [
                {
                  "id": "account",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "header": [
              {
                "key": "X-Auth-Token",
                "value": "{}",
                "description": "Arbitrary characterstring generated by theauthentication servicein response to validcredentials",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "NoteThis call returns an asynchronous response, See\nSynchronous and asynchronous responses\nfor more details and examples of the way that asynchronous responses work."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "224376d3-b960-413e-a6ed-be876dd3aa46"
            }
          ]
        }
      ]
    }
  ]
}