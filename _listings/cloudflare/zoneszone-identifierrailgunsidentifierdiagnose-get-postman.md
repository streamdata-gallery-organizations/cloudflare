{
  "info": {
    "name": "CloudFlare Test Railgun connection to the Zone",
    "_postman_id": "02c6abda-00d4-4196-815c-d627803caca7",
    "description": "Test Railgun connection to the Zone",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Performance",
      "item": [
        {
          "id": "1009b52a-abad-4c6f-a5ff-fab4c39e5c2a",
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
              "id": "22d106d9-485e-44c3-9fab-4bace9b0a144"
            }
          ]
        },
        {
          "id": "23109b1e-1cc9-44a8-a78e-22381b8ae02a",
          "name": "cloudflare-railgun-api",
          "request": {
            "url": "http://example.com/api/railguns?name=%7B%7D",
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
            "description": "Readable identifier of the railgun"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "78f91d6b-ed99-4c11-93ef-702a095d4a9e"
            }
          ]
        },
        {
          "id": "bc860419-e906-4130-88df-9294d0c539e5",
          "name": "cloudflare-railgun-api",
          "request": {
            "url": "http://example.com/api/railguns/:identifier",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Railgun detailsntt"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1eedfe24-933c-4b93-9b0b-242e0c8a6b0e"
            }
          ]
        },
        {
          "id": "f1f5bf54-5889-476f-b001-de0616f59626",
          "name": "cloudflare-railgun-api",
          "request": {
            "url": "http://example.com/api/railguns/:identifier",
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Disable and delete a Railgun"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ac7572d3-b559-4c9c-8af7-55478520cb3c"
            }
          ]
        },
        {
          "id": "db72dfc4-12c6-4d0c-8276-c548c1ca0dcd",
          "name": "cloudflare-railgun-api",
          "request": {
            "url": "http://example.com/api/railguns/:identifier?enabled=%7B%7D",
            "method": "PATCH",
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
            "description": "Enable or disable a Railgun for all zones connected to it"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1073c1ef-414e-4300-af13-1e695c26f34e"
            }
          ]
        },
        {
          "id": "a1ef9cb7-591e-4ccf-83a2-c164cb44574c",
          "name": "cloudflare-railgun-api1",
          "request": {
            "url": "http://example.com/api/railguns/:identifier/zones",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The zones that are currently using this Railgun"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0901dd8b-51f7-44c0-939c-55c908e09971"
            }
          ]
        },
        {
          "id": "324b9f62-b96a-4397-9a4a-e42dc7da9542",
          "name": "cloudflare-railgun-connections-for-a-zone-api",
          "request": {
            "url": "http://example.com/api/zones/:zone_identifier/railguns",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "A list of available Railguns the zone can use"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f5ffc064-e619-476c-b598-0144eea48887"
            }
          ]
        },
        {
          "id": "f4dc4835-e4eb-4acc-8c99-effb53af1c89",
          "name": "cloudflare-railgun-connections-for-a-zone-api1",
          "request": {
            "url": "http://example.com/api/zones/:zone_identifier/railguns/:identifier",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Details about a specific Railgun"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b01bd187-e225-4f0e-a05a-dbde00938d95"
            }
          ]
        },
        {
          "id": "fb1c379b-9eb2-4469-ada5-87a9c58e4119",
          "name": "cloudflare-railgun-connections-for-a-zone-api",
          "request": {
            "url": "http://example.com/api/zones/:zone_identifier/railguns/:identifier?connected=%7B%7D",
            "method": "PATCH",
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
            "description": "Connect or disconnect a Railgun"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5a98fbd8-3753-4bdb-8033-5616f4167e26"
            }
          ]
        },
        {
          "id": "39b3e8fa-69f5-4d76-9f3b-f40fa2acbe92",
          "name": "cloudflare-railgun-connections-for-a-zone-api2",
          "request": {
            "url": "http://example.com/api/zones/:zone_identifier/railguns/:identifier/diagnose",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Test Railgun connection to the Zone"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d434d5c7-c59c-45ff-bc82-daac8fd6a575"
            }
          ]
        }
      ]
    }
  ]
}