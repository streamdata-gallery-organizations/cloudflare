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
  /zones/:zone_id/firewall/access_rules/rules:
    post:
      summary: Make a new IP, IP range, or country access rule for the zone
      description: Make a new IP, IP range, or country access rule for the zone
      operationId: cloudflare-firewall-access-rule-for-a-zone-api
      parameters:
      - in: query
        name: configuration
        description: Rule configurationtttttttttttttttttttttOne of the following:tttttttttttttttttttttttttttttShow
          definition &raquo;ttttttttttttttttttttttttttttttttttttttName /typetttttttttttDescription
          /exampletttttttttttConstraintstttttttttttttttttttttttttttttttttttttttttttttttttttttttttargettttttttttttttstring
      - in: query
        name: mode
        description: The action to apply to a matched requestttttttttttttttchallenge
      - in: query
        name: value
        description: The IP address to target in requeststtttttttttttttttttttttttttttttttttt1
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
      - firewall access rule
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