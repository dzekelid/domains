---
name: SendGrid
x-slug: sendgrid
description: Delivering your transactional and marketing emails through the worlds
  largest cloud-based email delivery platform. Send with confidence.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
x-kinRank: "9"
x-alexaRank: "10000"
tags: Domains
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/sendgrid/apis.md
specificationVersion: "0.14"
apis:
- name: SendGrid Get Whitelabel Domains
  x-api-slug: sendgrid
  description: "**This endpoint allows you to retrieve a list of all domain whitelabels
    you have created.**\n\nA domain whitelabel allows you to remove the \u201Cvia\u201D
    or \u201Csent on behalf of\u201D message that your recipients see when they read
    your emails. Whitelabeling a domain allows you to replace sendgrid.net with your
    personal sending domain. You will be required to create a subdomain so that SendGrid
    can generate the DNS records which you must give to your host provider. If you
    choose to use Automated Security, SendGrid will provide you with 3 CNAME records.
    If you turn Automated Security off, you will be given 2 TXT records and 1 MX record.\n\nFor
    more information on whitelabeling, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Settings/Whitelabel/index.html)"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//whitelabel/domains
  tags: Email,Whitelabel, Domains
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/sendgrid/whitelabeldomains-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/sendgrid/whitelabeldomains-get-openapi.md
- name: SendGrid Add Whitelabel Domains
  x-api-slug: sendgrid
  description: "**This endpoint allows you to create a whitelabel for one of your
    domains.**\n\nIf you are creating a domain whitelabel that you would like a subuser
    to use, you have two options:\n1. Use the \"username\" parameter. This allows
    you to create a whitelabel on behalf of your subuser. This means the subuser is
    able to see and modify the created whitelabel.\n2. Use the Association workflow
    (see Associate Domain section). This allows you to assign a whitelabel created
    by the parent to a subuser. This means the subuser will default to the assigned
    whitelabel, but will not be able to see or modify that whitelabel. However, if
    the subuser creates their own whitelabel it will overwrite the assigned whitelabel.\n\nA
    domain whitelabel allows you to remove the \u201Cvia\u201D or \u201Csent on behalf
    of\u201D message that your recipients see when they read your emails. Whitelabeling
    a domain allows you to replace sendgrid.net with your personal sending domain.
    You will be required to create a subdomain so that SendGrid can generate the DNS
    records which you must give to your host provider. If you choose to use Automated
    Security, SendGrid will provide you with 3 CNAME records. If you turn Automated
    Security off, you will be given 2 TXT records and 1 MX record.\n\nFor more information
    on whitelabeling, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Settings/Whitelabel/index.html)"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//whitelabel/domains
  tags: Email,Whitelabel, Domains
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/sendgrid/whitelabeldomains-post-openapi.md
- name: SendGrid Get Whitelabel Domains Default
  x-api-slug: sendgrid
  description: "**This endpoint allows you to retrieve the default whitelabel for
    a domain.**\n\nA domain whitelabel allows you to remove the \u201Cvia\u201D or
    \u201Csent on behalf of\u201D message that your recipients see when they read
    your emails. Whitelabeling a domain allows you to replace sendgrid.net with your
    personal sending domain. You will be required to create a subdomain so that SendGrid
    can generate the DNS records which you must give to your host provider. If you
    choose to use Automated Security, SendGrid will provide you with 3 CNAME records.
    If you turn Automated Security off, you will be given 2 TXT records and 1 MX record.\n\nFor
    more information on whitelabeling, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Settings/Whitelabel/index.html)\n\n##
    URI Parameters\n| URI Parameter   | Type   | Description  |\n|---|---|---|\n|
    domain | string  |The domain to find a default domain whitelabel for. |"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//whitelabel/domains/default
  tags: Email,Whitelabel, Domains, Default
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/sendgrid/whitelabeldomainsdefault-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/sendgrid/whitelabeldomainsdefault-get-openapi.md
- name: SendGrid Delete Whitelabel Domains Subuser
  x-api-slug: sendgrid
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
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//whitelabel/domains/subuser
  tags: Email,Whitelabel, Domains, Subuser
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/sendgrid/whitelabeldomainssubuser-delete-openapi.md
- name: SendGrid Get Whitelabel Domains Subuser
  x-api-slug: sendgrid
  description: "**This endpoint allows you to retrieve all of the whitelabels that
    have been assigned to a specific subuser.**\n\nA domain whitelabel allows you
    to remove the \u201Cvia\u201D or \u201Csent on behalf of\u201D message that your
    recipients see when they read your emails. Whitelabeling a domain allows you to
    replace sendgrid.net with your personal sending domain. You will be required to
    create a subdomain so that SendGrid can generate the DNS records which you must
    give to your host provider. If you choose to use Automated Security, SendGrid
    will provide you with 3 CNAME records. If you turn Automated Security off, you
    will be given 2 TXT records and 1 MX record.\n\nDomain whitelabels can be associated
    with (i.e. assigned to) subusers from a parent account. This functionality allows
    subusers to send mail using their parent's whitelabels. To associate a whitelabel
    with a subuser, the parent account must first create the whitelabel and validate
    it. The the parent may then associate the whitelabel via the subuser management
    tools.\n\nFor more information on whitelabeling, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Settings/Whitelabel/index.html)\n\n##
    URI Parameters\n| URI Parameter   | Type  | Description  |\n|---|---|---|\n| username
    | string  | Username of the subuser to find associated whitelabels for. |"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//whitelabel/domains/subuser
  tags: Email,Whitelabel, Domains, Subuser
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/sendgrid/whitelabeldomainssubuser-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/sendgrid/whitelabeldomainssubuser-get-openapi.md
- name: SendGrid Delete Whitelabel Domains Domain
  x-api-slug: sendgrid
  description: "**This endpoint allows you to delete a domain whitelabel.**\n\nA domain
    whitelabel allows you to remove the \u201Cvia\u201D or \u201Csent on behalf of\u201D
    message that your recipients see when they read your emails. Whitelabeling a domain
    allows you to replace sendgrid.net with your personal sending domain. You will
    be required to create a subdomain so that SendGrid can generate the DNS records
    which you must give to your host provider. If you choose to use Automated Security,
    SendGrid will provide you with 3 CNAME records. If you turn Automated Security
    off, you will be given 2 TXT records and 1 MX record.\n\nFor more information
    on whitelabeling, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Settings/Whitelabel/index.html)"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//whitelabel/domains/{domain_id}
  tags: Email,Whitelabel, Domains, Domain
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/sendgrid/whitelabeldomainsdomain-id-delete-openapi.md
- name: SendGrid Get Whitelabel Domains Domain
  x-api-slug: sendgrid
  description: "**This endpoint allows you to retrieve a specific domain whitelabel.**\n\nA
    domain whitelabel allows you to remove the \u201Cvia\u201D or \u201Csent on behalf
    of\u201D message that your recipients see when they read your emails. Whitelabeling
    a domain allows you to replace sendgrid.net with your personal sending domain.
    You will be required to create a subdomain so that SendGrid can generate the DNS
    records which you must give to your host provider. If you choose to use Automated
    Security, SendGrid will provide you with 3 CNAME records. If you turn Automated
    Security off, you will be given 2 TXT records and 1 MX record.\n\nFor more information
    on whitelabeling, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Settings/Whitelabel/index.html)"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//whitelabel/domains/{domain_id}
  tags: Email,Whitelabel, Domains, Domain
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/sendgrid/whitelabeldomainsdomain-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/sendgrid/whitelabeldomainsdomain-id-get-openapi.md
- name: SendGrid Patch Whitelabel Domains Domain
  x-api-slug: sendgrid
  description: "**This endpoint allows you to update the settings for a domain whitelabel.**\n\nA
    domain whitelabel allows you to remove the \u201Cvia\u201D or \u201Csent on behalf
    of\u201D message that your recipients see when they read your emails. Whitelabeling
    a domain allows you to replace sendgrid.net with your personal sending domain.
    You will be required to create a subdomain so that SendGrid can generate the DNS
    records which you must give to your host provider. If you choose to use Automated
    Security, SendGrid will provide you with 3 CNAME records. If you turn Automated
    Security off, you will be given 2 TXT records and 1 MX record.\n\nFor more information
    on whitelabeling, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Settings/Whitelabel/index.html)"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//whitelabel/domains/{domain_id}
  tags: Email,Whitelabel, Domains, Domain
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/sendgrid/whitelabeldomainsdomain-id-patch-openapi.md
- name: SendGrid Add Whitelabel Domains Domain  Subuser
  x-api-slug: sendgrid
  description: "**This endpoint allows you to associate a specific domain whitelabel
    with a subuser.**\n\nA domain whitelabel allows you to remove the \u201Cvia\u201D
    or \u201Csent on behalf of\u201D message that your recipients see when they read
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
    URI Parameters\n| URI Parameter   | Type   | Description  |\n|---|---|---|\n|
    domain_id | integer   | ID of the domain whitelabel to associate with the subuser.
    |"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//whitelabel/domains/{domain_id}/subuser
  tags: Email,Whitelabel, Domains, Domain, , Subuser
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/sendgrid/whitelabeldomainsdomain-idsubuser-post-openapi.md
- name: SendGrid Add Whitelabel Domains  Ips
  x-api-slug: sendgrid
  description: "**This endpoint allows you to add an IP address to a domain whitelabel.**\n\nA
    domain whitelabel allows you to remove the \u201Cvia\u201D or \u201Csent on behalf
    of\u201D message that your recipients see when they read your emails. Whitelabeling
    a domain allows you to replace sendgrid.net with your personal sending domain.
    You will be required to create a subdomain so that SendGrid can generate the DNS
    records which you must give to your host provider. If you choose to use Automated
    Security, SendGrid will provide you with 3 CNAME records. If you turn Automated
    Security off, you will be given 2 TXT records and 1 MX record.\n\nFor more information
    on whitelabeling, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Settings/Whitelabel/index.html)\n\n##
    URI Parameters\n| URI Parameter   | Type  |  Description  |\n|---|---|---|\n|
    id | integer  | ID of the domain to which you are adding an IP |"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//whitelabel/domains/{id}/ips
  tags: Email,Whitelabel, Domains, , Ips
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/sendgrid/whitelabeldomainsidips-post-openapi.md
- name: SendGrid Delete Whitelabel Domains  Ips Ip
  x-api-slug: sendgrid
  description: "**This endpoint allows you to remove a domain's IP address from that
    domain's whitelabel.**\n\nA domain whitelabel allows you to remove the \u201Cvia\u201D
    or \u201Csent on behalf of\u201D message that your recipients see when they read
    your emails. Whitelabeling a domain allows you to replace sendgrid.net with your
    personal sending domain. You will be required to create a subdomain so that SendGrid
    can generate the DNS records which you must give to your host provider. If you
    choose to use Automated Security, SendGrid will provide you with 3 CNAME records.
    If you turn Automated Security off, you will be given 2 TXT records and 1 MX record.\n\nFor
    more information on whitelabeling, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Settings/Whitelabel/index.html)\n\n##
    URI Parameters\n| URI Parameter   | Type  | Description  |\n|---|---|---|\n| id
    | integer  | ID of the domain whitelabel to delete the IP from. |\n| ip | string
    | IP to remove from the domain whitelabel. |"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//whitelabel/domains/{id}/ips/{ip}
  tags: Email,Whitelabel, Domains, , Ips, Ip
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/sendgrid/whitelabeldomainsidipsip-delete-openapi.md
- name: SendGrid Add Whitelabel Domains  Valate
  x-api-slug: sendgrid
  description: "**This endpoint allows you to validate a domain whitelabel. If it
    fails, it will return an error message describing why the whitelabel could not
    be validated.**\n\nA domain whitelabel allows you to remove the \u201Cvia\u201D
    or \u201Csent on behalf of\u201D message that your recipients see when they read
    your emails. Whitelabeling a domain allows you to replace sendgrid.net with your
    personal sending domain. You will be required to create a subdomain so that SendGrid
    can generate the DNS records which you must give to your host provider. If you
    choose to use Automated Security, SendGrid will provide you with 3 CNAME records.
    If you turn Automated Security off, you will be given 2 TXT records and 1 MX record.\n\nFor
    more information on whitelabeling, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Settings/Whitelabel/index.html)\n\n##
    URI Parameters\n| URI Parameter   | Type   | Description  |\n|---|---|---|\n|
    id | integer  |ID of the domain whitelabel to validate. |"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//whitelabel/domains/{id}/validate
  tags: Email,Whitelabel, Domains, , Valate
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/sendgrid/whitelabeldomainsidvalidate-post-openapi.md
- name: SendGrid
  x-api-slug: sendgrid
  description: SendGrids cloud-based email infrastructure relieves businesses of the
    cost and complexity of maintaining custom email systems. SendGrid provides reliable
    delivery, scalability and real-time analytics along with flexible APIs that make
    custom integration a breeze.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3
  tags: Domains
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/sendgrid/openapi.md
x-common:
- type: x--net-library
  url: https://sendgrid.com/docs/Code_Examples/csharp.html
- type: x-base
  url: https://api.sendgrid.com
- type: x-blog
  url: http://blog.sendgrid.com/
- type: x-blog-rss
  url: http://feeds.feedburner.com/sendgrid/CDXr
- type: x-contact-form
  url: https://sendgrid.com/contact
- type: x-crunchbase
  url: http://www.crunchbase.com/company/sendgrid
- type: x-crunchbase
  url: https://crunchbase.com/organization/sendgrid
- type: x-developer
  url: https://sendgrid.com/developers
- type: x-documentation
  url: https://sendgrid.com/docs/index.html
- type: x-email
  url: privacy@sendgrid.com
- type: x-email
  url: legal@sendgrid.com
- type: x-email
  url: dpo@sendgrid.com
- type: x-forum
  url: http://support.sendgrid.com/forums
- type: x-github
  url: https://github.com/sendgrid
- type: x-go-library
  url: https://sendgrid.com/docs/Code_Examples/go.html
- type: x-ios-library
  url: https://sendgrid.com/docs/Code_Examples/ios.html
- type: x-java-library
  url: https://sendgrid.com/docs/Code_Examples/java.html
- type: x-labs
  url: http://labs.sendgrid.com/
- type: x-linkedin
  url: https://www.linkedin.com/company/sendgrid
- type: x-node-js-library
  url: https://sendgrid.com/docs/Code_Examples/nodejs.html
- type: x-partners
  url: https://sendgrid.com/partners
- type: x-perl-library
  url: https://sendgrid.com/docs/Code_Examples/perl.html
- type: x-php-library
  url: https://sendgrid.com/docs/Code_Examples/php.html
- type: x-pricing
  url: https://sendgrid.com/transactional-email/pricing
- type: x-privacy
  url: https://sendgrid.com/privacy
- type: x-python-library
  url: https://sendgrid.com/docs/Code_Examples/python.html
- type: x-ruby-library
  url: https://sendgrid.com/docs/Code_Examples/ruby.html
- type: x-security
  url: https://sendgrid.com/security
- type: x-selfservice-registration
  url: https://sendgrid.com/user/signup
- type: x-terms-of-service
  url: https://sendgrid.com/tos
- type: x-twitter
  url: https://twitter.com/SendGrid
- type: x-website
  url: http://sendgrid.com
- type: x-website
  url: https://sendgrid.com/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---