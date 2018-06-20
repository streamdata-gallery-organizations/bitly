---
swagger: "2.0"
x-collection-name: Bitly
x-complete: 0
info:
  title: Bitly Link Metrics API Link Referrers
  description: Returns metrics about the pages referring click traffic to a single
    Bitlink.
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