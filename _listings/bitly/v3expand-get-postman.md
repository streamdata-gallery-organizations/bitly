{
  "info": {
    "name": "Bitly Link API Get Expand",
    "_postman_id": "b270a968-3b2c-4553-adc8-4fab44b46390",
    "description": "Get expand.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Search",
      "item": [
        {
          "id": "fecb8dcd-7f9f-42db-b61a-cec16092404d",
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
              "id": "1c4ac6e6-c22d-4030-82a1-1edf18cc053e"
            }
          ]
        }
      ]
    },
    {
      "name": "Expand",
      "item": [
        {
          "id": "6f77a443-5e6e-4b4c-811f-24536a537a9a",
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
              "id": "8843a382-33e7-4e66-b5db-f9302e166163"
            }
          ]
        }
      ]
    }
  ]
}