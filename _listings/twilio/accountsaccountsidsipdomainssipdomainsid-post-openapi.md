---
swagger: "2.0"
x-collection-name: Twilio
x-complete: 0
info:
  title: Twilio Add Domains
  description: Update the attributes of a domain.
  termsOfService: https://www.twilio.com/legal/tos
  version: v1
host: api.twilio.com
basePath: /2010-04-01/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /Accounts/{AccountSid}/SIP/Domains/{SipDomainSid}/CredentialListMappings/{CLSid}:
    delete:
      summary: Delete Domains Credentials
      description: Remove a CredentialListMapping from a domain
      operationId: remove-a-credentiallistmapping-from-a-domain
      x-api-path-slug: accountsaccountsidsipdomainssipdomainsidcredentiallistmappingsclsid-delete
      parameters:
      - in: path
        name: AccountSid
        description: The ID for the Twilio account
      - in: path
        name: CLSid
        description: A 34 character string that uniquely identifies the credential
          list
      - in: path
        name: SipDomainSid
        description: A 34 character string that uniquely identifies the SIP domain
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
      - SIP Domains
  /Accounts/{AccountSid}/SIP/Domains/{SipDomainSid}/CredentialListMappings:
    get:
      summary: Get Domains Credentials
      description: Get the user lists mapped to this domain.
      operationId: get-the-user-lists-mapped-to-this-domain
      x-api-path-slug: accountsaccountsidsipdomainssipdomainsidcredentiallistmappings-get
      parameters:
      - in: path
        name: AccountSid
        description: The ID for the Twilio account
      - in: path
        name: SipDomainSid
        description: A 34 character string that uniquely identifies the SIP domain
      responses:
        200:
          description: OK
      tags:
      - SIP Domains
    post:
      summary: Add Domains Credentials
      description: Map a CredentialList to the domain.
      operationId: map-a-credentiallist-to-the-domain
      x-api-path-slug: accountsaccountsidsipdomainssipdomainsidcredentiallistmappings-post
      parameters:
      - in: path
        name: AccountSid
        description: The ID for the Twilio account
      - in: path
        name: SipDomainSid
        description: A 34 character string that uniquely identifies the SIP domain
      responses:
        200:
          description: OK
      tags:
      - SIP Domains
  /Accounts/{AccountSid}/SIP/Domains/{SipDomainSid}/IpAccessControlListMappings/{ALSid}:
    delete:
      summary: Delete Domains Credentials
      description: Remove a mapping from this domain.
      operationId: remove-a-mapping-from-this-domain
      x-api-path-slug: accountsaccountsidsipdomainssipdomainsidipaccesscontrollistmappingsalsid-delete
      parameters:
      - in: path
        name: AccountSid
        description: The ID for the Twilio account
      - in: path
        name: ALSid
      - in: path
        name: SipDomainSid
        description: A 34 character string that uniquely identifies the SIP domain
      responses:
        200:
          description: OK
      tags:
      - SIP Domains
    get:
      summary: Get Domains IP Access Control List Mappings
      description: Return a specific IpAccessControlListMapping instance by Sid.
      operationId: return-a-specific-ipaccesscontrollistmapping-instance-by-sid
      x-api-path-slug: accountsaccountsidsipdomainssipdomainsidipaccesscontrollistmappingsalsid-get
      parameters:
      - in: path
        name: AccountSid
        description: The ID for the Twilio account
      - in: path
        name: ALSid
      - in: path
        name: SipDomainSid
        description: A 34 character string that uniquely identifies the SIP domain
      responses:
        200:
          description: OK
      tags:
      - SIP Domains
  /Accounts/{AccountSid}/SIP/Domains/{SipDomainSid}/IpAccessControlListMappings:
    get:
      summary: Get Domains IP Access Control List Mapping
      description: Return the IpAccessControlListMappings that are associated to this
        domain.
      operationId: return-the-ipaccesscontrollistmappings-that-are-associated-to-this-domain
      x-api-path-slug: accountsaccountsidsipdomainssipdomainsidipaccesscontrollistmappings-get
      parameters:
      - in: path
        name: AccountSid
        description: The ID for the Twilio account
      - in: path
        name: SipDomainSid
        description: A 34 character string that uniquely identifies the SIP domain
      responses:
        200:
          description: OK
      tags:
      - SIP Domains
    post:
      summary: Add Domains IP Access Control List Mappings
      description: Map an IpAccessControlList to this domain.
      operationId: map-an-ipaccesscontrollist-to-this-domain
      x-api-path-slug: accountsaccountsidsipdomainssipdomainsidipaccesscontrollistmappings-post
      parameters:
      - in: path
        name: AccountSid
        description: The ID for the Twilio account
      - in: path
        name: SipDomainSid
        description: A 34 character string that uniquely identifies the SIP domain
      responses:
        200:
          description: OK
      tags:
      - SIP Domains
  /Accounts/{AccountSid}/SIP/Domains/{SipDomainSid}:
    delete:
      summary: Delete Domains IP Access Control List Mappings
      description: Delete a domain. If you have created subdomains of a domain, you
        will not be able to delete the domain until you first delete all subdomains
        of it.
      operationId: delete-a-domain-if-you-have-created-subdomains-of-a-domain-you-will-not-be-able-to-delete-the-domain
      x-api-path-slug: accountsaccountsidsipdomainssipdomainsid-delete
      parameters:
      - in: path
        name: AccountSid
        description: The ID for the Twilio account
      - in: path
        name: SipDomainSid
        description: A 34 character string that uniquely identifies the SIP domain
      responses:
        200:
          description: OK
      tags:
      - SIP Domains
    get:
      summary: Get Domains
      description: Return a specific instance by Sid.
      operationId: return-a-specific-instance-by-sid
      x-api-path-slug: accountsaccountsidsipdomainssipdomainsid-get
      parameters:
      - in: path
        name: AccountSid
        description: The ID for the Twilio account
      - in: path
        name: SipDomainSid
        description: A 34 character string that uniquely identifies the SIP domain
      responses:
        200:
          description: OK
      tags:
      - SIP Domains
    post:
      summary: Add Domains
      description: Update the attributes of a domain.
      operationId: update-the-attributes-of-a-domain
      x-api-path-slug: accountsaccountsidsipdomainssipdomainsid-post
      parameters:
      - in: path
        name: AccountSid
        description: The ID for the Twilio account
      - in: path
        name: SipDomainSid
        description: A 34 character string that uniquely identifies the SIP domain
      responses:
        200:
          description: OK
      tags:
      - SIP Domains
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