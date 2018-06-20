---
swagger: "2.0"
x-collection-name: Bitly
x-complete: 0
info:
  title: Bitly User Metrics API User Popular Earned By Shortens
  description: Returns the top links to your tracking domain (or domains) created
    by users not associated with your account, ordered by shortens.
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
  /v3/user/clicks:
    get:
      summary: User Clicks
      description: Returns the aggregate number of clicks on all of the authenticated
        users Bitlinks.
      operationId: userClicks
      x-api-path-slug: v3userclicks-get
      parameters:
      - in: query
        name: format
        description: json, xml, txt
      - in: query
        name: limit
        description: 1 to 1000 (default=100)
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
      - User
      - Clicks
  /v3/user/countries:
    get:
      summary: User Countries
      description: Returns aggregate metrics about the countries referring click traffic
        to all of the authenticated users Bitlinks.
      operationId: userCountries
      x-api-path-slug: v3usercountries-get
      parameters:
      - in: query
        name: limit
        description: 1 to 1000 (default=100)
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
        description: Successful response
      - in: query
        name: unit_reference_ts
        description: 'an epoch timestamp, indicating the most recent time for which
          to pull metrics, default: now'
      responses:
        200:
          description: OK
      tags:
      - User
      - Countries
  /v3/user/popular_earned_by_clicks:
    get:
      summary: User Popular Earned By Clicks
      description: Returns the top links to your tracking domain (or domains) created
        by users not associated with your account, ordered by clicks.
      operationId: userPopularEarnedbyClicks
      x-api-path-slug: v3userpopular-earned-by-clicks-get
      parameters:
      - in: query
        name: domain
        description: a tracking domain as returned from /v3/user/tracking_domain_list
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
      - User
      - Popular
      - Earned
      - Clicks
  /v3/user/popular_earned_by_shortens:
    get:
      summary: User Popular Earned By Shortens
      description: Returns the top links to your tracking domain (or domains) created
        by users not associated with your account, ordered by shortens.
      operationId: userPopularEarnedByShortens
      x-api-path-slug: v3userpopular-earned-by-shortens-get
      parameters:
      - in: query
        name: domain
        description: a tracking domain as returned from /v3/user/tracking_domain_list
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
      - User
      - Popular
      - Earned
      - Shortens
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