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
  /zones/:zone_identifier/keyless_certificates/:identifier:
    delete:
      summary: 'Delete Keyless configuration permission needed: #ssl:edit'
      description: ' Delete Keyless configuration permission needed: #ssl:editntt  '
      operationId: cloudflare-keyless-ssl-for-a-zone-api
      responses:
        200:
          description: OK
      tags:
      - keyless certificates
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