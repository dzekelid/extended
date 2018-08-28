---
swagger: "2.0"
x-collection-name: Xignite
x-complete: 0
info:
  title: Xignite NASDAQ Last Sale Get Extended Quotes
  description: Returns real-time NASDAQ BASIC quotes for given securities.
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
  /GetGlobalHistoricalQuotesRangeExtended:
    get:
      summary: Get Global Historical Quotes Range Extended
      description: This operation returns a complete range of global historical quotes
        extended for a given equity. This includes the adjusted price as specified.
      operationId: postGetglobalhistoricalquotesrangeextended
      x-api-path-slug: getglobalhistoricalquotesrangeextended-get
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
      - Global
      - Historical
      - Quotes
      - Range
      - Extended
  /GetGlobalHistoricalWeeklyQuotesRangeExtended:
    get:
      summary: Get Global Historical Weekly Quotes Range Extended
      description: Returns a range of weekly Global Historical quotes extended for
        a security. For more information, go to http://www.xignite.com/
      operationId: postGetglobalhistoricalweeklyquotesrangeextended
      x-api-path-slug: getglobalhistoricalweeklyquotesrangeextended-get
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
      - Global
      - Historical
      - Weekly
      - Quotes
      - Range
      - Extended
  /GetGlobalHistoricalMonthlyQuotesRangeExtended:
    get:
      summary: Get Global Historical Monthly Quotes Range Extended
      description: This operation returns a range of monthly quotes extended for an
        equity based on the specified date range. This includes the adjusted price
        as specified.
      operationId: postGetglobalhistoricalmonthlyquotesrangeextended
      x-api-path-slug: getglobalhistoricalmonthlyquotesrangeextended-get
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
      - Global
      - Historical
      - Monthly
      - Quotes
      - Range
      - Extended
  /GetRealTimeExtendedMetalQuote:
    get:
      summary: Get Real Time Extended Metal Quote
      description: Get real time extended metal quote.
      operationId: GetRealTimeExtendedMetalQuote
      x-api-path-slug: getrealtimeextendedmetalquote-get
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
      - Real
      - Time
      - Extended
      - Metal
      - Quote
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
  /GetExtendedEquityOptionBySymbols:
    get:
      summary: Get Extended Equity Option By Symbols
      description: Returns an array of specific equity extended options.
      operationId: GetExtendedEquityOptionBySymbols
      x-api-path-slug: getextendedequityoptionbysymbols-get
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
      - Symbols
  /GetExtendedDividendHistory:
    get:
      summary: Get Extended Dividend History
      description: Get extended dividend history for a stock.
      operationId: postGetextendeddivendhistory
      x-api-path-slug: getextendeddividendhistory-get
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
      - Extended
      - Dividend
      - History
  /GetExtendedDividendHistoryRange:
    get:
      summary: Get Extended Dividend History Range
      description: Get extended dividend history range for a stock.
      operationId: postGetextendeddivendhistoryrange
      x-api-path-slug: getextendeddividendhistoryrange-get
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
      - Extended
      - Dividend
      - History
      - Range
  /GetAllExtendedDividends:
    get:
      summary: Get All Extended Dividends
      description: Get all extended dividend for a date range.
      operationId: postGetallextendeddivends
      x-api-path-slug: getallextendeddividends-get
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
      - Extended
      - Dividends
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
  /GetHistoricalSwapRateExtended:
    get:
      summary: Get Historical Swap Rate Extended
      description: Returns historical swap rate
      operationId: postGethistoricalswaprateextended
      x-api-path-slug: gethistoricalswaprateextended-get
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
      - Historical
      - Swap
      - Rate
      - Extended
  /GetHistoricalSwapRateExtendedRange:
    get:
      summary: Get Historical Swap Rate Extended Range
      description: Returns historical Swap rate range
      operationId: postGethistoricalswaprateextendedrange
      x-api-path-slug: gethistoricalswaprateextendedrange-get
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
      - Historical
      - Swap
      - Rate
      - Extended
      - Range
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