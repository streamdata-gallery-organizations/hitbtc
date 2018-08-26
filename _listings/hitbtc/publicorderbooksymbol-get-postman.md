{
  "info": {
    "name": "HitBTC Orderbook",
    "_postman_id": "101fa3f5-8029-48d0-a09d-9dc4b63dab9f",
    "description": "Orderbook.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Available",
      "item": [
        {
          "id": "01a7a65d-06f7-4283-9cd1-1f52638a4062",
          "name": "getPublicSymbol",
          "request": {
            "url": "{{default}}/public/symbol",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Available currency symbols."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6f61f1e2-c316-475f-90e0-86810444f967"
            }
          ]
        },
        {
          "id": "89439a46-749c-4c13-b87b-364fa4631e8c",
          "name": "getPublicCurrency",
          "request": {
            "url": "{{default}}/public/currency",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Available currencies."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "37333e30-b3a7-4c03-bb41-d640cd691ad3"
            }
          ]
        }
      ]
    },
    {
      "name": "Symbol",
      "item": [
        {
          "id": "eef7eff5-ece8-4e68-8adb-7b00bc2b1722",
          "name": "getPublicSymbolSymbol",
          "request": {
            "url": {
              "host": "{{default}}",
              "path": [
                "public/symbol/:symbol"
              ],
              "variable": [
                {
                  "id": "symbol",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get symbol info."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9d4c19e7-d10d-4dab-94da-e7f698cb6441"
            }
          ]
        }
      ]
    },
    {
      "name": "Currency",
      "item": [
        {
          "id": "f80d5f82-4b5b-445c-86ad-6469fd24318a",
          "name": "getPublicCurrencyCurrency",
          "request": {
            "url": {
              "host": "{{default}}",
              "path": [
                "public/currency/:currency"
              ],
              "variable": [
                {
                  "id": "currency",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get currency info."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fbb25d0d-4a0e-4b0a-bde5-8be0b265ca8b"
            }
          ]
        }
      ]
    },
    {
      "name": "Ticker",
      "item": [
        {
          "id": "5c64ef0d-3a86-445e-ac25-d94e37f94fe0",
          "name": "getPublicTicker",
          "request": {
            "url": "{{default}}/public/ticker",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Ticker list for all symbols."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7b334b1b-9315-4f10-a50d-a4ecf84d63ea"
            }
          ]
        }
      ]
    },
    {
      "name": "Tickersymbol",
      "item": [
        {
          "id": "be684d89-cfbe-48d2-9390-e6aa485b429a",
          "name": "getPublicTickerSymbol",
          "request": {
            "url": {
              "host": "{{default}}",
              "path": [
                "public/ticker/:symbol"
              ],
              "variable": [
                {
                  "id": "symbol",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Ticker for symbol."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ce366543-c42b-48eb-942a-74562a61adc8"
            }
          ]
        }
      ]
    },
    {
      "name": "Trades",
      "item": [
        {
          "id": "eeda5a4b-9e54-47bb-b345-817a5f602ff0",
          "name": "getPublicTradesSymbol",
          "request": {
            "url": {
              "host": "{{default}}",
              "path": [
                "public/trades/:symbol"
              ],
              "query": [
                {
                  "key": "by",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "from",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "limit",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "offset",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "sort",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "till",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "symbol",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Trades."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "768371ac-ff45-4bd8-afe3-6c8ee9aa1a31"
            }
          ]
        }
      ]
    },
    {
      "name": "Orderbook",
      "item": [
        {
          "id": "387ae5b7-1633-470e-bf36-f0205478fc71",
          "name": "getPublicOrderbookSymbol",
          "request": {
            "url": {
              "host": "{{default}}",
              "path": [
                "public/orderbook/:symbol"
              ],
              "query": [
                {
                  "key": "limit",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "symbol",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Orderbook."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "df6ab311-d6b7-42d7-a169-675269ca4787"
            }
          ]
        }
      ]
    }
  ],
  "variable": [
    {
      "key": "default",
      "value": "http://www.example.com/api/2"
    }
  ]
}