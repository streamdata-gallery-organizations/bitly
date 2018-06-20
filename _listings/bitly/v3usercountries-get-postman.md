{
  "info": {
    "name": "Bitly User Metrics API User Countries",
    "_postman_id": "35080af9-0cf4-44f2-a0bd-e42da6d83d8e",
    "description": "Returns aggregate metrics about the countries referring click traffic to all of the authenticated users Bitlinks.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "User",
      "item": [
        {
          "id": "3c86d24a-badb-412b-b707-b156cecbf839",
          "name": "userCountries",
          "request": {
            "url": "http://api-ssl.bitly.com/v3/v3/user/countries?limit=%7B%7D&rollup=%7B%7D&timezone=%7B%7D&unit=%7B%7D&units=%7B%7D&unit_reference_ts=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns aggregate metrics about the countries referring click traffic to all of the authenticated users Bitlinks."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7bb039ca-210c-4a0e-96ef-9ced05facf67"
            }
          ]
        }
      ]
    }
  ]
}