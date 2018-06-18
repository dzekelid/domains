---
swagger: "2.0"
x-collection-name: AWS CloudSearch
x-complete: 0
info:
  title: AWS CloudSearch Describe Domains
  version: 1.0.0
  description: Gets information about the search domains owned by this account.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=CreateDomain:
    get:
      summary: Create Domain
      description: Creates a new search domain.
      operationId: CreateDomain
      x-api-path-slug: actioncreatedomain-get
      parameters:
      - in: query
        name: DomainName
        description: A name for the domain you are creating
        type: string
      responses:
        200:
          description: OK
      tags:
      - Domains
  /?Action=DeleteDomain:
    get:
      summary: Delete Domain
      description: Permanently deletes a search domain and all of its data.
      operationId: DeleteDomain
      x-api-path-slug: actiondeletedomain-get
      parameters:
      - in: query
        name: DomainName
        description: The name of the domain you want to permanently delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Domains
  /?Action=DescribeDomains:
    get:
      summary: Describe Domains
      description: Gets information about the search domains owned by this account.
      operationId: DescribeDomains
      x-api-path-slug: actiondescribedomains-get
      parameters:
      - in: query
        name: DomainNames.member.N
        description: The names of the domains you want to include in the response
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