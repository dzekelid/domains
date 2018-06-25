---
name: Oxford Dictionaries
x-slug: oxford-dictionaries
description: If you&rsquo;re looking to enhance your app or website with dictionary
  data, don&rsquo;t compromise on quality. The Oxford Dictionaries API offers easy
  and intuitive access to Oxfords dictionary content, which is trusted around the
  world. Here at Oxford Dictionaries, home of the OED, we love words. That&rsquo;s
  why we have experienced lexicographers tracking the living language, delving deep
  into our corpora and monitoring a wide range of media in order to understand how
  words are being used and how language is evolving. This research is used by our
  editors to write and edit dictionary entries and translations, meaning we&rsquo;re
  able to offer up-to-date, accurate, and reliable lexical content in multiple languages.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/oxford-dictionaries-api.png
x-kinRank: "7"
x-alexaRank: "0"
tags: Domains
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/oxford-dictionaries/apis.md
specificationVersion: "0.14"
apis:
- name: Oxford Dictionaries Lists available domains in a bilingual dataset
  x-api-slug: oxford-dictionaries
  description: Returns a list of the available [domains](documentation/glossary?term=domain)
    for a given bilingual language dataset.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/oxford-dictionaries-api.png
  humanURL: https://developer.oxforddictionaries.com/
  baseURL: https://od-api-demo.oxforddictionaries.com:443//api/v1//domains/{source_domains_language}/{target_domains_language}
  tags: Domains,Source,Domains,Language,Target,Domains,Language
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/oxford-dictionaries/domainssource-domains-languagetarget-domains-language-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/oxford-dictionaries/domainssource-domains-languagetarget-domains-language-get-openapi.md
- name: Oxford Dictionaries Lists available domains in a monolingual dataset
  x-api-slug: oxford-dictionaries
  description: Returns a list of the available [domains](documentation/glossary?term=domain)
    for a given monolingual language dataset.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/oxford-dictionaries-api.png
  humanURL: https://developer.oxforddictionaries.com/
  baseURL: https://od-api-demo.oxforddictionaries.com:443//api/v1//domains/{source_language}
  tags: Domains,Source,Language
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/oxford-dictionaries/domainssource-language-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/oxford-dictionaries/domainssource-language-get-openapi.md
- name: Oxford Dictionaries Lists available domains in a given bilingual language
    dataset.
  x-api-slug: oxford-dictionaries
  description: Returns a list of the available [domains](/glossary?tag=#domains&expand)
    for a given bilingual language dataset.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/oxford-dictionaries-api.png
  humanURL: https://developer.oxforddictionaries.com/
  baseURL: https://od-api-demo.oxforddictionaries.com:443//api/v1//domains/{source_language}/{target_language}
  tags: Domains,Source,Language,Target,Language
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/oxford-dictionaries/domainssource-languagetarget-language-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/oxford-dictionaries/domainssource-languagetarget-language-get-openapi.md
- name: Oxford Dictionaries
  x-api-slug: oxford-dictionaries
  description: If you&rsquo;re looking to enhance your app or website with dictionary
    data, don&rsquo;t compromise on quality. The Oxford Dictionaries API offers easy
    and intuitive access to Oxfords dictionary content, which is trusted around the
    world. Here at Oxford Dictionaries, home of the OED, we love words. That&rsquo;s
    why we have experienced lexicographers tracking the living language, delving deep
    into our corpora and monitoring a wide range of media in order to understand how
    words are being used and how language is evolving. This research is used by our
    editors to write and edit dictionary entries and translations, meaning we&rsquo;re
    able to offer up-to-date, accurate, and reliable lexical content in multiple languages.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/oxford-dictionaries-api.png
  humanURL: https://developer.oxforddictionaries.com/
  baseURL: https://od-api-demo.oxforddictionaries.com:443//api/v1
  tags: Domains
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/domains/master/_listings/oxford-dictionaries/openapi.md
x-common:
- type: x-blog
  url: https://api-blog.oxforddictionaries.com/
- type: x-developer
  url: https://developer.oxforddictionaries.com/
- type: x-faq
  url: https://developer.oxforddictionaries.com/faq
- type: x-forum
  url: https://forum.oxforddictionaries.com/api/
- type: x-twitter
  url: https://twitter.com/OxfordWordsAPI
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---