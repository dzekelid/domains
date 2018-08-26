---
swagger: "2.0"
x-collection-name: DigitalOcean
x-complete: 0
info:
  title: Digital Ocean List all Domains
  description: "To retrieve a list of all of the domains in your account, send a GET
    request to /v2/domains.\r\n\r\nThe response will be a JSON object with a key called
    domains."
  version: 1.0.0
host: example.com
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
      summary: List all Domains
      description: "To retrieve a list of all of the domains in your account, send
        a GET request to /v2/domains.\r\n\r\nThe response will be a JSON object with
        a key called domains."
      operationId: DomainsGet
      x-api-path-slug: domains-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - List
      - ""
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