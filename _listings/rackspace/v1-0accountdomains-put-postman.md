{
  "info": {
    "name": "Rackspace Update domains",
    "_postman_id": "97382083-aae8-4309-af31-0eef68cad3cf",
    "description": "NoteThis call returns an asynchronous response, as described in\nSynchronous and asynchronous responses.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Limits",
      "item": [
        {
          "id": "45fd0906-3e76-4c54-8ccb-3c01e00791af",
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
              "id": "8163a071-0d3d-4f15-bb86-c973264cf345"
            }
          ]
        },
        {
          "id": "68b34c34-9d9e-4065-990f-4df4337d921d",
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
              "id": "41288b8f-24a8-4cb6-b5bf-c90e289b3d0f"
            }
          ]
        },
        {
          "id": "d0ab34ef-1138-46d1-b362-e8745cf6e4d5",
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
              "id": "8de8bd73-5283-44a2-a1f8-0e11a827b956"
            }
          ]
        }
      ]
    },
    {
      "name": "Domains",
      "item": [
        {
          "id": "3b257b74-2735-4c1b-ac25-185fc8cb4741",
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
              "id": "100b6b71-09a4-4f4d-8eb0-90c8672487ce"
            }
          ]
        },
        {
          "id": "fe7bcb8b-9292-4d1b-bfa5-026708b0c842",
          "name": "update-domains",
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
            "method": "PUT",
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
            "description": "NoteThis call returns an asynchronous response, as described in\nSynchronous and asynchronous responses."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3176b724-b1d6-46bf-aa4d-8514672ef2c1"
            }
          ]
        },
        {
          "id": "b2fb0a7c-bb20-48a7-b30c-2c2358ce7c2d",
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
              "id": "80c1de8a-59ff-4d27-a7d7-457bd3b9d19b"
            }
          ]
        }
      ]
    }
  ]
}