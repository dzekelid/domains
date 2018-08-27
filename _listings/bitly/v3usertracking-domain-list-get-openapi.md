---
swagger: "2.0"
x-collection-name: Bitly
x-complete: 0
info:
  title: Bitly User API User Tracking Domain List
  description: Returns a list of tracking domains a user has configured.
  termsOfService: http://dev.bitly.com/best_practices.html
  version: v3
host: api-ssl.bitly.com
basePath: /v3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v3/user/tracking_domain_list:
    get:
      summary: User Tracking Domain List
      description: Returns a list of tracking domains a user has configured.
      operationId: userTrackingDomainList
      x-api-path-slug: v3usertracking-domain-list-get
      parameters:
      - in: query
        name: tracking_domains
        description: a list of tracking domains configured for the authenticated user
      responses:
        200:
          description: OK
      tags:
      - User
      - Tracking
      - Domain
      - List
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