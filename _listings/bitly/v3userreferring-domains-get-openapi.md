---
swagger: "2.0"
x-collection-name: Bitly
x-complete: 0
info:
  title: Bitly User Metrics API User Referring Domains
  description: eturns aggregate metrics about the domains referring click traffic
    to all of the authenticated users Bitlinks. If the user is a master account, or
    is a subaccount with full_reports permission, the user may choose to view the
    metrics of any account belonging to the master account.
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
  /v3/user/popular_links:
    get:
      summary: User Popular Links
      description: Returns the authenticated users most-clicked Bitlinks (ordered
        by number of clicks) in a given time period.
      operationId: userPopularLinks
      x-api-path-slug: v3userpopular-links-get
      parameters:
      - in: query
        name: limit
        description: "1"
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
      - User
      - Popular
      - Links
  /v3/user/popular_owned_by_clicks:
    get:
      summary: User Popular Owned By Clicks
      description: Returns the top links to your tracking domain (or domains) created
        by you or your subaccounts ordered by clicks.
      operationId: userPopularOwnedByClicks
      x-api-path-slug: v3userpopular-owned-by-clicks-get
      parameters:
      - in: query
        name: domain
        description: a tracking domain as returned from /v3/user/tracking_domain_list
          (may be specified multiple times)
      - in: query
        name: limit
        description: "1"
      - in: query
        name: subaccount
        description: restrict to links created by this subaccount (may be specified
          multiple times)
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
      - Owned
      - Clicks
  /v3/user/popular_owned_by_shortens:
    get:
      summary: User Popular Owned by Shortens
      description: Returns the top links to your tracking domain (or domains) created
        by you or your subaccounts ordered by number of shortens.
      operationId: userPopularOwnedByShortens
      x-api-path-slug: v3userpopular-owned-by-shortens-get
      parameters:
      - in: query
        name: domain
        description: a tracking domain as returned from /v3/user/tracking_domain_list
          (may be specified multiple times)
      - in: query
        name: limit
        description: "1"
      - in: query
        name: subaccount
        description: restrict to links created by this subaccount (may be specified
          multiple times)
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
      - Owned
      - By
      - Shortens
  /v3/user/referrers:
    get:
      summary: User Referrers
      description: Returns aggregate metrics about the pages referring click traffic
        to all of the authenticated users Bitlinks.
      operationId: userReferrers
      x-api-path-slug: v3userreferrers-get
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
      - Referrers
  /v3/user/referring_domains:
    get:
      summary: User Referring Domains
      description: eturns aggregate metrics about the domains referring click traffic
        to all of the authenticated users Bitlinks. If the user is a master account,
        or is a subaccount with full_reports permission, the user may choose to view
        the metrics of any account belonging to the master account.
      operationId: userReferringDomains
      x-api-path-slug: v3userreferring-domains-get
      parameters:
      - in: query
        name: exclude_social_networks
        description: If true, exclude domains that are part of a social network that
          bitly tracks (default=true)
      - in: query
        name: limit
        description: 1 to 1000 (default=100)
      - in: query
        name: login
        description: an optional string consisting of the account name used to report
          the appropriate statistics; defaults to the current user
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
      - Referring
      - Domains
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