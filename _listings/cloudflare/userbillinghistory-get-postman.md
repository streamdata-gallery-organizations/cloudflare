{
  "info": {
    "name": "CloudFlare Access your billing history object",
    "_postman_id": "733022b8-2797-4794-b1cd-c977bb821dad",
    "description": "Access your billing history object",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Billing History",
      "item": [
        {
          "id": "7c0ae7fa-55f3-43fa-bda3-8ec00866857a",
          "name": "cloudflare-user-billing-history-api",
          "request": {
            "url": "http://example.com/api/user/billing/history?action=%7B%7D&occured_at=%7B%7D&order=%7B%7D&page=%7B%7D&per_page=%7B%7D&type=%7B%7D",
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
            "description": "Access your billing history object"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d3fb2bd3-23a8-4cba-b0cf-5c09b87a6514"
            }
          ]
        }
      ]
    }
  ]
}