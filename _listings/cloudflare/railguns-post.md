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
  /railguns:
    post:
      summary: Readable identifier of the railgun
      description: Readable identifier of the railgun
      operationId: cloudflare-railgun-api
      parameters:
      - in: query
        name: name
        description: Readable identifier of the railgunttttttttttttttMy Railgun
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
      - performance
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