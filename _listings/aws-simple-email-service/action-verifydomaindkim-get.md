---
swagger: "2.0"
info:
  title: AWS Simple Email Service API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=VerifyDomainDkim&k=1:
    get:
      summary: ' Verify Domain Dkim '
      description: Returns a set of DKIM tokens for a domain
      operationId: verifyDomainDkim
      parameters:
      - in: query
        name: Domain
        description: The name of the domain to be verified for Easy DKIM signing
        type: string
      responses:
        200:
          description: OK
      tags:
      - domains
definitions: []
x-collection-name: AWS Simple Email Service
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