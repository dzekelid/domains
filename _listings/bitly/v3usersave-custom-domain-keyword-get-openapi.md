---
swagger: "2.0"
x-collection-name: Bitly
x-complete: 0
info:
  title: Bitly Link API Get User Save Custom Domain Keyword
  description: Get user save custom domain keyword.
  termsOfService: http://dev.bitly.com/best_practices.html
  version: "3.0"
host: api-ssl.bitly.com
basePath: /v3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v3/user/save_custom_domain_keyword:
    get:
      summary: Get User Save Custom Domain Keyword
      description: Get user save custom domain keyword.
      operationId: getV3UserSaveCustomDomainKeyword
      x-api-path-slug: v3usersave-custom-domain-keyword-get
      parameters:
      - in: query
        name: keyword_link
        description: the Custom Bitlink (short domain and keyword combination) to
          set
      - in: query
        name: overwrite
        description: Ovewrite existing entry if one exists
      - in: query
        name: target_link
        description: the Bitlink the specified keyword will map to (as returned from
          /v3/shorten)
      responses:
        200:
          description: OK
      tags:
      - User
      - Save
      - Custom
      - Domain
      - Keyword
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