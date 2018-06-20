{
  "info": {
    "name": "Bitly Link API Get Shorten",
    "_postman_id": "36948bd3-7361-4b62-bb4a-d670532d9c73",
    "description": "Get shorten.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Search",
      "item": [
        {
          "id": "bcaae58d-68fe-494f-a293-4b254b3c5a7e",
          "name": "getSearch",
          "request": {
            "url": "http://api-ssl.bitly.com/v3/search?cities=%7B%7D&domain=%7B%7D&fields=%7B%7D&full_domain=%7B%7D&lang=%7B%7D&limit=%7B%7D&offset=%7B%7D&query=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get search."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "55d5516c-8e20-4afc-b8fd-c318dd17d763"
            }
          ]
        }
      ]
    },
    {
      "name": "Expand",
      "item": [
        {
          "id": "094f75e9-5105-4c80-9be1-7b9e66abbdd4",
          "name": "getV3Expand",
          "request": {
            "url": "http://api-ssl.bitly.com/v3/v3/expand?format=%7B%7D&hash=%7B%7D&shortUrl=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get expand."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "28d3584a-b9cf-4db4-aa1e-0b42b55c47ad"
            }
          ]
        }
      ]
    },
    {
      "name": "Info",
      "item": [
        {
          "id": "bf660e3f-4349-43ad-be7d-bf550e26aab4",
          "name": "getV3Info",
          "request": {
            "url": "http://api-ssl.bitly.com/v3/v3/info?expand_user=%7B%7D&hash=%7B%7D&shortUrl=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get info."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "72a11b20-0d9e-4c2c-bc9b-f69774b08543"
            }
          ]
        }
      ]
    },
    {
      "name": "Link",
      "item": [
        {
          "id": "e8208f83-ce2f-4566-b8eb-adf4a00d2c63",
          "name": "getV3LinkLookup",
          "request": {
            "url": "http://api-ssl.bitly.com/v3/v3/link/lookup?url=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get link lookup."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "186f4e59-8fef-4cb3-b6e5-137df1d907f4"
            }
          ]
        }
      ]
    },
    {
      "name": "Shorten",
      "item": [
        {
          "id": "a953ab9a-6f9a-4ac7-91d1-863547f9c669",
          "name": "getV3Shorten",
          "request": {
            "url": "http://api-ssl.bitly.com/v3/v3/shorten?domain=%7B%7D&format=%7B%7D&longUrl=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get shorten."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "82f3271b-1f33-4981-a319-77cd79085e5c"
            }
          ]
        }
      ]
    }
  ]
}