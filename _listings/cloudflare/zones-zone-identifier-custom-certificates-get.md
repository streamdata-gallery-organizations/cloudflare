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
  /zones/:zone_identifier/custom_certificates:
    get:
      summary: List, search, sort, and filter all of your custom SSL certificates
      description: List, search, sort, and filter all of your custom SSL certificates
      operationId: cloudflare-custom-ssl-for-a-zone-api
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