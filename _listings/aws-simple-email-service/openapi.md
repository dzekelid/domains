---
swagger: "2.0"
x-collection-name: AWS Simple Email Service
x-complete: 1
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
  /?Action=VerifyDomainDkim:
    get:
      summary: Verify Domain Dkim
      description: Returns a set of DKIM tokens for a domain.
      operationId: verifyDomainDkim
      x-api-path-slug: actionverifydomaindkim-get
      parameters:
      - in: query
        name: Domain
        description: The name of the domain to be verified for Easy DKIM signing
        type: string
      responses:
        200:
          description: OK
      tags:
      - Domains
---