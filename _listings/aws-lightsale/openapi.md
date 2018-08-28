swagger: "2.0"
x-collection-name: AWS Lightsale
x-complete: 1
info:
  title: AWS Lightsale API
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
      description: Creates a domain resource for the specified domain (e.
      operationId: createDomain
      x-api-path-slug: actioncreatedomain-get
      parameters:
      - in: query
        name: domainName
        description: The domain name to manage (e
        type: string
      responses:
        200:
          description: OK
      tags:
      - Domains
  /?Action=CreateDomainEntry:
    get:
      summary: Create Domain Entry
      description: |-
        Creates one of the following entry records associated with the domain: A record, CNAME
              record, TXT record, or MX record.
      operationId: createDomainEntry
      x-api-path-slug: actioncreatedomainentry-get
      parameters:
      - in: query
        name: domainEntry
        description: An array of key-value pairs containing information about the
          domain entry      request
        type: string
      - in: query
        name: domainName
        description: The domain name (e
        type: string
      responses:
        200:
          description: OK
      tags:
      - Domains
  /?Action=DeleteDomain:
    get:
      summary: Delete Domain
      description: Deletes the specified domain recordset and all of its domain records.
      operationId: deleteDomain
      x-api-path-slug: actiondeletedomain-get
      parameters:
      - in: query
        name: domainName
        description: The specific domain name to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Domains
  /?Action=DeleteDomainEntry:
    get:
      summary: Delete Domain Entry
      description: Deletes a specific domain entry.
      operationId: deleteDomainEntry
      x-api-path-slug: actiondeletedomainentry-get
      parameters:
      - in: query
        name: domainEntry
        description: An array of key-value pairs containing information about your
          domain entries
        type: string
      - in: query
        name: domainName
        description: The name of the domain entry to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Domains
  /?Action=GetDomain:
    get:
      summary: Get Domain
      description: Returns information about a specific domain recordset.
      operationId: getDomain
      x-api-path-slug: actiongetdomain-get
      parameters:
      - in: query
        name: domainName
        description: The domain name for which your want to return information about
        type: string
      responses:
        200:
          description: OK
      tags:
      - Domains
  /?Action=GetDomains:
    get:
      summary: Get Domains
      description: Returns a list of all domains in the user's account.
      operationId: getDomains
      x-api-path-slug: actiongetdomains-get
      parameters:
      - in: query
        name: pageToken
        description: A token used for advancing to the next page of results from your
          get domains      request
        type: string
      responses:
        200:
          description: OK
      tags:
      - Domains
  /?Action=UpdateDomainEntry:
    get:
      summary: Update Domain Entry
      description: Updates a domain recordset after it is created.
      operationId: updateDomainEntry
      x-api-path-slug: actionupdatedomainentry-get
      parameters:
      - in: query
        name: domainEntry
        description: An array of key-value pairs containing information about the
          domain entry
        type: string
      - in: query
        name: domainName
        description: The name of the domain recordset to update
        type: string
      responses:
        200:
          description: OK
      tags:
      - Domains