---
swagger: "2.0"
x-collection-name: DomainTools
x-complete: 0
info:
  title: Domain Search API Domain Search
  description: Searches active and deleted domain names that match a query string
  version: 1.0.0
host: api.domaintools.com
basePath: /v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{domain}:
    get:
      summary: Domain Profile
      description: Basic registrant, server, and registration data for a domain name,
        plus preview data for other products
      operationId: domainProfile
      x-api-path-slug: domain-get
      parameters:
      - in: path
        name: domain
        description: The domain to profile
        type: string
        format: string
      responses:
        1:
          description: Photoset not found - The photoset id passed was not the id
            of avalid photoset owned by the calling user
        2:
          description: Photo not found - The photo id passed was not the id of a valid
            photo owned by the calling user
        95:
          description: SSL is required - SSL is required to access the Flickr API
        96:
          description: Invalid signature - The passed signature was invalid
        97:
          description: Missing signature - The call required signing but no signature
            was sent
        98:
          description: Login failed / Invalid auth token - The login details or auth
            token passed were invalid
        99:
          description: User not logged in / Insufficient permissions - The method
            requires user authentication but the user was not logged in, or the authenticated
            method call did not have the required permissions
        100:
          description: Invalid API Key - The API key passed was not valid or has expired
        105:
          description: Service currently unavailable - The requested service is temporarily
            unavailable
        106:
          description: Write operation failed - The requested operation failed due
            to a temporary issue
        111:
          description: Format "xxx" not found - The requested response format was
            not found
        112:
          description: Method "xxx" not found - The requested method was not found
        114:
          description: Invalid SOAP envelope - The SOAP envelope send in the request
            could not be parsed
        115:
          description: Invalid XML-RPC Method Call - The XML-RPC request document
            could not be parsed
        116:
          description: Bad URL found - One or more arguments contained a URL that
            has been used for abuse on Flickr
        200:
          description: OK
      tags:
      - Domains
  /domain-search/:
    get:
      summary: Domain Search
      description: Searches active and deleted domain names that match a query string
      operationId: domainSearch
      x-api-path-slug: domainsearch-get
      parameters:
      - in: query
        name: active_only
        description: Return only domains currently registered
        type: string
        format: string
      - in: query
        name: anchor_left
        description: Return only domains that start with the query term
        type: string
        format: string
      - in: query
        name: anchor_right
        description: Return only domains that end with the query term
        type: string
        format: string
      - in: query
        name: deleted_only
        description: Return only domains previously registered but not currently registered
        type: string
        format: string
      - in: query
        name: exclude_query
        description: Terms to exclude from matching ??? each term in the query string
          must be at least three characters long
        type: string
        format: string
      - in: query
        name: has_hyphen
        description: Return results with hyphens in the domain name
        type: string
        format: string
      - in: query
        name: has_number
        description: Return results with numbers in the domain name
        type: string
        format: string
      - in: query
        name: max_length
        description: Limit the maximum domain character coun
        type: string
        format: string
      - in: query
        name: min_length
        description: Limit the minumum domain character count
        type: string
        format: string
      - in: query
        name: page
        description: Sets the page of results to retrieve from the server
        type: string
        format: string
      - in: query
        name: query
        description: Query string ??? each term in the query string must be at least
          three characters long
        type: string
        format: string
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