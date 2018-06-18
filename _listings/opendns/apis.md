---
name: OpenDNS
x-slug: opendns
description: OpenDNS was founded in 2006 and acquired by Cisco in 2015. Today, more
  than 12,000 business worldwide rely on our enterprise security products. Cisco Umbrella
  is a cloud security platform that provides the first line of defense against threats
  on the i...
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20022-opendns.jpg
x-kinRank: "8"
x-alexaRank: "4178"
tags: Domains
created: "2018-06-18"
modified: "2018-06-18"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/opendns/apis.md
specificationVersion: "0.14"
apis:
- name: OpenDNS Domain Status and Categorization
  x-api-slug: opendns
  description: This API method returns the domain status, which the quickest and easiest
    way to know whether a domain has been flagged as malicious by the OpenDNS Security
    Labs team (score of -1 for status), if it is believed to be safe (score of 1),
    or if it has yet to be given a status (score of 0).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20022-opendns.jpg
  humanURL: https://www.opendns.com/
  baseURL: https://///domains/categories/
  tags: Domains
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/opendns/domainscategories-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/opendns/domainscategories-get-openapi.md
- name: OpenDNS Co-Occurrences for a Domain
  x-api-slug: opendns
  description: This API method returns a list of co-occurences for the specified domain.
    A co-occurrence is when two or more domains are being accessed by the same users
    within a small window of time. Being a co-occurrence isn't necessarily a bad thing,
    legitimate sites co-occur with each other as a part of normal web activity. However,
    unusual or suspicious co-occurence can provide additional information regarding
    attacks.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20022-opendns.jpg
  humanURL: https://www.opendns.com/
  baseURL: https://///recommendations/{name}/
  tags: Domains
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/opendns/recommendationsname-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/opendns/recommendationsname-get-openapi.md
- name: OpenDNS Related Domains
  x-api-slug: opendns
  description: This API method returns a list of domain names that have been frequently
    seen requested b around the same time (up to 60 seconds before or after) as the
    given domain name, but that are not frequently associated with other domain names.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20022-opendns.jpg
  humanURL: https://www.opendns.com/
  baseURL: https://///links/{name}/
  tags: Related Domains
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/opendns/linksname-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/opendns/linksname-get-openapi.md
- name: OpenDNS Latest Malicious Domains
  x-api-slug: opendns
  description: "The latest_domains endpoint shows whether the IP address you\u2019ve
    entered as input has any known malicious domains associated with it."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20022-opendns.jpg
  humanURL: https://www.opendns.com/
  baseURL: https://///ips/{ip}/latest_domains
  tags: Malicious Domains
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/opendns/ipsiplatest-domains-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/opendns/ipsiplatest-domains-get-openapi.md
- name: OpenDNS Get Domains
  x-api-slug: opendns
  description: "To gather the lists of domains already added to the shared customer\u2019s
    domain list, run a GET request against the domains endpoint of the API."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20022-opendns.jpg
  humanURL: https://www.opendns.com/
  baseURL: https://///domains
  tags: Domains
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/opendns/domains-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/opendns/domains-get-openapi.md
- name: OpenDNS Delete Domain
  x-api-slug: opendns
  description: "To delete a domain from the shared customer\u2019s domain list, run
    a DELETE request against the domains endpoint of the API."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20022-opendns.jpg
  humanURL: https://www.opendns.com/
  baseURL: https://///domains
  tags: Domains
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/opendns/domains-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/opendns/domains-delete-openapi.md
- name: OpenDNS
  x-api-slug: opendns
  description: OpenDNS was founded in 2006 and acquired by Cisco in 2015. Today, more
    than 12,000 business worldwide rely on our enterprise security products. Cisco
    Umbrella is a cloud security platform that provides the first line of defense
    against threats on the i...
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20022-opendns.jpg
  humanURL: https://www.opendns.com/
  baseURL: https:///
  tags: Domains
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/opendns/openapi.md
x-common:
- type: x-blog
  url: https://blog.opendns.com/
- type: x-blog-rss
  url: https://blog.opendns.com/feed/
- type: x-crunchbase
  url: https://crunchbase.com/organization/opendns
- type: x-developer
  url: https://docs.opendns.com/
- type: x-email
  url: support@opendns.com
- type: x-github
  url: https://github.com/opendns
- type: x-twitter
  url: https://twitter.com/OpenDNS
- type: x-website
  url: https://www.opendns.com/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---