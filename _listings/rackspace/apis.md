---
name: Rackspace
x-slug: rackspace
description: Host on our dedicated or cloud infrastructure or through one of our partners.
  Leverage our expertise to run fast and lean. We offer web, app or email hosting,
  data services and managed security solutions.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/241-rackspace.jpg
x-kinRank: "9"
x-alexaRank: "4115"
tags: Domains
created: "2018-06-18"
modified: "2018-06-18"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/rackspace/apis.md
specificationVersion: "0.14"
apis:
- name: Rackspace List domains
  x-api-slug: rackspace
  description: |-
    These calls provide a list of all DNS domains manageable by a given account.
    The resulting list is flat, and does not break the domains down hierarchically
    by subdomain. All representative domains are included in the list, even if a
    domain is conceptually a subdomain of another domain in the list.Note
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/241-rackspace.jpg
  humanURL: http://www.rackspace.com/
  baseURL: |
    https://///v1.0/{account}/domains
  tags: Domains
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/rackspace/v1-0accountdomains-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/rackspace/v1-0accountdomains-get-openapi.md
- name: Rackspace Create domain
  x-api-slug: rackspace
  description: |-
    NoteThis call returns an asynchronous response, See
    Synchronous and asynchronous responses
    for more details and examples of the way that asynchronous responses work.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/241-rackspace.jpg
  humanURL: http://www.rackspace.com/
  baseURL: |
    https://///v1.0/{account}/domains
  tags: Domains
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/rackspace/v1-0accountdomains-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/rackspace/v1-0accountdomains-post-openapi.md
- name: Rackspace Update domains
  x-api-slug: rackspace
  description: |-
    NoteThis call returns an asynchronous response, as described in
    Synchronous and asynchronous responses.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/241-rackspace.jpg
  humanURL: http://www.rackspace.com/
  baseURL: |
    https://///v1.0/{account}/domains
  tags: Domains
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/rackspace/v1-0accountdomains-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/rackspace/v1-0accountdomains-put-openapi.md
- name: Rackspace Delete domains
  x-api-slug: rackspace
  description: |-
    NoteThis call returns an asynchronous response, as described in
    Synchronous and asynchronous responses.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/241-rackspace.jpg
  humanURL: http://www.rackspace.com/
  baseURL: |
    https://///v1.0/{account}/domains
  tags: Domains
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/rackspace/v1-0accountdomains-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/rackspace/v1-0accountdomains-delete-openapi.md
- name: Rackspace Search domains
  x-api-slug: rackspace
  description: 'NoteFilter criteria may consist of:'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/241-rackspace.jpg
  humanURL: http://www.rackspace.com/
  baseURL: |
    https://///v1.0/{account}/domains/search
  tags: Domains
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/rackspace/v1-0accountdomainssearch-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/rackspace/v1-0accountdomainssearch-get-openapi.md
- name: Rackspace List domain details without subdomains
  x-api-slug: rackspace
  description: |-
    This call provides the detailed output for a specified domain configured and
    associated with an account. This call is not capable of returning details for a
    domain that has been deleted.This call does not require a request body.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/241-rackspace.jpg
  humanURL: http://www.rackspace.com/
  baseURL: |
    https://///v1.0/{account}/domains/{domainId}
  tags: Domains
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/rackspace/v1-0accountdomainsdomainid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/rackspace/v1-0accountdomainsdomainid-get-openapi.md
- name: Rackspace Update domain
  x-api-slug: rackspace
  description: |-
    NoteThis call returns an asynchronous response. Refer to
    Synchronous and asynchronous responses
    for more details and examples of the way that asynchronous responses work.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/241-rackspace.jpg
  humanURL: http://www.rackspace.com/
  baseURL: |
    https://///v1.0/{account}/domains/{domainId}
  tags: Domains
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/rackspace/v1-0accountdomainsdomainid-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/rackspace/v1-0accountdomainsdomainid-put-openapi.md
- name: Rackspace Delete domain
  x-api-slug: rackspace
  description: |-
    NoteThis call returns an asynchronous response, as described in
    Synchronous and asynchronous responses.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/241-rackspace.jpg
  humanURL: http://www.rackspace.com/
  baseURL: |
    https://///v1.0/{account}/domains/{domainId}
  tags: Domains
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/rackspace/v1-0accountdomainsdomainid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/rackspace/v1-0accountdomainsdomainid-delete-openapi.md
- name: Rackspace Show domain changes
  x-api-slug: rackspace
  description: |-
    This call shows all changes to a specified domain since a specified
    date/time. The since parameter is optional and defaults to midnight of the
    current day. See Date/Time format for details on how
    to specify this parameter's value.The examples below show the requests and corresponding responses to list the
    domain changes since midnight, GMT-5, on September 13, 2011.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/241-rackspace.jpg
  humanURL: http://www.rackspace.com/
  baseURL: |
    https://///v1.0/{account}/domains/{domainId}/changes
  tags: Domains
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/rackspace/v1-0accountdomainsdomainidchanges-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/rackspace/v1-0accountdomainsdomainidchanges-get-openapi.md
- name: Rackspace Export domain
  x-api-slug: rackspace
  description: |-
    NoteThis call returns an asynchronous response. Refer to
    Synchronous and asynchronous responses.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/241-rackspace.jpg
  humanURL: http://www.rackspace.com/
  baseURL: |
    https://///v1.0/{account}/domains/{domainId}/export
  tags: Domains
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/rackspace/v1-0accountdomainsdomainidexport-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/rackspace/v1-0accountdomainsdomainidexport-get-openapi.md
- name: Rackspace Clone domain
  x-api-slug: rackspace
  description: |-
    Creates a specified domain ( example2.com ) by cloning a domain with id
    domainId. All options except cloneName assume a default value of true.Note
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/241-rackspace.jpg
  humanURL: http://www.rackspace.com/
  baseURL: |
    https://///v1.0/{account}/domains/{domainId}/clone
  tags: Domains
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/rackspace/v1-0accountdomainsdomainidclone-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/rackspace/v1-0accountdomainsdomainidclone-post-openapi.md
- name: Rackspace Import domain
  x-api-slug: rackspace
  description: |-
    NoteThis call returns an asynchronous response, as described in
    Synchronous and asynchronous responses.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/241-rackspace.jpg
  humanURL: http://www.rackspace.com/
  baseURL: |
    https://///v1.0/{account}/domains/import
  tags: Domains
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/rackspace/v1-0accountdomainsimport-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/rackspace/v1-0accountdomainsimport-post-openapi.md
- name: Rackspace List subdomains
  x-api-slug: rackspace
  description: |-
    This call provides a list of all DNS domains that are subdomains for a
    specified domain. The resulting list is flat, and does not break the domains
    down hierarchically by subdomain.Note
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/241-rackspace.jpg
  humanURL: http://www.rackspace.com/
  baseURL: |
    https://///v1.0/{account}/domains/{domainId}/subdomains
  tags: Subdomains
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/rackspace/v1-0accountdomainsdomainidsubdomains-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/rackspace/v1-0accountdomainsdomainidsubdomains-get-openapi.md
- name: Rackspace
  x-api-slug: rackspace
  description: Host on our dedicated or cloud infrastructure or through one of our
    partners. Leverage our expertise to run fast and lean. We offer web, app or email
    hosting, data services and managed security solutions.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/241-rackspace.jpg
  humanURL: http://www.rackspace.com/
  baseURL: https:///
  tags: Domains
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/rackspace/openapi.md
x-common:
- type: x-base
  url: https://dfw.servers.api.rackspacecloud.com/
- type: x-blog
  url: http://www.rackspace.com/blog/
- type: x-blog-rss
  url: http://www.rackspace.com/blog/feed/rss/
- type: x-crunchbase
  url: http://www.crunchbase.com/company/rackspace
- type: x-crunchbase
  url: https://crunchbase.com/organization/rackspace
- type: x-developer
  url: http://docs.rackspace.com/
- type: x-email
  url: abuse@rackspace.com
- type: x-email
  url: abuse@rackspace.co.uk
- type: x-email
  url: legalnotice@rackspace.com
- type: x-email
  url: rackspacepartners@rackspace.com
- type: x-email
  url: channel@rackspace.co.uk
- type: x-email
  url: asia.partner@rackspace.com
- type: x-email
  url: anz.partner@rackspace.com
- type: x-email
  url: publicrelations@rackspace.com
- type: x-email
  url: michael.house@rackspace.co.uk
- type: x-email
  url: daniela.jimenezparke@rackspace.com
- type: x-github
  url: https://github.com/rackspace
- type: x-pricing
  url: https://www.rackspace.com/calculator
- type: x-twitter
  url: https://twitter.com/rackspace
- type: x-website
  url: http://www.rackspace.com/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---