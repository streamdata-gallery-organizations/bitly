---
swagger: "2.0"
x-collection-name: Bitly
x-complete: 0
info:
  title: Bitly Domains API Get Realtime Hot Phrases
  description: Returns phrases that are receiving a consistently high volume of click
    traffic, and the individual links (hashes) driving traffic to pages containing
    these phrases.
  version: 1.0.0
host: api-ssl.bitly.com
basePath: /
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
      description: Given a long URL, returns a bitly short URL.
      operationId: Get_shorten_
      x-api-path-slug: v3shorten-get
      parameters:
      - in: query
        name: domain
        description: (optional) refers to a preferred domain; either bit
      - in: query
        name: format
        description: Response format
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
      description: Given a bitly URL or hash (or multiple), returns the target (long)
        URL.
      operationId: Get_expand_
      x-api-path-slug: v3expand-get
      parameters:
      - in: query
        name: format
        description: Response format
      - in: query
        name: hash
        description: Refers to one or more bitly hashes
      - in: query
        name: shortUrl
        description: Short URL to be expanded
      responses:
        200:
          description: OK
      tags:
      - Expand
  /v3/link/lookup:
    get:
      summary: Get Link Lookup
      description: This is used to query for a bitly link based on a long URL.
      operationId: Get_lookup_
      x-api-path-slug: v3linklookup-get
      parameters:
      - in: query
        name: format
        description: Response format
      - in: query
        name: url
        description: One or more long URLs to lookup
      responses:
        200:
          description: OK
      tags:
      - Link
      - Lookup
  /v3/info:
    get:
      summary: Get Info
      description: This is used to return the page title for a given bitly link.
      operationId: Get_info_
      x-api-path-slug: v3info-get
      parameters:
      - in: query
        name: format
        description: Response format
      - in: query
        name: hash
        description: Refers to one or more bitly hashes
      - in: query
        name: shortUrl
        description: Refers to one or more short URLs
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