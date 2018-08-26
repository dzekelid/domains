---
name: AWS Elasticsearch Service
x-slug: aws-elasticsearch-service
description: Amazon Elasticsearch Service makes it easy to deploy, operate, and scale
  Elasticsearch for log analytics, full text search, application monitoring, and more.
  Amazon Elasticsearch Service is a fully managed service that delivers Elasticsearch&rsquo;s
  easy-to-use APIs and real-time capabilities along with the availability, scalability,
  and security required by production workloads. The service offers built-in integrations
  with Kibana, Logstash, and AWS services including Amazon Kinesis Firehose, AWS Lambda,
  and Amazon CloudWatch so that you can go from raw data to actionable insights quickly.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Analytics_AmazonElasticsearchService.png
x-kinRank: "10"
x-alexaRank: "0"
tags: Domains
created: "2018-08-25"
modified: "2018-08-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/aws-elasticsearch-service/apis.md
specificationVersion: "0.14"
apis:
- name: AWS Elasticsearch Service API - Create Elasticsearch Domain
  x-api-slug: 20150101esdomain-post
  description: |-
    Creates a new Amazon ES domain. Use the HTTP POST method with this
                    operation. For more information, see Creating Amazon ES Domains.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Analytics_AmazonElasticsearchService.png
  humanURL: https://aws.amazon.com/elasticsearch-service/
  baseURL: :///
  tags: Amazon Web Services, Search, Logging, Documents, Stack Network, API Service
    Provider, API Service Provider, API Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/aws-elasticsearch-service/20150101esdomain-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/aws-elasticsearch-service/20150101esdomain-post-openapi.md
- name: AWS Elasticsearch Service API - Delete Elasticsearch Domain
  x-api-slug: 20150101esdomaindomain-name-delete
  description: |-
    Deletes an Amazon ES domain and all of its data. A domain cannot be recovered after it
                    is deleted. Use the DELETE HTTP method with this operation.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Analytics_AmazonElasticsearchService.png
  humanURL: https://aws.amazon.com/elasticsearch-service/
  baseURL: :///
  tags: Amazon Web Services, Search, Logging, Documents, Stack Network, API Service
    Provider, API Service Provider, API Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/aws-elasticsearch-service/20150101esdomaindomain-name-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/aws-elasticsearch-service/20150101esdomaindomain-name-delete-openapi.md
- name: AWS Elasticsearch Service API - Add Tags
  x-api-slug: 20150101tags-post
  description: |-
    Attaches resource tags to an Amazon ES domain. Use the POST HTTP method
                    with this operation. For more information, see Tagging Amazon ES
                    Domains.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Analytics_AmazonElasticsearchService.png
  humanURL: https://aws.amazon.com/elasticsearch-service/
  baseURL: :///
  tags: Amazon Web Services, Search, Logging, Documents, Stack Network, API Service
    Provider, API Service Provider, API Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/aws-elasticsearch-service/20150101tags-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/aws-elasticsearch-service/20150101tags-post-openapi.md
x-common:
- type: x-api-gallery
  url: http://aws.elasticache.api.gallery.streamdata.io
- type: x-api-stack
  url: http://aws.elasticsearch.service.stack.network
- type: x-console
  url: https://console.aws.amazon.com/es/home?region=us-east-1
- type: x-documentation
  url: http://docs.aws.amazon.com/elasticsearch-service/latest/developerguide/es-configuration-api.html
- type: x-faq
  url: https://aws.amazon.com/elasticsearch-service/faqs/
- type: x-getting-started
  url: https://aws.amazon.com/elasticsearch-service/getting-started/
- type: x-pricing
  url: https://aws.amazon.com/elasticsearch-service/pricing/
- type: x-website
  url: https://aws.amazon.com/elasticsearch-service/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---