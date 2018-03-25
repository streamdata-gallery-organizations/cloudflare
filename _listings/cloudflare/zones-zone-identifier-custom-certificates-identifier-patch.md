---
swagger: "2.0"
info:
  title: CloudFlare
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /zones/:zone_identifier/custom_certificates/:identifier:
    patch:
      summary: Upload a new private key and/or PEM/CRT for the SSL certificate
      description: Upload a new private key and/or PEM/CRT for the SSL certificate
      operationId: cloudflare-custom-ssl-for-a-zone-api
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
      - certificates
definitions: []
x-collection-name: CloudFlare
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