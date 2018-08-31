{
  "info": {
    "name": "HitBTC Withdraw Crypro",
    "_postman_id": "a28eb50e-0528-457d-a8de-c1c61bf9f16a",
    "description": "Withdraw crypro.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Available",
      "item": [
        {
          "id": "f3dab0ec-b961-4242-920a-c8635426fc94",
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
              "id": "e9272a6b-b0d3-4f6b-b940-f52eafa60098"
            }
          ]
        },
        {
          "id": "5401e980-3a4e-4284-a06a-319fe19337fd",
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
              "id": "e3cc678f-26c6-4080-86f4-50848ec97088"
            }
          ]
        }
      ]
    },
    {
      "name": "Symbol",
      "item": [
        {
          "id": "32efe55b-a9be-4651-88e0-c4f2cf45151f",
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
              "id": "dc5b5155-a253-4176-bd82-9920c0653f7a"
            }
          ]
        }
      ]
    },
    {
      "name": "Currency",
      "item": [
        {
          "id": "6828478a-e2f9-42cc-bdf0-94c49c6107f0",
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
              "id": "79627709-7b64-4b78-b0ee-ddaf8ef711b6"
            }
          ]
        }
      ]
    },
    {
      "name": "Ticker",
      "item": [
        {
          "id": "8a8c1fcf-02a0-4ca6-a733-e58367c0edcf",
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
              "id": "3f343caf-6a6f-491d-b02c-b8f7c769bfc2"
            }
          ]
        }
      ]
    },
    {
      "name": "Tickersymbol",
      "item": [
        {
          "id": "978d1f85-c3a1-443e-be75-b379ef4114ab",
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
              "id": "db19b410-ffa1-4287-94fa-dab55ac62147"
            }
          ]
        }
      ]
    },
    {
      "name": "Trades",
      "item": [
        {
          "id": "04d4f633-1f61-48c5-bc94-7c138819de4c",
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
              "id": "c00aab6c-3763-43d1-b5a8-ffbd6c0b9039"
            }
          ]
        }
      ]
    },
    {
      "name": "Orderbook",
      "item": [
        {
          "id": "8ab88f02-9a7c-4bd8-b74b-0c5d0de431f6",
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
              "id": "47746d20-7abc-42b5-951e-348dda37b001"
            }
          ]
        }
      ]
    },
    {
      "name": "Candles",
      "item": [
        {
          "id": "47cfc6f1-0e61-40e7-80ee-e06d948920ae",
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
              "id": "2ca30132-7ea4-4e0a-8a2d-f0d050ad4c92"
            }
          ]
        }
      ]
    },
    {
      "name": "List",
      "item": [
        {
          "id": "b2c07c84-c619-465c-b6ec-ff2126c7a77c",
          "name": "getOrder",
          "request": {
            "url": "{{default}}/order?symbol=%7B%7D",
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
            "description": "List your current open orders."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3fa873c7-f554-4541-960c-8eeeddcffdc7"
            }
          ]
        }
      ]
    },
    {
      "name": "New",
      "item": [
        {
          "id": "c2c12397-5919-4401-9321-5ff4bc2ab681",
          "name": "postOrder",
          "request": {
            "url": "{{default}}/order",
            "method": "POST",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "clientOrderId",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "expireTime",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "price",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "quantity",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "side",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "stopPrice",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "strictValidate",
                  "value": "{}",
                  "disabled": false,
                  "description": "Strict validate amount and price precision without rounding"
                },
                {
                  "key": "symbol",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "timeInForce",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "type",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                }
              ]
            },
            "description": "Create new order."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b4748d88-d66e-4eca-bbe2-0de3aa4764a1"
            }
          ]
        },
        {
          "id": "5c16bb4d-0969-4462-a3b7-ef43c0ee2e80",
          "name": "putOrderClientorder",
          "request": {
            "url": {
              "host": "{{default}}",
              "path": [
                "order/:clientOrderId"
              ],
              "variable": [
                {
                  "id": "clientOrderId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "expireTime",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "price",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "quantity",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "side",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "stopPrice",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "strictValidate",
                  "value": "{}",
                  "disabled": false,
                  "description": "Strict validate amount and price precision without rounding"
                },
                {
                  "key": "symbol",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "timeInForce",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "type",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                }
              ]
            },
            "description": "Create new order."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "75a0d985-4f45-4172-add9-80eb404f279d"
            }
          ]
        }
      ]
    },
    {
      "name": "Cancel",
      "item": [
        {
          "id": "4ee7b9bd-2628-4af9-9e1b-1760dd3dfa23",
          "name": "deleteOrder",
          "request": {
            "url": "{{default}}/order",
            "method": "DELETE",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "symbol",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                }
              ]
            },
            "description": "Cancel all open orders."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a9954ebb-498d-4c68-aa78-e44af97ee952"
            }
          ]
        },
        {
          "id": "7ec5aa2c-3559-49da-b294-afcf829b331b",
          "name": "deleteOrderClientorder",
          "request": {
            "url": {
              "host": "{{default}}",
              "path": [
                "order/:clientOrderId"
              ],
              "variable": [
                {
                  "id": "clientOrderId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
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
            "description": "Cancel order."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3343ac84-fc00-4ce9-9ed4-e2b1a04be4ee"
            }
          ]
        },
        {
          "id": "f6e45a96-209b-49bb-a1e3-722188cd8172",
          "name": "patchOrderClientorder",
          "request": {
            "url": {
              "host": "{{default}}",
              "path": [
                "order/:clientOrderId"
              ],
              "variable": [
                {
                  "id": "clientOrderId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PATCH",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "price",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "quantity",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "requestClientId",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                }
              ]
            },
            "description": "Cancel replace order."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a187d916-b4ab-4ff0-86cc-2f87b3347bff"
            }
          ]
        }
      ]
    },
    {
      "name": "Single",
      "item": [
        {
          "id": "7590b3da-5518-4d7f-90a0-4a47b13a4496",
          "name": "getOrderClientorder",
          "request": {
            "url": {
              "host": "{{default}}",
              "path": [
                "order/:clientOrderId"
              ],
              "query": [
                {
                  "key": "wait",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "clientOrderId",
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
            "description": "Get a single order by clientorderid."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "43af1970-917b-4c78-a2fd-776eed4c3afe"
            }
          ]
        }
      ]
    },
    {
      "name": "Trading",
      "item": [
        {
          "id": "2486c2d8-7799-4c3b-b6f2-2d1e2676401e",
          "name": "getTradingBalance",
          "request": {
            "url": "{{default}}/trading/balance",
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
            "description": "Get trading balance."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0c35877a-c663-4ebe-88c3-004d504427e9"
            }
          ]
        },
        {
          "id": "821925c7-6c01-4dde-8910-c757db225181",
          "name": "getTradingFeeSymbol",
          "request": {
            "url": {
              "host": "{{default}}",
              "path": [
                "trading/fee/:symbol"
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
            "description": "Get trading fee rate."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "46b639fa-d8b3-4b2a-b463-4d8c0f27fcbd"
            }
          ]
        }
      ]
    },
    {
      "name": "Historical",
      "item": [
        {
          "id": "cc91b1c2-26c5-424e-ab67-821792538505",
          "name": "getHistoryTrades",
          "request": {
            "url": "{{default}}/history/trades?by=%7B%7D&from=%7B%7D&limit=%7B%7D&offset=%7B%7D&sort=%7B%7D&symbol=%7B%7D&till=%7B%7D",
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
            "description": "Get historical trades."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "85ced902-8c26-42d0-b515-46c4edb88d9c"
            }
          ]
        },
        {
          "id": "6e948446-40e5-4fdf-9ff2-174cffbd7536",
          "name": "getHistoryOrder",
          "request": {
            "url": "{{default}}/history/order?clientOrderId=%7B%7D&from=%7B%7D&limit=%7B%7D&offset=%7B%7D&symbol=%7B%7D&till=%7B%7D",
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
            "description": "Get historical orders."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b326a5fa-d2e8-4ebe-89d7-87edd4876291"
            }
          ]
        },
        {
          "id": "2cc98494-a492-4a9a-b6eb-2b55ba5578cb",
          "name": "getHistoryOrderTrades",
          "request": {
            "url": {
              "host": "{{default}}",
              "path": [
                "history/order/:id/trades"
              ],
              "variable": [
                {
                  "id": "id",
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
            "description": "Get historical trades by specified order."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5032cc13-8a9c-4d1f-ac33-56455828529a"
            }
          ]
        }
      ]
    },
    {
      "name": "Main",
      "item": [
        {
          "id": "a8ef3ce4-b4d5-499f-9f95-a3b13d8ff23a",
          "name": "getAccountBalance",
          "request": {
            "url": "{{default}}/account/balance",
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
            "description": "Get main acccount balance."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "10dd3534-a0ec-4500-84e5-d5ecfb84bde3"
            }
          ]
        }
      ]
    },
    {
      "name": "Account",
      "item": [
        {
          "id": "e6a73c76-7e66-4c63-a599-7063db8f62a2",
          "name": "getAccountTransactions",
          "request": {
            "url": "{{default}}/account/transactions?by=%7B%7D&currency=%7B%7D&from=%7B%7D&limit=%7B%7D&offset=%7B%7D&sort=%7B%7D&till=%7B%7D",
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
            "description": "Get account transactions."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "66729e98-8943-446e-8fd3-c3976ede9f75"
            }
          ]
        },
        {
          "id": "ac63a49e-33b5-44ca-b3b0-e9e11792962e",
          "name": "getAccountTransactions",
          "request": {
            "url": {
              "host": "{{default}}",
              "path": [
                "account/transactions/:id"
              ],
              "variable": [
                {
                  "id": "id",
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
            "description": "Get account transaction by id."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6d80f28f-2e09-4400-ba18-a187d72c60c0"
            }
          ]
        }
      ]
    },
    {
      "name": "Withdraw",
      "item": [
        {
          "id": "91c3e5cd-662f-498f-abfb-b03ea0f210e3",
          "name": "postAccountCryptoWithdraw",
          "request": {
            "url": "{{default}}/account/crypto/withdraw",
            "method": "POST",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "address",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "amount",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "autoCommit",
                  "value": "{}",
                  "disabled": false,
                  "description": "If Auto commit disabled you should commit it or rollback within 1 hour"
                },
                {
                  "key": "currency",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "includeFee",
                  "value": "{}",
                  "disabled": false,
                  "description": "If enabled, then fee will be subtracted from amount"
                },
                {
                  "key": "networkFee",
                  "value": "{}",
                  "disabled": false,
                  "description": "Suggest preferred network fee"
                },
                {
                  "key": "paymentId",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                }
              ]
            },
            "description": "Withdraw crypro."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2db910b6-c38b-4bc0-b6b5-f98a701ae1a9"
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