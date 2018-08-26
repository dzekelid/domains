---
swagger: "2.0"
x-collection-name: Twilio
x-complete: 0
info:
  title: Twilio Add Domains
  description: Update the attributes of a domain.
  termsOfService: https://www.twilio.com/legal/tos
  version: v1
host: api.twilio.com
basePath: /2010-04-01/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /Accounts/{AccountSid}/SIP/Domains:
    get:
      summary: Get Domains
      description: Returns a paged list of the domains for an account.
      operationId: returns-a-paged-list-of-the-domains-for-an-account
      x-api-path-slug: accountsaccountsidsipdomains-get
      parameters:
      - in: path
        name: AccountSid
        description: The ID for the Twilio account
      responses:
        200:
          description: OK
      tags:
      - SIP Domains
    post:
      summary: Add Domains
      description: Creates a new Domain and returns its instance resource. You must
        pick a unique domain name that ends in .sip.twilio.com.nAfter creating a Domain,
        you must map it to an authentication method before the domain is ready to
        receive traffic.n
      operationId: creates-a-new-domain-and-returns-its-instance-resource-you-must-pick-a-unique-domain-name-that-ends-
      x-api-path-slug: accountsaccountsidsipdomains-post
      parameters:
      - in: path
        name: AccountSid
        description: The ID for the Twilio account
      responses:
        200:
          description: OK
      tags:
      - SIP Domains
  /Accounts/{AccountSid}/SIP/Domains/{SipDomainSid}:
    get:
      summary: Get Domains
      description: Return a specific instance by Sid.
      operationId: return-a-specific-instance-by-sid
      x-api-path-slug: accountsaccountsidsipdomainssipdomainsid-get
      parameters:
      - in: path
        name: AccountSid
        description: The ID for the Twilio account
      - in: path
        name: SipDomainSid
        description: A 34 character string that uniquely identifies the SIP domain
      responses:
        200:
          description: OK
      tags:
      - SIP Domains
    post:
      summary: Add Domains
      description: Update the attributes of a domain.
      operationId: update-the-attributes-of-a-domain
      x-api-path-slug: accountsaccountsidsipdomainssipdomainsid-post
      parameters:
      - in: path
        name: AccountSid
        description: The ID for the Twilio account
      - in: path
        name: SipDomainSid
        description: A 34 character string that uniquely identifies the SIP domain
      responses:
        200:
          description: OK
      tags:
      - SIP Domains
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---