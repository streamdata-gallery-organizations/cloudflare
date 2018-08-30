{
  "info": {
    "name": "CloudFlare Individual information about a rule",
    "_postman_id": "a8aeb721-e0ed-44b5-b558-89b955714d22",
    "description": "Individual information about a rule",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Subscriptions",
      "item": [
        {
          "id": "f3736c91-2ca9-4ab4-8f93-2d9f93937bdb",
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
              "id": "7d5d1a02-9e3a-43c0-a26b-cf937a64c5bb"
            }
          ]
        },
        {
          "id": "a2275de7-7bde-4abd-b9da-a0a68bef0c22",
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
              "id": "df4003a9-c8f6-441d-bdda-eb2ac5435221"
            }
          ]
        }
      ]
    },
    {
      "name": "Zones",
      "item": [
        {
          "id": "ae1e4b0b-2acb-4e79-8fec-00d3554f505f",
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
              "id": "28e416fb-a4a1-486f-bb41-f745c507d7a5"
            }
          ]
        },
        {
          "id": "e6025c52-f777-4a3d-9684-e872262c8b31",
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
              "id": "371dbf7a-405a-44e9-b75b-6786419e0e4a"
            }
          ]
        },
        {
          "id": "a1d713be-b798-470d-b603-f76cd9a4fad5",
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
              "id": "7910cade-300b-4bec-aeea-dfc0967bf1be"
            }
          ]
        }
      ]
    },
    {
      "name": "Certificates",
      "item": [
        {
          "id": "82367ecc-10af-4bc7-baf2-2ff5e5123f8c",
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
              "id": "2f1d9b00-b2bd-4c75-98e2-eeec35007ffa"
            }
          ]
        },
        {
          "id": "5b426319-f71e-4d11-9578-4ad77d7db8e3",
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
              "id": "a35f274d-1a2a-4670-8d69-568d096dff59"
            }
          ]
        },
        {
          "id": "e270446b-ba16-4daf-b804-aca0054e523c",
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
              "id": "a3d517c0-7dcc-4710-a99e-36605a63703c"
            }
          ]
        },
        {
          "id": "0d148c7d-6a46-46b5-b180-a3a23a4bebd2",
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
              "id": "67d4db1e-ae98-4d3a-ac58-acf2039ea574"
            }
          ]
        },
        {
          "id": "273c1779-4de2-4315-98df-cda1ec626664",
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
              "id": "461c2616-8418-4b12-ac6f-04fc9d8decd6"
            }
          ]
        },
        {
          "id": "6426c735-18e5-4f86-934f-4102ae09e0fa",
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
              "id": "2007d735-3dbb-4a64-80ac-52448db0bd28"
            }
          ]
        }
      ]
    },
    {
      "name": "Records",
      "item": [
        {
          "id": "097e0a62-6502-48ae-87ca-e9d1bdf58fba",
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
              "id": "d3ceb945-557c-4109-9119-aad02e9971ba"
            }
          ]
        },
        {
          "id": "2a736bfa-2ff0-4a4a-a323-e8bfa2be4c96",
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
              "id": "73179c67-00b4-45fa-8705-c5fd9f08b7c0"
            }
          ]
        },
        {
          "id": "7ebabb9b-f7cd-4541-a721-3e16235cb482",
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
              "id": "d39a6a6f-4b87-427f-a27e-1f3bfac851a2"
            }
          ]
        },
        {
          "id": "011e3fdf-1933-43aa-9d4f-279d264f5f11",
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
              "id": "603220ad-9b8c-4ae5-b35f-7d252ddca3c6"
            }
          ]
        },
        {
          "id": "10473a9c-94ad-472c-b114-1ff827c9fe8e",
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
              "id": "743e3f31-02e0-4754-87d1-a4bbef29df9e"
            }
          ]
        }
      ]
    },
    {
      "name": "Firewall Access Rule",
      "item": [
        {
          "id": "4214991f-4e6c-4851-99ab-3b69fa2efb8d",
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
              "id": "d34d7211-edbb-41cf-991c-b0e3d1a9f2f1"
            }
          ]
        },
        {
          "id": "dfb21acb-73c6-43a0-b1f1-6aa9758c4042",
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
              "id": "81609cc8-f3c9-44dd-b14a-6cf66f207581"
            }
          ]
        },
        {
          "id": "9fea9a7d-7271-45f0-9022-911a6abd7713",
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
              "id": "8e302fe7-a341-4596-a712-66c61ad087c8"
            }
          ]
        },
        {
          "id": "913fd2ca-a315-432c-8af5-734452829591",
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
              "id": "2cfacd05-88c9-4d59-9d51-181d5daf7657"
            }
          ]
        }
      ]
    },
    {
      "name": "Keyless Certificates",
      "item": [
        {
          "id": "6541c48d-0da3-4164-afbb-8e53ac09e8ae",
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
              "id": "6ebfcb91-6dc7-4bae-a8e5-dd81544ab8e8"
            }
          ]
        },
        {
          "id": "f43dd06b-9682-402d-8ea1-45e74e6754e7",
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
              "id": "9c938ebb-68de-46fe-9222-2dd784a908a6"
            }
          ]
        },
        {
          "id": "d7fb0ef6-389c-4b73-91bd-e52849f2adce",
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
              "id": "39f6966f-bb2c-435b-9397-a7f380eb33f9"
            }
          ]
        },
        {
          "id": "e89742f7-5324-4473-bfae-4fd8914cb4a0",
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
              "id": "4b62566e-1fd1-45aa-b264-eae68e69bd40"
            }
          ]
        },
        {
          "id": "12096b9d-f729-4e29-8fc8-fadd76c4afa3",
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
              "id": "8de36a06-c768-47c6-b1cb-914551ce75b1"
            }
          ]
        }
      ]
    },
    {
      "name": "Organization Invites",
      "item": [
        {
          "id": "62c03259-0165-4c77-9dca-deac62d5e36d",
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
              "id": "cec46004-1070-4673-8d26-5918f7fab845"
            }
          ]
        },
        {
          "id": "b2ad199f-e89c-44f7-9888-f5ad88939ba4",
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
              "id": "2f93f29b-1f03-407c-bd4e-4ccad8a29bd4"
            }
          ]
        },
        {
          "id": "e70aa7d5-f12b-4ed4-b91a-6ca47e3cf966",
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
              "id": "e30ad7f3-35bb-4945-9fda-9eea300e168a"
            }
          ]
        },
        {
          "id": "d2f93f1f-9091-4eef-b87f-0580487e2b34",
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
              "id": "bd97fd5e-53f0-426d-a646-ef6181573598"
            }
          ]
        },
        {
          "id": "a46466af-d1a2-46d1-a816-71853588e720",
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
              "id": "3cd2ca96-6c3a-43e5-9d04-d75bceab204e"
            }
          ]
        }
      ]
    },
    {
      "name": "Organization Members",
      "item": [
        {
          "id": "64687318-ac9a-4622-a583-5278738af0df",
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
              "id": "200542c1-eae3-40af-b6b2-0b2e8a8339e3"
            }
          ]
        },
        {
          "id": "dbff5602-aebe-420b-b184-96eead0f6e7f",
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
              "id": "88c0d62f-67f9-4370-a8d7-c62fcf973507"
            }
          ]
        },
        {
          "id": "fb733029-88c7-439b-8d5f-6678553d9f15",
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
              "id": "b79d73cd-8502-4c33-a30c-9fadf3841a37"
            }
          ]
        },
        {
          "id": "35ee52a4-40ea-459d-a4e7-ad7ce4aada45",
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
              "id": "3754b277-b67e-4671-9efe-18dc490f641b"
            }
          ]
        }
      ]
    },
    {
      "name": "Organization Roles",
      "item": [
        {
          "id": "7d5b10eb-68d8-48a3-a2c7-697cd99fc0ec",
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
              "id": "649609d1-ff4e-43d8-a90f-4c49bfceb3d9"
            }
          ]
        },
        {
          "id": "ad1d39ae-3fa3-4711-8a4d-fa79a720e86f",
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
              "id": "864766f8-2c1e-4607-9978-7566232ebe72"
            }
          ]
        }
      ]
    },
    {
      "name": "Organization Firewall Access Rules",
      "item": [
        {
          "id": "71f1f39d-c092-4984-961a-053ccd9c822c",
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
              "id": "12bb68c6-23e1-4484-8238-823949c028ac"
            }
          ]
        },
        {
          "id": "4e29a230-5caa-4e5c-a2b4-cc7eb0aee898",
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
              "id": "417a3f34-44b4-4c30-9429-bc8f28ce5f48"
            }
          ]
        },
        {
          "id": "670037e2-a98b-441f-8b45-951c7d8c5449",
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
              "id": "23270c80-7c6a-4c5f-89cf-9142645f53f5"
            }
          ]
        },
        {
          "id": "5ee00df6-e762-4d80-8593-9beba81c154c",
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
              "id": "3a36fa9a-116c-4c34-b502-18f6c38c4a8b"
            }
          ]
        }
      ]
    },
    {
      "name": "Organizations",
      "item": [
        {
          "id": "f405aaa4-ea56-4f6b-9535-ea88e29f99fb",
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
              "id": "9459c1ec-e2a5-44b7-a86d-fcb9b6a94b79"
            }
          ]
        },
        {
          "id": "38b73270-47c4-4c5d-8c4d-f45e5bdc5e47",
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
              "id": "a1c7e16c-d9b6-4b38-aeeb-78e777d419d4"
            }
          ]
        }
      ]
    },
    {
      "name": "Performance",
      "item": [
        {
          "id": "193d3ace-3d77-49dc-89c6-0be7a68d3faa",
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
              "id": "d5a9b2f9-6860-44ad-8bfd-17bb592aa5ad"
            }
          ]
        },
        {
          "id": "5415a612-4c7c-4097-a3d7-176666acddd1",
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
              "id": "88912754-48f2-42fa-a121-9782e003c8de"
            }
          ]
        },
        {
          "id": "ba351dc7-50df-4105-b97c-0c09a32b583c",
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
              "id": "c9020f2e-0c10-4077-849e-1edfc129a99c"
            }
          ]
        },
        {
          "id": "1e455930-7d8f-489c-90d0-e743bc0f10c1",
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
              "id": "9c73ef2c-a824-4c6c-95a1-46544200fbd9"
            }
          ]
        },
        {
          "id": "f3f1399c-f2d8-432c-8542-85623ebacd81",
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
              "id": "a75d41ff-436c-4030-ac50-7e942b6664cd"
            }
          ]
        },
        {
          "id": "3ae47dbc-8f0f-4df8-8bd4-f7a6b56055f2",
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
              "id": "1fab9d40-3aaf-42db-8f8f-5c74e0dd40f5"
            }
          ]
        },
        {
          "id": "6bbec2cf-4c46-4a84-bfc0-1cf8ac6a6aad",
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
              "id": "84ea6c14-631a-47cb-b487-fc8079032540"
            }
          ]
        },
        {
          "id": "42a08d31-8069-40b7-b8c5-c577a78d1387",
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
              "id": "44b84a52-b256-479a-afcf-d2ff2f1db9f6"
            }
          ]
        },
        {
          "id": "e9d780ad-faed-4f49-9e9d-050d7925dcc6",
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
              "id": "8cae2b7a-fa7d-48d6-8b31-4f0dfaa70aac"
            }
          ]
        },
        {
          "id": "3c7f1d28-4f52-41c6-a8a2-9bcb373a50a6",
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
              "id": "81ac529d-0bef-4f4e-95f7-98553e3e6cc4"
            }
          ]
        }
      ]
    },
    {
      "name": "Users",
      "item": [
        {
          "id": "ee975358-3378-49ce-95d4-cb9f4fe5e99a",
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
              "id": "d93d5f9b-550a-413b-8743-9048b6b7847c"
            }
          ]
        },
        {
          "id": "ac6ea663-3346-4971-9457-66b418f884f6",
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
              "id": "79058a05-862c-44bb-b09a-cca4a15e373c"
            }
          ]
        }
      ]
    },
    {
      "name": "Billing History",
      "item": [
        {
          "id": "ea863aa1-c232-4071-868a-420df304c123",
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
              "id": "4bd1a942-fc61-4016-ae84-f17108f534b6"
            }
          ]
        }
      ]
    },
    {
      "name": "Billing Profile",
      "item": [
        {
          "id": "f2cf25e1-ffd1-44ba-9ab1-161868da626b",
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
              "id": "8dbde336-eb2a-48f5-af08-e921d673e6d3"
            }
          ]
        }
      ]
    },
    {
      "name": "User Level Firewall Access Rule",
      "item": [
        {
          "id": "1c753b77-f930-43b3-a68e-1909dd01c347",
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
              "id": "fde5e346-70ed-41c3-916f-2c0916d1de23"
            }
          ]
        },
        {
          "id": "3092d421-0068-4691-b974-ec2993324ddc",
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
              "id": "a5399afa-5f60-4d25-af44-8bd1318b3930"
            }
          ]
        },
        {
          "id": "0daede8d-7cd4-4fd4-b4c0-95d8686a7b41",
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
              "id": "a20e442f-9233-420b-a2cd-fefed0c6e86a"
            }
          ]
        },
        {
          "id": "3bfc4ff0-5936-4b53-9b5a-35900a407c9e",
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
              "id": "dbfd0286-c6c1-4680-a18f-19fc063b535d"
            }
          ]
        }
      ]
    },
    {
      "name": "User Invites",
      "item": [
        {
          "id": "2db5a652-c699-43b9-a20d-7970a8d513f0",
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
              "id": "922a7f59-8dc2-41ff-84e3-4e8c6fba9f34"
            }
          ]
        },
        {
          "id": "308c5d4a-63fb-4a9e-8424-f2b4e014e1f8",
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
              "id": "6073ca4f-7564-4395-ad59-5bf16e9c074e"
            }
          ]
        },
        {
          "id": "bad6389c-3b8f-4dab-97a7-1b3f72bb748d",
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
              "id": "435ed0f9-9f69-487e-9911-da4063192a67"
            }
          ]
        }
      ]
    },
    {
      "name": "User Organizations",
      "item": [
        {
          "id": "6ade0f57-61e7-4d99-ac3f-9f32d8af6c8d",
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
              "id": "4ed9f12e-e343-4db5-901e-f3dab281b0bd"
            }
          ]
        },
        {
          "id": "b43e8d33-0da8-44a6-88a1-386ae3c58906",
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
              "id": "611f6e27-1768-456e-ac0b-9a76617c73a7"
            }
          ]
        },
        {
          "id": "ca82a903-9c62-40c4-a13a-cfcd6abc233d",
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
              "id": "9077ce15-8578-4290-89de-64132ad1e79b"
            }
          ]
        }
      ]
    },
    {
      "name": "WAF Rule Groups",
      "item": [
        {
          "id": "849d774f-86eb-4c42-9d94-8e8a2418c1f4",
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
              "id": "48ac23d6-9331-4ebb-83eb-67e877cdac67"
            }
          ]
        },
        {
          "id": "fa86ca5f-5fbe-4ca3-812a-f3a7efe87945",
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
              "id": "8f36d148-72da-4eb0-a52b-9e046db13c60"
            }
          ]
        },
        {
          "id": "6c7cfa7e-81b5-4807-a4b4-e60a46e1f1f0",
          "name": "cloudflare-waf-rule-groups-api",
          "request": {
            "url": "http://example.com/api/zones/:zone_identifier/firewall/waf/packages/:package_identifier/groups/:identifier?mode=%7B%7D",
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
   