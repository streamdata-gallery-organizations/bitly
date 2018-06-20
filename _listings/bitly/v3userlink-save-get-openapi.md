---
swagger: "2.0"
x-collection-name: Bitly
x-complete: 0
info:
  title: Bitly Link API Get User Link Save
  description: Get user link save.
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
  /v3/shorten:
    get:
      summary: Get Shorten
      description: Get shorten.
      operationId: getV3Shorten
      x-api-path-slug: v3shorten-get
      parameters:
      - in: query
        name: domain
        description: until we have model
      - in: query
        name: format
        description: json, xml, txt
      - in: query
        name: longUrl
        description: 'a long URL to be shortened (example: http://betaworks'
      responses:
        200:
          description: OK
      tags:
      - Shorten
  /v3/user/link_edit:
    get:
      summary: Get User Link Edit
      description: Get user link edit.
      operationId: getV3UserLinkEdit
      x-api-path-slug: v3userlink-edit-get
      parameters:
      - in: query
        name: archived
        description: indicating whether or not link is to be archived
      - in: query
        name: clear_deeplinks
        description: indicating that all deeplinks should be removed form the bitlink
      - in: query
        name: deeplinks
        description: urlencoded json array of deeplink items
      - in: query
        name: edit
        description: a comma separated string of fields to be edited
      - in: query
        name: link
        description: Successful response
      - in: query
        name: note
        description: a description of, or note about, this Bitlink
      - in: query
        name: private
        description: boolean true or false indicating privacy setting (defaults to
          user-level setting)
      - in: query
        name: title
        description: the title of this Bitlink
      - in: query
        name: user_ts
        description: timestamp as an integer epoch
      responses:
        200:
          description: OK
      tags:
      - User
      - Link
      - Edit
  /v3/user/link_lookup:
    get:
      summary: Get User Link Lookup
      description: Get user link lookup.
      operationId: getV3UserLinkLookup
      x-api-path-slug: v3userlink-lookup-get
      parameters:
      - in: query
        name: link
        description: one or more Bitlinks to lookup
      - in: query
        name: url
        description: one or more long URLs to lookup
      responses:
        200:
          description: OK
      tags:
      - User
      - Link
      - Lookup
  /v3/user/link_save:
    get:
      summary: Get User Link Save
      description: Get user link save.
      operationId: getV3UserLinkSave
      x-api-path-slug: v3userlink-save-get
      parameters:
      - in: query
        name: deeplinks
        description: urlencoded json array of deeplink items
      - in: query
        name: domain
        description: the short domain to use; either bit
      - in: query
        name: longUrl
        description: the URL to be saved as a Bitlink
      - in: query
        name: note
        description: a description of, or note about, this Bitlink
      - in: query
        name: private
        description: indicating privacy setting (defaults to user-level setting)
      - in: query
        name: title
        description: the title of this Bitlink
      - in: query
        name: user_ts
        description: timestamp as an integer epoch
      responses:
        200:
          description: OK
      tags:
      - User
      - Link
      - Save
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