---
swagger: "2.0"
x-collection-name: Bitly
x-complete: 0
info:
  title: Bitly User Metrics API User Referring Domains
  description: eturns aggregate metrics about the domains referring click traffic
    to all of the authenticated users Bitlinks. If the user is a master account, or
    is a subaccount with full_reports permission, the user may choose to view the
    metrics of any account belonging to the master account.
  termsOfService: http://dev.bitly.com/best_practices.html
  version: v3
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
  /link/referrers_by_domain:
    get:
      summary: Link Referrers by Domain
      description: Returns metrics about the pages referring click traffic to a single
        Bitlink, grouped by referring domain.
      operationId: linkReferrersByDomain
      x-api-path-slug: linkreferrers-by-domain-get
      parameters:
      - in: query
        name: link
        description: a Bitlink
      - in: query
        name: timezone
        description: an integer hour offset from UTC (-14
      - in: query
        name: unit
        description: minute | hour | day | week | month default:day
      - in: query
        name: units
        description: an integer representing the time units to query data for
      - in: query
        name: unit_reference_ts
        description: an epoch timestamp, indicating the most recent time for which
          to pull metrics
      responses:
        200:
          description: OK
      tags:
      - Link
      - Referrers
      - By
      - Domain
  /v3/user/tracking_domain_list:
    get:
      summary: User Tracking Domain List
      description: Returns a list of tracking domains a user has configured.
      operationId: userTrackingDomainList
      x-api-path-slug: v3usertracking-domain-list-get
      parameters:
      - in: query
        name: tracking_domains
        description: a list of tracking domains configured for the authenticated user
      responses:
        200:
          description: OK
      tags:
      - User
      - Tracking
      - Domain
      - List
  /v3/user/referring_domains:
    get:
      summary: User Referring Domains
      description: eturns aggregate metrics about the domains referring click traffic
        to all of the authenticated users Bitlinks. If the user is a master account,
        or is a subaccount with full_reports permission, the user may choose to view
        the metrics of any account belonging to the master account.
      operationId: userReferringDomains
      x-api-path-slug: v3userreferring-domains-get
      parameters:
      - in: query
        name: exclude_social_networks
        description: If true, exclude domains that are part of a social network that
          bitly tracks (default=true)
      - in: query
        name: limit
        description: 1 to 1000 (default=100)
      - in: query
        name: login
        description: an optional string consisting of the account name used to report
          the appropriate statistics; defaults to the current user
      - in: query
        name: rollup
        description: Return data for multiple units rolled up to a single result instead
          of a separate value for each period of time
      - in: query
        name: timezone
        description: 'an integer hour offset from UTC (-14 to 14), or a timezone string
          default: America/New_York'
      - in: query
        name: unit
        description: 'minute, hour, day, week or month, default: day'
      - in: query
        name: units
        description: an integer representing the time units to query data for
      - in: query
        name: unit_reference_ts
        description: 'an epoch timestamp, indicating the most recent time for which
          to pull metrics, default: now'
      responses:
        200:
          description: OK
      tags:
      - User
      - Referring
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