---
swagger: "2.0"
x-collection-name: Predix
x-complete: 0
info:
  title: Predix Assets Gets all user-defined domain objects.
  description: |-
    This is a user-defined domain object collection.

    You can create your own custom domain objects, add properties to them, define relationships, and so on.
  version: 1.0.0
host: predix-apphub-arcs-prod.run.aws-usw02-pr.ice.predix.io
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/:
    get:
      summary: Get a listing of user-defined domain object collections
      description: Returns the names of all user-defined domain object collections
        with counts of domain objects contained.
      operationId: getV1
      x-api-path-slug: v1-get
      responses:
        200:
          description: Successful response
      tags:
      - Listing
      - Of
      - User-defined
      - Domain
      - Object
      - Collections
  /v1/{collection}:
    get:
      summary: Gets all user-defined domain objects.
      description: |-
        This is a user-defined domain object collection.

        You can create your own custom domain objects, add properties to them, define relationships, and so on.
      operationId: getV1Collection
      x-api-path-slug: v1collection-get
      parameters:
      - in: path
        name: collection
        description: Name of the user-defined domain object collection
      - in: query
        name: fields
        description: Fields to be returned from each entity (comma separated)
      - in: query
        name: filter
        description: GEL query filter
      - in: query
        name: pageSize
        description: Limits the number of entities returned
      responses:
        200:
          description: Successful response
      tags:
      - S
      - ""
      - User-defined
      - Domain
      - Objects
    post:
      summary: Create one or more user-defined domain objects
      description: |-
        This is a user-defined domain object collection.

        You can create your own custom domain objects, add properties to them, define relationships, and so on.

        The following characters are not allowed in any attribute names: $ < > : | ( ) , = ! ? &
      operationId: postV1Collection
      x-api-path-slug: v1collection-post
      parameters:
      - in: body
        name: body
        description: Array of entities to create
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: collection
        description: Name of the user-defined domain object collection
      responses:
        200:
          description: Successful response
      tags:
      - More
      - User-defined
      - Domain
      - Objects
  /v1/{collection}/{id}:
    put:
      summary: Update a user-defined domain object
      description: |-
        This is a user-defined domain object collection.

        You can create your own custom domain objects, add properties to them, define relationships, and so on.

        The following characters are not allowed in any attribute names: $ < > : | ( ) , = ! ? &
      operationId: putV1Collection
      x-api-path-slug: v1collectionid-put
      parameters:
      - in: body
        name: body
        description: Array of one entity to create/update
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: collection
        description: Name of the user-defined domain object collection
      - in: path
        name: id
        description: ID of the domain object to update
      responses:
        200:
          description: Successful response
      tags:
      - User-defined
      - Domain
      - Object
    patch:
      summary: Patch a user-defined domain object
      description: |-
        This is a user-defined domain object collection.

        You can create your own custom domain objects, add properties to them, define relationships, and so on.

        Update specific model using http PATCH requests. Request format should follow JSON PATCH format. Supported operations on each attribute are add, remove, replace, move, copy, test. Refer RFC link for more details on request format. https://tools.ietf.org/html/rfc6902
      operationId: patchV1Collection
      x-api-path-slug: v1collectionid-patch
      parameters:
      - in: body
        name: body
        description: 'Array of patch operations to apply to the domain object (see:
          https://tools'
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: collection
        description: Name of the user-defined domain object collection
      - in: path
        name: id
        description: ID of the domain object to patch
      responses:
        200:
          description: Successful response
      tags:
      - User-defined
      - Domain
      - Object
    delete:
      summary: Delete a user-defined domain object
      description: |-
        This is a user-defined domain object collection.

        You can create your own custom domain objects, add properties to them, define relationships, and so on.
      operationId: deleteV1Collection
      x-api-path-slug: v1collectionid-delete
      parameters:
      - in: path
        name: collection
        description: Name of the user-defined domain object collection
      - in: path
        name: id
        description: ID of the domain object to delete
      responses:
        200:
          description: Successful response
      tags:
      - User-defined
      - Domain
      - Object
  /v1/system/audit:
    get:
      summary: Get domain object audit records.
      description: For detailed documentation of all available query options please
        refer to Predix Asset Documentation.
      operationId: getV1SystemAudit
      x-api-path-slug: v1systemaudit-get
      parameters:
      - in: query
        name: fields
        description: Fields to be returned from the entity (comma separated)
      responses:
        200:
          description: Successful response
      tags:
      - Domain
      - Object
      - Audit
      - Records
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