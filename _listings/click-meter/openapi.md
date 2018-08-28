swagger: "2.0"
x-collection-name: Click Meter
x-complete: 1
info:
  title: Click Meter
  description: api-dashboard-for-clickmeter-api
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
  /domains/{id}:
    delete:
      summary: Delete a domain
      description: Delete a domain.
      operationId: deleteDomains
      x-api-path-slug: domainsid-delete
      parameters:
      - in: path
        name: id
        description: Id of domain
      responses:
        200:
          description: OK
      tags:
      - Domains
      - Id
    get:
      summary: Get a domain
      description: Get a domain.
      operationId: getDomains
      x-api-path-slug: domainsid-get
      parameters:
      - in: path
        name: id
        description: Id of domain
      responses:
        200:
          description: OK
      tags:
      - Domains
      - Id
    post:
      summary: Update a domain
      description: Update a domain.
      operationId: postDomains
      x-api-path-slug: domainsid-post
      parameters:
      - in: path
        name: id
        description: Id of domain
      - in: body
        name: value
        description: The domain to update
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Domains
      - Id