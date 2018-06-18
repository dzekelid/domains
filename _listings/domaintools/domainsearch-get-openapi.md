---
swagger: "2.0"
x-collection-name: DomainTools
x-complete: 0
info:
  title: Domain Search API Domain Search
  description: Searches active and deleted domain names that match a query string
  version: 1.0.0
host: api.domaintools.com
basePath: /v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /domain-search/:
    get:
      summary: Domain Search
      description: Searches active and deleted domain names that match a query string
      operationId: domainSearch
      x-api-path-slug: domainsearch-get
      parameters:
      - in: query
        name: active_only
        description: Return only domains currently registered
        type: string
        format: string
      - in: query
        name: anchor_left
        description: Return only domains that start with the query term
        type: string
        format: string
      - in: query
        name: anchor_right
        description: Return only domains that end with the query term
        type: string
        format: string
      - in: query
        name: deleted_only
        description: Return only domains previously registered but not currently registered
        type: string
        format: string
      - in: query
        name: exclude_query
        description: Terms to exclude from matching  each term in the query string
          must be at least three characters long
        type: string
        format: string
      - in: query
        name: has_hyphen
        description: Return results with hyphens in the domain name
        type: string
        format: string
      - in: query
        name: has_number
        description: Return results with numbers in the domain name
        type: string
        format: string
      - in: query
        name: max_length
        description: Limit the maximum domain character coun
        type: string
        format: string
      - in: query
        name: min_length
        description: Limit the minumum domain character count
        type: string
        format: string
      - in: query
        name: page
        description: Sets the page of results to retrieve from the server
        type: string
        format: string
      - in: query
        name: query
        description: Query string  each term in the query string must be at least
          three characters long
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Domains
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