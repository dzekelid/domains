---
swagger: "2.0"
x-collection-name: SendGrid
x-complete: 0
info:
  title: SendGrid Delete Whitelabel Domains Subuser
  description: "**This endpoint allows you to disassociate a specific whitelabel from
    a subuser.**\n\nA domain whitelabel allows you to remove the \u201Cvia\u201D or
    \u201Csent on behalf of\u201D message that your recipients see when they read
    your emails. Whitelabeling a domain allows you to replace sendgrid.net with your
    personal sending domain. You will be required to create a subdomain so that SendGrid
    can generate the DNS records which you must give to your host provider. If you
    choose to use Automated Security, SendGrid will provide you with 3 CNAME records.
    If you turn Automated Security off, you will be given 2 TXT records and 1 MX record.\n\nDomain
    whitelabels can be associated with (i.e. assigned to) subusers from a parent account.
    This functionality allows subusers to send mail using their parent's whitelabels.
    To associate a whitelabel with a subuser, the parent account must first create
    the whitelabel and validate it. The the parent may then associate the whitelabel
    via the subuser management tools.\n\nFor more information on whitelabeling, please
    see our [User Guide](https://sendgrid.com/docs/User_Guide/Settings/Whitelabel/index.html)\n\n##
    URI Parameters\n| URI Parameter   | Type  | Required?  | Description  |\n|---|---|---|---|\n|
    username | string  | required  | Username for the subuser to find associated whitelabels
    for. |"
  version: 1.0.0
host: api.sendgrid.com
basePath: /v3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /whitelabel/domains:
    get:
      summary: Get Whitelabel Domains
      description: "**This endpoint allows you to retrieve a list of all domain whitelabels
        you have created.**\n\nA domain whitelabel allows you to remove the \u201Cvia\u201D
        or \u201Csent on behalf of\u201D message that your recipients see when they
        read your emails. Whitelabeling a domain allows you to replace sendgrid.net
        with your personal sending domain. You will be required to create a subdomain
        so that SendGrid can generate the DNS records which you must give to your
        host provider. If you choose to use Automated Security, SendGrid will provide
        you with 3 CNAME records. If you turn Automated Security off, you will be
        given 2 TXT records and 1 MX record.\n\nFor more information on whitelabeling,
        please see our [User Guide](https://sendgrid.com/docs/User_Guide/Settings/Whitelabel/index.html)"
      operationId: whitelabel.domains.get
      x-api-path-slug: whitelabeldomains-get
      parameters:
      - in: query
        name: domain
        description: Search for domain whitelabels that match the given domain
      - in: query
        name: exclude_subusers
        description: Exclude subuser domains from the result
      - in: query
        name: limit
        description: Number of domains to return
      - in: query
        name: No Name
      - in: query
        name: offset
        description: Paging offset
      - in: query
        name: username
        description: The username associated with a whitelabel
      responses:
        200:
          description: OK
      tags:
      - Email
      - Whitelabel
      - Domains
    post:
      summary: Add Whitelabel Domains
      description: "**This endpoint allows you to create a whitelabel for one of your
        domains.**\n\nIf you are creating a domain whitelabel that you would like
        a subuser to use, you have two options:\n1. Use the \"username\" parameter.
        This allows you to create a whitelabel on behalf of your subuser. This means
        the subuser is able to see and modify the created whitelabel.\n2. Use the
        Association workflow (see Associate Domain section). This allows you to assign
        a whitelabel created by the parent to a subuser. This means the subuser will
        default to the assigned whitelabel, but will not be able to see or modify
        that whitelabel. However, if the subuser creates their own whitelabel it will
        overwrite the assigned whitelabel.\n\nA domain whitelabel allows you to remove
        the \u201Cvia\u201D or \u201Csent on behalf of\u201D message that your recipients
        see when they read your emails. Whitelabeling a domain allows you to replace
        sendgrid.net with your personal sending domain. You will be required to create
        a subdomain so that SendGrid can generate the DNS records which you must give
        to your host provider. If you choose to use Automated Security, SendGrid will
        provide you with 3 CNAME records. If you turn Automated Security off, you
        will be given 2 TXT records and 1 MX record.\n\nFor more information on whitelabeling,
        please see our [User Guide](https://sendgrid.com/docs/User_Guide/Settings/Whitelabel/index.html)"
      operationId: whitelabel.domains.post
      x-api-path-slug: whitelabeldomains-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Whitelabel
      - Domains
  /whitelabel/domains/default:
    get:
      summary: Get Whitelabel Domains Default
      description: "**This endpoint allows you to retrieve the default whitelabel
        for a domain.**\n\nA domain whitelabel allows you to remove the \u201Cvia\u201D
        or \u201Csent on behalf of\u201D message that your recipients see when they
        read your emails. Whitelabeling a domain allows you to replace sendgrid.net
        with your personal sending domain. You will be required to create a subdomain
        so that SendGrid can generate the DNS records which you must give to your
        host provider. If you choose to use Automated Security, SendGrid will provide
        you with 3 CNAME records. If you turn Automated Security off, you will be
        given 2 TXT records and 1 MX record.\n\nFor more information on whitelabeling,
        please see our [User Guide](https://sendgrid.com/docs/User_Guide/Settings/Whitelabel/index.html)\n\n##
        URI Parameters\n| URI Parameter   | Type   | Description  |\n|---|---|---|\n|
        domain | string  |The domain to find a default domain whitelabel for. |"
      operationId: whitelabel.domains.default.get
      x-api-path-slug: whitelabeldomainsdefault-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Whitelabel
      - Domains
      - Default
  /whitelabel/domains/subuser:
    delete:
      summary: Delete Whitelabel Domains Subuser
      description: "**This endpoint allows you to disassociate a specific whitelabel
        from a subuser.**\n\nA domain whitelabel allows you to remove the \u201Cvia\u201D
        or \u201Csent on behalf of\u201D message that your recipients see when they
        read your emails. Whitelabeling a domain allows you to replace sendgrid.net
        with your personal sending domain. You will be required to create a subdomain
        so that SendGrid can generate the DNS records which you must give to your
        host provider. If you choose to use Automated Security, SendGrid will provide
        you with 3 CNAME records. If you turn Automated Security off, you will be
        given 2 TXT records and 1 MX record.\n\nDomain whitelabels can be associated
        with (i.e. assigned to) subusers from a parent account. This functionality
        allows subusers to send mail using their parent's whitelabels. To associate
        a whitelabel with a subuser, the parent account must first create the whitelabel
        and validate it. The the parent may then associate the whitelabel via the
        subuser management tools.\n\nFor more information on whitelabeling, please
        see our [User Guide](https://sendgrid.com/docs/User_Guide/Settings/Whitelabel/index.html)\n\n##
        URI Parameters\n| URI Parameter   | Type  | Required?  | Description  |\n|---|---|---|---|\n|
        username | string  | required  | Username for the subuser to find associated
        whitelabels for. |"
      operationId: whitelabel.domains.subuser.delete
      x-api-path-slug: whitelabeldomainssubuser-delete
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Whitelabel
      - Domains
      - Subuser
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