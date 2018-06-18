---
name: DomainTools
x-slug: domaintools
description: DomainTools helps security analysts turn threat data into threat intelligence.
  We take indicators from your network, including domains and IPs, and connect them
  with nearly every active domain on the Internet. Those connections inform risk assessments,...
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/393-domaintools.jpg
x-kinRank: "7"
x-alexaRank: "6104"
tags: Domains
created: "2018-06-18"
modified: "2018-06-18"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/domaintools/apis.md
specificationVersion: "0.14"
apis:
- name: Domain Profile API Domain Profile
  x-api-slug: domain-profile-api
  description: Basic registrant, server, and registration data for a domain name,
    plus preview data for other products
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/393-domaintools.jpg
  humanURL: http://www.domaintools.com
  baseURL: http://api.domaintools.com/v1//{domain}
  tags: Domains
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/domaintools/domain-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/domaintools/domain-get-openapi.md
- name: Domain Profile API
  x-api-slug: domain-profile-api
  description: DomainTools helps security analysts turn threat data into threat intelligence.
    We take indicators from your network, including domains and IPs, and connect them
    with nearly every active domain on the Internet. Those connections inform risk
    assessments,...
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/393-domaintools.jpg
  humanURL: http://www.domaintools.com
  baseURL: http://api.domaintools.com/v1
  tags: Domains
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/domaintools/openapi.md
- name: Domain Search API Domain Search
  x-api-slug: domain-search-api
  description: Searches active and deleted domain names that match a query string
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/393-domaintools.jpg
  humanURL: http://www.domaintools.com
  baseURL: http://api.domaintools.com//v2//domain-search/
  tags: Domains
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/domaintools/domainsearch-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/domaintools/domainsearch-get-openapi.md
- name: Domain Search API
  x-api-slug: domain-search-api
  description: DomainTools helps security analysts turn threat data into threat intelligence.
    We take indicators from your network, including domains and IPs, and connect them
    with nearly every active domain on the Internet. Those connections inform risk
    assessments,...
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/393-domaintools.jpg
  humanURL: http://www.domaintools.com
  baseURL: http://api.domaintools.com//v2
  tags: Domains
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/domaintools/openapi.md
x-common:
- type: x-base
  url: http://api.domaintools.com/
- type: x-blog-rss
  url: http://blog.domaintools.com/feed/
- type: x-crunchbase
  url: http://www.crunchbase.com/company/domain-tools
- type: x-crunchbase
  url: https://crunchbase.com/organization/domain-tools
- type: x-developer
  url: http://www.domaintools.com/api/docs/
- type: x-email
  url: sales@domaintools.com
- type: x-github
  url: https://github.com/DomainTools
- type: x-pricing
  url: https://www.domaintools.com/products/domain-research/pricing/
- type: x-twitter
  url: https://twitter.com/DomainTools
- type: x-website
  url: http://www.domaintools.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---