---
swagger: "2.0"
x-collection-name: Flickr
x-complete: 0
info:
  title: Flickr Stats Get Collection Domains
  description: Get a list of referring domains for a collection
  version: 1.0.0
host: api.flickr.com
basePath: /services/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest/?method=flickr.stats.getCollectionDomains:
    get:
      summary: Stats Get Collection Domains
      description: Get a list of referring domains for a collection
      operationId: getRestMethodFlickr.stats.getcollectiondomains
      x-api-path-slug: restmethodflickr-stats-getcollectiondomains-get
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: collection_id
        description: The id of the collection to get stats for
      - in: query
        name: date
        description: Stats will be returned for this date
      - in: query
        name: format
        description: Response format
      - in: query
        name: page
        description: The page of results to return
      - in: query
        name: per_page
        description: Number of domains to return per page
      responses:
        200:
          description: OK
      tags:
      - Stats
      - GetCollectionDomains
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