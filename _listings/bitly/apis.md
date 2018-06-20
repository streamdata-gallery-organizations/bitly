---
name: Bitly
x-slug: bitly
description: Get the most out of your social and online marketing efforts. Own, understand
  and activate your best audience through the power of the link with Bitly Enterprise.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1503-bitly.jpg
x-kinRank: "8"
x-alexaRank: "737"
tags: Bitly
created: "2018-06-19"
modified: "2018-06-19"
url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bitly/master/_listings/bitly/apis.md
specificationVersion: "0.14"
apis:
- name: Bitly Domains API Get Shorten
  x-api-slug: bitly-domains-api
  description: Given a long URL, returns a bitly short URL.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1503-bitly.jpg
  humanURL: http://bitly.com
  baseURL: https://api-ssl.bitly.com////v3/shorten
  tags: Shorten
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bitly/master/_listings/bitly/v3shorten-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bitly/master/_listings/bitly/v3shorten-get-openapi.md
- name: Bitly Domains API Get Expand
  x-api-slug: bitly-domains-api
  description: Given a bitly URL or hash (or multiple), returns the target (long)
    URL.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1503-bitly.jpg
  humanURL: http://bitly.com
  baseURL: https://api-ssl.bitly.com////v3/expand
  tags: Expand
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bitly/master/_listings/bitly/v3expand-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bitly/master/_listings/bitly/v3expand-get-openapi.md
- name: Bitly Domains API Get Link Lookup
  x-api-slug: bitly-domains-api
  description: This is used to query for a bitly link based on a long URL.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1503-bitly.jpg
  humanURL: http://bitly.com
  baseURL: https://api-ssl.bitly.com////v3/link/lookup
  tags: Link,Lookup
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bitly/master/_listings/bitly/v3linklookup-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bitly/master/_listings/bitly/v3linklookup-get-openapi.md
- name: Bitly Domains API Get Info
  x-api-slug: bitly-domains-api
  description: This is used to return the page title for a given bitly link.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1503-bitly.jpg
  humanURL: http://bitly.com
  baseURL: https://api-ssl.bitly.com////v3/info
  tags: Info
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bitly/master/_listings/bitly/v3info-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bitly/master/_listings/bitly/v3info-get-openapi.md
- name: Bitly Domains API Get User Info
  x-api-slug: bitly-domains-api
  description: Return information about a user.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1503-bitly.jpg
  humanURL: http://bitly.com
  baseURL: https://api-ssl.bitly.com////v3/user/info
  tags: User,Info
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bitly/master/_listings/bitly/v3userinfo-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bitly/master/_listings/bitly/v3userinfo-get-openapi.md
- name: Bitly Domains API Get User Link History
  x-api-slug: bitly-domains-api
  description: Returns entries from a user's link history in reverse chronological
    order.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1503-bitly.jpg
  humanURL: http://bitly.com
  baseURL: https://api-ssl.bitly.com////v3/user/link_history
  tags: User,Link,History
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bitly/master/_listings/bitly/v3userlink-history-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bitly/master/_listings/bitly/v3userlink-history-get-openapi.md
- name: Bitly Domains API Get User Popular Links
  x-api-slug: bitly-domains-api
  description: Returns the authenticated user's most-clicked bitly links (ordered
    by number of clicks) in a given time period.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1503-bitly.jpg
  humanURL: http://bitly.com
  baseURL: https://api-ssl.bitly.com////v3/user/popular_links
  tags: User,Popular,Links
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bitly/master/_listings/bitly/v3userpopular-links-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bitly/master/_listings/bitly/v3userpopular-links-get-openapi.md
- name: Bitly Domains API Get Link Clicks
  x-api-slug: bitly-domains-api
  description: Returns entries from a user's link history in reverse chronological
    order.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1503-bitly.jpg
  humanURL: http://bitly.com
  baseURL: https://api-ssl.bitly.com////v3/link/clicks
  tags: Link,Clicks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bitly/master/_listings/bitly/v3linkclicks-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bitly/master/_listings/bitly/v3linkclicks-get-openapi.md
- name: Bitly Domains API Get Link Countries
  x-api-slug: bitly-domains-api
  description: Returns metrics about the countries referring click traffic to a single
    bitly link.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1503-bitly.jpg
  humanURL: http://bitly.com
  baseURL: https://api-ssl.bitly.com////v3/link/countries
  tags: Link,Countries
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bitly/master/_listings/bitly/v3linkcountries-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bitly/master/_listings/bitly/v3linkcountries-get-openapi.md
- name: Bitly Domains API Get Link Referrers
  x-api-slug: bitly-domains-api
  description: Returns metrics about the pages referring click traffic to a single
    bitly link.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1503-bitly.jpg
  humanURL: http://bitly.com
  baseURL: https://api-ssl.bitly.com////v3/link/referrers
  tags: Link,Referrers
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bitly/master/_listings/bitly/v3linkreferrers-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bitly/master/_listings/bitly/v3linkreferrers-get-openapi.md
- name: Bitly Domains API Get Link Shares
  x-api-slug: bitly-domains-api
  description: Returns metrics about a shares of a single link.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1503-bitly.jpg
  humanURL: http://bitly.com
  baseURL: https://api-ssl.bitly.com////v3/link/shares
  tags: Link,Shares
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bitly/master/_listings/bitly/v3linkshares-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bitly/master/_listings/bitly/v3linkshares-get-openapi.md
- name: Bitly Domains API Get Search
  x-api-slug: bitly-domains-api
  description: Search links receiving clicks across bitly by content, language, location,
    and more.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1503-bitly.jpg
  humanURL: http://bitly.com
  baseURL: https://api-ssl.bitly.com////v3/search
  tags: Search
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bitly/master/_listings/bitly/v3search-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bitly/master/_listings/bitly/v3search-get-openapi.md
- name: Bitly Domains API Get Realtime Bursting Phrases
  x-api-slug: bitly-domains-api
  description: Returns phrases that are receiving an uncharacteristically high volume
    of click traffic, and the individual links (hashes) driving traffic to pages containing
    these phrases.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1503-bitly.jpg
  humanURL: http://bitly.com
  baseURL: https://api-ssl.bitly.com////v3/realtime/bursting_phrases
  tags: Realtime,Bursting,Phrases
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bitly/master/_listings/bitly/v3realtimebursting-phrases-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bitly/master/_listings/bitly/v3realtimebursting-phrases-get-openapi.md
- name: Bitly Domains API Get Realtime Hot Phrases
  x-api-slug: bitly-domains-api
  description: Returns phrases that are receiving a consistently high volume of click
    traffic, and the individual links (hashes) driving traffic to pages containing
    these phrases.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1503-bitly.jpg
  humanURL: http://bitly.com
  baseURL: https://api-ssl.bitly.com////v3/realtime/hot_phrases
  tags: Realtime,Hot,Phrases
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bitly/master/_listings/bitly/v3realtimehot-phrases-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bitly/master/_listings/bitly/v3realtimehot-phrases-get-openapi.md
- name: Bitly Domains API
  x-api-slug: bitly-domains-api
  description: Get the most out of your social and online marketing efforts. Own,
    understand and activate your best audience through the power of the link with
    Bitly Enterprise.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1503-bitly.jpg
  humanURL: http://bitly.com
  baseURL: https://api-ssl.bitly.com//
  tags: Bitly
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bitly/master/_listings/bitly/openapi.md
- name: Bitly Link API Get Search
  x-api-slug: bitly-link-api
  description: Get search.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1503-bitly.jpg
  humanURL: http://bitly.com
  baseURL: https://api-ssl.bitly.com//v3//search
  tags: Search
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bitly/master/_listings/bitly/search-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bitly/master/_listings/bitly/search-get-openapi.md
- name: Bitly Link API Get Expand
  x-api-slug: bitly-link-api
  description: Get expand.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1503-bitly.jpg
  humanURL: http://bitly.com
  baseURL: https://api-ssl.bitly.com//v3//v3/expand
  tags: Expand
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bitly/master/_listings/bitly/v3expand-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bitly/master/_listings/bitly/v3expand-get-openapi.md
- name: Bitly Link API Get Info
  x-api-slug: bitly-link-api
  description: Get info.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1503-bitly.jpg
  humanURL: http://bitly.com
  baseURL: https://api-ssl.bitly.com//v3//v3/info
  tags: Info
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bitly/master/_listings/bitly/v3info-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bitly/master/_listings/bitly/v3info-get-openapi.md
- name: Bitly Link API Get Link Lookup
  x-api-slug: bitly-link-api
  description: Get link lookup.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1503-bitly.jpg
  humanURL: http://bitly.com
  baseURL: https://api-ssl.bitly.com//v3//v3/link/lookup
  tags: Link,Lookup
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bitly/master/_listings/bitly/v3linklookup-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bitly/master/_listings/bitly/v3linklookup-get-openapi.md
- name: Bitly Link API Get Shorten
  x-api-slug: bitly-link-api
  description: Get shorten.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1503-bitly.jpg
  humanURL: http://bitly.com
  baseURL: https://api-ssl.bitly.com//v3//v3/shorten
  tags: Shorten
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bitly/master/_listings/bitly/v3shorten-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bitly/master/_listings/bitly/v3shorten-get-openapi.md
- name: Bitly Link API Get User Link Edit
  x-api-slug: bitly-link-api
  description: Get user link edit.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1503-bitly.jpg
  humanURL: http://bitly.com
  baseURL: https://api-ssl.bitly.com//v3//v3/user/link_edit
  tags: User,Link,Edit
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bitly/master/_listings/bitly/v3userlink-edit-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bitly/master/_listings/bitly/v3userlink-edit-get-openapi.md
- name: Bitly Link API Get User Link Lookup
  x-api-slug: bitly-link-api
  description: Get user link lookup.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1503-bitly.jpg
  humanURL: http://bitly.com
  baseURL: https://api-ssl.bitly.com//v3//v3/user/link_lookup
  tags: User,Link,Lookup
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bitly/master/_listings/bitly/v3userlink-lookup-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bitly/master/_listings/bitly/v3userlink-lookup-get-openapi.md
- name: Bitly Link API Get User Link Save
  x-api-slug: bitly-link-api
  description: Get user link save.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1503-bitly.jpg
  humanURL: http://bitly.com
  baseURL: https://api-ssl.bitly.com//v3//v3/user/link_save
  tags: User,Link,Save
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bitly/master/_listings/bitly/v3userlink-save-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bitly/master/_listings/bitly/v3userlink-save-get-openapi.md
- name: Bitly Link API Get User Save Custom Domain Keyword
  x-api-slug: bitly-link-api
  description: Get user save custom domain keyword.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1503-bitly.jpg
  humanURL: http://bitly.com
  baseURL: https://api-ssl.bitly.com//v3//v3/user/save_custom_domain_keyword
  tags: User,Save,Custom,Domain,Keyword
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bitly/master/_listings/bitly/v3usersave-custom-domain-keyword-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bitly/master/_listings/bitly/v3usersave-custom-domain-keyword-get-openapi.md
- name: Bitly Link API
  x-api-slug: bitly-link-api
  description: Get the most out of your social and online marketing efforts. Own,
    understand and activate your best audience through the power of the link with
    Bitly Enterprise.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1503-bitly.jpg
  humanURL: http://bitly.com
  baseURL: https://api-ssl.bitly.com//v3
  tags: Bitly
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bitly/master/_listings/bitly/openapi.md
- name: Bitly Link Metrics API Link Clicks
  x-api-slug: bitly-link-metrics-api
  description: Returns the number of clicks on a single Bitlink.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1503-bitly.jpg
  humanURL: http://bitly.com
  baseURL: https://api-ssl.bitly.com//v3//link/clicks
  tags: Link,Clicks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bitly/master/_listings/bitly/linkclicks-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bitly/master/_listings/bitly/linkclicks-get-openapi.md
- name: Bitly Link Metrics API Link Clicks by Country
  x-api-slug: bitly-link-metrics-api
  description: Returns metrics about the countries referring click traffic to a single
    Bitlink.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1503-bitly.jpg
  humanURL: http://bitly.com
  baseURL: https://api-ssl.bitly.com//v3//link/countries
  tags: Link,Countries
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bitly/master/_listings/bitly/linkcountries-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bitly/master/_listings/bitly/linkcountries-get-openapi.md
- name: Bitly Link Metrics API User Who Encoded Link
  x-api-slug: bitly-link-metrics-api
  description: Returns users who have encoded this long URL (optionally only those
    in the requesting users social graph).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1503-bitly.jpg
  humanURL: http://bitly.com
  baseURL: https://api-ssl.bitly.com//v3//link/encoders
  tags: Link,Encoders
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bitly/master/_listings/bitly/linkencoders-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bitly/master/_listings/bitly/linkencoders-get-openapi.md
- name: Bitly Link Metrics API Users Who Encoded Link
  x-api-slug: bitly-link-metrics-api
  description: Returns users who have encoded this link (optionally only those in
    the requesting users social graph), sorted by the number of clicks on each encoding
    users link.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1503-bitly.jpg
  humanURL: http://bitly.com
  baseURL: https://api-ssl.bitly.com//v3//link/encoders_by_count
  tags: Link,Encoders,By,Count
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bitly/master/_listings/bitly/linkencoders-by-count-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bitly/master/_listings/bitly/linkencoders-by-count-get-openapi.md
- name: Bitly Link Metrics API Number of Encoders
  x-api-slug: bitly-link-metrics-api
  description: Returns the number of users who have shortened (encoded) a single Bitlink.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1503-bitly.jpg
  humanURL: http://bitly.com
  baseURL: https://api-ssl.bitly.com//v3//link/encoders_count
  tags: Link,Encoders,Count
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bitly/master/_listings/bitly/linkencoders-count-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bitly/master/_listings/bitly/linkencoders-count-get-openapi.md
- name: Bitly Link Metrics API Link Referrers
  x-api-slug: bitly-link-metrics-api
  description: Returns metrics about the pages referring click traffic to a single
    Bitlink.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1503-bitly.jpg
  humanURL: http://bitly.com
  baseURL: https://api-ssl.bitly.com//v3//link/referrers
  tags: Link,Referrers
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bitly/master/_listings/bitly/linkreferrers-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bitly/master/_listings/bitly/linkreferrers-get-openapi.md
- name: Bitly Link Metrics API Link Referrers by Domain
  x-api-slug: bitly-link-metrics-api
  description: Returns metrics about the pages referring click traffic to a single
    Bitlink, grouped by referring domain.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1503-bitly.jpg
  humanURL: http://bitly.com
  baseURL: https://api-ssl.bitly.com//v3//link/referrers_by_domain
  tags: Link,Referrers,By,Domain
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bitly/master/_listings/bitly/linkreferrers-by-domain-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bitly/master/_listings/bitly/linkreferrers-by-domain-get-openapi.md
- name: Bitly Link Metrics API
  x-api-slug: bitly-link-metrics-api
  description: Get the most out of your social and online marketing efforts. Own,
    understand and activate your best audience through the power of the link with
    Bitly Enterprise.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1503-bitly.jpg
  humanURL: http://bitly.com
  baseURL: https://api-ssl.bitly.com//v3
  tags: Bitly
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bitly/master/_listings/bitly/openapi.md
- name: Bitly Organization Metric API Organization Brand Messages
  x-api-slug: bitly-organization-metric-api
  description: Returns the top Bitlinks created by you with traffic, that did not
    also have non-organization traffic in the same time period, ordered by clicks.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1503-bitly.jpg
  humanURL: http://bitly.com
  baseURL: https://api-ssl.bitly.com//v3//v3/organization/brand_messages
  tags: Organization,Brand,Messages
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bitly/master/_listings/bitly/v3organizationbrand-messages-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bitly/master/_listings/bitly/v3organizationbrand-messages-get-openapi.md
- name: Bitly Organization Metric API Organization Clicks
  x-api-slug: bitly-organization-metric-api
  description: Returns the number of clicks on Bitlinks created by your organization
    or by other Bitly users that point to your domains.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1503-bitly.jpg
  humanURL: http://bitly.com
  baseURL: https://api-ssl.bitly.com//v3//v3/organization/clicks
  tags: Organization,Clicks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bitly/master/_listings/bitly/v3organizationclicks-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bitly/master/_listings/bitly/v3organizationclicks-get-openapi.md
- name: Bitly Organization Metric API Organization Intersecting Links
  x-api-slug: bitly-organization-metric-api
  description: Returns the top links shared by both your audience and by your account,
    ordered by clicks.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1503-bitly.jpg
  humanURL: http://bitly.com
  baseURL: https://api-ssl.bitly.com//v3//v3/organization/intersecting_links
  tags: Organization,Intersecting,Links
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bitly/master/_listings/bitly/v3organizationintersecting-links-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bitly/master/_listings/bitly/v3organizationintersecting-links-get-openapi.md
- name: Bitly Organization Metric API Organization Leaderboard
  x-api-slug: bitly-organization-metric-api
  description: Returns the top-performing organization members ordered by clicks or
    shortens.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1503-bitly.jpg
  humanURL: http://bitly.com
  baseURL: https://api-ssl.bitly.com//v3//v3/organization/leaderboard
  tags: Organization,Leaderboard
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bitly/master/_listings/bitly/v3organizationleaderboard-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bitly/master/_listings/bitly/v3organizationleaderboard-get-openapi.md
- name: Bitly Organization Metric API Organization Missed Opportunities
  x-api-slug: bitly-organization-metric-api
  description: Returns the top links shared by your audience, but not by you, ordered
    by clicks.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1503-bitly.jpg
  humanURL: http://bitly.com
  baseURL: https://api-ssl.bitly.com//v3//v3/organization/missed_opportunities
  tags: Organization,Missed,Opportunities
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bitly/master/_listings/bitly/v3organizationmissed-opportunities-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bitly/master/_listings/bitly/v3organizationmissed-opportunities-get-openapi.md
- name: Bitly Organization Metric API Organization Popular Links
  x-api-slug: bitly-organization-metric-api
  description: Returns the top links shared by you or your audience, ordered by clicks
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1503-bitly.jpg
  humanURL: http://bitly.com
  baseURL: https://api-ssl.bitly.com//v3//v3/organization/popular_links
  tags: Organization,Popular,Links
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bitly/master/_listings/bitly/v3organizationpopular-links-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bitly/master/_listings/bitly/v3organizationpopular-links-get-openapi.md
- name: Bitly Organization Metric API Organization Shorten Counts
  x-api-slug: bitly-organization-metric-api
  description: Returns the number of Bitlinks created by your organization or by other
    Bitly users that point to your domains.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1503-bitly.jpg
  humanURL: http://bitly.com
  baseURL: https://api-ssl.bitly.com//v3//v3/organization/shorten_counts
  tags: Organization,Shorten,Counts
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bitly/master/_listings/bitly/v3organizationshorten-counts-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bitly/master/_listings/bitly/v3organizationshorten-counts-get-openapi.md
- name: Bitly Organization Metric API
  x-api-slug: bitly-organization-metric-api
  description: Get the most out of your social and online marketing efforts. Own,
    understand and activate your best audience through the power of the link with
    Bitly Enterprise.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1503-bitly.jpg
  humanURL: http://bitly.com
  baseURL: https://api-ssl.bitly.com//v3
  tags: Bitly
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bitly/master/_listings/bitly/openapi.md
- name: Bitly User API OAuth App
  x-api-slug: bitly-user-api
  description: Return information about an OAuth app.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1503-bitly.jpg
  humanURL: http://bitly.com
  baseURL: https://api-ssl.bitly.com//v3//v3/oauth/app
  tags: OAuth,App
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bitly/master/_listings/bitly/v3oauthapp-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bitly/master/_listings/bitly/v3oauthapp-get-openapi.md
- name: Bitly User API User Info
  x-api-slug: bitly-user-api
  description: Return or update information about a user.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1503-bitly.jpg
  humanURL: http://bitly.com
  baseURL: https://api-ssl.bitly.com//v3//v3/user/info
  tags: User,Info
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bitly/master/_listings/bitly/v3userinfo-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bitly/master/_listings/bitly/v3userinfo-get-openapi.md
- name: Bitly User API User Link History
  x-api-slug: bitly-user-api
  description: Returns entries from a users link history in reverse chronological
    order.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1503-bitly.jpg
  humanURL: http://bitly.com
  baseURL: https://api-ssl.bitly.com//v3//v3/user/link_history
  tags: User,Link,History
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bitly/master/_listings/bitly/v3userlink-history-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bitly/master/_listings/bitly/v3userlink-history-get-openapi.md
- name: Bitly User API User Network History
  x-api-slug: bitly-user-api
  description: Returns entries from a users network history in reverse chronogical
    order. (A users network history includes publicly saved links from Twitter and
    Facebook connections.)
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1503-bitly.jpg
  humanURL: http://bitly.com
  baseURL: https://api-ssl.bitly.com//v3//v3/user/network_history
  tags: User,Network,History
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bitly/master/_listings/bitly/v3usernetwork-history-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bitly/master/_listings/bitly/v3usernetwork-history-get-openapi.md
- name: Bitly User API User Tracking Domain List
  x-api-slug: bitly-user-api
  description: Returns a list of tracking domains a user has configured.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1503-bitly.jpg
  humanURL: http://bitly.com
  baseURL: https://api-ssl.bitly.com//v3//v3/user/tracking_domain_list
  tags: User,Tracking,Domain,List
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bitly/master/_listings/bitly/v3usertracking-domain-list-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bitly/master/_listings/bitly/v3usertracking-domain-list-get-openapi.md
- name: Bitly User API
  x-api-slug: bitly-user-api
  description: Get the most out of your social and online marketing efforts. Own,
    understand and activate your best audience through the power of the link with
    Bitly Enterprise.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1503-bitly.jpg
  humanURL: http://bitly.com
  baseURL: https://api-ssl.bitly.com//v3
  tags: Bitly
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bitly/master/_listings/bitly/openapi.md
- name: Bitly User Metrics API User Clicks
  x-api-slug: bitly-user-metrics-api
  description: Returns the aggregate number of clicks on all of the authenticated
    users Bitlinks.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1503-bitly.jpg
  humanURL: http://bitly.com
  baseURL: https://api-ssl.bitly.com//v3//v3/user/clicks
  tags: User,Clicks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bitly/master/_listings/bitly/v3userclicks-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bitly/master/_listings/bitly/v3userclicks-get-openapi.md
- name: Bitly User Metrics API User Countries
  x-api-slug: bitly-user-metrics-api
  description: Returns aggregate metrics about the countries referring click traffic
    to all of the authenticated users Bitlinks.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1503-bitly.jpg
  humanURL: http://bitly.com
  baseURL: https://api-ssl.bitly.com//v3//v3/user/countries
  tags: User,Countries
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bitly/master/_listings/bitly/v3usercountries-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bitly/master/_listings/bitly/v3usercountries-get-openapi.md
- name: Bitly User Metrics API User Popular Earned By Clicks
  x-api-slug: bitly-user-metrics-api
  description: Returns the top links to your tracking domain (or domains) created
    by users not associated with your account, ordered by clicks.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1503-bitly.jpg
  humanURL: http://bitly.com
  baseURL: https://api-ssl.bitly.com//v3//v3/user/popular_earned_by_clicks
  tags: User,Popular,Earned,Clicks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bitly/master/_listings/bitly/v3userpopular-earned-by-clicks-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bitly/master/_listings/bitly/v3userpopular-earned-by-clicks-get-openapi.md
- name: Bitly User Metrics API User Popular Earned By Shortens
  x-api-slug: bitly-user-metrics-api
  description: Returns the top links to your tracking domain (or domains) created
    by users not associated with your account, ordered by shortens.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1503-bitly.jpg
  humanURL: http://bitly.com
  baseURL: https://api-ssl.bitly.com//v3//v3/user/popular_earned_by_shortens
  tags: User,Popular,Earned,Shortens
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bitly/master/_listings/bitly/v3userpopular-earned-by-shortens-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bitly/master/_listings/bitly/v3userpopular-earned-by-shortens-get-openapi.md
- name: Bitly User Metrics API User Popular Links
  x-api-slug: bitly-user-metrics-api
  description: Returns the authenticated users most-clicked Bitlinks (ordered by number
    of clicks) in a given time period.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1503-bitly.jpg
  humanURL: http://bitly.com
  baseURL: https://api-ssl.bitly.com//v3//v3/user/popular_links
  tags: User,Popular,Links
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bitly/master/_listings/bitly/v3userpopular-links-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bitly/master/_listings/bitly/v3userpopular-links-get-openapi.md
- name: Bitly User Metrics API User Popular Owned By Clicks
  x-api-slug: bitly-user-metrics-api
  description: Returns the top links to your tracking domain (or domains) created
    by you or your subaccounts ordered by clicks.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1503-bitly.jpg
  humanURL: http://bitly.com
  baseURL: https://api-ssl.bitly.com//v3//v3/user/popular_owned_by_clicks
  tags: User,Popular,Owned,Clicks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bitly/master/_listings/bitly/v3userpopular-owned-by-clicks-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bitly/master/_listings/bitly/v3userpopular-owned-by-clicks-get-openapi.md
- name: Bitly User Metrics API User Popular Owned by Shortens
  x-api-slug: bitly-user-metrics-api
  description: Returns the top links to your tracking domain (or domains) created
    by you or your subaccounts ordered by number of shortens.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1503-bitly.jpg
  humanURL: http://bitly.com
  baseURL: https://api-ssl.bitly.com//v3//v3/user/popular_owned_by_shortens
  tags: User,Popular,Owned,By,Shortens
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bitly/master/_listings/bitly/v3userpopular-owned-by-shortens-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bitly/master/_listings/bitly/v3userpopular-owned-by-shortens-get-openapi.md
- name: Bitly User Metrics API User Referrers
  x-api-slug: bitly-user-metrics-api
  description: Returns aggregate metrics about the pages referring click traffic to
    all of the authenticated users Bitlinks.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1503-bitly.jpg
  humanURL: http://bitly.com
  baseURL: https://api-ssl.bitly.com//v3//v3/user/referrers
  tags: User,Referrers
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bitly/master/_listings/bitly/v3userreferrers-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bitly/master/_listings/bitly/v3userreferrers-get-openapi.md
- name: Bitly User Metrics API User Referring Domains
  x-api-slug: bitly-user-metrics-api
  description: eturns aggregate metrics about the domains referring click traffic
    to all of the authenticated users Bitlinks. If the user is a master account, or
    is a subaccount with full_reports permission, the user may choose to view the
    metrics of any account belonging to the master account.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1503-bitly.jpg
  humanURL: http://bitly.com
  baseURL: https://api-ssl.bitly.com//v3//v3/user/referring_domains
  tags: User,Referring,Domains
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bitly/master/_listings/bitly/v3userreferring-domains-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bitly/master/_listings/bitly/v3userreferring-domains-get-openapi.md
- name: Bitly User Metrics API User Shorten Counts
  x-api-slug: bitly-user-metrics-api
  description: Returns the number of Bitlinks created in a given time period by the
    authenticated user.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1503-bitly.jpg
  humanURL: http://bitly.com
  baseURL: https://api-ssl.bitly.com//v3//v3/user/shorten_counts
  tags: User,Shorten,Counts
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bitly/master/_listings/bitly/v3usershorten-counts-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bitly/master/_listings/bitly/v3usershorten-counts-get-openapi.md
- name: Bitly User Metrics API
  x-api-slug: bitly-user-metrics-api
  description: Get the most out of your social and online marketing efforts. Own,
    understand and activate your best audience through the power of the link with
    Bitly Enterprise.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1503-bitly.jpg
  humanURL: http://bitly.com
  baseURL: https://api-ssl.bitly.com//v3
  tags: Bitly
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bitly/master/_listings/bitly/openapi.md
x-common:
- type: x--net-library
  url: http://code.google.com/p/bitly-dot-net
- type: x-application-management
  url: http://dev.bitly.com/my_apps.html
- type: x-base
  url: http://api.bitly.com
- type: x-best-practices
  url: http://dev.bitly.com/best_practices.html
- type: x-blog
  url: http://word.bitly.com/
- type: x-blog-rss
  url: http://word.bitly.com/rss
- type: x-crunchbase
  url: http://www.crunchbase.com/company/bit-ly
- type: x-crunchbase
  url: https://crunchbase.com/organization/hootsuite
- type: x-crunchbase
  url: https://crunchbase.com/organization/bitly
- type: x-developer
  url: http://data.info.yorku.ca/
- type: x-email
  url: media@hootsuite.com
- type: x-email
  url: legal@hootsuite.com
- type: x-email
  url: privacy@hootsuite.com
- type: x-email
  url: hootsuite-dpa@hootsuite.com
- type: x-email
  url: security@hootsuite.com
- type: x-email
  url: app.directory@hootsuite.com
- type: x-email
  url: apis@hootsuite.com
- type: x-email
  url: partnersupport@hootsuite.com
- type: x-email
  url: partners@bitly.com
- type: x-email
  url: press@bitly.com
- type: x-email
  url: office@bitly.com
- type: x-email
  url: support@bitly.com
- type: x-email
  url: api@bitly.com
- type: x-forum
  url: http://dev.bitly.com/api_discussion_group.html
- type: x-github
  url: https://github.com/bitly
- type: x-java-library
  url: https://github.com/stackmagic/bitly-api-client
- type: x-javascript-library
  url: https://npmjs.org/package/node-bitlyapi
- type: x-partners
  url: https://bitly.com/pages/partners
- type: x-php-library
  url: http://github.com/Falicon/BitlyPHP
- type: x-privacy
  url: https://bitly.com/pages/privacy
- type: x-python-library
  url: http://github.com/bitly/bitly-api-python
- type: x-ruby-library
  url: http://github.com/nas/url_shortener
- type: x-sdks-io
  url: https://sdks.io/SDK/View/bitly-13
- type: x-support
  url: http://support.bitly.com/
- type: x-temboo-pdk
  url: https://live.temboo.com/library/Library/Bitly/
- type: x-terms-of-service
  url: https://bitly.com/pages/terms-of-service
- type: x-twitter
  url: https://twitter.com/Bitly
- type: x-twitter
  url: https://twitter.com/hootsuite
- type: x-website
  url: http://bitly.com
- type: x-website
  url: http://dev.bitly.com/data_apis.html
- type: x-website
  url: http://bit.ly/1j56kms
- type: x-website
  url: http://hootsuite.com
- type: x-website
  url: http://bit.ly
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---