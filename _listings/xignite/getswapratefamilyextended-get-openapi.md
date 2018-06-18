---
swagger: "2.0"
x-collection-name: Xignite
x-complete: 0
info:
  title: Xignite Money Markets Get Swap Rate Family Extended
  description: Returns latest Swap rate family
  version: 1.0.0
host: www.xignite.com
basePath: xMoneyMarkets.json/XigniteMoneyMarkets
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /GetSwapRateExtended:
    get:
      summary: Get Swap Rate Extended
      description: Returns latest Swap rate
      operationId: postGetswaprateextended
      x-api-path-slug: getswaprateextended-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Swap
      - Rate
      - Extended
  /GetSwapRateFamilyExtended:
    get:
      summary: Get Swap Rate Family Extended
      description: Returns latest Swap rate family
      operationId: postGetswapratefamilyextended
      x-api-path-slug: getswapratefamilyextended-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Swap
      - Rate
      - Family
      - Extended
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