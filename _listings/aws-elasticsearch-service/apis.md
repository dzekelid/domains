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
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/aws-elasticsearch-service/apis.md
specificationVersion: "0.14"
apis:
- name: Amazon Elasticsearch Service API Create Elasticsearch Domain
  x-api-slug: amazon-elasticsearch-service-api
  description: |-
    Creates a new Amazon ES domain. Use the HTTP POST method with this
                    operation. For more information, see Creating Amazon ES Domains.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Analytics_AmazonElasticsearchService.png
  humanURL: https://aws.amazon.com/elasticsearch-service/
  baseURL: ://///2015-01-01/es/domain
  tags: Domains
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/aws-elasticsearch-service/20150101esdomain-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/aws-elasticsearch-service/20150101esdomain-post-openapi.md
- name: Amazon Elasticsearch Service API Delete Elasticsearch Domain
  x-api-slug: amazon-elasticsearch-service-api
  description: |-
    Deletes an Amazon ES domain and all of its data. A domain cannot be recovered after it
                    is deleted. Use the DELETE HTTP method with this operation.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Analytics_AmazonElasticsearchService.png
  humanURL: https://aws.amazon.com/elasticsearch-service/
  baseURL: ://///2015-01-01/es/domain/{domain_name}
  tags: Domains
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/aws-elasticsearch-service/20150101esdomaindomain-name-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/aws-elasticsearch-service/20150101esdomaindomain-name-delete-openapi.md
- name: Amazon Elasticsearch Service API Describe Elasticsearch Domain
  x-api-slug: amazon-elasticsearch-service-api
  description: |-
    Describes the domain configuration for the specified Amazon ES domain, including the
                    domain ID, domain service endpoint, and domain ARN. Use the HTTP GET
                    method with this operation.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Analytics_AmazonElasticsearchService.png
  humanURL: https://aws.amazon.com/elasticsearch-service/
  baseURL: ://///2015-01-01/es/domain/{domain_name}
  tags: Domains
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/aws-elasticsearch-service/20150101esdomaindomain-name-get-openapi.md
- name: Amazon Elasticsearch Service API Describe Elasticsearch Domains
  x-api-slug: amazon-elasticsearch-service-api
  description: |-
    Describes the domain configuration for up to five specified Amazon ES domains.
                    Information includes the domain ID, domain service endpoint, and domain ARN. Use the
                    HTTP POST method with this operation.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Analytics_AmazonElasticsearchService.png
  humanURL: https://aws.amazon.com/elasticsearch-service/
  baseURL: ://///2015-01-01/es/domain-info
  tags: Domains
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/aws-elasticsearch-service/20150101esdomaininfo-post-openapi.md
- name: Amazon Elasticsearch Service API List Domain Names
  x-api-slug: amazon-elasticsearch-service-api
  description: Displays the names of all Amazon ES domains owned by the current user.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Analytics_AmazonElasticsearchService.png
  humanURL: https://aws.amazon.com/elasticsearch-service/
  baseURL: ://///2015-01-01/domain
  tags: Domains
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/aws-elasticsearch-service/20150101domain-get-openapi.md
- name: Amazon Elasticsearch Service API Describe Elasticsearch Domain Config
  x-api-slug: amazon-elasticsearch-service-api
  description: |-
    Displays the configuration of an Amazon ES domain. Use the HTTP GET method
                    with this operation.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Analytics_AmazonElasticsearchService.png
  humanURL: https://aws.amazon.com/elasticsearch-service/
  baseURL: ://///2015-01-01/es/domain/{domain_name}/config
  tags: Domains
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/aws-elasticsearch-service/20150101esdomaindomain-nameconfig-get-openapi.md
- name: Amazon Elasticsearch Service API Update Elasticsearch Domain Config
  x-api-slug: amazon-elasticsearch-service-api
  description: |-
    Modifies the configuration of an Amazon ES domain, such as the instance type and the
                    number of instances. Use the POST HTTP method with this
                    operation.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Analytics_AmazonElasticsearchService.png
  humanURL: https://aws.amazon.com/elasticsearch-service/
  baseURL: ://///2015-01-01/es/domain/{domain_name}/config
  tags: Domains
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/aws-elasticsearch-service/20150101esdomaindomain-nameconfig-post-openapi.md
- name: Amazon Elasticsearch Service API
  x-api-slug: amazon-elasticsearch-service-api
  description: Amazon Elasticsearch Service makes it easy to deploy, operate, and
    scale Elasticsearch for log analytics, full text search, application monitoring,
    and more. Amazon Elasticsearch Service is a fully managed service that delivers
    Elasticsearch&rsquo;s easy-to-use APIs and real-time capabilities along with the
    availability, scalability, and security required by production workloads. The
    service offers built-in integrations with Kibana, Logstash, and AWS services including
    Amazon Kinesis Firehose, AWS Lambda, and Amazon CloudWatch so that you can go
    from raw data to actionable insights quickly.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Analytics_AmazonElasticsearchService.png
  humanURL: https://aws.amazon.com/elasticsearch-service/
  baseURL: :///
  tags: Domains
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/aws-elasticsearch-service/openapi.md
x-common:
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