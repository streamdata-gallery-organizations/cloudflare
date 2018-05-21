{
  "info": {
    "name": "CloudFlare List, search, sort, and filter a zones&#39; DNS records",
    "_postman_id": "7670a66b-e00e-48ea-ae9a-2a6dbcbbabcc",
    "description": "List, search, sort, and filter a zones&#39; DNS records",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Records",
      "item": [
        {
          "id": "50e6865d-4931-4198-bb84-957a7434fbc3",
          "name": "cloudflare-dns-records-for-a-zone-api",
          "request": {
            "url": "http://example.com/api/zones/:zone_identifier/dns_records?content=%7B%7D&direction=%7B%7D&match=%7B%7D&name=%7B%7D&order=%7B%7D&page=%7B%7D&per_page=%7B%7D&type=%7B%7D",
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
            "description": "List, search, sort, and filter a zones&#39; DNS records"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1fc1f226-e2af-4cfc-a79f-80d51ebf5dce"
            }
          ]
        }
      ]
    }
  ]
}