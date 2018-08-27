---
swagger: "2.0"
x-collection-name: Oxford Dictionaries
x-complete: 1
info:
  title: Oxford Dictionaries
  description: if-youre-looking-to-enhance-your-app-or-website-with-dictionary-data-dont-compromise-on-quality--the-oxford-dictionaries-api-offers-easy-and-intuitive-access-to-oxfords-dictionary-content-which-is-trusted-around-the-world--here-at-oxford-dictionaries-home-of-the-oed-we-love-words--thats-why-we-have-experienced-lexicographers-tracking-the-living-language-delving-deep-into-our-corpora-and-monitoring-a-wide-range-of-media-in-order-to-understand-how-words-are-being-used-and-how-language-is-evolving--this-research-is-used-by-our-editors-to-write-and-edit-dictionary-entries-and-translations-meaning-were-able-to-offer-uptodate-accurate-and-reliable-lexical-content-in-multiple-languages-
  termsOfService: http://helloreverb.com/terms/
  version: 1.8.0
host: od-api-demo.oxforddictionaries.com:443
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /domains/{source_domains_language}/{target_domains_language}:
    get:
      summary: Lists available domains in a bilingual dataset
      description: Returns a list of the available [domains](documentation/glossary?term=domain)
        for a given bilingual language dataset.
      operationId: getDomainsSourceDomainsLanguageTargetDomainsLanguage
      x-api-path-slug: domainssource-domains-languagetarget-domains-language-get
      parameters:
      - in: query
        name: No Name
      - in: path
        name: source_domains_language
        description: IANA language code
      - in: path
        name: target_domains_language
        description: IANA language code
      responses:
        200:
          description: OK
      tags:
      - Domains
      - Source
      - Domains
      - Language
      - Target
      - Domains
      - Language
  /domains/{source_language}:
    get:
      summary: Lists available domains in a monolingual dataset
      description: Returns a list of the available [domains](documentation/glossary?term=domain)
        for a given monolingual language dataset.
      operationId: getDomainsSourceLanguage
      x-api-path-slug: domainssource-language-get
      parameters:
      - in: query
        name: No Name
      - in: path
        name: source_language
        description: IANA language code
      responses:
        200:
          description: OK
      tags:
      - Domains
      - Source
      - Language
  /domains/{source_language}/{target_language}:
    get:
      summary: Lists available domains in a given bilingual language dataset.
      description: Returns a list of the available [domains](/glossary?tag=#domains&expand)
        for a given bilingual language dataset.
      operationId: getDomainsSourceLanguageTargetLanguage
      x-api-path-slug: domainssource-languagetarget-language-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Domains
      - Source
      - Language
      - Target
      - Language
---