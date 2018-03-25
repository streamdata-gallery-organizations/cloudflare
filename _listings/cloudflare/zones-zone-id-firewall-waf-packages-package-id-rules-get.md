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
  /zones/:zone_id/firewall/waf/packages/:package_id/rules:
    get:
      summary: Search, sort, and filter rules within a package
      description: Search, sort, and filter rules within a package
      operationId: cloudflare-waf-rules-api
      parameters:
      - in: query
        name: description
        description: Public description of the rulettttttttttttttSQL injection prevention
          for SELECT statements
      - in: query
        name: direction
        description: Direction to order rulesttttttttttttttdesc
      - in: query
        name: group_id
        description: WAF group identifier tagttttttttttttttde677e5818985db1285d0e80225f06e5
      - in: query
        name: match
        description: Whether to match all search requirements or at least one (any)ttttttttttttttall
      - in: query
        name: mode
        description: The rule modetttttttttttttttttttttOne of the following:ttttttttttttttttttttttWhether
          or not the anomaly-based rule will be used when evaluating the request
      - in: query
        name: order
        description: Field to order rules byttttttttttttttstatus
      - in: query
        name: page
        description: Page number of paginated resultstttttttttttttt1
      - in: query
        name: per_page
        description: Number of rules per pagetttttttttttttt50
      - in: query
        name: priority
        description: The order in which the individual rule is executed within the
          related grouptttttttttttttt5
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
      - waf rules
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