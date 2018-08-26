---
swagger: "2.0"
x-collection-name: HitBTC
x-complete: 0
info:
  title: HitBTC Cancel All Open Orders
  description: Cancel all open orders.
  version: 1.0.0
basePath: /api/2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /public/symbol:
    get:
      summary: Available Currency Symbols
      description: Available currency symbols.
      operationId: getPublicSymbol
      x-api-path-slug: publicsymbol-get
      responses:
        200:
          description: OK
      tags:
      - Available
      - Currency
      - Symbols
  /public/symbol/{symbol}:
    get:
      summary: Get Symbol Info
      description: Get symbol info.
      operationId: getPublicSymbolSymbol
      x-api-path-slug: publicsymbolsymbol-get
      parameters:
      - in: path
        name: symbol
      responses:
        200:
          description: OK
      tags:
      - Symbol
      - Info
  /public/currency:
    get:
      summary: Available Currencies
      description: Available currencies.
      operationId: getPublicCurrency
      x-api-path-slug: publiccurrency-get
      responses:
        200:
          description: OK
      tags:
      - Available
      - Currencies
  /public/currency/{currency}:
    get:
      summary: Get Currency Info
      description: Get currency info.
      operationId: getPublicCurrencyCurrency
      x-api-path-slug: publiccurrencycurrency-get
      parameters:
      - in: path
        name: currency
      responses:
        200:
          description: OK
      tags:
      - Currency
      - Info
  /public/ticker:
    get:
      summary: Ticker List For All Symbols
      description: Ticker list for all symbols.
      operationId: getPublicTicker
      x-api-path-slug: publicticker-get
      responses:
        200:
          description: OK
      tags:
      - Ticker
      - List
      - Symbols
  /public/ticker/{symbol}:
    get:
      summary: Ticker For Symbol
      description: Ticker for symbol.
      operationId: getPublicTickerSymbol
      x-api-path-slug: publictickersymbol-get
      parameters:
      - in: path
        name: symbol
      responses:
        200:
          description: OK
      tags:
      - Tickersymbol
  /public/trades/{symbol}:
    get:
      summary: Trades
      description: Trades.
      operationId: getPublicTradesSymbol
      x-api-path-slug: publictradessymbol-get
      parameters:
      - in: query
        name: by
        description: Filter field
      - in: query
        name: from
        description: If filter by timestamp, then datetime in iso format or timestamp
          in millisecond otherwise trade id
      - in: query
        name: limit
      - in: query
        name: offset
      - in: query
        name: sort
        description: Sort direction
      - in: path
        name: symbol
      - in: query
        name: till
        description: If filter by timestamp, then datetime in iso format or timestamp
          in millisecond otherwise trade id
      responses:
        200:
          description: OK
      tags:
      - Trades
  /public/orderbook/{symbol}:
    get:
      summary: Orderbook
      description: Orderbook.
      operationId: getPublicOrderbookSymbol
      x-api-path-slug: publicorderbooksymbol-get
      parameters:
      - in: query
        name: limit
        description: 0 - full orderbook otherwise number of levels
      - in: path
        name: symbol
      responses:
        200:
          description: OK
      tags:
      - Orderbook
  /public/candles/{symbol}:
    get:
      summary: Candles
      description: Candles.
      operationId: getPublicCandlesSymbol
      x-api-path-slug: publiccandlessymbol-get
      parameters:
      - in: query
        name: limit
      - in: query
        name: period
      - in: path
        name: symbol
      responses:
        200:
          description: OK
      tags:
      - Candles
  /order:
    get:
      summary: List Your Current Open Orders
      description: List your current open orders.
      operationId: getOrder
      x-api-path-slug: order-get
      parameters:
      - in: query
        name: symbol
      responses:
        200:
          description: OK
      tags:
      - List
      - Your
      - Current
      - Open
      - Orders
    post:
      summary: Create New Order
      description: Create new order.
      operationId: postOrder
      x-api-path-slug: order-post
      parameters:
      - in: formData
        name: clientOrderId
      - in: formData
        name: expireTime
      - in: formData
        name: price
      - in: formData
        name: quantity
      - in: formData
        name: side
      - in: formData
        name: stopPrice
      - in: formData
        name: strictValidate
        description: Strict validate amount and price precision without rounding
      - in: formData
        name: symbol
      - in: formData
        name: timeInForce
      - in: formData
        name: type
      responses:
        200:
          description: OK
      tags:
      - New
      - Order
    delete:
      summary: Cancel All Open Orders
      description: Cancel all open orders.
      operationId: deleteOrder
      x-api-path-slug: order-delete
      parameters:
      - in: formData
        name: symbol
      responses:
        200:
          description: OK
      tags:
      - Cancel
      - ""
      - Open
      - Orders
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