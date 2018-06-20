---
swagger: "2.0"
x-collection-name: Bitly
x-complete: 0
info:
  title: Bitly Link API Get Link Lookup
  description: Get link lookup.
  termsOfService: http://dev.bitly.com/best_practices.html
  version: "3.0"
host: api-ssl.bitly.com
basePath: /v3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /search:
    get:
      summary: Get Search
      description: Get search.
      operationId: getSearch
      x-api-path-slug: search-get
      parameters:
      - in: query
        name: cities
        description: show links active in this city (ordered like country-state-city,
          e
      - in: query
        name: domain
        description: restrict results to this web domain (like bitly
      - in: query
        name: fields
        description: which fields to return in the response (comma-separated)
      - in: query
        name: full_domain
        description: restrict results to this full web domain (like blog
      - in: query
        name: lang
        description: favor results in this language (two letter ISO code)
      - in: query
        name: limit
      - in: query
        name: offset
        description: which result to start with (defaults to 0)
      - in: query
        name: query
        description: string to query for
      responses:
        200:
          description: OK
      tags:
      - Search
  /v3/expand:
    get:
      summary: Get Expand
      description: Get expand.
      operationId: getV3Expand
      x-api-path-slug: v3expand-get
      parameters:
      - in: query
        name: format
        description: json, xml, txt
      - in: query
        name: hash
        description: refers to one or more bitly hashes
      - in: query
        name: shortUrl
        description: refers to one or more Bitlinks
      responses:
        200:
          description: OK
      tags:
      - Expand
  /v3/info:
    get:
      summary: Get Info
      description: Get info.
      operationId: getV3Info
      x-api-path-slug: v3info-get
      parameters:
      - in: query
        name: expand_user
        description: optional true|false - include extra user info in response
      - in: query
        name: hash
        description: refers to one or more bitly hashes, (e
      - in: query
        name: shortUrl
        description: refers to one or more Bitlinks e
      responses:
        200:
          description: OK
      tags:
      - Info
  /v3/link/lookup:
    get:
      summary: Get Link Lookup
      description: Get link lookup.
      operationId: getV3LinkLookup
      x-api-path-slug: v3linklookup-get
      parameters:
      - in: query
        name: url
        description: one or more long URLs to lookup
      responses:
        200:
          description: OK
      tags:
      - Link
      - Lookup
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