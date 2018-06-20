{
  "info": {
    "name": "Bitly User API User Network History",
    "_postman_id": "314e6039-c0bf-4766-a336-9ea11ab3070f",
    "description": "Returns entries from a users network history in reverse chronogical order. (A users network history includes publicly saved links from Twitter and Facebook connections.)",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "OAuth",
      "item": [
        {
          "id": "872b19ef-72ed-4547-905e-4d76f6f32ea5",
          "name": "oauthApp",
          "request": {
            "url": "http://api-ssl.bitly.com/v3/v3/oauth/app?client_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Return information about an OAuth app."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3ff5e218-d298-4cdf-b202-9475d84118c7"
            }
          ]
        }
      ]
    },
    {
      "name": "User",
      "item": [
        {
          "id": "5593aaa0-29ea-4a16-aadd-ab627727525d",
          "name": "userInfo",
          "request": {
            "url": "http://api-ssl.bitly.com/v3/v3/user/info?full_name=%7B%7D&login=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Return or update information about a user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "346cca25-ce22-4a78-b591-5585bd2383e6"
            }
          ]
        },
        {
          "id": "5861248b-0998-42d5-8341-872c0c58f79c",
          "name": "userLinkHistory",
          "request": {
            "url": "http://api-ssl.bitly.com/v3/v3/user/link_history?archived=%7B%7D&campaign_id=%7B%7D&created_after=%7B%7D&created_before=%7B%7D&exact_domain=%7B%7D&expand_client_id=%7B%7D&keyword=%7B%7D&limit=%7B%7D&link=%7B%7D&modified_after=%7B%7D&offset=%7B%7D&private=%7B%7D&query=%7B%7D&root_domain=%7B%7D&user=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns entries from a users link history in reverse chronological order."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4ea8e8ef-7e07-4361-afb0-331785d736f4"
            }
          ]
        },
        {
          "id": "5c38da98-4eba-4956-a5dd-fccf563ee6b0",
          "name": "userNetworkHistory",
          "request": {
            "url": "http://api-ssl.bitly.com/v3/v3/user/network_history?expand_client_id=%7B%7D&expand_user=%7B%7D&limit=%7B%7D&offset=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns entries from a users network history in reverse chronogical order. (A users network history includes publicly saved links from Twitter and Facebook connections.)"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9fe90195-4c4d-4385-bcf5-96a182bc24da"
            }
          ]
        }
      ]
    }
  ]
}