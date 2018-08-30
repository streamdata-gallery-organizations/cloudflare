---
swagger: "2.0"
x-collection-name: CloudFlare
x-complete: 0
info:
  title: CloudFlare If a zone has multiple SSL certificates, you can set the order
    in which they should be used during a request
  version: 1.0.0
  description: If a zone has multiple SSL certificates, you can set the order in which
    they should be used during a request
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /user/billing/subscriptions/apps:
    get:
      summary: List all of your app subscriptions
      description: List all of your app subscriptions
      operationId: cloudflare-app-subscription-api
      x-api-path-slug: userbillingsubscriptionsapps-get
      parameters:
      - in: query
        name: activated_on
        description: When the subscription was activated2014-03-01T12:20:00Z
      - in: query
        name: cancelled_on
        description: When the subscription was cancelled2014-04-01T12:20:00Z
      - in: query
        name: direction
        description: Direction to order subscriptionsdesc
      - in: query
        name: expired_on
        description: When the subscription expired2014-04-02T12:20:00Z
      - in: query
        name: expires_on
        description: When the subscription will expire2014-03-31T12:20:00Z
      - in: query
        name: match
        description: Whether to match all search requirements or at least one (any)all
      - in: query
        name: order
        description: Field to order subscriptions bystatus
      - in: query
        name: page
        description: Page number of paginated results1
      - in: query
        name: per_page
        description: Number of items per page20
      - in: query
        name: price
        description: The price of the subscription that will be billed, in US dollars20
      - in: query
        name: renewed_on
        description: When the subscription was renewed2014-05-11T12:20:00Z
      - in: query
        name: status
        description: The state of the subscriptionactive
      - in: header
        name: X-AUTH-EMAIL
        description: Email address associated with your account
      - in: header
        name: X-AUTH-KEY
        description: API key generated on the My Account page
      responses:
        200:
          description: OK
      tags:
      - Subscriptions
  /user/billing/subscriptions/apps/:identifier:
    get:
      summary: Billing subscription details
      description: Billing subscription details
      operationId: cloudflare-app-subscription-api
      x-api-path-slug: userbillingsubscriptionsappsidentifier-get
      responses:
        200:
          description: OK
      tags:
      - Subscriptions
  /zones/:zone_identifier/custom_pages:
    get:
      summary: A list of available Custom Pages the zone can use
      description: A list of available Custom Pages the zone can use
      operationId: cloudflare-custom-pages-for-a-zone-api
      x-api-path-slug: zoneszone-identifiercustom-pages-get
      responses:
        200:
          description: OK
      tags:
      - Zones
  /zones/:zone_identifier/custom_pages/:identifier:
    get:
      summary: Details about a specific Custom page details
      description: Details about a specific Custom page details
      operationId: cloudflare-custom-pages-for-a-zone-api
      x-api-path-slug: zoneszone-identifiercustom-pagesidentifier-get
      responses:
        200:
          description: OK
      tags:
      - Zones
    put:
      summary: Update Custom page URL
      description: Update Custom page URL
      operationId: cloudflare-custom-pages-for-a-zone-api
      x-api-path-slug: zoneszone-identifiercustom-pagesidentifier-put
      parameters:
      - in: query
        name: state
        description: The Custom Page statettttttttttttttdefault
      - in: query
        name: url
        description: A URL that is associated with the Custom Page
      - in: header
        name: X-AUTH-EMAIL
        description: Email address associated with your account
      - in: header
        name: X-AUTH-KEY
        description: API key generated on the My Account page
      responses:
        200:
          description: OK
      tags:
      - Zones
  /zones/:zone_identifier/custom_certificates:
    get:
      summary: List, search, sort, and filter all of your custom SSL certificates
      description: List, search, sort, and filter all of your custom SSL certificates
      operationId: cloudflare-custom-ssl-for-a-zone-api
      x-api-path-slug: zoneszone-identifiercustom-certificates-get
      parameters:
      - in: query
        name: direction
        description: Direction to order zonesttttttttttttttdesc
      - in: query
        name: match
        description: Whether to match all search requirements or at least one (any)ttttttttttttttall
      - in: query
        name: order
        description: Field to order certificates byttttttttttttttstatus
      - in: query
        name: page
        description: Page number of paginated resultstttttttttttttt1
      - in: query
        name: per_page
        description: Number of zones per pagetttttttttttttt20
      - in: query
        name: status
        description: Status of the zones custom SSLttttttttttttttactive
      - in: header
        name: X-AUTH-EMAIL
        description: Email address associated with your account
      - in: header
        name: X-AUTH-KEY
        description: API key generated on the My Account page
      responses:
        200:
          description: OK
      tags:
      - Certificates
    post:
      summary: Upload a new SSL certificate for a zone
      description: Upload a new SSL certificate for a zone
      operationId: cloudflare-custom-ssl-for-a-zone-api
      x-api-path-slug: zoneszone-identifiercustom-certificates-post
      parameters:
      - in: query
        name: certificate
        description: The zones SSL certificate or certificate and the intermediate(s)tttttttttttttt-----BEGIN
          CERTIFICATE----- MIIDtTCCAp2gAwIBAgIJAM15n7fdxhRtMA0GCSqGSIb3DQEBBQUAMEUxCzAJBgNV
          BAYTAlVTMRMwEQYDVQQIEwpTb21lLVN0YXRlMSEwHwYDVQQKExhJbnRlcm5ldCBX aWRnaXRzIFB0eSBMdGQwHhcNMTQwMzExMTkyMTU5WhcNMTQwNDEwMTkyMTU5WjBF
          MQswCQYDVQQGEwJVUzETMBEGA1UECBMKU29tZS1TdGF0ZTEhMB8GA1UEChMYSW50 ZXJuZXQgV2lkZ2l0cyBQdHkgTHRkMIIBIjANBgkqhkiG9w0BAQEFAAOCAQ8AMIIB
          CgKCAQEAvq3sKsHpeduJHimOK+fvQdKsI8z8A05MZyyLp2/R/GE8FjNv+hkVY1WQ LIyTNNQH7CJecE1nbTfo8Y56S7x/rhxC6/DJ8MIulapFPnorq46KU6yRxiM0MQ3N
          nTJHlHA2ozZta6YBBfVfhHWl1F0IfNbXCLKvGwWWMbCx43OfW6KTkbRnE6gFWKuO fSO5h2u5TaWVuSIzBvYs7Vza6m+gtYAvKAJV2nSZ+eSEFPDo29corOy8+huEOUL8
          5FAw4BFPsr1TlrlGPFitduQUHGrSL7skk1ESGza0to3bOtrodKei2s9bk5MXm7lZ qI+WZJX4Zu9+mzZhc9pCVi8r/qlXuQIDAQABo4GnMIGkMB0GA1UdDgQWBBRvavf+
          sWM4IwKiH9X9w1vl6nUVRDB1BgNVHSMEbjBsgBRvavf+sWM4IwKiH9X9w1vl6nUV RKFJpEcwRTELMAkGA1UEBhMCVVMxEzARBgNVBAgTClNvbWUtU3RhdGUxITAfBgNV
          BAoTGEludGVybmV0IFdpZGdpdHMgUHR5IEx0ZIIJAM15n7fdxhRtMAwGA1UdEwQF MAMBAf8wDQYJKoZIhvcNAQEFBQADggEBABY2ZzBaW0dMsAAT7tPJzrVWVzQx6KU4
          UEBLudIlWPlkAwTnINCWR/8eNjCCmGA4heUdHmazdpPa8RzwOmc0NT1NQqzSyktt vTqb4iHD7+8f9MqJ9/FssCfTtqr/Qst/hGH4Wmdf1EJ/6FqYAAb5iRlPgshFZxU8
          uXtA8hWn6fK6eISD9HBdcAFToUvKNZ1BIDPvh9f95Ine8ar6yGd56TUNrHR8eHBs ESxz5ddVR/oWRysNJ+aGAyYqHS8S/ttmC7r4XCAHqXptkHPCGRqkAhsterYhd4I8
          /cBzejUobNCjjHFbtkAL/SjxZOLW+pNkZwfeYdM8iPkD54Uua1v2tdw= -----END CERTIFICATE-----
      - in: query
        name: private_key
        description: The zones private keytttttttttttttt-----BEGIN RSA PRIVATE KEY-----MIIEowIBAAKCAQEAl
          1cSc0vfcJLI4ZdWjiZZqy86Eof4czCwilyjXdvHqbdgDjz9H6K/0FX78EzVdfyExESptPCDl5YYjvcZyAWlgNfYEpFpGeoh/pTFW3hlyKImh4EgBXbDrR251J
          Ew2Nf56X3duibI6X20gKZA6cvdmWeKh MOOXuh1bSPU3dkb4YOF/fng5iGrx0q3txdMQXTPMZ1uXHFcBH7idgViYesXUBhdll3GP1N
          Y8laq0yrqh 8HMsZK m27MebqonbNmjOqE218lVEvjCdRO6xvNXrO6vNJBoGn2eGwZ8BVd0mTA3Tj43/2cmxQFY9FLq56cCXqYI1fbRRib
          ZLrjSNkwIDAQABAoIBABfAjjsjjxc0NxcYvKOMUb9Rpj8Sx6U/o/tDC5u XmsGX37aaJmC5yw9BQiAxgvXtQryEl5uoNoqOdsxzKV6yM0vPcwKEJVBd4G6yx6AjVJZnc2qf72erR7BbA2CQh
          scMDRBKE041HhgTBRNP6roim0SOgYP5JZIrGAQXNIkyE0fZc5gZNUt388ne/mjWM6Xi08BDGurLC68nsdt7Nd
          UYqeBVxo2EqChp5vKYZYEcG8h9XBj4u4NIwg1Mty2JqX30uBjoHvF5w/pMs8lG uvj6JR9I
          19wtCuccbAJl 4cUq03UQoIDmwejea oC8A8WJr3vVpODDWrvAsjllGPBECgYEAyQRa6edYO6bsSvgbM13qXW9OQTn9YmgzfN24Ux1D66TQU6sBSLdfSHshDhTCi
          Ax 698aJNRWujAakA2DDgspSx98aRnHbF zvY7i7iWGesN6uN0zL 6/MK5uWoieGZRjgk230fLk00l4/FK1mJIp0apr0Lis9xmDjP5AaUPTUUCgYEAwXuhTHZWPT6v8YwOksjbuK
          UDkIIvyMux53kb73vrkgMboS4DB1zMLNyG 9EghS414CFROUwGl4ZUKboH1Jo5G34y8VgDuHjirTqL2H6
          zNpML iMrWCXjpFKkxwPbeQnEAZ 5Rud4d PTyXAt71blZHE9tZ4KHy8cU1iKc9APcCgYAIqKZd4vg7AZK2G//X85iv06aUSrIudfyZyVcyRVVyphPPNtOEVVnGXn9rAtvqeIrOo52BR68
          cj4vlXp hkDuEH QVBuY/NdQhOzFtPrKPQTJdGjIlQ2x65Vidj7r3sRukNkLPyV2v D885zcpTkp83JFuWTYiIrg275DIuAI3QKBgAglM0IrzS
          g3vlVQxvM1ussgRgkkYeybHq82 wUW 3DXLqeXb0s1DedplUkuoabZriz0Wh4GZFSmtA5ZpZC
          uV697lkYsndmp2xRhaekllW7bu pY5q88URwO2p8CO5AZ6CWFWuBwSDML5VOapGRqDRgwaD
          oGpb7fb7IgHOls7AoGBAJnL6Q8t35uYJ8J8hY7wso88IE04z6VaT8WganxcndesWER9eFQDHDDy//ZYeyt6M41uIY
          CL Vkm9Kwl/bHLJKdnOE1a9NdE6mtfah0Bk2u/YOuzyu5mmcgZiX X/OZuEbGmmbZOR1FCuIyrNYfwYohhcZP7/r0Ia/1GpkHc3Bi-----END
          RSA PRIVATE KEY-----
      - in: header
        name: X-AUTH-EMAIL
        description: Email address associated with your account
      - in: header
        name: X-AUTH-KEY
        description: API key generated on the My Account page
      responses:
        200:
          description: OK
      tags:
      - Certificates
  /zones/:zone_identifier/custom_certificates/:identifier:
    delete:
      summary: 'Delete an SSL certificate permission needed: #ssl:edit'
      description: 'Delete an SSL certificate permission needed: #ssl:editntt'
      operationId: cloudflare-custom-ssl-for-a-zone-api
      x-api-path-slug: zoneszone-identifiercustom-certificatesidentifier-delete
      responses:
        200:
          description: OK
      tags:
      - Certificates
    get:
      summary: 'SSL configuration details permission needed: #ssl:read'
      description: 'SSL configuration details permission needed: #ssl:readntt'
      operationId: cloudflare-custom-ssl-for-a-zone-api
      x-api-path-slug: zoneszone-identifiercustom-certificatesidentifier-get
      responses:
        200:
          description: OK
      tags:
      - Certificates
    patch:
      summary: Upload a new private key and/or PEM/CRT for the SSL certificate
      description: Upload a new private key and/or PEM/CRT for the SSL certificate
      operationId: cloudflare-custom-ssl-for-a-zone-api
      x-api-path-slug: zoneszone-identifiercustom-certificatesidentifier-patch
      parameters:
      - in: query
        name: certificate
        description: The zones SSL certificate or certificate and the intermediate(s)tttttttttttttt-----BEGIN
          CERTIFICATE----- MIIDtTCCAp2gAwIBAgIJAM15n7fdxhRtMA0GCSqGSIb3DQEBBQUAMEUxCzAJBgNV
          BAYTAlVTMRMwEQYDVQQIEwpTb21lLVN0YXRlMSEwHwYDVQQKExhJbnRlcm5ldCBX aWRnaXRzIFB0eSBMdGQwHhcNMTQwMzExMTkyMTU5WhcNMTQwNDEwMTkyMTU5WjBF
          MQswCQYDVQQGEwJVUzETMBEGA1UECBMKU29tZS1TdGF0ZTEhMB8GA1UEChMYSW50 ZXJuZXQgV2lkZ2l0cyBQdHkgTHRkMIIBIjANBgkqhkiG9w0BAQEFAAOCAQ8AMIIB
          CgKCAQEAvq3sKsHpeduJHimOK+fvQdKsI8z8A05MZyyLp2/R/GE8FjNv+hkVY1WQ LIyTNNQH7CJecE1nbTfo8Y56S7x/rhxC6/DJ8MIulapFPnorq46KU6yRxiM0MQ3N
          nTJHlHA2ozZta6YBBfVfhHWl1F0IfNbXCLKvGwWWMbCx43OfW6KTkbRnE6gFWKuO fSO5h2u5TaWVuSIzBvYs7Vza6m+gtYAvKAJV2nSZ+eSEFPDo29corOy8+huEOUL8
          5FAw4BFPsr1TlrlGPFitduQUHGrSL7skk1ESGza0to3bOtrodKei2s9bk5MXm7lZ qI+WZJX4Zu9+mzZhc9pCVi8r/qlXuQIDAQABo4GnMIGkMB0GA1UdDgQWBBRvavf+
          sWM4IwKiH9X9w1vl6nUVRDB1BgNVHSMEbjBsgBRvavf+sWM4IwKiH9X9w1vl6nUV RKFJpEcwRTELMAkGA1UEBhMCVVMxEzARBgNVBAgTClNvbWUtU3RhdGUxITAfBgNV
          BAoTGEludGVybmV0IFdpZGdpdHMgUHR5IEx0ZIIJAM15n7fdxhRtMAwGA1UdEwQF MAMBAf8wDQYJKoZIhvcNAQEFBQADggEBABY2ZzBaW0dMsAAT7tPJzrVWVzQx6KU4
          UEBLudIlWPlkAwTnINCWR/8eNjCCmGA4heUdHmazdpPa8RzwOmc0NT1NQqzSyktt vTqb4iHD7+8f9MqJ9/FssCfTtqr/Qst/hGH4Wmdf1EJ/6FqYAAb5iRlPgshFZxU8
          uXtA8hWn6fK6eISD9HBdcAFToUvKNZ1BIDPvh9f95Ine8ar6yGd56TUNrHR8eHBs ESxz5ddVR/oWRysNJ+aGAyYqHS8S/ttmC7r4XCAHqXptkHPCGRqkAhsterYhd4I8
          /cBzejUobNCjjHFbtkAL/SjxZOLW+pNkZwfeYdM8iPkD54Uua1v2tdw= -----END CERTIFICATE-----
      - in: query
        name: private_key
        description: The zones private keytttttttttttttt-----BEGIN RSA PRIVATE KEY-----MIIEowIBAAKCAQEAl
          1cSc0vfcJLI4ZdWjiZZqy86Eof4czCwilyjXdvHqbdgDjz9H6K/0FX78EzVdfyExESptPCDl5YYjvcZyAWlgNfYEpFpGeoh/pTFW3hlyKImh4EgBXbDrR251J
          Ew2Nf56X3duibI6X20gKZA6cvdmWeKh MOOXuh1bSPU3dkb4YOF/fng5iGrx0q3txdMQXTPMZ1uXHFcBH7idgViYesXUBhdll3GP1N
          Y8laq0yrqh 8HMsZK m27MebqonbNmjOqE218lVEvjCdRO6xvNXrO6vNJBoGn2eGwZ8BVd0mTA3Tj43/2cmxQFY9FLq56cCXqYI1fbRRib
          ZLrjSNkwIDAQABAoIBABfAjjsjjxc0NxcYvKOMUb9Rpj8Sx6U/o/tDC5u XmsGX37aaJmC5yw9BQiAxgvXtQryEl5uoNoqOdsxzKV6yM0vPcwKEJVBd4G6yx6AjVJZnc2qf72erR7BbA2CQh
          scMDRBKE041HhgTBRNP6roim0SOgYP5JZIrGAQXNIkyE0fZc5gZNUt388ne/mjWM6Xi08BDGurLC68nsdt7Nd
          UYqeBVxo2EqChp5vKYZYEcG8h9XBj4u4NIwg1Mty2JqX30uBjoHvF5w/pMs8lG uvj6JR9I
          19wtCuccbAJl 4cUq03UQoIDmwejea oC8A8WJr3vVpODDWrvAsjllGPBECgYEAyQRa6edYO6bsSvgbM13qXW9OQTn9YmgzfN24Ux1D66TQU6sBSLdfSHshDhTCi
          Ax 698aJNRWujAakA2DDgspSx98aRnHbF zvY7i7iWGesN6uN0zL 6/MK5uWoieGZRjgk230fLk00l4/FK1mJIp0apr0Lis9xmDjP5AaUPTUUCgYEAwXuhTHZWPT6v8YwOksjbuK
          UDkIIvyMux53kb73vrkgMboS4DB1zMLNyG 9EghS414CFROUwGl4ZUKboH1Jo5G34y8VgDuHjirTqL2H6
          zNpML iMrWCXjpFKkxwPbeQnEAZ 5Rud4d PTyXAt71blZHE9tZ4KHy8cU1iKc9APcCgYAIqKZd4vg7AZK2G//X85iv06aUSrIudfyZyVcyRVVyphPPNtOEVVnGXn9rAtvqeIrOo52BR68
          cj4vlXp hkDuEH QVBuY/NdQhOzFtPrKPQTJdGjIlQ2x65Vidj7r3sRukNkLPyV2v D885zcpTkp83JFuWTYiIrg275DIuAI3QKBgAglM0IrzS
          g3vlVQxvM1ussgRgkkYeybHq82 wUW 3DXLqeXb0s1DedplUkuoabZriz0Wh4GZFSmtA5ZpZC
          uV697lkYsndmp2xRhaekllW7bu pY5q88URwO2p8CO5AZ6CWFWuBwSDML5VOapGRqDRgwaD
          oGpb7fb7IgHOls7AoGBAJnL6Q8t35uYJ8J8hY7wso88IE04z6VaT8WganxcndesWER9eFQDHDDy//ZYeyt6M41uIY
          CL Vkm9Kwl/bHLJKdnOE1a9NdE6mtfah0Bk2u/YOuzyu5mmcgZiX X/OZuEbGmmbZOR1FCuIyrNYfwYohhcZP7/r0Ia/1GpkHc3Bi-----END
          RSA PRIVATE KEY-----
      - in: header
        name: X-AUTH-EMAIL
        description: Email address associated with your account
      - in: header
        name: X-AUTH-KEY
        description: API key generated on the My Account page
      responses:
        200:
          description: OK
      tags:
      - Certificates
  /zones/:zone_identifier/custom_certificates/prioritize:
    put:
      summary: If a zone has multiple SSL certificates, you can set the order in which
        they should be used during a request
      description: If a zone has multiple SSL certificates, you can set the order
        in which they should be used during a request
      operationId: cloudflare-custom-ssl-for-a-zone-api
      x-api-path-slug: zoneszone-identifiercustom-certificatesprioritize-put
      parameters:
      - in: query
        name: certificates
        description: Array of ordered certificates
      - in: header
        name: X-AUTH-EMAIL
        description: Email address associated with your account
      - in: header
        name: X-AUTH-KEY
        description: API key generated on the My Account page
      responses:
        200:
          description: OK
      tags:
      - Certificates
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---