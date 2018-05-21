{
  "info": {
    "name": "CloudFlare Get information about a specific role for an organization",
    "_postman_id": "5a44413a-d200-4225-80b7-8592d879dde5",
    "description": "Get information about a specific role for an organization",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Organization Roles",
      "item": [
        {
          "id": "a8eb8203-947f-43ef-85fe-d669051aa5c1",
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
              "id": "f11b645e-1316-411d-8b27-a01789625f4e"
            }
          ]
        },
        {
          "id": "47a8b6e7-e202-401b-a8cf-191e6c270f8c",
          "name": "cloudflare-organization-roles-api1",
          "request": {
            "url": "http://example.com/api/organizations/:organization_identifier/roles/:identifier",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get information about a specific role for an organization"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c42911f8-50e4-4e53-a7c5-7bcdd7db259c"
            }
          ]
        }
      ]
    }
  ]
}