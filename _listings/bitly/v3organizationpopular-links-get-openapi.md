---
swagger: "2.0"
x-collection-name: Bitly
x-complete: 0
info:
  title: Bitly Organization Metric API Organization Popular Links
  description: Returns the top links shared by you or your audience, ordered by clicks
  termsOfService: http://dev.bitly.com/best_practices.html
  version: v3
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
  /link/clicks:
    get:
      summary: Link Clicks
      description: Returns the number of clicks on a single Bitlink.
      operationId: linkClicks
      x-api-path-slug: linkclicks-get
      parameters:
      - in: query
        name: format
        description: json, xml, txt
      - in: query
        name: limit
        description: 1 to 1000 (default=100)
      - in: query
        name: link
        description: a Bitlink
      - in: query
        name: rollup
        description: Return data for multiple units rolled up to a single result instead
          of a separate value for each period of time
      - in: query
        name: timezone
        description: 'an integer hour offset from UTC (-14 to 14), or a timezone string
          default: America/New_York'
      - in: query
        name: unit
        description: 'minute, hour, day, week or month, default: day'
      - in: query
        name: units
        description: an integer representing the time units to query data for
      - in: query
        name: unit_reference_ts
        description: 'an epoch timestamp, indicating the most recent time for which
          to pull metrics, default: now'
      responses:
        200:
          description: OK
      tags:
      - Link
      - Clicks
  /link/countries:
    get:
      summary: Link Clicks by Country
      description: Returns metrics about the countries referring click traffic to
        a single Bitlink.
      operationId: linkClicksbyCountry
      x-api-path-slug: linkcountries-get
      parameters:
      - in: query
        name: link
        description: a Bitlink
      - in: query
        name: timezone
        description: an integer hour offset from UTC (-14
      - in: query
        name: unit
        description: minute | hour | day | week | month default:day
      - in: query
        name: units
        description: an integer representing the time units to query data for
      - in: query
        name: unit_reference_ts
        description: an epoch timestamp, indicating the most recent time for which
          to pull metrics
      responses:
        200:
          description: OK
      tags:
      - Link
      - Countries
  /link/encoders:
    get:
      summary: User Who Encoded Link
      description: Returns users who have encoded this long URL (optionally only those
        in the requesting users social graph).
      operationId: userWhoEncodedLink
      x-api-path-slug: linkencoders-get
      parameters:
      - in: query
        name: expand_user
        description: include display names of encoders
      - in: query
        name: limit
        description: 'integer in the range of 1 to 25 that specifies the number of
          records to return (default: 10)'
      - in: query
        name: link
        description: a Bitlink
      - in: query
        name: my_network
        description: restrict to my network
      - in: query
        name: subaccounts
        description: true or false - restrict to this enterprise account and its subaccounts
      responses:
        200:
          description: OK
      tags:
      - Link
      - Encoders
  /link/encoders_by_count:
    get:
      summary: Users Who Encoded Link
      description: Returns users who have encoded this link (optionally only those
        in the requesting users social graph), sorted by the number of clicks on each
        encoding users link.
      operationId: usersWhoEncodedLink
      x-api-path-slug: linkencoders-by-count-get
      parameters:
      - in: query
        name: expand_user
        description: include display names of encoders
      - in: query
        name: limit
        description: integer in the range 1:100 that specifies the number of records
          to return (default:10)
      - in: query
        name: link
        description: a Bitlink
      - in: query
        name: my_network
        description: restrict to my network
      - in: query
        name: subaccounts
        description: restrict to this enterprise account and its subaccounts
      responses:
        200:
          description: OK
      tags:
      - Link
      - Encoders
      - By
      - Count
  /link/encoders_count:
    get:
      summary: Number of Encoders
      description: Returns the number of users who have shortened (encoded) a single
        Bitlink.
      operationId: numberOfEncoders
      x-api-path-slug: linkencoders-count-get
      parameters:
      - in: query
        name: link
        description: a Bitlink
      responses:
        200:
          description: OK
      tags:
      - Link
      - Encoders
      - Count
  /link/referrers:
    get:
      summary: Link Referrers
      description: Returns metrics about the pages referring click traffic to a single
        Bitlink.
      operationId: linkReferrers
      x-api-path-slug: linkreferrers-get
      parameters:
      - in: query
        name: link
        description: a Bitlink
      - in: query
        name: timezone
        description: an integer hour offset from UTC (-14
      - in: query
        name: unit
        description: minute | hour | day | week | month default:day
      - in: query
        name: units
        description: an integer representing the time units to query data for
      - in: query
        name: unit_reference_ts
        description: an epoch timestamp, indicating the most recent time for which
          to pull metrics
      responses:
        200:
          description: OK
      tags:
      - Link
      - Referrers
  /link/referrers_by_domain:
    get:
      summary: Link Referrers by Domain
      description: Returns metrics about the pages referring click traffic to a single
        Bitlink, grouped by referring domain.
      operationId: linkReferrersByDomain
      x-api-path-slug: linkreferrers-by-domain-get
      parameters:
      - in: query
        name: link
        description: a Bitlink
      - in: query
        name: timezone
        description: an integer hour offset from UTC (-14
      - in: query
        name: unit
        description: minute | hour | day | week | month default:day
      - in: query
        name: units
        description: an integer representing the time units to query data for
      - in: query
        name: unit_reference_ts
        description: an epoch timestamp, indicating the most recent time for which
          to pull metrics
      responses:
        200:
          description: OK
      tags:
      - Link
      - Referrers
      - By
      - Domain
  /v3/organization/brand_messages:
    get:
      summary: Organization Brand Messages
      description: Returns the top Bitlinks created by you with traffic, that did
        not also have non-organization traffic in the same time period, ordered by
        clicks.
      operationId: organizationBrandMessages
      x-api-path-slug: v3organizationbrand-messages-get
      parameters:
      - in: query
        name: domain
        description: a tracking or e2e domain for this organization
      - in: query
        name: limit
        description: "1"
      - in: query
        name: timezone
        description: an integer hour offset from UTC (-14
      - in: query
        name: unit
        description: hour | day | week | month default:day
      - in: query
        name: units
        description: an integer representing the time units to query data for
      - in: query
        name: unit_reference_ts
        description: an epoch timestamp, indicating the most recent time for which
          to pull metrics
      responses:
        200:
          description: OK
      tags:
      - Organization
      - Brand
      - Messages
  /v3/organization/clicks:
    get:
      summary: Organization Clicks
      description: Returns the number of clicks on Bitlinks created by your organization
        or by other Bitly users that point to your domains.
      operationId: organizationClicks
      x-api-path-slug: v3organizationclicks-get
      parameters:
      - in: query
        name: domain
        description: filter to a tracking or e2e domain for this organization
      - in: query
        name: limit
        description: "1"
      - in: query
        name: login
        description: an account in this organization
      - in: query
        name: timezone
        description: an integer hour offset from UTC (-14
      - in: query
        name: unit
        description: hour | day | week | month default:day
      - in: query
        name: units
        description: an integer representing the time units to query data for
      - in: query
        name: unit_reference_ts
        description: an epoch timestamp, indicating the most recent time for which
          to pull metrics
      responses:
        200:
          description: OK
      tags:
      - Organization
      - Clicks
  /v3/organization/intersecting_links:
    get:
      summary: Organization Intersecting Links
      description: Returns the top links shared by both your audience and by your
        account, ordered by clicks.
      operationId: organizationIntersectingLinks
      x-api-path-slug: v3organizationintersecting-links-get
      parameters:
      - in: query
        name: domain
        description: a tracking or e2e domain for this organization
      - in: query
        name: limit
        description: "1"
      - in: query
        name: timezone
        description: an integer hour offset from UTC (-14
      - in: query
        name: unit
        description: hour | day | week | month default:day
      - in: query
        name: units
        description: an integer representing the time units to query data for
      - in: query
        name: unit_reference_ts
        description: an epoch timestamp, indicating the most recent time for which
          to pull metrics
      responses:
        200:
          description: OK
      tags:
      - Organization
      - Intersecting
      - Links
  /v3/organization/leaderboard:
    get:
      summary: Organization Leaderboard
      description: Returns the top-performing organization members ordered by clicks
        or shortens.
      operationId: organizationLeaderBoard
      x-api-path-slug: v3organizationleaderboard-get
      parameters:
      - in: query
        name: domain
        description: a tracking or e2e domain for this organization
      - in: query
        name: limit
        description: "1"
      - in: query
        name: orderby
        description: either clicks or shortens
      - in: query
        name: timezone
        description: an integer hour offset from UTC (-14
      - in: query
        name: unit
        description: hour | day | week | month default:day
      - in: query
        name: units
        description: an integer representing the time units to query data for
      - in: query
        name: unit_reference_ts
        description: an epoch timestamp, indicating the most recent time for which
          to pull metrics
      responses:
        200:
          description: OK
      tags:
      - Organization
      - Leaderboard
  /v3/organization/missed_opportunities:
    get:
      summary: Organization Missed Opportunities
      description: Returns the top links shared by your audience, but not by you,
        ordered by clicks.
      operationId: organizationMissedOpportunities
      x-api-path-slug: v3organizationmissed-opportunities-get
      parameters:
      - in: query
        name: an epoch timestamp, indicating the most recent time for which to pull
          metrics. default:now
        description: hour | day | week | month default:day
      - in: query
        name: domain
        description: a tracking or e2e domain for this organization
      - in: query
        name: limit
        description: "1"
      - in: query
        name: timezone
        description: an integer hour offset from UTC (-14
      - in: query
        name: unit
        description: hour | day | week | month default:day
      - in: query
        name: units
        description: an integer representing the time units to query data for
      - in: query
        name: unit_reference_ts
        description: an epoch timestamp, indicating the most recent time for which
          to pull metrics
      responses:
        200:
          description: OK
      tags:
      - Organization
      - Missed
      - Opportunities
  /v3/organization/popular_links:
    get:
      summary: Organization Popular Links
      description: Returns the top links shared by you or your audience, ordered by
        clicks
      operationId: organizationPopularLinks
      x-api-path-slug: v3organizationpopular-links-get
      parameters:
      - in: query
        name: domain
        description: a tracking or e2e domain for this organization
      - in: query
        name: limit
        description: "1"
      - in: query
        name: timezone
        description: an integer hour offset from UTC (-14
      - in: query
        name: unit
        description: hour | day | week | month default:day
      - in: query
        name: units
        description: an integer representing the time units to query data for
      - in: query
        name: unit_reference_ts
        description: an epoch timestamp, indicating the most recent time for which
          to pull metrics
      responses:
        200:
          description: OK
      tags:
      - Organization
      - Popular
      - Links
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