{
  "info": {
    "name": "CloudFlare Billing subscription details",
    "_postman_id": "7a2e9688-5ad1-46b8-9ba2-027e883e2f42",
    "description": "Billing subscription details",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Subscriptions",
      "item": [
        {
          "id": "f291e7bc-a908-4023-9405-2d480068b099",
          "name": "cloudflare-app-subscription-api",
          "request": {
            "url": "http://example.com/api/user/billing/subscriptions/apps?activated_on=%7B%7D&cancelled_on=%7B%7D&direction=%7B%7D&expired_on=%7B%7D&expires_on=%7B%7D&match=%7B%7D&order=%7B%7D&page=%7B%7D&per_page=%7B%7D&price=%7B%7D&renewed_on=%7B%7D&status=%7B%7D",
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
            "description": "List all of your app subscriptions"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "beba517e-d08b-4d96-9872-1f4de1b94675"
            }
          ]
        },
        {
          "id": "8e8184c4-a58f-47dd-8fc0-de79b3d0cc59",
          "name": "cloudflare-app-subscription-api",
          "request": {
            "url": "http://example.com/api/user/billing/subscriptions/apps/:identifier",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Billing subscription details"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "77564cd3-044e-4822-baa6-c77b38daab4b"
            }
          ]
        }
      ]
    }
  ]
}