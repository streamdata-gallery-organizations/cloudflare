{
  "info": {
    "name": "CloudFlare List, search, sort and filter your Railguns",
    "_postman_id": "9ea87084-38c0-48a1-bd9f-729a38700dba",
    "description": "List, search, sort and filter your Railguns",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Performance",
      "item": [
        {
          "id": "bcdfde35-e055-4c40-8b23-4bca812abda1",
          "name": "cloudflare-railgun-api",
          "request": {
            "url": "http://example.com/api/railguns?direction=%7B%7D&page=%7B%7D&per_page=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "X-AUTH-EMAIL",
                "value": "{}",
                "description": "Email address associated with your account",
                "disabled": false
              },
              {
                "key": "X-AUTH-KEY",
                "value": "{}",
                "description": "API key generated on the My Account page",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "List, search, sort and filter your Railguns"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1383df0a-0440-4ee8-8006-85f7ff01dec6"
            }
          ]
        }
      ]
    }
  ]
}