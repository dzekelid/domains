---
swagger: "2.0"
x-collection-name: Swagger
x-complete: 1
info:
  title: Swagger Hub Registry
  description: the-registry-api-for-swaggerhub
  contact:
    name: SwaggerHub
    url: http://swaggerhub.com
    email: info@swaggerhub.com
  version: 1.0.45
host: api.swaggerhub.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /domains:
    get:
      summary: Retrieves a list of currently defined domains in APIs.json format
      description: Retrieves a list of currently defined domains in apis.json format.
      operationId: searchDomains
      x-api-path-slug: domains-get
      parameters:
      - in: query
        name: limit
        description: number of results per page
      - in: query
        name: order
        description: sort order
      - in: query
        name: page
        description: page to return
      - in: query
        name: query
        description: free text query to match
      - in: query
        name: sort
        description: sort criteria or result set* NAME -* UPATED* CREATED* OWNER
      - in: query
        name: state
        description: matches against published state of the spec* UNPUBLISHED - spec
          is a draft, a work in progress* PUBLISHED - spec is a stable version ready
          for consuming from client applications* ANY - either PUBLISHED or UNPUBLISHED
      - in: query
        name: tag
        description: matches against tags associated with a domain
      responses:
        200:
          description: OK
      tags:
      - Domains
  /domains/{owner}:
    get:
      summary: Retrieves an APIs.json listing of all domains defined for this owner
      description: Retrieves an apis.json listing of all domains defined for this
        owner.
      operationId: getOwnerDomains
      x-api-path-slug: domainsowner-get
      parameters:
      - in: query
        name: limit
        description: number of results per page
      - in: query
        name: order
        description: sort order
      - in: path
        name: owner
        description: API or Domaion owner identifier
      - in: query
        name: page
        description: page to return
      - in: query
        name: sort
        description: sort criteria or result set* NAME -* UPATED* CREATED* OWNER
      responses:
        200:
          description: OK
      tags:
      - Domains
      - Owner
  /domains/{owner}/{domain}:
    delete:
      summary: Deletes the specified domain
      description: Deletes the specified domain.
      operationId: deleteDomain
      x-api-path-slug: domainsownerdomain-delete
      parameters:
      - in: path
        name: domain
        description: domain identifier
      - in: query
        name: force
        description: force update
      - in: path
        name: owner
        description: API or Domaion owner identifier
      responses:
        200:
          description: OK
      tags:
      - Domains
      - Owner
      - Domain
    get:
      summary: Retrieves an APIs.json listing for all domain versions for this owner
        and domain
      description: Retrieves an apis.json listing for all domain versions for this
        owner and domain.
      operationId: getDomainVersions
      x-api-path-slug: domainsownerdomain-get
      parameters:
      - in: path
        name: domain
        description: domain identifier
      - in: path
        name: owner
        description: API or Domaion owner identifier
      responses:
        200:
          description: OK
      tags:
      - Domains
      - Owner
      - Domain
    post:
      summary: Saves the provided Swagger definition of a domain
      description: Saves the provided swagger definition of a domain.
      operationId: saveDomainDefinition
      x-api-path-slug: domainsownerdomain-post
      parameters:
      - in: body
        name: definition
        description: the Swagger definition of this Domain
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: domain
        description: domain identifier
      - in: query
        name: force
        description: force update
      - in: query
        name: isPrivate
        description: Defines whether the API has to be private
      - in: path
        name: owner
        description: API or Domaion owner identifier
      - in: query
        name: version
        description: domain version
      responses:
        200:
          description: OK
      tags:
      - Domains
      - Owner
      - Domain
  /domains/{owner}/{domain}/{version}:
    delete:
      summary: Deletes a particular version of the specified domain
      description: Deletes a particular version of the specified domain.
      operationId: deleteDomainVersion
      x-api-path-slug: domainsownerdomainversion-delete
      parameters:
      - in: path
        name: domain
        description: domain identifier
      - in: query
        name: force
        description: force update
      - in: path
        name: owner
        description: API or Domaion owner identifier
      - in: path
        name: version
        description: version identifier
      responses:
        200:
          description: OK
      tags:
      - Domains
      - Owner
      - Domain
      - Version
    get:
      summary: Retrieves the Swagger definition for the specified domain and version
      description: Retrieves the swagger definition for the specified domain and version.
      operationId: getDomainDefinition
      x-api-path-slug: domainsownerdomainversion-get
      parameters:
      - in: path
        name: domain
        description: domain identifier
      - in: path
        name: owner
        description: API or Domaion owner identifier
      - in: path
        name: version
        description: version identifier
      responses:
        200:
          description: OK
      tags:
      - Domains
      - Owner
      - Domain
      - Version
  /domains/{owner}/{domain}/{version}/domain.json:
    get:
      summary: Retrieves the definition for the specified domain and version in JSON
        format
      description: Retrieves the definition for the specified domain and version in
        json format.
      operationId: getDomainJsonDefinition
      x-api-path-slug: domainsownerdomainversiondomain-json-get
      parameters:
      - in: path
        name: domain
        description: domain identifier
      - in: path
        name: owner
        description: API or Domaion owner identifier
      - in: path
        name: version
        description: version identifier
      responses:
        200:
          description: OK
      tags:
      - Domains
      - Owner
      - Domain
      - Version
      - Domain
      - Json
  /domains/{owner}/{domain}/{version}/domain.yaml:
    get:
      summary: Retrieves the definition for the specified domain and version in YAML
        format
      description: Retrieves the definition for the specified domain and version in
        yaml format.
      operationId: getDomainYamlDefinition
      x-api-path-slug: domainsownerdomainversiondomain-yaml-get
      parameters:
      - in: path
        name: domain
        description: domain identifier
      - in: path
        name: owner
        description: API or Domaion owner identifier
      - in: path
        name: version
        description: version identifier
      responses:
        200:
          description: OK
      tags:
      - Domains
      - Owner
      - Domain
      - Version
      - Domain
      - Yaml
  /domains/.template:
    get:
      summary: Retrieves list of domains templates
      description: Retrieves list of domains templates.
      operationId: getDomainTemplates
      x-api-path-slug: domains-template-get
      responses:
        200:
          description: OK
      tags:
      - Domains
      - ""
      - Template
  /domains/{owner}/.refs:
    get:
      summary: Retrieves an APIs.json listing of entries referensing owner domains
      description: Retrieves an apis.json listing of entries referensing owner domains.
      operationId: getOwnerReferences
      x-api-path-slug: domainsowner-refs-get
      parameters:
      - in: path
        name: owner
        description: API owner identifier
      responses:
        200:
          description: OK
      tags:
      - Domains
      - Owner
      - ""
      - Refs
  /domains/{owner}/{domain}/.newname:
    post:
      summary: Renames domain
      description: Renames domain.
      operationId: renameDomain
      x-api-path-slug: domainsownerdomain-newname-post
      parameters:
      - in: path
        name: domain
        description: domain identifier
      - in: query
        name: force
        description: force update
      - in: query
        name: newName
        description: New name
      - in: path
        name: owner
        description: API owner identifier
      responses:
        200:
          description: OK
      tags:
      - Domains
      - Owner
      - Domain
      - ""
      - Newname
  /domains/{owner}/{domain}/.transfer:
    post:
      summary: transfers domain to another owner
      description: Transfers domain to another owner.
      operationId: transferDomain
      x-api-path-slug: domainsownerdomain-transfer-post
      parameters:
      - in: path
        name: domain
        description: domain identifier
      - in: query
        name: force
        description: force update
      - in: query
        name: newOwner
        description: New owner
      - in: path
        name: owner
        description: API owner identifier
      responses:
        200:
          description: OK
      tags:
      - Domains
      - Owner
      - Domain
      - ""
      - Transfer
  /domains/{owner}/{domain}/{version}/.bump:
    post:
      summary: Adds domain version
      description: Adds domain version.
      operationId: bumpDomain
      x-api-path-slug: domainsownerdomainversion-bump-post
      parameters:
      - in: path
        name: domain
        description: domain identifier
      - in: query
        name: force
        description: force update
      - in: query
        name: isPrivate
        description: Defines whether the API has to be private
      - in: query
        name: newVersion
        description: New domain version
      - in: path
        name: owner
        description: API owner identifier
      - in: path
        name: version
        description: version identifier
      responses:
        200:
          description: OK
      tags:
      - Domains
      - Owner
      - Domain
      - Version
      - ""
      - Bump
  /domains/{owner}/{domain}/{version}/.comment:
    get:
      summary: Returns the list of comments for the specified domain
      description: Returns the list of comments for the specified domain.
      operationId: getDomainComments
      x-api-path-slug: domainsownerdomainversion-comment-get
      parameters:
      - in: path
        name: domain
        description: domain identifier
      - in: path
        name: owner
        description: API owner identifier
      - in: path
        name: version
        description: version identifier
      responses:
        200:
          description: OK
      tags:
      - Domains
      - Owner
      - Domain
      - Version
      - ""
      - Comment
    post:
      summary: Adds a new comment to the specified domain
      description: Adds a new comment to the specified domain.
      operationId: addDomainComment
      x-api-path-slug: domainsownerdomainversion-comment-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: domain
        description: domain identifier
      - in: path
        name: owner
        description: API owner identifier
      - in: path
        name: version
        description: version identifier
      responses:
        200:
          description: OK
      tags:
      - Domains
      - Owner
      - Domain
      - Version
      - ""
      - Comment
  /domains/{owner}/{domain}/{version}/.comment/batch:
    post:
      summary: Updates passed batch of comments
      description: Updates passed batch of comments.
      operationId: updateDomainComments
      x-api-path-slug: domainsownerdomainversion-commentbatch-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: domain
        description: domain identifier
      - in: path
        name: owner
        description: API owner identifier
      - in: path
        name: version
        description: version identifier
      responses:
        200:
          description: OK
      tags:
      - Domains
      - Owner
      - Domain
      - Version
      - ""
      - Comment
      - Batch
  /domains/{owner}/{domain}/{version}/.comment/{comment}:
    delete:
      summary: Deletes specified comment
      description: Deletes specified comment.
      operationId: deleteDomainComment
      x-api-path-slug: domainsownerdomainversion-commentcomment-delete
      parameters:
      - in: path
        name: comment
        description: comment identifier
      - in: path
        name: domain
        description: domain identifier
      - in: path
        name: owner
        description: API owner identifier
      - in: path
        name: version
        description: version identifier
      responses:
        200:
          description: OK
      tags:
      - Domains
      - Owner
      - Domain
      - Version
      - ""
      - Comment
      - Comment
    patch:
      summary: Updates specified comment
      description: Updates specified comment.
      operationId: updateDomainComment
      x-api-path-slug: domainsownerdomainversion-commentcomment-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: comment
        description: comment identifier
      - in: path
        name: domain
        description: domain identifier
      - in: path
        name: owner
        description: API owner identifier
      - in: path
        name: version
        description: version identifier
      responses:
        200:
          description: OK
      tags:
      - Domains
      - Owner
      - Domain
      - Version
      - ""
      - Comment
      - Comment
  /domains/{owner}/{domain}/{version}/.comment/{comment}/reply:
    post:
      summary: Adds a new reply to the specified comment
      description: Adds a new reply to the specified comment.
      operationId: addDomainCommentReply
      x-api-path-slug: domainsownerdomainversion-commentcommentreply-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: comment
        description: comment identifier
      - in: path
        name: domain
        description: domain identifier
      - in: path
        name: owner
        description: API owner identifier
      - in: path
        name: version
        description: version identifier
      responses:
        200:
          description: OK
      tags:
      - Domains
      - Owner
      - Domain
      - Version
      - ""
      - Comment
      - Comment
      - Reply
  /domains/{owner}/{domain}/{version}/.comment/{comment}/reply/{reply}:
    delete:
      summary: Deletes specified comment reply
      description: Deletes specified comment reply.
      operationId: deleteDomainCommentReply
      x-api-path-slug: domainsownerdomainversion-commentcommentreplyreply-delete
      parameters:
      - in: path
        name: comment
        description: comment identifier
      - in: path
        name: domain
        description: domain identifier
      - in: path
        name: owner
        description: API owner identifier
      - in: path
        name: reply
        description: reply identifier
      - in: path
        name: version
        description: version identifier
      responses:
        200:
          description: OK
      tags:
      - Domains
      - Owner
      - Domain
      - Version
      - ""
      - Comment
      - Comment
      - Reply
      - Reply
    patch:
      summary: Updates specified comment reply
      description: Updates specified comment reply.
      operationId: updateDomainCommentReply
      x-api-path-slug: domainsownerdomainversion-commentcommentreplyreply-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: comment
        description: comment identifier
      - in: path
        name: domain
        description: domain identifier
      - in: path
        name: owner
        description: API owner identifier
      - in: path
        name: reply
        description: reply identifier
      - in: path
        name: version
        description: version identifier
      responses:
        200:
          description: OK
      tags:
      - Domains
      - Owner
      - Domain
      - Version
      - ""
      - Comment
      - Comment
      - Reply
      - Reply
  /domains/{owner}/{domain}/{version}/.comment/{comment}/status/{status}:
    put:
      summary: Updates status to the specified comment
      description: Updates status to the specified comment.
      operationId: setDomainCommentStatus
      x-api-path-slug: domainsownerdomainversion-commentcommentstatusstatus-put
      parameters:
      - in: path
        name: comment
        description: comment identifier
      - in: path
        name: domain
        description: domain identifier
      - in: path
        name: owner
        description: API owner identifier
      - in: path
        name: status
        description: comment status
      - in: path
        name: version
        description: version identifier
      responses:
        200:
          description: OK
      tags:
      - Domains
      - Owner
      - Domain
      - Version
      - ""
      - Comment
      - Comment
      - Status
      - Status
  /domains/{owner}/{domain}/{version}/.draft:
    delete:
      summary: Deletes a particular version of the specified Domain
      description: Deletes a particular version of the specified domain.
      operationId: deleteDraftDomain
      x-api-path-slug: domainsownerdomainversion-draft-delete
      parameters:
      - in: path
        name: domain
        description: domain identifier
      - in: path
        name: owner
        description: API owner identifier
      - in: path
        name: version
        description: version identifier
      responses:
        200:
          description: OK
      tags:
      - Domains
      - Owner
      - Domain
      - Version
      - ""
      - Draft
    get:
      summary: Retrieves the draft for the specified domain
      description: Retrieves the draft for the specified domain.
      operationId: getDraftDomain
      x-api-path-slug: domainsownerdomainversion-draft-get
      parameters:
      - in: path
        name: domain
        description: domain identifier
      - in: path
        name: owner
        description: API owner identifier
      - in: path
        name: version
        description: version identifier
      responses:
        200:
          description: OK
      tags:
      - Domains
      - Owner
      - Domain
      - Version
      - ""
      - Draft
    put:
      summary: Saves the provided draft for a domain.
      description: Saves the provided draft for a domain..
      operationId: saveDraftDomain
      x-api-path-slug: domainsownerdomainversion-draft-put
      parameters:
      - in: body
        name: definition
        description: the Swagger definition of this Domain
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: domain
        description: domain identifier
      - in: path
        name: owner
        description: API owner identifier
      - in: path
        name: version
        description: version identifier
      responses:
        200:
          description: OK
      tags:
      - Domains
      - Owner
      - Domain
      - Version
      - ""
      - Draft
  /domains/{owner}/{domain}/{version}/.fork:
    post:
      summary: Forks the provided domain definition
      description: Forks the provided domain definition.
      operationId: forkDomain
      x-api-path-slug: domainsownerdomainversion-fork-post
      parameters:
      - in: path
        name: domain
        description: domain identifier
      - in: query
        name: force
        description: force update
      - in: query
        name: isPrivate
        description: Defines whether the API has to be private
      - in: body
        name: newSpec
        description: New spec id
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: owner
        description: API owner identifier
      - in: path
        name: version
        description: version identifier
      responses:
        200:
          description: OK
      tags:
      - Domains
      - Owner
      - Domain
      - Version
      - ""
      - Fork
  /domains/{owner}/{domain}/{version}/.template:
    post:
      summary: Creates Domain by template
      description: Creates domain by template.
      operationId: saveDomainDefinitionByTemplate
      x-api-path-slug: domainsownerdomainversion-template-post
      parameters:
      - in: path
        name: domain
        description: domain identifier
      - in: query
        name: isPrivate
        description: Defines whether the API has to be private
      - in: path
        name: owner
        description: API owner identifier
      - in: query
        name: template
        description: Template id
      - in: path
        name: version
        description: version identifier
      responses:
        200:
          description: OK
      tags:
      - Domains
      - Owner
      - Domain
      - Version
      - ""
      - Template
---