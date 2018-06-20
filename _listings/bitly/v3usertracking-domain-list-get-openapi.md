---
swagger: "2.0"
x-collection-name: Bitly
x-complete: 0
info:
  title: Bitly User API User Tracking Domain List
  description: Returns a list of tracking domains a user has configured.
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
  /v3/oauth/app:
    get:
      summary: OAuth App
      description: Return information about an OAuth app.
      operationId: oauthApp
      x-api-path-slug: v3oauthapp-get
      parameters:
      - in: query
        name: client_id
        description: the client ID of the app
      responses:
        200:
          description: OK
      tags:
      - OAuth
      - App
  /v3/user/info:
    get:
      summary: User Info
      description: Return or update information about a user.
      operationId: userInfo
      x-api-path-slug: v3userinfo-get
      parameters:
      - in: query
        name: full_name
        description: set the users full name value
      - in: query
        name: login
        description: the bitly login of the user whose info to look up
      responses:
        200:
          description: OK
      tags:
      - User
      - Info
  /v3/user/link_history:
    get:
      summary: User Link History
      description: Returns entries from a users link history in reverse chronological
        order.
      operationId: userLinkHistory
      x-api-path-slug: v3userlink-history-get
      parameters:
      - in: query
        name: archived
        description: on, offor both whether to include or exclude archived history
          entries
      - in: query
        name: campaign_id
        description: filter to return only links for the given campaign_id, can be
          provided multiple times
      - in: query
        name: created_after
        description: timestamp as an integer unix epoch
      - in: query
        name: created_before
        description: timestamp as an integer unix epoch
      - in: query
        name: exact_domain
        description: n exact domain to filter on history entries
      - in: query
        name: expand_client_id
        description: whether to provide additional information about encoding application
      - in: query
        name: keyword
        description: custom keyword to filter on history entries
      - in: query
        name: limit
        description: 'integer in the range 1 to 100 default: 50, specifying the max
          number of results to return'
      - in: query
        name: link
        description: optional the Bitlink or Bitlinks to return metadata for (when
          specified, overrides all other options), can be provided multiple times
      - in: query
        name: modified_after
        description: timestamp as an integer unix epoch
      - in: query
        name: offset
        description: integer specifying the numbered result at which to start (for
          pagination)
      - in: query
        name: private
        description: on, off and both whether to include or exclude private history
          entries
      - in: query
        name: query
        description: optional ad hoc text search string
      - in: query
        name: root_domain
        description: a root domain to filter on history entries
      - in: query
        name: user
        description: the user for whom to retrieve history entries (if different from
          authenticated user)
      responses:
        200:
          description: OK
      tags:
      - User
      - Link
      - History
  /v3/user/network_history:
    get:
      summary: User Network History
      description: Returns entries from a users network history in reverse chronogical
        order. (A users network history includes publicly saved links from Twitter
        and Facebook connections.)
      operationId: userNetworkHistory
      x-api-path-slug: v3usernetwork-history-get
      parameters:
      - in: query
        name: expand_client_id
        description: whether to provide additional information about encoding application
      - in: query
        name: expand_user
        description: include extra user info in response (login, avatar_url, display_name,
          profile_url, full_name)
      - in: query
        name: limit
        description: 'integer in the range of 1 to 100 that specifies the number of
          records to return (default: 20)'
      - in: query
        name: offset
        description: integer that specifies the first record to return
      responses:
        200:
          description: OK
      tags:
      - User
      - Network
      - History
  /v3/user/tracking_domain_list:
    get:
      summary: User Tracking Domain List
      description: Returns a list of tracking domains a user has configured.
      operationId: userTrackingDomainList
      x-api-path-slug: v3usertracking-domain-list-get
      parameters:
      - in: query
        name: tracking_domains
        description: a list of tracking domains configured for the authenticated user
      responses:
        200:
          description: OK
      tags:
      - User
      - Tracking
      - Domain
      - List
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