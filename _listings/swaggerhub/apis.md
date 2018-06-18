---
name: SwaggerHub
x-slug: swaggerhub
description: The place for teams to collaborate and coordinate the entire workflow
  of an APIs lifecycle. SwaggerHub&rsquo;s built-in editors let you rapidly create
  the Swagger definition that everything else is based on, in an intuitive interface
  that lets you write, visualize and validate all at the same time.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/SwaggerHub_Logo_Horizontal_Color.png
x-kinRank: "8"
x-alexaRank: "0"
tags: Domains
created: "2018-06-18"
modified: "2018-06-18"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/swaggerhub/apis.md
specificationVersion: "0.14"
apis:
- name: Swagger Hub Registry Retrieves a list of currently defined domains in APIs.json
    format
  x-api-slug: swagger-hub-registry
  description: Retrieves a list of currently defined domains in apis.json format.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/SwaggerHub_Logo_Horizontal_Color.png
  humanURL: http://swaggerhub.com
  baseURL: https://api.swaggerhub.com////domains
  tags: Domains
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/swaggerhub/domains-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/swaggerhub/domains-get-openapi.md
- name: Swagger Hub Registry Retrieves an APIs.json listing of all domains defined
    for this owner
  x-api-slug: swagger-hub-registry
  description: Retrieves an apis.json listing of all domains defined for this owner.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/SwaggerHub_Logo_Horizontal_Color.png
  humanURL: http://swaggerhub.com
  baseURL: https://api.swaggerhub.com////domains/{owner}
  tags: Domains,Owner
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/swaggerhub/domainsowner-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/swaggerhub/domainsowner-get-openapi.md
- name: Swagger Hub Registry Deletes the specified domain
  x-api-slug: swagger-hub-registry
  description: Deletes the specified domain.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/SwaggerHub_Logo_Horizontal_Color.png
  humanURL: http://swaggerhub.com
  baseURL: https://api.swaggerhub.com////domains/{owner}/{domain}
  tags: Domains,Owner,Domain
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/swaggerhub/domainsownerdomain-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/swaggerhub/domainsownerdomain-delete-openapi.md
- name: Swagger Hub Registry Retrieves an APIs.json listing for all domain versions
    for this owner and domain
  x-api-slug: swagger-hub-registry
  description: Retrieves an apis.json listing for all domain versions for this owner
    and domain.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/SwaggerHub_Logo_Horizontal_Color.png
  humanURL: http://swaggerhub.com
  baseURL: https://api.swaggerhub.com////domains/{owner}/{domain}
  tags: Domains,Owner,Domain
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/swaggerhub/domainsownerdomain-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/swaggerhub/domainsownerdomain-get-openapi.md
- name: Swagger Hub Registry Saves the provided Swagger definition of a domain
  x-api-slug: swagger-hub-registry
  description: Saves the provided swagger definition of a domain.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/SwaggerHub_Logo_Horizontal_Color.png
  humanURL: http://swaggerhub.com
  baseURL: https://api.swaggerhub.com////domains/{owner}/{domain}
  tags: Domains,Owner,Domain
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/swaggerhub/domainsownerdomain-post-openapi.md
- name: Swagger Hub Registry Deletes a particular version of the specified domain
  x-api-slug: swagger-hub-registry
  description: Deletes a particular version of the specified domain.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/SwaggerHub_Logo_Horizontal_Color.png
  humanURL: http://swaggerhub.com
  baseURL: https://api.swaggerhub.com////domains/{owner}/{domain}/{version}
  tags: Domains,Owner,Domain,Version
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/swaggerhub/domainsownerdomainversion-delete-openapi.md
- name: Swagger Hub Registry Retrieves the Swagger definition for the specified domain
    and version
  x-api-slug: swagger-hub-registry
  description: Retrieves the swagger definition for the specified domain and version.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/SwaggerHub_Logo_Horizontal_Color.png
  humanURL: http://swaggerhub.com
  baseURL: https://api.swaggerhub.com////domains/{owner}/{domain}/{version}
  tags: Domains,Owner,Domain,Version
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/swaggerhub/domainsownerdomainversion-get-openapi.md
- name: Swagger Hub Registry Retrieves the definition for the specified domain and
    version in JSON format
  x-api-slug: swagger-hub-registry
  description: Retrieves the definition for the specified domain and version in json
    format.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/SwaggerHub_Logo_Horizontal_Color.png
  humanURL: http://swaggerhub.com
  baseURL: https://api.swaggerhub.com////domains/{owner}/{domain}/{version}/domain.json
  tags: Domains,Owner,Domain,Version,Domain,Json
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/swaggerhub/domainsownerdomainversiondomain-json-get-openapi.md
- name: Swagger Hub Registry Retrieves the definition for the specified domain and
    version in YAML format
  x-api-slug: swagger-hub-registry
  description: Retrieves the definition for the specified domain and version in yaml
    format.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/SwaggerHub_Logo_Horizontal_Color.png
  humanURL: http://swaggerhub.com
  baseURL: https://api.swaggerhub.com////domains/{owner}/{domain}/{version}/domain.yaml
  tags: Domains,Owner,Domain,Version,Domain,Yaml
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/swaggerhub/domainsownerdomainversiondomain-yaml-get-openapi.md
- name: Swagger Hub Registry Retrieves list of domains templates
  x-api-slug: swagger-hub-registry
  description: Retrieves list of domains templates.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/SwaggerHub_Logo_Horizontal_Color.png
  humanURL: http://swaggerhub.com
  baseURL: https://api.swaggerhub.com////domains/.template
  tags: Domains,,Template
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/swaggerhub/domains-template-get-openapi.md
- name: Swagger Hub Registry Retrieves an APIs.json listing of entries referensing
    owner domains
  x-api-slug: swagger-hub-registry
  description: Retrieves an apis.json listing of entries referensing owner domains.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/SwaggerHub_Logo_Horizontal_Color.png
  humanURL: http://swaggerhub.com
  baseURL: https://api.swaggerhub.com////domains/{owner}/.refs
  tags: Domains,Owner,,Refs
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/swaggerhub/domainsowner-refs-get-openapi.md
- name: Swagger Hub Registry Renames domain
  x-api-slug: swagger-hub-registry
  description: Renames domain.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/SwaggerHub_Logo_Horizontal_Color.png
  humanURL: http://swaggerhub.com
  baseURL: https://api.swaggerhub.com////domains/{owner}/{domain}/.newname
  tags: Domains,Owner,Domain,,Newname
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/swaggerhub/domainsownerdomain-newname-post-openapi.md
- name: Swagger Hub Registry transfers domain to another owner
  x-api-slug: swagger-hub-registry
  description: Transfers domain to another owner.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/SwaggerHub_Logo_Horizontal_Color.png
  humanURL: http://swaggerhub.com
  baseURL: https://api.swaggerhub.com////domains/{owner}/{domain}/.transfer
  tags: Domains,Owner,Domain,,Transfer
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/swaggerhub/domainsownerdomain-transfer-post-openapi.md
- name: Swagger Hub Registry Adds domain version
  x-api-slug: swagger-hub-registry
  description: Adds domain version.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/SwaggerHub_Logo_Horizontal_Color.png
  humanURL: http://swaggerhub.com
  baseURL: https://api.swaggerhub.com////domains/{owner}/{domain}/{version}/.bump
  tags: Domains,Owner,Domain,Version,,Bump
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/swaggerhub/domainsownerdomainversion-bump-post-openapi.md
- name: Swagger Hub Registry Returns the list of comments for the specified domain
  x-api-slug: swagger-hub-registry
  description: Returns the list of comments for the specified domain.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/SwaggerHub_Logo_Horizontal_Color.png
  humanURL: http://swaggerhub.com
  baseURL: https://api.swaggerhub.com////domains/{owner}/{domain}/{version}/.comment
  tags: Domains,Owner,Domain,Version,,Comment
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/swaggerhub/domainsownerdomainversion-comment-get-openapi.md
- name: Swagger Hub Registry Adds a new comment to the specified domain
  x-api-slug: swagger-hub-registry
  description: Adds a new comment to the specified domain.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/SwaggerHub_Logo_Horizontal_Color.png
  humanURL: http://swaggerhub.com
  baseURL: https://api.swaggerhub.com////domains/{owner}/{domain}/{version}/.comment
  tags: Domains,Owner,Domain,Version,,Comment
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/swaggerhub/domainsownerdomainversion-comment-post-openapi.md
- name: Swagger Hub Registry Updates passed batch of comments
  x-api-slug: swagger-hub-registry
  description: Updates passed batch of comments.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/SwaggerHub_Logo_Horizontal_Color.png
  humanURL: http://swaggerhub.com
  baseURL: https://api.swaggerhub.com////domains/{owner}/{domain}/{version}/.comment/batch
  tags: Domains,Owner,Domain,Version,,Comment,Batch
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/swaggerhub/domainsownerdomainversion-commentbatch-post-openapi.md
- name: Swagger Hub Registry Deletes specified comment
  x-api-slug: swagger-hub-registry
  description: Deletes specified comment.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/SwaggerHub_Logo_Horizontal_Color.png
  humanURL: http://swaggerhub.com
  baseURL: https://api.swaggerhub.com////domains/{owner}/{domain}/{version}/.comment/{comment}
  tags: Domains,Owner,Domain,Version,,Comment,Comment
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/swaggerhub/domainsownerdomainversion-commentcomment-delete-openapi.md
- name: Swagger Hub Registry Updates specified comment
  x-api-slug: swagger-hub-registry
  description: Updates specified comment.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/SwaggerHub_Logo_Horizontal_Color.png
  humanURL: http://swaggerhub.com
  baseURL: https://api.swaggerhub.com////domains/{owner}/{domain}/{version}/.comment/{comment}
  tags: Domains,Owner,Domain,Version,,Comment,Comment
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/swaggerhub/domainsownerdomainversion-commentcomment-patch-openapi.md
- name: Swagger Hub Registry Adds a new reply to the specified comment
  x-api-slug: swagger-hub-registry
  description: Adds a new reply to the specified comment.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/SwaggerHub_Logo_Horizontal_Color.png
  humanURL: http://swaggerhub.com
  baseURL: https://api.swaggerhub.com////domains/{owner}/{domain}/{version}/.comment/{comment}/reply
  tags: Domains,Owner,Domain,Version,,Comment,Comment,Reply
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/swaggerhub/domainsownerdomainversion-commentcommentreply-post-openapi.md
- name: Swagger Hub Registry Deletes specified comment reply
  x-api-slug: swagger-hub-registry
  description: Deletes specified comment reply.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/SwaggerHub_Logo_Horizontal_Color.png
  humanURL: http://swaggerhub.com
  baseURL: https://api.swaggerhub.com////domains/{owner}/{domain}/{version}/.comment/{comment}/reply/{reply}
  tags: Domains,Owner,Domain,Version,,Comment,Comment,Reply,Reply
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/swaggerhub/domainsownerdomainversion-commentcommentreplyreply-delete-openapi.md
- name: Swagger Hub Registry Updates specified comment reply
  x-api-slug: swagger-hub-registry
  description: Updates specified comment reply.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/SwaggerHub_Logo_Horizontal_Color.png
  humanURL: http://swaggerhub.com
  baseURL: https://api.swaggerhub.com////domains/{owner}/{domain}/{version}/.comment/{comment}/reply/{reply}
  tags: Domains,Owner,Domain,Version,,Comment,Comment,Reply,Reply
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/swaggerhub/domainsownerdomainversion-commentcommentreplyreply-patch-openapi.md
- name: Swagger Hub Registry Updates status to the specified comment
  x-api-slug: swagger-hub-registry
  description: Updates status to the specified comment.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/SwaggerHub_Logo_Horizontal_Color.png
  humanURL: http://swaggerhub.com
  baseURL: https://api.swaggerhub.com////domains/{owner}/{domain}/{version}/.comment/{comment}/status/{status}
  tags: Domains,Owner,Domain,Version,,Comment,Comment,Status,Status
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/swaggerhub/domainsownerdomainversion-commentcommentstatusstatus-put-openapi.md
- name: Swagger Hub Registry Deletes a particular version of the specified Domain
  x-api-slug: swagger-hub-registry
  description: Deletes a particular version of the specified domain.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/SwaggerHub_Logo_Horizontal_Color.png
  humanURL: http://swaggerhub.com
  baseURL: https://api.swaggerhub.com////domains/{owner}/{domain}/{version}/.draft
  tags: Domains,Owner,Domain,Version,,Draft
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/swaggerhub/domainsownerdomainversion-draft-delete-openapi.md
- name: Swagger Hub Registry Retrieves the draft for the specified domain
  x-api-slug: swagger-hub-registry
  description: Retrieves the draft for the specified domain.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/SwaggerHub_Logo_Horizontal_Color.png
  humanURL: http://swaggerhub.com
  baseURL: https://api.swaggerhub.com////domains/{owner}/{domain}/{version}/.draft
  tags: Domains,Owner,Domain,Version,,Draft
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/swaggerhub/domainsownerdomainversion-draft-get-openapi.md
- name: Swagger Hub Registry Saves the provided draft for a domain.
  x-api-slug: swagger-hub-registry
  description: Saves the provided draft for a domain..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/SwaggerHub_Logo_Horizontal_Color.png
  humanURL: http://swaggerhub.com
  baseURL: https://api.swaggerhub.com////domains/{owner}/{domain}/{version}/.draft
  tags: Domains,Owner,Domain,Version,,Draft
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/swaggerhub/domainsownerdomainversion-draft-put-openapi.md
- name: Swagger Hub Registry Forks the provided domain definition
  x-api-slug: swagger-hub-registry
  description: Forks the provided domain definition.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/SwaggerHub_Logo_Horizontal_Color.png
  humanURL: http://swaggerhub.com
  baseURL: https://api.swaggerhub.com////domains/{owner}/{domain}/{version}/.fork
  tags: Domains,Owner,Domain,Version,,Fork
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/swaggerhub/domainsownerdomainversion-fork-post-openapi.md
- name: Swagger Hub Registry Creates Domain by template
  x-api-slug: swagger-hub-registry
  description: Creates domain by template.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/SwaggerHub_Logo_Horizontal_Color.png
  humanURL: http://swaggerhub.com
  baseURL: https://api.swaggerhub.com////domains/{owner}/{domain}/{version}/.template
  tags: Domains,Owner,Domain,Version,,Template
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/swaggerhub/domainsownerdomainversion-template-post-openapi.md
- name: Swagger Hub Registry
  x-api-slug: swagger-hub-registry
  description: The place for teams to collaborate and coordinate the entire workflow
    of an APIs lifecycle. SwaggerHub&rsquo;s built-in editors let you rapidly create
    the Swagger definition that everything else is based on, in an intuitive interface
    that lets you write, visualize and validate all at the same time.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/SwaggerHub_Logo_Horizontal_Color.png
  humanURL: http://swaggerhub.com
  baseURL: https://api.swaggerhub.com//
  tags: Domains
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/swaggerhub/openapi.md
x-common:
- type: x-github
  url: https://github.com/swagger-hub
- type: x-twitter
  url: https://twitter.com/swaggerhub
- type: x-website
  url: http://swaggerhub.com
- type: x-website
  url: https://swaggerhub.com/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---