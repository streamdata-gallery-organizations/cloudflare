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
  /user:
    patch:
      summary: Update part of your user details
      description: Update part of your user details
      operationId: cloudflare-user-api
      parameters:
      - in: query
        name: country
        description: The country in which the user lives
      - in: query
        name: first_name
        description: Users first nameJohn
      - in: query
        name: last_name
        description: Users last nameAppleseed
      - in: query
        name: telephone
        description: Users telephone number+1 123-123-1234
      - in: header
        name: X-AUTH-EMAIL
        description: Email address associated with your account
      - in: header
        name: X-AUTH-KEY
        description: API key generated on the My Account page
      - in: query
        name: zipcode
        description: The zipcode or postal code where the user lives
      responses:
        200:
          description: OK
      tags:
      - users
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