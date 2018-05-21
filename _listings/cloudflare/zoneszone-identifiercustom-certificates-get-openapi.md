---
swagger: "2.0"
x-collection-name: CloudFlare
x-complete: 0
info:
  title: CloudFlare List, search, sort, and filter all of your custom SSL certificates
  version: 1.0.0
  description: List, search, sort, and filter all of your custom SSL certificates
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