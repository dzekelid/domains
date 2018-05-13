{
  "info": {
    "name": "Twilio Delete Domains Credentials",
    "_postman_id": "525a2e01-6093-4ac8-a7ae-a2762913aa06",
    "description": "Remove a mapping from this domain.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "sip domains",
      "item": [
        {
          "id": "57f161a7-0c3f-4e35-9369-6d3435741cb9",
          "name": "remove-a-mapping-from-this-domain",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.twilio.com",
              "path": [
                "2010-04-01",
                "Accounts/:AccountSid/SIP/Domains/:SipDomainSid/IpAccessControlListMappings/:ALSid"
              ],
              "variable": [
                {
                  "id": "AccountSid",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "ALSid",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "SipDomainSid",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Remove a mapping from this domain"
          },
          "response": [
            {
              "header": [
                {
                  "key": "Content-Type",
                  "value": "application/json",
                  "disabled": false
                }
              ],
              "body": "[\r\n  {\r\n    \"Sid\": \"Sid\",\r\n    \"AccountSid\": \"AccountSid\",\r\n    \"FriendlyName\": \"FriendlyName\",\r\n    \"DateCreated\": \"DateCreated\",\r\n    \"DateUpdated\": \"DateUpdated\",\r\n    \"Uri\": \"Uri\"\r\n  }\r\n]",
              "status": "Successful response",
              "code": 200,
              "name": "Response_200",
              "id": "be80530e-25c8-47d5-baed-65276d165915"
            }
          ]
        }
      ]
    }
  ]
}