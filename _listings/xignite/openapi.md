---
swagger: "2.0"
x-collection-name: Xignite
x-complete: 1
info:
  title: Xignite NASDAQ Last Sale
  description: provides-realtime-access-to-last-sale-nasdaq-amex-and-nyse-information-
  version: 1.0.0
host: nasdaqlastsale.xignite.com
basePath: xNASDAQLastSale.json/XigniteNASDAQLastSale
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /GetExtendedQuote:
    get:
      summary: Get Extended Quote
      description: Returns a real-time NASDAQ BASIC quote for given security.
      operationId: GetExtendedQuote
      x-api-path-slug: getextendedquote-get
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
      - Quote
  /GetExtendedQuotes:
    get:
      summary: Get Extended Quotes
      description: Returns real-time NASDAQ BASIC quotes for given securities.
      operationId: GetExtendedQuotes
      x-api-path-slug: getextendedquotes-get
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
      - Quotes
---