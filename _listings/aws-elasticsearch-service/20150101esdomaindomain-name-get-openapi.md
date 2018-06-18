---
swagger: "2.0"
x-collection-name: AWS Elasticsearch Service
x-complete: 0
info:
  title: Amazon Elasticsearch Service API Describe Elasticsearch Domain
  version: 1.0.0
  description: |-
    Describes the domain configuration for the specified Amazon ES domain, including the
                    domain ID, domain service endpoint, and domain ARN. Use the HTTP GET
                    method with this operation.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /2015-01-01/es/domain:
    post:
      summary: Create Elasticsearch Domain
      description: |-
        Creates a new Amazon ES domain. Use the HTTP POST method with this
                        operation. For more information, see Creating Amazon ES Domains.
      operationId: createElasticsearchDomain
      x-api-path-slug: 20150101esdomain-post
      responses:
        200:
          description: OK
      tags:
      - Domains
  /2015-01-01/es/domain/{domain_name}:
    delete:
      summary: Delete Elasticsearch Domain
      description: |-
        Deletes an Amazon ES domain and all of its data. A domain cannot be recovered after it
                        is deleted. Use the DELETE HTTP method with this operation.
      operationId: deleteElasticsearchDomain
      x-api-path-slug: 20150101esdomaindomain-name-delete
      responses:
        200:
          description: OK
      tags:
      - Domains
    get:
      summary: Describe Elasticsearch Domain
      description: |-
        Describes the domain configuration for the specified Amazon ES domain, including the
                        domain ID, domain service endpoint, and domain ARN. Use the HTTP GET
                        method with this operation.
      operationId: describeElasticsearchDomain
      x-api-path-slug: 20150101esdomaindomain-name-get
      parameters:
      - in: query
        name: DomainName
        description: Name of the Amazon ES domain that you want to                                        describe
        type: string
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