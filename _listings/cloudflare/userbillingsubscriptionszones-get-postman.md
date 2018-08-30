{
  "info": {
    "name": "CloudFlare List all of your zone plan subscriptions",
    "_postman_id": "6fa6245e-42fb-4d01-b351-1809774b8722",
    "description": "List all of your zone plan subscriptions",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Subscriptions",
      "item": [
        {
          "id": "d38017c7-e0f0-4294-8391-86fc4454dbcc",
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
              "id": "68b98b8c-b8e0-4285-809c-1f129d49540c"
            }
          ]
        },
        {
          "id": "80da7adc-2182-46e5-a012-8cb01753d14a",
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
              "id": "8284c9d3-1afe-402c-8581-57739e055c83"
            }
          ]
        }
      ]
    },
    {
      "name": "Zones",
      "item": [
        {
          "id": "4ee9ecea-1c61-4c2f-b714-a2db0a254567",
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
              "id": "be4ee38c-466d-4b58-8485-59255c3c830c"
            }
          ]
        },
        {
          "id": "8698f774-6b03-4974-a9fe-e1b8b9160ee3",
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
              "id": "c3e74bae-36ec-4420-8dba-61995aafdd73"
            }
          ]
        },
        {
          "id": "25ed9117-4bcd-4ffc-b1ea-2f3468126466",
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
              "id": "6a78a9fe-b154-4c76-ba38-5af924c8a77d"
            }
          ]
        },
        {
          "id": "59f1dddd-edaf-4ad6-afd6-b046c86b3c7a",
          "name": "cloudflare-zone-analytics-api",
          "request": {
            "url": "http://example.com/api/zones/:zone_identifier/analytics/colos?continuous=%7B%7D&since=%7B%7D&until=%7B%7D",
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
            "description": "This view provides a breakdown of analytics data by datacenter"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "eb5f3516-99d4-4fed-99da-e3a45ac99873"
            }
          ]
        },
        {
          "id": "e5fc0e94-ef3d-4edd-a1dd-7b79e55e639f",
          "name": "cloudflare-zone-analytics-api1",
          "request": {
            "url": "http://example.com/api/zones/:zone_identifier/analytics/dashboard?continuous=%7B%7D&since=%7B%7D&until=%7B%7D",
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
            "description": "The dashboard view provides both totals and timeseries data for the given zone and time period across the entire CloudFlare network"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9aabd082-bb29-4496-a142-d2267f52a202"
            }
          ]
        },
        {
          "id": "714a6503-10eb-4758-be16-0a8124d7b63b",
          "name": "cloudflare-zone-api",
          "request": {
            "url": "http://example.com/api/zones?direction=%7B%7D&match=%7B%7D&name=%7B%7D&order=%7B%7D&page=%7B%7D&per_page=%7B%7D&status=%7B%7D",
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
            "description": "List, search, sort, and filter your zones"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6a8061ed-0740-4717-8e71-8aa8475c7eb3"
            }
          ]
        },
        {
          "id": "dbd0479e-6cfd-4dea-bfc0-7e87ae21740e",
          "name": "cloudflare-zone-api",
          "request": {
            "url": "http://example.com/api/zones?name=%7B%7D",
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
            "description": "The domain name"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ab2b53b6-2215-41cf-b86a-6b4e696eac39"
            }
          ]
        },
        {
          "id": "0dda623a-2547-451a-82b4-e7e3fd7baf3d",
          "name": "cloudflare-zone-api",
          "request": {
            "url": "http://example.com/api/zones/:identifier",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Zone details permission needed: #zone:readntt"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "342d522a-b634-48a2-84c7-a44411ed9c68"
            }
          ]
        },
        {
          "id": "010782f2-0140-4d54-8272-a18baf45b434",
          "name": "cloudflare-zone-api",
          "request": {
            "url": "http://example.com/api/zones/:identifier",
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete an existing zone"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dd0bda64-1204-4a1e-a4f2-781b2bea69c8"
            }
          ]
        },
        {
          "id": "22adecf7-4add-4cfe-9ef0-6dbe2f15be34",
          "name": "cloudflare-zone-api",
          "request": {
            "url": "http://example.com/api/zones/:identifier?paused=%7B%7D&plan=%7B%7D&vanity_name_servers=%7B%7D",
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
            "description": "Only one zone property can be changed at a time"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "09d485d3-9d1d-40b0-b112-a63b46704c0a"
            }
          ]
        },
        {
          "id": "ebe13b09-b19f-4b04-bf78-99860594ba1c",
          "name": "cloudflare-zone-api",
          "request": {
            "url": "http://example.com/api/zones/:identifier/activation_check",
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Initiate another zone activation check permission needed: #zone:editntt"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a4a866d2-3e91-41bb-817e-a4c58d973ebd"
            }
          ]
        },
        {
          "id": "6d48db0f-71a8-4fde-ae4b-2583f66547cf",
          "name": "cloudflare-zone-api",
          "request": {
            "url": "http://example.com/api/zones/:identifier/purge_cache?files=%7B%7D&purge_everything=%7B%7D&tags=%7B%7D",
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
            "description": "Remove ALL files from CloudFlare&#39;s cache"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8459f8f4-ba1f-442a-81c6-212abfcd5d71"
            }
          ]
        }
      ]
    },
    {
      "name": "Certificates",
      "item": [
        {
          "id": "bc29187e-7322-4281-9472-82e61cfa1a09",
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
              "id": "14373ac2-be4c-4b88-90d1-f4ec771c5a7d"
            }
          ]
        },
        {
          "id": "cdc21c07-c86b-41f7-ab20-667291fd0f10",
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
              "id": "7531f858-eb5c-484d-a8ef-a106fcf7f30d"
            }
          ]
        },
        {
          "id": "2d6083bf-5f6b-4389-886a-83a005b9bcba",
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
              "id": "4fbef9ae-ee05-4764-8dea-57091104c107"
            }
          ]
        },
        {
          "id": "bd0297ca-b3bb-4e6c-aad1-391c127131a8",
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
              "id": "7bbcc6cb-c217-43e3-9f07-ba102af4736b"
            }
          ]
        },
        {
          "id": "75b546aa-1eeb-4c80-a2c0-99553bdc0adb",
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
              "id": "eab82ef2-d21e-4c1c-a317-31b38fea65c2"
            }
          ]
        },
        {
          "id": "1d0b3572-45dc-4938-84d6-0d8ddcb7ffa1",
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
              "id": "5a213a2b-8915-4523-8c24-dbdc2a3c4429"
            }
          ]
        }
      ]
    },
    {
      "name": "Records",
      "item": [
        {
          "id": "8a63c289-28c9-46b6-830d-9fe6450bed27",
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
              "id": "c50eb5cb-e3c0-4ca0-b1b1-994af6b5233f"
            }
          ]
        },
        {
          "id": "67ab66ee-1814-41f5-80c7-2d04310c7e3f",
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
              "id": "1c7d38f9-ea78-4c3f-a174-756aa63892d7"
            }
          ]
        },
        {
          "id": "bf913099-c886-45d8-91f4-083b974990af",
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
              "id": "3a1989a4-95ff-4cd3-969f-63fada650b55"
            }
          ]
        },
        {
          "id": "5b68ace1-7d88-4100-9ef8-3d8d23d5b011",
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
              "id": "91f57df5-aa66-4ced-9d55-c6df7e99ac3a"
            }
          ]
        },
        {
          "id": "d0067304-369d-487c-8084-30a2be3219f8",
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
              "id": "61be3311-0f20-473e-8816-c5efd729fbdb"
            }
          ]
        }
      ]
    },
    {
      "name": "Firewall Access Rule",
      "item": [
        {
          "id": "38f89337-d25d-413a-b979-454b250c1983",
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
              "id": "327ba653-2015-4f49-9626-9e88127b24e1"
            }
          ]
        },
        {
          "id": "7a7248c1-c4a4-4fef-83b3-4e7373ca6485",
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
              "id": "4626500b-656c-4eb7-b679-ed448300596a"
            }
          ]
        },
        {
          "id": "e12a4951-0e0a-441b-99d8-b634d5c35a6d",
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
              "id": "9877690f-e92a-457e-868b-3aa79a423b0f"
            }
          ]
        },
        {
          "id": "3600cf54-c200-4ddd-ab6c-8e05e02b47b4",
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
              "id": "64b790f7-ba29-4584-af4b-6b200d97de3f"
            }
          ]
        }
      ]
    },
    {
      "name": "Keyless Certificates",
      "item": [
        {
          "id": "a3e94523-bc78-46fd-91bc-59be237ba76e",
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
              "id": "61b0db4f-91ca-4baf-aeba-55bbc4e45040"
            }
          ]
        },
        {
          "id": "207cd57f-e0d6-450b-ba92-f39d596247a0",
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
              "id": "479d46d0-fdf8-4be6-b3af-a0947b60725a"
            }
          ]
        },
        {
          "id": "ceba338a-17c5-430f-b251-c54cb25d261b",
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
              "id": "9417c98d-a0ef-49eb-8370-de1e8ab0bcfb"
            }
          ]
        },
        {
          "id": "f17ae00d-bfaa-450f-a7fa-192e18faa2e7",
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
              "id": "e6a81a97-e3d0-4b43-a9b6-6043c5bc6067"
            }
          ]
        },
        {
          "id": "b59b3b3d-9f70-41b0-8cbe-79835bed2f04",
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
              "id": "9058e4b0-b546-47a8-a280-59ca14758191"
            }
          ]
        }
      ]
    },
    {
      "name": "Organization Invites",
      "item": [
        {
          "id": "2a928582-4264-4fdd-bacf-09befcc17fae",
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
              "id": "85da6275-2cde-4ae8-9898-825981597654"
            }
          ]
        },
        {
          "id": "d8e0fa2c-42c6-4dec-b20f-9c277f5a7229",
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
              "id": "e90946d5-ef24-4a55-8d13-0ddfefa2d293"
            }
          ]
        },
        {
          "id": "d2f61533-73d3-49ca-bafb-5baa13650bc1",
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
              "id": "20ee6d78-a04e-4dac-be16-0b19f97e719e"
            }
          ]
        },
        {
          "id": "f0695acd-ffaa-419b-9f2f-9d727550ae57",
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
              "id": "5182f337-4d97-4b2b-8272-7035f1754ca9"
            }
          ]
        },
        {
          "id": "816a4670-a7c1-4c98-ba4a-4ce7ed596049",
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
              "id": "9f0d22df-38a3-4da1-b586-5d6188c2e8e4"
            }
          ]
        }
      ]
    },
    {
      "name": "Organization Members",
      "item": [
        {
          "id": "ec5c7bab-76a3-44cc-b3de-bfb7c58bf815",
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
              "id": "96e1f923-82a1-48a6-9366-c367535e64be"
            }
          ]
        },
        {
          "id": "3475e8c8-8a22-44d7-9a15-acac781b4912",
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
              "id": "000425fb-f744-47c6-b66f-c1c6c8b17ff7"
            }
          ]
        },
        {
          "id": "d6227306-010a-4266-9795-90b24c1161d5",
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
              "id": "768bce67-604c-440e-ae2e-13b2f28c1e3d"
            }
          ]
        },
        {
          "id": "e187265d-3a46-4c3f-bc1a-d6ea68e04468",
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
              "id": "b7f112da-bc1f-4aef-b937-057ff0250150"
            }
          ]
        }
      ]
    },
    {
      "name": "Organization Roles",
      "item": [
        {
          "id": "bcda7af4-0c9f-4496-90ac-90ff700437bd",
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
              "id": "1fcad20a-a328-4fc5-9296-a65910bd6995"
            }
          ]
        },
        {
          "id": "11ebddb4-c073-441f-8f8d-78a75fa8a674",
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
              "id": "0e620ad5-c5e6-4f56-89ca-49c6b322a201"
            }
          ]
        }
      ]
    },
    {
      "name": "Organization Firewall Access Rules",
      "item": [
        {
          "id": "85fe25f2-321c-4a39-9925-164c249b1d78",
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
              "id": "7c008ea0-1c80-4bf9-97ba-eb460648b5b7"
            }
          ]
        },
        {
          "id": "970e26f5-b549-4ce2-a307-5c721ea7a465",
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
              "id": "757a8dba-923b-4fde-81d0-7151f6ab6806"
            }
          ]
        },
        {
          "id": "2036e5b3-f913-4010-b957-eaa8886a771d",
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
              "id": "935c2333-ca8d-421b-a232-4d730c4ff1c2"
            }
          ]
        },
        {
          "id": "69228cba-01da-46a1-884f-3199549585fe",
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
              "id": "903b9cf7-d946-480f-b848-f55fe97cfc96"
            }
          ]
        }
      ]
    },
    {
      "name": "Organizations",
      "item": [
        {
          "id": "bedfc879-3e82-4bcc-86aa-f12530d1e85e",
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
              "id": "fff2ae81-c1e7-40df-a8f8-02c4d0bcf5ac"
            }
          ]
        },
        {
          "id": "ef8c0ae3-3806-49de-89dd-58fc24913ef7",
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
              "id": "18020714-43ee-48e3-be54-94bff75173e1"
            }
          ]
        }
      ]
    },
    {
      "name": "Performance",
      "item": [
        {
          "id": "230f7cc1-f9be-4c6f-961b-fcdb8a290c3a",
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
              "id": "6c1d1069-7fe7-4ba0-aadc-ba3f85b59b84"
            }
          ]
        },
        {
          "id": "8807af58-263e-46b8-b5de-2b9144078f67",
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
              "id": "429b777c-e8ca-4001-b539-b818e504d4d6"
            }
          ]
        },
        {
          "id": "cd3110f6-50af-4bfe-bd1b-41fdd9e2240a",
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
              "id": "4325d5b4-ebfb-4477-92ff-8ed670d5e4c9"
            }
          ]
        },
        {
          "id": "e57acc0e-5ce4-48a4-9e3a-7dd75efe0497",
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
              "id": "65fd8098-dadf-4f07-945d-486f4468ef4c"
            }
          ]
        },
        {
          "id": "a57fe2a0-fdec-4dfd-aa69-a8ace22bbe69",
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
              "id": "0bff7408-8094-4e7f-af8e-36db5466da3a"
            }
          ]
        },
        {
          "id": "69fc993a-fd51-4165-8300-8d93f0568640",
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
              "id": "2279d810-8fcd-479f-882b-f79507ad8138"
            }
          ]
        },
        {
          "id": "98845ba0-183d-4265-8635-1bef03208883",
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
              "id": "7af795ab-0464-46da-ab90-87bc24e04bfe"
            }
          ]
        },
        {
          "id": "86c1452e-5303-43f3-81d3-352cd2f5f0f7",
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
              "id": "ecf2c59b-f231-47e6-889c-a1ea4ac58284"
            }
          ]
        },
        {
          "id": "b8c1abf2-268f-4949-ba0a-81275cccdea7",
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
              "id": "f1f79708-4701-4cc0-8d63-74c1d003d05e"
            }
          ]
        },
        {
          "id": "9d2cb4fa-b812-42a4-897a-5ea913e14f5e",
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
              "id": "12acad10-7baf-4674-a984-a1a61d56226f"
            }
          ]
        }
      ]
    },
    {
      "name": "Users",
      "item": [
        {
          "id": "42577a90-6c0e-4a8a-9273-21fd2a0c5163",
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
              "id": "d082e7fe-5869-4a38-9575-a9382e544eab"
            }
          ]
        },
        {
          "id": "5c42fdf2-9c2e-4a34-a16c-6365d352e8d1",
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
              "id": "48ac8e7f-dc8c-49fe-8673-236963b1c9b8"
            }
          ]
        }
      ]
    },
    {
      "name": "Billing History",
      "item": [
        {
          "id": "e6338876-659b-4558-a817-36061697ea35",
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
              "id": "7636e8c0-39b3-4b5c-bd4f-5db7d7ea3d88"
            }
          ]
        }
      ]
    },
    {
      "name": "Billing Profile",
      "item": [
        {
          "id": "4fa31a4b-6383-4751-84a0-82ad4d51cdc4",
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
              "id": "f7ae9deb-666c-4cff-9e06-6cbddc9b94bd"
            }
          ]
        }
      ]
    },
    {
      "name": "User Level Firewall Access Rule",
      "item": [
        {
          "id": "4c340be9-48e7-4fae-9146-afd22799fe32",
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
              "id": "c626dfc7-593a-4dc7-90bf-a8bd3b3b83ed"
            }
          ]
        },
        {
          "id": "5ee0c988-6bf3-4881-b3ac-1ce1b1d198d4",
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
              "id": "7a0fbbb0-6e6a-4e8d-b412-ea00ddaf13cc"
            }
          ]
        },
        {
          "id": "314df676-eee2-4c57-b943-379e02b80e5f",
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
              "id": "7685b855-d123-41df-8ae9-2c5c0afa435a"
            }
          ]
        },
        {
          "id": "72525799-7767-43c9-8b8c-d8115b439111",
          "name": "cloudflare-userlevel-firewall-access-rule-api",
          "request": {
            "url": "http://example.com/api/user/fir