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
  /zones/:zone_identifier/dns_records/:identifier:
    put:
      summary: 'Update DNS record permission needed: #dns_records:edit'
      description: ' Update DNS record permission needed: #dns_records:editntt  '
      operationId: cloudflare-dns-records-for-a-zone-api
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