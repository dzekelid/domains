---
swagger: "2.0"
x-collection-name: Click Meter
x-complete: 0
info:
  title: Click Meter Retrieve count of domains
  description: Retrieve count of domains.
  contact:
    name: Api Support
    url: http://www.clickmeter.com/api
    email: api@clickmeter.com
  version: v2
host: apiv2.clickmeter.com:80
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /domains:
    get:
      summary: Retrieve a list of domains
      description: Retrieve a list of domains.
      operationId: getDomains
      x-api-path-slug: domains-get
      parameters:
      - in: query
        name: limit
        description: Limit results to this number
      - in: query
        name: name
        description: Filter domains with this anmen
      - in: query
        name: offset
        description: Offset where to start from
      - in: query
        name: type
        description: Type of domain (system/go/personal/dedicated)
      responses:
        200:
          description: OK
      tags:
      - Domains
    post:
      summary: Create a domain
      description: Create a domain.
      operationId: postDomains
      x-api-path-slug: domains-post
      parameters:
      - in: body
        name: value
        description: The domain to create
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Domains
  /domains/count:
    get:
      summary: Retrieve count of domains
      description: Retrieve count of domains.
      operationId: getDomainsCount
      x-api-path-slug: domainscount-get
      parameters:
      - in: query
        name: name
        description: Filter domains with this anmen
      - in: query
        name: type
        description: Type of domain (system/go/personal/dedicated)
      responses:
        200:
          description: OK
      tags:
      - Domains
      - Count
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