---
swagger: "2.0"
x-collection-name: Heroku
x-complete: 1
info:
  title: Heroku
  description: manage-your-heroku-apps-configs-collaborators--resources
  version: "1"
host: api.heroku.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /apps/{app}/domains:
    parameters:
      summary: Parameters Application Domains
      description: Parameters application domains.
      operationId: parametersAppsAppDomains
      x-api-path-slug: appsappdomains-parameters
      responses:
        200:
          description: OK
      tags:
      - Parameters
      - Application
      - Domains
    get:
      summary: Get Application Domains
      description: List domains for an app.
      operationId: getAppsAppDomains
      x-api-path-slug: appsappdomains-get
      parameters:
      - in: header
        name: Accept
        description: Content type
      - in: query
        name: Accept
        description: Content type
      - in: query
        name: app
        description: The app name
      - in: path
        name: app
      responses:
        200:
          description: OK
      tags:
      - Application
      - Domains
  /apps/{app}/domains/{domain_name}:
    parameters:
      summary: Parameters Application Domain Name
      description: Parameters application domain name.
      operationId: parametersAppsAppDomainsDomainName
      x-api-path-slug: appsappdomainsdomain-name-parameters
      responses:
        200:
          description: OK
      tags:
      - Parameters
      - Application
      - Domain
      - Name
    delete:
      summary: Delete Application Domain Name
      description: Delete application domain name.
      operationId: deleteAppsAppDomainsDomainName
      x-api-path-slug: appsappdomainsdomain-name-delete
      parameters:
      - in: header
        name: Accept
        description: Content type
      - in: query
        name: Accept
        description: Content type
      - in: query
        name: app
        description: The app name
      - in: path
        name: app
      - in: query
        name: domain_name
        description: The domain to remove
      - in: path
        name: domain_name
      responses:
        200:
          description: OK
      tags:
      - Application
      - Domain
      - Name
---