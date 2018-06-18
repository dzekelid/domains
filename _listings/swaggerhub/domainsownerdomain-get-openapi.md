---
swagger: "2.0"
x-collection-name: SwaggerHub
x-complete: 0
info:
  title: Swagger Hub Registry Retrieves an APIs.json listing for all domain versions
    for this owner and domain
  description: Retrieves an apis.json listing for all domain versions for this owner
    and domain.
  contact:
    name: SwaggerHub
    url: http://swaggerhub.com
    email: info@swaggerhub.com
  version: 1.0.45
host: api.swaggerhub.com
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
      summary: Retrieves a list of currently defined domains in APIs.json format
      description: Retrieves a list of currently defined domains in apis.json format.
      operationId: searchDomains
      x-api-path-slug: domains-get
      parameters:
      - in: query
        name: limit
        description: number of results per page
      - in: query
        name: order
        description: sort order
      - in: query
        name: page
        description: page to return
      - in: query
        name: query
        description: free text query to match
      - in: query
        name: sort
        description: sort criteria or result set* NAME -* UPATED* CREATED* OWNER
      - in: query
        name: state
        description: matches against published state of the spec* UNPUBLISHED - spec
          is a draft, a work in progress* PUBLISHED - spec is a stable version ready
          for consuming from client applications* ANY - either PUBLISHED or UNPUBLISHED
      - in: query
        name: tag
        description: matches against tags associated with a domain
      responses:
        200:
          description: OK
      tags:
      - Domains
  /domains/{owner}:
    get:
      summary: Retrieves an APIs.json listing of all domains defined for this owner
      description: Retrieves an apis.json listing of all domains defined for this
        owner.
      operationId: getOwnerDomains
      x-api-path-slug: domainsowner-get
      parameters:
      - in: query
        name: limit
        description: number of results per page
      - in: query
        name: order
        description: sort order
      - in: path
        name: owner
        description: API or Domaion owner identifier
      - in: query
        name: page
        description: page to return
      - in: query
        name: sort
        description: sort criteria or result set* NAME -* UPATED* CREATED* OWNER
      responses:
        200:
          description: OK
      tags:
      - Domains
      - Owner
  /domains/{owner}/{domain}:
    delete:
      summary: Deletes the specified domain
      description: Deletes the specified domain.
      operationId: deleteDomain
      x-api-path-slug: domainsownerdomain-delete
      parameters:
      - in: path
        name: domain
        description: domain identifier
      - in: query
        name: force
        description: force update
      - in: path
        name: owner
        description: API or Domaion owner identifier
      responses:
        200:
          description: OK
      tags:
      - Domains
      - Owner
      - Domain
    get:
      summary: Retrieves an APIs.json listing for all domain versions for this owner
        and domain
      description: Retrieves an apis.json listing for all domain versions for this
        owner and domain.
      operationId: getDomainVersions
      x-api-path-slug: domainsownerdomain-get
      parameters:
      - in: path
        name: domain
        description: domain identifier
      - in: path
        name: owner
        description: API or Domaion owner identifier
      responses:
        200:
          description: OK
      tags:
      - Domains
      - Owner
      - Domain
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