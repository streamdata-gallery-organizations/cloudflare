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
  /zones/:zone_identifier/dns_records:
    get:
      summary: List, search, sort, and filter a zones&#39; DNS records
      description: List, search, sort, and filter a zones&#39; DNS records
      operationId: cloudflare-dns-records-for-a-zone-api
      parameters:
      - in: query
        name: content
        description: DNS record contenttttttttttttttt127
      - in: query
        name: direction
        description: Direction to order domainsttttttttttttttdesc
      - in: query
        name: match
        description: Whether to match all search requirements or at least one (any)ttttttttttttttall
      - in: query
        name: name
        description: DNS record namettttttttttttttexample
      - in: query
        name: order
        description: Field to order records bytttttttttttttttype
      - in: query
        name: page
        description: Page number of paginated resultstttttttttttttt1
      - in: query
        name: per_page
        description: Number of DNS records per pagetttttttttttttt20
      - in: query
        name: type
        description: DNS record typettttttttttttttA
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
      - records
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