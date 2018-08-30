---
swagger: "2.0"
x-collection-name: Bitly
x-complete: 0
info:
  title: Bitly Link API Get User Save Custom Domain Keyword
  description: Get user save custom domain keyword.
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
  /v3/user/info:
    get:
      summary: Get User Info
      description: Return information about a user.
      operationId: Get_user_info_
      x-api-path-slug: v3userinfo-get
      parameters:
      - in: query
        name: format
        description: Response format
      - in: query
        name: login
        description: (optional) the bitly login of the user whose info to look up
      responses:
        200:
          description: OK
      tags:
      - User
      - Info
  /v3/user/link_history:
    get:
      summary: Get User Link History
      description: Returns entries from a user's link history in reverse chronological
        order.
      operationId: Get_user_link_history_
      x-api-path-slug: v3userlink-history-get
      parameters:
      - in: query
        name: created_after
        description: (optional) timestamp as an integer unix epoch
      - in: query
        name: created_before
        description: (optional) timestamp as an integer unix epoch
      - in: query
        name: format
        description: Response format
      - in: query
        name: limit
        description: '(optional) integer in the range 1 to 100 -    default: 50, specifying
          the max number of results to return'
      - in: query
        name: user
        description: (optional)    the user for whom to retrieve history entries (if
          different from authenticated user)
      responses:
        200:
          description: OK
      tags:
      - User
      - Link
      - History
  /v3/user/popular_links:
    get:
      summary: Get User Popular Links
      description: Returns the authenticated user's most-clicked bitly links (ordered
        by number of clicks) in a given time period.
      operationId: Get_user_popular_links_
      x-api-path-slug: v3userpopular-links-get
      parameters:
      - in: query
        name: format
        description: Response format
      - in: query
        name: limit
        description: (optional) 1 to 1000 (default=100)
      - in: query
        name: rollup
        description: (optional) true or false
      - in: query
        name: timezone
        description: (optional) an integer hour offset from UTC (-14 to 14)
      - in: query
        name: unit
        description: minute, hour, day, week or month
      - in: query
        name: units
        description: an integer representing the time units to query data for
      responses:
        200:
          description: OK
      tags:
      - User
      - Popular
      - Links
  /v3/link/clicks:
    get:
      summary: Get Link Clicks
      description: Returns entries from a user's link history in reverse chronological
        order.
      operationId: Get_link_clicks_
      x-api-path-slug: v3linkclicks-get
      parameters:
      - in: query
        name: format
        description: Response format
      - in: query
        name: limit
        description: (optional) 1 to 1000 (default=100)
      - in: query
        name: link
        description: a bltly link
      - in: query
        name: rollup
        description: (optional) true or false
      - in: query
        name: timezone
        description: (optional) an integer hour offset from UTC (-14 to 14)
      - in: query
        name: unit
        description: minute, hour, day, week or month
      - in: query
        name: units
        description: an integer representing the time units to query data for
      responses:
        200:
          description: OK
      tags:
      - Link
      - Clicks
  /v3/link/countries:
    get:
      summary: Get Link Countries
      description: Returns metrics about the countries referring click traffic to
        a single bitly link.
      operationId: Get_link_countries_
      x-api-path-slug: v3linkcountries-get
      parameters:
      - in: query
        name: format
        description: Response format
      - in: query
        name: limit
        description: (optional) 1 to 1000 (default=100)
      - in: query
        name: link
        description: a bltly link
      - in: query
        name: rollup
        description: (optional) true or false
      - in: query
        name: timezone
        description: (optional) an integer hour offset from UTC (-14 to 14)
      - in: query
        name: unit
        description: minute, hour, day, week or month
      - in: query
        name: units
        description: an integer representing the time units to query data for
      responses:
        200:
          description: OK
      tags:
      - Link
      - Countries
  /v3/link/referrers:
    get:
      summary: Get Link Referrers
      description: Returns metrics about the pages referring click traffic to a single
        bitly link.
      operationId: Get_link_referrers_
      x-api-path-slug: v3linkreferrers-get
      parameters:
      - in: query
        name: format
        description: Response format
      - in: query
        name: limit
        description: (optional) 1 to 1000 (default=100)
      - in: query
        name: link
        description: a bltly link
      - in: query
        name: rollup
        description: (optional) true or false
      - in: query
        name: timezone
        description: (optional) an integer hour offset from UTC (-14 to 14)
      - in: query
        name: unit
        description: minute, hour, day, week or month
      - in: query
        name: units
        description: an integer representing the time units to query data for
      responses:
        200:
          description: OK
      tags:
      - Link
      - Referrers
  /v3/link/shares:
    get:
      summary: Get Link Shares
      description: Returns metrics about a shares of a single link.
      operationId: Get_link_shares_
      x-api-path-slug: v3linkshares-get
      parameters:
      - in: query
        name: format
        description: Response format
      - in: query
        name: limit
        description: (optional) 1 to 1000 (default=100)
      - in: query
        name: link
        description: a bltly link
      - in: query
        name: rollup
        description: (optional) true or false
      - in: query
        name: timezone
        description: (optional) an integer hour offset from UTC (-14 to 14)
      - in: query
        name: unit
        description: minute, hour, day, week or month
      - in: query
        name: units
        description: an integer representing the time units to query data for
      responses:
        200:
          description: OK
      tags:
      - Link
      - Shares
  /v3/search:
    get:
      summary: Get Search
      description: Search links receiving clicks across bitly by content, language,
        location, and more.
      operationId: Get_realtime_search_
      x-api-path-slug: v3search-get
      parameters:
      - in: query
        name: cities
        description: (optional) show links active in this city (ordered like country-state-city,
          e
      - in: query
        name: domain
        description: (optional) restrict results to this web domain
      - in: query
        name: format
        description: Response format
      - in: query
        name: lang
        description: (optional) favor results in this language (two letter ISO code)
      - in: query
        name: limit
        description: (optional) the maximum number of links to return
      - in: query
        name: offset
        description: (optional) which result to start with (defaults to 0)
      - in: query
        name: query
        description: string to query for
      responses:
        200:
          description: OK
      tags:
      - Search
  /v3/realtime/bursting_phrases:
    get:
      summary: Get Realtime Bursting Phrases
      description: Returns phrases that are receiving an uncharacteristically high
        volume of click traffic, and the individual links (hashes) driving traffic
        to pages containing these phrases.
      operationId: Get_realtime_bursting_phrases_
      x-api-path-slug: v3realtimebursting-phrases-get
      parameters:
      - in: query
        name: format
        description: Response format
      responses:
        200:
          description: OK
      tags:
      - Realtime
      - Bursting
      - Phrases
  /v3/realtime/hot_phrases:
    get:
      summary: Get Realtime Hot Phrases
      description: Returns phrases that are receiving a consistently high volume of
        click traffic, and the individual links (hashes) driving traffic to pages
        containing these phrases.
      operationId: Get_realtime_hot_phrases_
      x-api-path-slug: v3realtimehot-phrases-get
      parameters:
      - in: query
        name: format
        description: Response format
      responses:
        200:
          description: OK
      tags:
      - Realtime
      - Hot
      - Phrases
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
  /v3/user/save_custom_domain_keyword:
    get:
      summary: Get User Save Custom Domain Keyword
      description: Get user save custom domain keyword.
      operationId: getV3UserSaveCustomDomainKeyword
      x-api-path-slug: v3usersave-custom-domain-keyword-get
      parameters:
      - in: query
        name: keyword_link
        description: the Custom Bitlink (short domain and keyword combination) to
          set
      - in: query
        name: overwrite
        description: Ovewrite existing entry if one exists
      - in: query
        name: target_link
        description: the Bitlink the specified keyword will map to (as returned from
          /v3/shorten)
      responses:
        200:
          description: OK
      tags:
      - User
      - Save
      - Custom
      - Domain
      - Keyword
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