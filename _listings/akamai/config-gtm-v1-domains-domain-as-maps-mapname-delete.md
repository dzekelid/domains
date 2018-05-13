---
swagger: "2.0"
info:
  title: Akamai API Remove an AS Map
  description: Remove an AS Map
  version: 1.0.0
host: developer.akamai.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /config-gtm/v1/domains/{domain}/as-maps/{mapName}:
    delete:
      summary: Remove an AS Map
      description: Remove an AS Map
      operationId: configgtmv1domainsdomainasmapsmapname
      parameters:
      - in: query
        name: domain
        description: Name of Traffic Management domain
        type: string
      - in: query
        name: mapName
        description: Name of AS Map to create, update or delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - configurations
      - gtm
      - domains
      - as
      - maps
definitions: []
x-collection-name: Akamai
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