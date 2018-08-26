{
  "info": {
    "name": "HitBTC Candles",
    "_postman_id": "f2259107-59a1-40f1-bc46-c1a93370edb6",
    "description": "Candles.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Available",
      "item": [
        {
          "id": "40ac14fa-f8c2-40a2-97ef-6fd561026e95",
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
              "id": "2773f55f-4d4c-404f-b53b-a5b75901c0ca"
            }
          ]
        },
        {
          "id": "4dde02ed-6211-43cf-a7b1-8276d62f61fa",
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
              "id": "ed3ea733-118c-434f-a482-8021be09dd98"
            }
          ]
        }
      ]
    },
    {
      "name": "Symbol",
      "item": [
        {
          "id": "5c93b720-7ad9-4955-acc5-3cf33299749b",
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
              "id": "e5fc6f2e-bdf1-497d-96d2-87885fbf66fa"
            }
          ]
        }
      ]
    },
    {
      "name": "Currency",
      "item": [
        {
          "id": "72f3f197-2e69-407d-ba84-67b0a5815b90",
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
              "id": "9b8642fb-b39e-4a44-9d53-bbe9965902a3"
            }
          ]
        }
      ]
    },
    {
      "name": "Ticker",
      "item": [
        {
          "id": "17fbbb9a-2352-4364-8b88-ebca3cfbf287",
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
              "id": "09f6ef50-ae5d-4a5a-ac2d-0dec9f6312b7"
            }
          ]
        }
      ]
    },
    {
      "name": "Tickersymbol",
      "item": [
        {
          "id": "6a22208b-af06-43e6-8dc3-e6c85f45da94",
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
              "id": "31a41dcd-320d-40f0-92af-048f45d42c52"
            }
          ]
        }
      ]
    },
    {
      "name": "Trades",
      "item": [
        {
          "id": "18760293-59a0-49e0-bcd5-8b9d58b81c30",
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
              "id": "84959c05-a157-43b7-9e78-d7a7496beffa"
            }
          ]
        }
      ]
    },
    {
      "name": "Orderbook",
      "item": [
        {
          "id": "71c3220a-242d-4455-a8c3-944418384381",
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
              "id": "03a70e0f-caf8-4275-a313-0e0b10188810"
            }
          ]
        }
      ]
    },
    {
      "name": "Candles",
      "item": [
        {
          "id": "a619f47f-e767-47af-8eb5-29e59f43ca0c",
          "name": "getPublicCandlesSymbol",
          "request": {
            "url": {
              "host": "{{default}}",
              "path": [
                "public/candles/:symbol"
              ],
              "query": [
                {
                  "key": "limit",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "period",
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
            "description": "Candles."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "abed2147-0a2c-4979-97c6-d8b37505df77"
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