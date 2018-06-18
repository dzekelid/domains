---
swagger: "2.0"
x-collection-name: OpenDNS
x-complete: 0
info:
  title: OpenDNS Delete Domain
  version: 1.0.0
  description: "To delete a domain from the shared customer\u2019s domain list, run
    a DELETE request against the domains endpoint of the API."
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /domains/categories/:
    get:
      summary: Domain Status and Categorization
      description: This API method returns the domain status, which the quickest and
        easiest way to know whether a domain has been flagged as malicious by the
        OpenDNS Security Labs team (score of -1 for status), if it is believed to
        be safe (score of 1), or if it has yet to be given a status (score of 0).
      operationId: domainStatus
      x-api-path-slug: domainscategories-get
      responses:
        200:
          description: OK
      tags:
      - Domains
  /recommendations/{name}/:
    get:
      summary: Co-Occurrences for a Domain
      description: This API method returns a list of co-occurences for the specified
        domain. A co-occurrence is when two or more domains are being accessed by
        the same users within a small window of time. Being a co-occurrence isn't
        necessarily a bad thing, legitimate sites co-occur with each other as a part
        of normal web activity. However, unusual or suspicious co-occurence can provide
        additional information regarding attacks.
      operationId: coOccurrencesDomain
      x-api-path-slug: recommendationsname-get
      parameters:
      - in: path
        name: name
        description: Domain Name
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Domains
  /links/{name}/:
    get:
      summary: Related Domains
      description: This API method returns a list of domain names that have been frequently
        seen requested b around the same time (up to 60 seconds before or after) as
        the given domain name, but that are not frequently associated with other domain
        names.
      operationId: relatedDomains
      x-api-path-slug: linksname-get
      parameters:
      - in: path
        name: name
        description: Domain Name
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Related Domains
  /ips/{ip}/latest_domains:
    get:
      summary: Latest Malicious Domains
      description: "The latest_domains endpoint shows whether the IP address you\u2019ve
        entered as input has any known malicious domains associated with it."
      operationId: latestMaliciousDomains
      x-api-path-slug: ipsiplatest-domains-get
      parameters:
      - in: path
        name: ip
        description: The IP Address
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Malicious Domains
  /domains:
    get:
      summary: Get Domains
      description: "To gather the lists of domains already added to the shared customer\u2019s
        domain list, run a GET request against the domains endpoint of the API."
      operationId: getDomains
      x-api-path-slug: domains-get
      responses:
        200:
          description: OK
      tags:
      - Domains
    delete:
      summary: Delete Domain
      description: "To delete a domain from the shared customer\u2019s domain list,
        run a DELETE request against the domains endpoint of the API."
      operationId: deleteDomain
      x-api-path-slug: domains-delete
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