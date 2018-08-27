---
swagger: "2.0"
x-collection-name: AWS CloudSearch
x-complete: 0
info:
  title: AWS CloudSearch Delete Domain
  version: 1.0.0
  description: Permanently deletes a search domain and all of its data.
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
  /?Action=ListDomainNames:
    get:
      summary: List Domain Names
      description: Lists all search domains owned by an account.
      operationId: ListDomainNames
      x-api-path-slug: actionlistdomainnames-get
      parameters:
      - in: query
        name: DomainNames
        description: The names of the search domains owned by an account
        type: string
      responses:
        200:
          description: OK
      tags:
      - Domains
  /2013-01-01/documents/batch:
    get:
      summary: Search Documents
      description: You use the document service API to add, replace, or delete documents
        in your Amazon CloudSearch domain. For more information managing the documents
        in your search domain, see Uploading Data to an Amazon CloudSearch Domain.
      operationId: search
      x-api-path-slug: 20130101documentsbatch-get
      parameters:
      - in: body
        name: fields
        description: A collection of one or more field_name properties that define
          the fields the document contains
        schema:
          $ref: '#/definitions/holder'
      - in: body
        name: field_name
        description: Specifies a field within the document being added
        schema:
          $ref: '#/definitions/holder'
      - in: body
        name: id
        description: An alphanumeric string
        schema:
          $ref: '#/definitions/holder'
      - in: body
        name: type
        description: The operation type, add or delete
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Search
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