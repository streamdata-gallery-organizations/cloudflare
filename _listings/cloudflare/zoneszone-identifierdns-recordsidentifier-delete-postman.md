{
  "info": {
    "name": "CloudFlare Delete DNS record permission needed: #dns_records:edit",
    "_postman_id": "f9d691cf-f75c-47a2-a4a3-c04e58fa6ade",
    "description": "Delete DNS record permission needed: #dns_records:editntt",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Records",
      "item": [
        {
          "id": "cf1366c2-c830-4a8d-9fd7-839c78a20f44",
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
              "id": "adc5ceac-fc72-4619-93bf-7e0f63863fd8"
            }
          ]
        },
        {
          "id": "c1ab3307-8da3-4f45-89d2-71cb6295074b",
          "name": "cloudflare-dns-records-for-a-zone-api",
          "request": {
            "url": "http://example.com/api/zones/:zone_identifier/dns_records?content=%7B%7D&name=%7B%7D&type=%7B%7D",
            "method": "POST",
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
            "description": "Create a new DNS record for a zone"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9e339919-bed8-4ac6-b111-35f3b5fe05ce"
            }
          ]
        },
        {
          "id": "7dde429c-e908-4e5f-b21d-675da39c60bb",
          "name": "cloudflare-dns-records-for-a-zone-api",
          "request": {
            "url": "http://example.com/api/zones/:zone_identifier/dns_records/:identifier",
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete DNS record permission needed: #dns_records:editntt"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d546dbd2-21ca-4793-879a-c80eb3f22baf"
            }
          ]
        }
      ]
    }
  ]
}