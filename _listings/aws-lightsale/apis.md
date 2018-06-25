---
name: AWS Lightsale
x-slug: aws-lightsale
description: Amazon Lightsail is the easiest way to get started with AWS for developers
  who just need virtual private servers. Lightsail includes everything you need to
  launch your project quickly - a virtual machine, SSD-based storage, data transfer,
  DNS management, and a static IP - for a low, predictable price. You manage those
  Lightsail servers through the Lightsail console or by using the API or command-line
  interface (CLI).
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-lightsail.png
x-kinRank: "10"
x-alexaRank: "0"
tags: Domains
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/aws-lightsale/apis.md
specificationVersion: "0.14"
apis:
- name: Amazon Lightsale API Create Domain
  x-api-slug: amazon-lightsale-api
  description: Creates a domain resource for the specified domain (e.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-lightsail.png
  humanURL: https://amazonlightsail.com/
  baseURL: ://///?Action=CreateDomain
  tags: Domains
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/aws-lightsale/actioncreatedomain-get-openapi.md
- name: Amazon Lightsale API Create Domain Entry
  x-api-slug: amazon-lightsale-api
  description: |-
    Creates one of the following entry records associated with the domain: A record, CNAME
          record, TXT record, or MX record.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-lightsail.png
  humanURL: https://amazonlightsail.com/
  baseURL: ://///?Action=CreateDomainEntry
  tags: Domains
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/aws-lightsale/actioncreatedomainentry-get-openapi.md
- name: Amazon Lightsale API Delete Domain
  x-api-slug: amazon-lightsale-api
  description: Deletes the specified domain recordset and all of its domain records.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-lightsail.png
  humanURL: https://amazonlightsail.com/
  baseURL: ://///?Action=DeleteDomain
  tags: Domains
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/aws-lightsale/actiondeletedomain-get-openapi.md
- name: Amazon Lightsale API Delete Domain Entry
  x-api-slug: amazon-lightsale-api
  description: Deletes a specific domain entry.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-lightsail.png
  humanURL: https://amazonlightsail.com/
  baseURL: ://///?Action=DeleteDomainEntry
  tags: Domains
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/aws-lightsale/actiondeletedomainentry-get-openapi.md
- name: Amazon Lightsale API Get Domain
  x-api-slug: amazon-lightsale-api
  description: Returns information about a specific domain recordset.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-lightsail.png
  humanURL: https://amazonlightsail.com/
  baseURL: ://///?Action=GetDomain
  tags: Domains
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/aws-lightsale/actiongetdomain-get-openapi.md
- name: Amazon Lightsale API Get Domains
  x-api-slug: amazon-lightsale-api
  description: Returns a list of all domains in the user's account.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-lightsail.png
  humanURL: https://amazonlightsail.com/
  baseURL: ://///?Action=GetDomains
  tags: Domains
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/aws-lightsale/actiongetdomains-get-openapi.md
- name: Amazon Lightsale API Update Domain Entry
  x-api-slug: amazon-lightsale-api
  description: Updates a domain recordset after it is created.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-lightsail.png
  humanURL: https://amazonlightsail.com/
  baseURL: ://///?Action=UpdateDomainEntry
  tags: Domains
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/aws-lightsale/actionupdatedomainentry-get-openapi.md
- name: Amazon Lightsale API
  x-api-slug: amazon-lightsale-api
  description: Amazon Lightsail is the easiest way to get started with AWS for developers
    who just need virtual private servers. Lightsail includes everything you need
    to launch your project quickly - a virtual machine, SSD-based storage, data transfer,
    DNS management, and a static IP - for a low, predictable price. You manage those
    Lightsail servers through the Lightsail console or by using the API or command-line
    interface (CLI).
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-lightsail.png
  humanURL: https://amazonlightsail.com/
  baseURL: :///
  tags: Domains
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/aws-lightsale/openapi.md
x-common:
- type: x-documentation
  url: https://docs.aws.amazon.com/lightsail/2016-11-28/api-reference/Welcome.html?fid=6DDA37DF97F08F8B-23761D4A79F7B1E
- type: x-pricing
  url: https://amazonlightsail.com/pricing/
- type: x-website
  url: https://amazonlightsail.com/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---