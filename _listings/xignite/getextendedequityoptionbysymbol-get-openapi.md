---
swagger: "2.0"
x-collection-name: Xignite
x-complete: 0
info:
  title: Xignite Global Real Time Options Get Extended Equity Option By Symbol
  description: Returns a specific equity extended option.
  version: 1.0.0
host: globalrealtimeoptions.xignite.com
basePath: xglobalrealtimeoptions.json/XigniteGlobalRealTimeOptions
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /GetAllExtendedEquityOptionChain:
    get:
      summary: Get All Extended Equity Option Chain
      description: Returns extended options chains for an equity.
      operationId: GetAllExtendedEquityOptionChain
      x-api-path-slug: getallextendedequityoptionchain-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Extended
      - Equity
      - Option
      - Chain
  /GetExtendedEquityOptionChain:
    get:
      summary: Get Extended Equity Option Chain
      description: Returns extended options chain for an equity.
      operationId: GetExtendedEquityOptionChain
      x-api-path-slug: getextendedequityoptionchain-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Extended
      - Equity
      - Option
      - Chain
  /GetExtendedEquityOption:
    get:
      summary: Get Extended Equity Option
      description: Returns a specific equity extended option.
      operationId: GetExtendedEquityOption
      x-api-path-slug: getextendedequityoption-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Extended
      - Equity
      - Option
  /GetExtendedEquityOptionBySymbol:
    get:
      summary: Get Extended Equity Option By Symbol
      description: Returns a specific equity extended option.
      operationId: GetExtendedEquityOptionBySymbol
      x-api-path-slug: getextendedequityoptionbysymbol-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Extended
      - Equity
      - Option
      - Symbol
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