{
  "info": {
    "name": "CloudFlare Update DNS record permission needed: #dns_records:edit",
    "_postman_id": "7bcbc2da-515d-4cc0-bc92-9fd993d499b2",
    "description": "Update DNS record permission needed: #dns_records:editntt",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Records",
      "item": [
        {
          "id": "133d590b-f09b-4282-b94f-f40ef021f44f",
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
              "id": "f17a7e2e-4f19-4f03-9ecc-c575d61653d6"
            }
          ]
        },
        {
          "id": "bceafad7-a3c4-4389-9313-9c1074c92d30",
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
              "id": "0ebebfda-ecff-404a-a13b-a7553fa7fc01"
            }
          ]
        },
        {
          "id": "db194e0b-3b7c-4f93-aa2e-73ed0f6be73b",
          "name": "cloudflare-dns-records-for-a-zone-api",
          "request": {
            "url": "http://example.com/api/zones/:zone_identifier/dns_records/:identifier",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "DNS record details permission needed: #dns_records:readntt"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f7ccdee6-e4dd-454a-ae7b-d924d8103462"
            }
          ]
        },
        {
          "id": "8fa934ab-c940-4e34-a1e4-d4597e1ae8a8",
          "name": "cloudflare-dns-records-for-a-zone-api",
          "request": {
            "url": "http://example.com/api/zones/:zone_identifier/dns_records/:identifier",
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Update DNS record permission needed: #dns_records:editntt"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ad72b62b-c6d5-41bf-835f-cc30bffaea5f"
            }
          ]
        },
        {
          "id": "049fe645-3777-4963-992d-336a972f331e",
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
              "id": "cfbc04d9-a6b2-4515-a9fa-a60726b8db01"
            }
          ]
        }
      ]
    }
  ]
}