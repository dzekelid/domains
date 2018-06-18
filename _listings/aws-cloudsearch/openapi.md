---
swagger: "2.0"
x-collection-name: AWS CloudSearch
x-complete: 1
info:
  title: AWS CloudSearch
  version: 1.0.0
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
---