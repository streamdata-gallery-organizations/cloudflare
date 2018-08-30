{
  "info": {
    "name": "CloudFlare Get a single rule group",
    "_postman_id": "49d50c0b-a8fe-48ba-9161-02e2893927cf",
    "description": "Get a single rule group",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Subscriptions",
      "item": [
        {
          "id": "a4bb9daa-1148-4c09-a37c-e7b5168dddae",
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
              "id": "8e070ad8-6e2d-419e-9381-24673a2e96f1"
            }
          ]
        },
        {
          "id": "fe2782bf-a3a0-429d-a1c9-24117e269c6d",
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
              "id": "2f451065-8890-4852-a672-28dfa9dd06da"
            }
          ]
        }
      ]
    },
    {
      "name": "Zones",
      "item": [
        {
          "id": "6783025d-e369-41ea-aa90-76006c02d7be",
          "name": "cloudflare-custom-pages-for-a-zone-api",
          "request": {
            "url": "http://example.com/api/zones/:zone_identifier/custom_pages",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "A list of available Custom Pages the zone can use"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c859a16f-1dfa-4cf5-a64d-eefcc1da404a"
            }
          ]
        },
        {
          "id": "75c160a1-bc55-45c1-a6ce-a0f55323f465",
          "name": "cloudflare-custom-pages-for-a-zone-api1",
          "request": {
            "url": "http://example.com/api/zones/:zone_identifier/custom_pages/:identifier",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Details about a specific Custom page details"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "98bae427-85c4-4e04-9856-d8d4601fdafa"
            }
          ]
        },
        {
          "id": "c1edd9bf-9d6e-4aff-88ab-9bac0a98abf5",
          "name": "cloudflare-custom-pages-for-a-zone-api",
          "request": {
            "url": "http://example.com/api/zones/:zone_identifier/custom_pages/:identifier?state=%7B%7D&url=%7B%7D",
            "method": "PUT",
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
            "description": "Update Custom page URL"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "297e094b-5a65-49f2-9294-95f08229bfa1"
            }
          ]
        }
      ]
    },
    {
      "name": "Certificates",
      "item": [
        {
          "id": "4ec4db0e-b4bf-433d-b081-c93448573c94",
          "name": "cloudflare-custom-ssl-for-a-zone-api",
          "request": {
            "url": "http://example.com/api/zones/:zone_identifier/custom_certificates?direction=%7B%7D&match=%7B%7D&order=%7B%7D&page=%7B%7D&per_page=%7B%7D&status=%7B%7D",
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
            "description": "List, search, sort, and filter all of your custom SSL certificates"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "90ad0052-7932-45cd-b3f1-00871399327e"
            }
          ]
        },
        {
          "id": "05858c5b-536b-4211-ae0c-cf2371b3c061",
          "name": "cloudflare-custom-ssl-for-a-zone-api",
          "request": {
            "url": "http://example.com/api/zones/:zone_identifier/custom_certificates?certificate=%7B%7D&private_key=%7B%7D",
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
            "description": "Upload a new SSL certificate for a zone"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a1efb45c-b48e-4045-bfd4-e5d69d30e857"
            }
          ]
        },
        {
          "id": "4688ad06-55ca-42b5-aa08-3ec1ce4c3718",
          "name": "cloudflare-custom-ssl-for-a-zone-api",
          "request": {
            "url": "http://example.com/api/zones/:zone_identifier/custom_certificates/:identifier",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "SSL configuration details permission needed: #ssl:readntt"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5295ede8-219c-400f-886e-9ddb4088d07a"
            }
          ]
        },
        {
          "id": "7f07e107-d952-4206-9cd1-37760849322c",
          "name": "cloudflare-custom-ssl-for-a-zone-api",
          "request": {
            "url": "http://example.com/api/zones/:zone_identifier/custom_certificates/:identifier",
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete an SSL certificate permission needed: #ssl:editntt"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3add3731-4e33-4638-a923-45da02bf26d1"
            }
          ]
        },
        {
          "id": "b1dfa2fa-8325-4316-adf4-392f5d11a404",
          "name": "cloudflare-custom-ssl-for-a-zone-api",
          "request": {
            "url": "http://example.com/api/zones/:zone_identifier/custom_certificates/:identifier?certificate=%7B%7D&private_key=%7B%7D",
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
            "description": "Upload a new private key and/or PEM/CRT for the SSL certificate"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "91b0edbf-cd7f-4fb0-9c9d-2be7d59dd75b"
            }
          ]
        },
        {
          "id": "a1df427a-7aef-4687-ad39-25f6c7296698",
          "name": "cloudflare-custom-ssl-for-a-zone-api",
          "request": {
            "url": "http://example.com/api/zones/:zone_identifier/custom_certificates/prioritize?certificates=%7B%7D",
            "method": "PUT",
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
            "description": "If a zone has multiple SSL certificates, you can set the order in which they should be used during a request"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fa53c155-37d4-40d8-9976-f466b293072e"
            }
          ]
        }
      ]
    },
    {
      "name": "Records",
      "item": [
        {
          "id": "58d08f12-92c6-4f47-b2b0-0d17bbbef23a",
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
              "id": "18f61c23-c199-41c2-bc71-e8d506c88ba6"
            }
          ]
        },
        {
          "id": "850cab72-f317-4061-81ff-1f221e8f162e",
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
              "id": "1c2506ce-86bb-4399-a72c-9405603d9a99"
            }
          ]
        },
        {
          "id": "352e89d5-8e9a-481d-9007-5bd2d7743912",
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
              "id": "3686decf-973d-464f-a7ab-a774845fd748"
            }
          ]
        },
        {
          "id": "1bc93887-f20f-4175-9dc0-e6a22295f90f",
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
              "id": "be76ea7e-761e-423e-a5ff-dea1e8814da8"
            }
          ]
        },
        {
          "id": "2c41ff8c-283d-4585-9fb1-6de110c8dbaa",
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
              "id": "0fde7c52-941e-4147-a2ba-1a00e5e4ae0b"
            }
          ]
        }
      ]
    },
    {
      "name": "Firewall Access Rule",
      "item": [
        {
          "id": "c9aabd47-4fab-42cb-b2d9-a44425e5d6bf",
          "name": "cloudflare-firewall-access-rule-for-a-zone-api",
          "request": {
            "url": "http://example.com/api/zones/:zone_id/firewall/access_rules/rules?configuration_target=%7B%7D&configuration_value=%7B%7D&direction=%7B%7D&match=%7B%7D&mode=%7B%7D&order=%7B%7D&page=%7B%7D&per_page=%7B%7D&scope_type=%7B%7D",
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
            "description": "Search, sort, and filter IP/country access rules"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fdaba7fa-1a9e-4dfe-8e5a-05ab4957cb1b"
            }
          ]
        },
        {
          "id": "ebe07e66-f8df-400e-90d9-1850b8d1a77a",
          "name": "cloudflare-firewall-access-rule-for-a-zone-api",
          "request": {
            "url": "http://example.com/api/zones/:zone_id/firewall/access_rules/rules?configuration=%7B%7D&mode=%7B%7D&value=%7B%7D",
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
            "description": "Make a new IP, IP range, or country access rule for the zone"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "15cc31d0-a910-46ba-a983-00e0fb1c675b"
            }
          ]
        },
        {
          "id": "aad974b7-a3c4-47f7-ad7d-ea609dc521d8",
          "name": "cloudflare-firewall-access-rule-for-a-zone-api",
          "request": {
            "url": "http://example.com/api/zones/:zone_id/firewall/access_rules/rules/:identifier?cascade=%7B%7D",
            "method": "DELETE",
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
            "description": "Remove an access rule so it is no longer evaluated during requests"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a884d670-c9b2-44cf-a49f-66ba2a037cf0"
            }
          ]
        },
        {
          "id": "ccd5c48c-f183-43ec-96e3-4f61a8058c3c",
          "name": "cloudflare-firewall-access-rule-for-a-zone-api",
          "request": {
            "url": "http://example.com/api/zones/:zone_id/firewall/access_rules/rules/:identifier?mode=%7B%7D&notes=%7B%7D",
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
            "description": "Update rule state and/or configuration for the zone"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "881692c6-30cb-4b84-8154-8a01c0986c45"
            }
          ]
        }
      ]
    },
    {
      "name": "Keyless Certificates",
      "item": [
        {
          "id": "e35c356b-bcfb-48de-b692-992753dce918",
          "name": "cloudflare-keyless-ssl-for-a-zone-api",
          "request": {
            "url": "http://example.com/api/zones/:zone_identifier/keyless_certificates",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List all Keyless SSL configurations for a given zone"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f631c4c7-ba45-4171-a5ea-73745dc75071"
            }
          ]
        },
        {
          "id": "96484d06-228e-4eeb-8404-3703a17fee99",
          "name": "cloudflare-keyless-ssl-for-a-zone-api",
          "request": {
            "url": "http://example.com/api/zones/:zone_identifier/keyless_certificates?certificate=%7B%7D&host=%7B%7D&name=%7B%7D&port=%7B%7D",
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
            "description": "The keyless SSL name"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f25bc6eb-b64f-4985-b493-d8a3c55a9a38"
            }
          ]
        },
        {
          "id": "6faf5453-9f67-40fc-8c1f-ee806308bb1f",
          "name": "cloudflare-keyless-ssl-for-a-zone-api1",
          "request": {
            "url": "http://example.com/api/zones/:zone_identifier/keyless_certificates/:identifier",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Details for one Keyless SSL configuration"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bb88f445-c3fd-4b5b-92fb-bd424eeb1ddb"
            }
          ]
        },
        {
          "id": "cbab4763-82a3-48b2-ac3c-2a75cc397f59",
          "name": "cloudflare-keyless-ssl-for-a-zone-api",
          "request": {
            "url": "http://example.com/api/zones/:zone_identifier/keyless_certificates/:identifier",
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete Keyless configuration permission needed: #ssl:editntt"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fcb07885-fd35-405a-925a-c36defb32790"
            }
          ]
        },
        {
          "id": "d09a72e3-6c2f-48fe-84dc-8de78d05c0f9",
          "name": "cloudflare-keyless-ssl-for-a-zone-api",
          "request": {
            "url": "http://example.com/api/zones/:zone_identifier/keyless_certificates/:identifier?host=%7B%7D&name=%7B%7D&port=%7B%7D",
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
            "description": "This will update attributes of a Keyless SSL"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5f9c8a49-abcc-4924-b740-609be4292ace"
            }
          ]
        }
      ]
    },
    {
      "name": "Organization Invites",
      "item": [
        {
          "id": "10171364-d455-45cc-b9c3-b61cc7706e9e",
          "name": "cloudflare-organization-invites-api",
          "request": {
            "url": "http://example.com/api/organizations/:organization_identifier/invite/:identifier?roles=%7B%7D",
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
            "description": "Change the Roles of a Pending Invite"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "df4774d5-6f8d-43f7-9399-3c54e29ddb9f"
            }
          ]
        },
        {
          "id": "a419f41e-6544-418d-bae0-913e24bafcbe",
          "name": "cloudflare-organization-invites-api",
          "request": {
            "url": "http://example.com/api/organizations/:organization_identifier/invites",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List all invitations associated with an organization"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bd6d1c35-be6e-4cc1-b1f0-f08ffb839370"
            }
          ]
        },
        {
          "id": "a1f8264c-af77-417f-9f38-0e2a34d4a106",
          "name": "cloudflare-organization-invites-api",
          "request": {
            "url": "http://example.com/api/organizations/:organization_identifier/invites?invited_member_email=%7B%7D&roles=%7B%7D",
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
            "description": "Invite a User to become a Member of an Organization"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1574cd96-ec13-4438-925d-ba67d16a6820"
            }
          ]
        },
        {
          "id": "6fe8c2bd-d012-4893-b154-7b046bd06dfd",
          "name": "cloudflare-organization-invites-api1",
          "request": {
            "url": "http://example.com/api/organizations/:organization_identifier/invites/:identifier",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get the details of an invitation"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ad94be90-c33e-4b5e-b2f4-b7c8b828f06c"
            }
          ]
        },
        {
          "id": "cba51e31-1b5e-4713-9797-06d77ad40de2",
          "name": "cloudflare-organization-invites-api",
          "request": {
            "url": "http://example.com/api/organizations/:organization_identifier/invites/:identifier",
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Cancel an existing invitation"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "165127ca-92e4-4788-855e-a4b60301048d"
            }
          ]
        }
      ]
    },
    {
      "name": "Organization Members",
      "item": [
        {
          "id": "b47a3556-bff7-4fe3-9413-986514a1d183",
          "name": "cloudflare-organization-members-api",
          "request": {
            "url": "http://example.com/api/organizations/:organization_identifier/members",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List all members of a organization"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "510f78ff-1f91-47bb-8475-d1d11e004921"
            }
          ]
        },
        {
          "id": "bd7d5741-1937-4ae9-b5e3-0be4cdbeacbe",
          "name": "cloudflare-organization-members-api1",
          "request": {
            "url": "http://example.com/api/organizations/:organization_identifier/members/:identifier",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get information about a specific member of an organization"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2b3383ed-8932-48ee-9147-63045cd11d7b"
            }
          ]
        },
        {
          "id": "b8ebcbc5-7c47-4700-a168-d3538aa449b5",
          "name": "cloudflare-organization-members-api",
          "request": {
            "url": "http://example.com/api/organizations/:organization_identifier/members/:identifier",
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Remove a member from an organization"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8123c14c-01cb-454d-9ccc-d72eaef26168"
            }
          ]
        },
        {
          "id": "7ab7bdc2-cafb-4c9a-a3b0-ad3486764d68",
          "name": "cloudflare-organization-members-api",
          "request": {
            "url": "http://example.com/api/organizations/:organization_identifier/members/:identifier?roles=%7B%7D",
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
            "description": "Change the Roles of an Organization&#39;s Member"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b3f7e32f-85d1-4ae0-b4a1-3da9acba12ff"
            }
          ]
        }
      ]
    },
    {
      "name": "Organization Roles",
      "item": [
        {
          "id": "b422fd62-3fba-47de-abf9-5d82b4d7d364",
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
              "id": "ad60166a-ff4e-41b6-b99b-c0308ee78ec5"
            }
          ]
        },
        {
          "id": "f080e24a-278a-4aa5-b2b0-61e44195f52c",
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
              "id": "791def07-e765-4851-845f-73af6e5b5c7f"
            }
          ]
        }
      ]
    },
    {
      "name": "Organization Firewall Access Rules",
      "item": [
        {
          "id": "05ab27ce-1cf8-4449-afd5-50edce29f192",
          "name": "cloudflare-organizationlevel-firewall-access-rule-api",
          "request": {
            "url": "http://example.com/api/organizations/:organization_id/firewall/access_rules/rules?configuration_target=%7B%7D&configuration_value=%7B%7D&direction=%7B%7D&match=%7B%7D&mode=%7B%7D&order=%7B%7D&page=%7B%7D&per_page=%7B%7D",
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
            "description": "Search, sort, and filter IP/country access rules"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "45d49eca-0b32-4a20-b20d-282eaf88a064"
            }
          ]
        },
        {
          "id": "7e180dbb-cd40-429a-b508-688f94abb785",
          "name": "cloudflare-organizationlevel-firewall-access-rule-api",
          "request": {
            "url": "http://example.com/api/organizations/:organization_id/firewall/access_rules/rules?configuration=%7B%7D&mode=%7B%7D&value=%7B%7D",
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
            "description": "Make a new IP, IP range, or country access rule for all zones owned by the organization"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "621d9ea9-5978-404f-90d1-76db5ed6026d"
            }
          ]
        },
        {
          "id": "09592a37-1864-45fd-a417-f2121f3489f4",
          "name": "cloudflare-organizationlevel-firewall-access-rule-api",
          "request": {
            "url": "http://example.com/api/organizations/:organization_id/firewall/access_rules/rules/:identifier",
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Remove an access rule so it is no longer evaluated during requests"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d42fdb2a-ce2b-43a0-ad35-ab2d33341c36"
            }
          ]
        },
        {
          "id": "36881e14-8a1b-4986-bd40-e4562c0d3e21",
          "name": "cloudflare-organizationlevel-firewall-access-rule-api",
          "request": {
            "url": "http://example.com/api/organizations/:organization_id/firewall/access_rules/rules/:identifier?configuration=%7B%7D&mode=%7B%7D&value=%7B%7D",
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
            "description": "Update rule state and/or configuration"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b5f23255-07f6-4624-af11-12c675c12148"
            }
          ]
        }
      ]
    },
    {
      "name": "Organizations",
      "item": [
        {
          "id": "0917fa5a-2b20-45e2-9c45-c48718c6ee4a",
          "name": "cloudflare-organizations-api",
          "request": {
            "url": "http://example.com/api/organizations/:identifier",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get information about a specific organization that you are a member of"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a7f25f22-66a5-4e75-a842-00bfdfe9c959"
            }
          ]
        },
        {
          "id": "8862fe00-baee-43ef-9eef-48cc923e9f80",
          "name": "cloudflare-organizations-api",
          "request": {
            "url": "http://example.com/api/organizations/:identifier?name=%7B%7D",
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
            "description": "Update an existing Organization"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "12df5217-0edb-4267-a00c-48ffcd7577d6"
            }
          ]
        }
      ]
    },
    {
      "name": "Performance",
      "item": [
        {
          "id": "db81cac5-5c3a-4515-8178-7878c7fffe09",
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
              "id": "72ecf0f9-7caf-4976-b09a-2f0bd39ff0bf"
            }
          ]
        },
        {
          "id": "f1c38b04-3e08-43b7-b4e5-e453eba7db0d",
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
              "id": "837efbd5-9f49-414e-b76d-0e9f2b22c0bf"
            }
          ]
        },
        {
          "id": "39318b95-2174-47eb-b4cf-626e1e9b7b65",
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
              "id": "998b7fad-84ff-4893-ab63-d39527df89f2"
            }
          ]
        },
        {
          "id": "47387ce2-f785-4550-8d62-3f2868d49ebf",
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
              "id": "b7e10767-ccc6-41e5-a967-c62d3b4de1d0"
            }
          ]
        },
        {
          "id": "ff4692c2-9d07-4253-a6f4-7b59d0a64983",
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
              "id": "e25f9743-5d5e-474d-9407-0d31470223c4"
            }
          ]
        },
        {
          "id": "1dfd2c1d-d7c0-4234-969f-461cab897c41",
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
              "id": "c57f76cc-642b-4dfd-8f1c-e354d904ddbd"
            }
          ]
        },
        {
          "id": "2916d05e-834a-4cd5-ad5a-77920a24fa83",
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
              "id": "f52e351b-074a-4f2c-a1d6-3ec5ab388469"
            }
          ]
        },
        {
          "id": "0c5f2275-8424-44e0-8fb5-c1672a602781",
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
              "id": "d1171054-7b79-4379-95eb-3ed066b07b70"
            }
          ]
        },
        {
          "id": "c5054d9a-526d-46fc-9ad3-d2fae62fbe1c",
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
              "id": "e9a7b8d7-c3dc-4fc6-9020-192b14298649"
            }
          ]
        },
        {
          "id": "4192e57a-3e26-43e6-9bef-133ec98b2a43",
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
              "id": "42d27c3d-e491-45f5-99a1-29334eec8c09"
            }
          ]
        }
      ]
    },
    {
      "name": "Users",
      "item": [
        {
          "id": "f7347c65-d476-4cea-94ee-c35bc30c3b01",
          "name": "cloudflare-user-api",
          "request": {
            "url": "http://example.com/api/user",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "User detailsn"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "859da191-4a17-41b5-87d4-3f041cc9def4"
            }
          ]
        },
        {
          "id": "3635cd91-6fbf-4cd7-ac6d-55d1a7359acb",
          "name": "cloudflare-user-api",
          "request": {
            "url": "http://example.com/api/user?country=%7B%7D&first_name=%7B%7D&last_name=%7B%7D&telephone=%7B%7D&zipcode=%7B%7D",
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
            "description": "Update part of your user details"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e6bbdff2-a521-4212-a912-3dcee142a265"
            }
          ]
        }
      ]
    },
    {
      "name": "Billing History",
      "item": [
        {
          "id": "7ec7efe5-d3ec-4f0b-bddc-8897bec59e60",
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
              "id": "16415b9c-4060-44de-b7d0-e8d1952ebb54"
            }
          ]
        }
      ]
    },
    {
      "name": "Billing Profile",
      "item": [
        {
          "id": "d50a8422-3ee6-4ecb-b03d-0f5cb8c10e03",
          "name": "cloudflare-user-billing-profile-api",
          "request": {
            "url": "http://example.com/api/user/billing/profile",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Access your billing profile object"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ee42a959-b75e-43d5-af40-c349bb3422e4"
            }
          ]
        }
      ]
    },
    {
      "name": "User Level Firewall Access Rule",
      "item": [
        {
          "id": "50a34866-5fbe-4a7a-a076-0dc248f18045",
          "name": "cloudflare-userlevel-firewall-access-rule-api",
          "request": {
            "url": "http://example.com/api/user/firewall/access_rules/rules?configuration_target=%7B%7D&configuration_value=%7B%7D&direction=%7B%7D&match=%7B%7D&mode=%7B%7D&order=%7B%7D&page=%7B%7D&per_page=%7B%7D",
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
            "description": "Search, sort, and filter IP/country access rules"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8c680e17-72c3-41b9-8b38-e0e8dde21356"
            }
          ]
        },
        {
          "id": "4826fc57-0558-4ecb-91c5-9a3cc2bebd0f",
          "name": "cloudflare-userlevel-firewall-access-rule-api",
          "request": {
            "url": "http://example.com/api/user/firewall/access_rules/rules?configuration=%7B%7D&mode=%7B%7D&value=%7B%7D",
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
            "description": "Make a new IP, IP range, or country access rule for all zones owned by the user"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9afceca9-9997-42b7-8f0b-ee97c7be8004"
            }
          ]
        },
        {
          "id": "cb5f1371-aeab-49d1-934b-0b674adafd57",
          "name": "cloudflare-userlevel-firewall-access-rule-api",
          "request": {
            "url": "http://example.com/api/user/firewall/access_rules/rules/:identifier",
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Remove an access rule so it is no longer evaluated during requests"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7f42c7a6-655a-4576-be72-76d1db16e2c4"
            }
          ]
        },
        {
          "id": "5191a5f5-2eeb-46fa-9848-92143d6b0426",
          "name": "cloudflare-userlevel-firewall-access-rule-api",
          "request": {
            "url": "http://example.com/api/user/firewall/access_rules/rules/:identifier?configuration=%7B%7D&mode=%7B%7D&value=%7B%7D",
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
            "description": "Update rule state and/or configuration"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f61eb3a0-24c7-43f7-94c5-4d532b5da014"
            }
          ]
        }
      ]
    },
    {
      "name": "User Invites",
      "item": [
        {
          "id": "bde4a2f0-9cb2-4da8-9c95-4056292141bd",
          "name": "cloudflare-userx27s-invites-api",
          "request": {
            "url": "http://example.com/api/user/invites",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List all invitations associated with my user"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6f16dc00-6300-4ae0-a3d8-063a5294c02e"
            }
          ]
        },
        {
          "id": "1ad4121a-663c-4b13-918e-6071d7d266fe",
          "name": "cloudflare-userx27s-invites-api1",
          "request": {
            "url": "http://example.com/api/user/invites/:identifier",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get the details of an invitation"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4bd363c2-7f4b-4754-9bf3-38829b1136d4"
            }
          ]
        },
        {
          "id": "54195434-0aef-4446-beae-4647067edc8c",
          "name": "cloudflare-userx27s-invites-api",
          "request": {
            "url": "http://example.com/api/user/invites/:identifier?status=%7B%7D",
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
            "description": "Respond to an invitation"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b5001712-fd59-4886-a55f-877182963c63"
            }
          ]
        }
      ]
    },
    {
      "name": "User Organizations",
      "item": [
        {
          "id": "d4c8c69c-b15d-4542-aa38-bb347ada731a",
          "name": "cloudflare-userx27s-organizations-api",
          "request": {
            "url": "http://example.com/api/user/organizations?direction=%7B%7D&match=%7B%7D&name=%7B%7D&order=%7B%7D&page=%7B%7D&per_page=%7B%7D&status=%7B%7D",
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
            "description": "List organizations the user is associated with"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ffe226e6-3336-4aac-beac-755856e6e75f"
            }
          ]
        },
        {
          "id": "80d4369f-9646-497b-89e9-22d4cbf15063",
          "name": "cloudflare-userx27s-organizations-api",
          "request": {
            "url": "http://example.com/api/user/organizations/:identifier",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a specific organization the user is associated with"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b219fe6f-2baf-4daf-80b6-f203f5e41308"
            }
          ]
        },
        {
          "id": "555069cb-79ea-4cf7-92cb-cbe91b4cfdcf",
          "name": "cloudflare-userx27s-organizations-api",
          "request": {
            "url": "http://example.com/api/user/organizations/:identifier",
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Remove association to an organization"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "54040ce3-7c1d-4608-a609-c54cb290d78b"
            }
          ]
        }
      ]
    },
    {
      "name": "WAF Rule Groups",
      "item": [
        {
          "id": "34779b11-29cc-44dc-9689-7e573c189a8d",
          "name": "cloudflare-waf-rule-groups-api",
          "request": {
            "url": "http://example.com/api/zones/:zone_identifier/firewall/waf/packages/:package_identifier/groups?direction=%7B%7D&match=%7B%7D&mode=%7B%7D&name=%7B%7D&order=%7B%7D&page=%7B%7D&per_page=%7B%7D&rules_count=%7B%7D",
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
            "description": "Search, list, and sort rule groups contained within a package"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "241f425f-f045-4a12-9b2a-01b3e2f87516"
            }
          ]
        },
        {
          "id": "63388607-847e-4bc8-aef5-9f784772a66c",
          "name": "cloudflare-waf-rule-groups-api",
          "request": {
            "url": "http://example.com/api/zones/:zone_identifier/firewall/waf/packages/:package_identifier/groups/:identifier",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a single rule group"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1093c210-8a31-4058-9bed-cdc464299b9b"
            }
          ]
        }
      ]
    }
  ]
}