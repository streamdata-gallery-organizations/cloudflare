{
  "info": {
    "name": "CloudFlare Get all available roles for an organization",
    "_postman_id": "b805a397-35a9-4bb9-9964-326d132db575",
    "description": "Get all available roles for an organization",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Organization Roles",
      "item": [
        {
          "id": "4a043472-2b67-491c-b0a9-7bd1c64d53d6",
          "name": "cloudflare-organization-roles-api",
          "request": {
            "url": "http://example.com/api/organizations/:organization_identifier/roles",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get all available roles for an organization"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "26345e77-ff92-4cab-bb75-9397d66ab36c"
            }
          ]
        }
      ]
    }
  ]
}