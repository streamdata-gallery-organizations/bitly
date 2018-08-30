{
  "info": {
    "name": "Bitly Domains API Get Realtime Bursting Phrases",
    "_postman_id": "0051df79-63df-4533-aa23-638e840d34ef",
    "description": "Returns phrases that are receiving an uncharacteristically high volume of click traffic, and the individual links (hashes) driving traffic to pages containing these phrases.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Shorten",
      "item": [
        {
          "id": "1229da2c-9453-4726-b81f-acad3a1fdd8a",
          "name": "Get_shorten_",
          "request": {
            "url": "http://api-ssl.bitly.com/v3/shorten?domain=%7B%7D&format=%7B%7D&longUrl=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Given a long URL, returns a bitly short URL."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a85d53ef-f2a6-48bf-b846-c5c0d93d7314"
            }
          ]
        }
      ]
    },
    {
      "name": "Expand",
      "item": [
        {
          "id": "5552e266-f646-41b3-875a-f6c74e6bfad6",
          "name": "Get_expand_",
          "request": {
            "url": "http://api-ssl.bitly.com/v3/expand?format=%7B%7D&hash=%7B%7D&shortUrl=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Given a bitly URL or hash (or multiple), returns the target (long) URL."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4dafc29e-53d9-472d-bfb5-36e64a6fb862"
            }
          ]
        }
      ]
    },
    {
      "name": "Link",
      "item": [
        {
          "id": "2b08419b-fa03-41fb-9b90-51960b9f7c60",
          "name": "Get_lookup_",
          "request": {
            "url": "http://api-ssl.bitly.com/v3/link/lookup?format=%7B%7D&url=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This is used to query for a bitly link based on a long URL."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "92e78e53-7021-4df8-9be4-6a63fa2b5e80"
            }
          ]
        },
        {
          "id": "5050e70f-60f5-41c0-9bb9-66d57412a4f1",
          "name": "Get_link_clicks_",
          "request": {
            "url": "http://api-ssl.bitly.com/v3/link/clicks?format=%7B%7D&limit=%7B%7D&link=%7B%7D&rollup=%7B%7D&timezone=%7B%7D&unit=%7B%7D&units=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns entries from a user's link history in reverse chronological order."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5f205b98-6062-4069-afc0-ac825fa4fdfd"
            }
          ]
        },
        {
          "id": "183bf354-0164-486c-bb58-500f8f943112",
          "name": "Get_link_countries_",
          "request": {
            "url": "http://api-ssl.bitly.com/v3/link/countries?format=%7B%7D&limit=%7B%7D&link=%7B%7D&rollup=%7B%7D&timezone=%7B%7D&unit=%7B%7D&units=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns metrics about the countries referring click traffic to a single bitly link."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f1d6c98f-3379-42f0-a98e-0a4a4fcf7124"
            }
          ]
        },
        {
          "id": "d74f5d0a-3c50-4e0d-8e91-77f2a707f656",
          "name": "Get_link_referrers_",
          "request": {
            "url": "http://api-ssl.bitly.com/v3/link/referrers?format=%7B%7D&limit=%7B%7D&link=%7B%7D&rollup=%7B%7D&timezone=%7B%7D&unit=%7B%7D&units=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns metrics about the pages referring click traffic to a single bitly link."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "95235aaf-fb82-41da-bd1c-f528c9106f79"
            }
          ]
        },
        {
          "id": "fe07f848-e3b4-4d4b-9d82-460985f6a7de",
          "name": "Get_link_shares_",
          "request": {
            "url": "http://api-ssl.bitly.com/v3/link/shares?format=%7B%7D&limit=%7B%7D&link=%7B%7D&rollup=%7B%7D&timezone=%7B%7D&unit=%7B%7D&units=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns metrics about a shares of a single link."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ec5d7130-643e-4d4f-91c4-29dc4bdcad00"
            }
          ]
        }
      ]
    },
    {
      "name": "Info",
      "item": [
        {
          "id": "1192b0e1-8397-48a1-a4da-43e9fb83af18",
          "name": "Get_info_",
          "request": {
            "url": "http://api-ssl.bitly.com/v3/info?format=%7B%7D&hash=%7B%7D&shortUrl=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This is used to return the page title for a given bitly link."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d4a4407c-612b-4b43-9146-4df8bec2d1b1"
            }
          ]
        }
      ]
    },
    {
      "name": "User",
      "item": [
        {
          "id": "48c3a9c7-c292-4384-90da-9b0f3f350e5b",
          "name": "Get_user_info_",
          "request": {
            "url": "http://api-ssl.bitly.com/v3/user/info?format=%7B%7D&login=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Return information about a user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4d52037e-5da9-4bb2-affd-f794d5c24977"
            }
          ]
        },
        {
          "id": "e44d866e-6a9e-4c63-9e23-0368db023e98",
          "name": "Get_user_link_history_",
          "request": {
            "url": "http://api-ssl.bitly.com/v3/user/link_history?created_after=%7B%7D&created_before=%7B%7D&format=%7B%7D&limit=%7B%7D&user=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns entries from a user's link history in reverse chronological order."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "caf22aca-7655-4d01-a93c-b2a61f3c5246"
            }
          ]
        },
        {
          "id": "ccedc513-eaed-41c6-b3a3-7e56d5ef14bd",
          "name": "Get_user_popular_links_",
          "request": {
            "url": "http://api-ssl.bitly.com/v3/user/popular_links?format=%7B%7D&limit=%7B%7D&rollup=%7B%7D&timezone=%7B%7D&unit=%7B%7D&units=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the authenticated user's most-clicked bitly links (ordered by number of clicks) in a given time period."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2c1c2710-ad70-4ef3-bfd1-d37470063250"
            }
          ]
        }
      ]
    },
    {
      "name": "Search",
      "item": [
        {
          "id": "71f0ff83-d622-494b-9d7d-92e5ef1f2f77",
          "name": "Get_realtime_search_",
          "request": {
            "url": "http://api-ssl.bitly.com/v3/search?cities=%7B%7D&domain=%7B%7D&format=%7B%7D&lang=%7B%7D&limit=%7B%7D&offset=%7B%7D&query=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Search links receiving clicks across bitly by content, language, location, and more."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1fa48bdf-6780-4b83-b94b-c73d7cee284d"
            }
          ]
        }
      ]
    },
    {
      "name": "Realtime",
      "item": [
        {
          "id": "5bc543bd-178c-4bdb-bb19-338eb2f90859",
          "name": "Get_realtime_bursting_phrases_",
          "request": {
            "url": "http://api-ssl.bitly.com/v3/realtime/bursting_phrases?format=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns phrases that are receiving an uncharacteristically high volume of click traffic, and the individual links (hashes) driving traffic to pages containing these phrases."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0bbec1a6-8768-4b3f-b73b-3a439e908019"
            }
          ]
        }
      ]
    }
  ]
}