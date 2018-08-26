{
  "info": {
    "name": "HitBTC Rollback Withdraw Crypro",
    "_postman_id": "713975ea-31ba-438b-a5b8-c554e6f27050",
    "description": "Rollback withdraw crypro.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Available",
      "item": [
        {
          "id": "c7d031a0-e195-4468-a08a-5eaf45a16af5",
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
              "id": "9597cb97-74d0-452a-9468-c4d4128698ed"
            }
          ]
        },
        {
          "id": "c7ca52e2-f901-421f-bdbe-8da124bfddcf",
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
              "id": "66e49f34-e1ec-477a-9ea0-acca7816ad00"
            }
          ]
        }
      ]
    },
    {
      "name": "Symbol",
      "item": [
        {
          "id": "e04c5e79-a368-4b10-adcc-49eb2ea5164e",
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
              "id": "16b9ef28-3b08-424f-9ad5-5197ae6aea01"
            }
          ]
        }
      ]
    },
    {
      "name": "Currency",
      "item": [
        {
          "id": "9969913e-e99c-41a7-ac61-7cc52e844e88",
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
              "id": "fc7aa163-af1c-4b6f-a03a-15f5a1176e65"
            }
          ]
        }
      ]
    },
    {
      "name": "Ticker",
      "item": [
        {
          "id": "e8a65641-4405-4028-af02-7d89b1ff8243",
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
              "id": "61c26f47-9e9a-4ce9-aa46-41886194b407"
            }
          ]
        }
      ]
    },
    {
      "name": "Tickersymbol",
      "item": [
        {
          "id": "d389552b-51ad-4583-a818-4886e0a2aa24",
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
              "id": "3dfbde0c-41ca-4317-8786-8bfb7ff52f90"
            }
          ]
        }
      ]
    },
    {
      "name": "Trades",
      "item": [
        {
          "id": "9b8ed284-3bd4-48f5-8cf8-dbb46fcca694",
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
              "id": "88a0255c-62fb-4d7a-a341-590382fd05ef"
            }
          ]
        }
      ]
    },
    {
      "name": "Orderbook",
      "item": [
        {
          "id": "a7d4a374-867a-4d9f-bde4-adca9591f9ca",
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
              "id": "d3e8047f-fa7d-4bad-9060-3b31462635a9"
            }
          ]
        }
      ]
    },
    {
      "name": "Candles",
      "item": [
        {
          "id": "158c620e-d3d3-43e4-aff3-cfebfcdab1c9",
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
              "id": "68562101-86d2-4b2c-85bc-0e2ae20d1102"
            }
          ]
        }
      ]
    },
    {
      "name": "List",
      "item": [
        {
          "id": "697b2b2d-bdde-4518-ad1d-088e4d21be5e",
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
              "id": "62d71bc2-f48d-431a-a43a-a9935867aa8e"
            }
          ]
        }
      ]
    },
    {
      "name": "New",
      "item": [
        {
          "id": "8a4fffe8-8bae-46ae-a285-25c623284c4f",
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
              "id": "4c616f6e-9798-4898-b7f4-9ac58f6661dc"
            }
          ]
        },
        {
          "id": "a7e25973-7d62-47cf-a9b1-2216887df6c3",
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
              "id": "6da6bcd3-2071-4e3a-bd81-a75602a1cdcd"
            }
          ]
        }
      ]
    },
    {
      "name": "Cancel",
      "item": [
        {
          "id": "9e3b3d20-f20e-47f7-8be9-52b4af0d1468",
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
              "id": "c6647a6b-6162-4c05-a7d3-74435fa7de46"
            }
          ]
        },
        {
          "id": "2c7431f5-8fcc-4b1c-8a25-7c903067e90e",
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
              "id": "893444ef-d979-4b15-8eed-20694a5889e4"
            }
          ]
        },
        {
          "id": "d660f61a-9a8d-43e4-9e8b-b9570311efd6",
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
              "id": "973a09fa-6f49-459b-98fe-8fe6a004bac9"
            }
          ]
        }
      ]
    },
    {
      "name": "Single",
      "item": [
        {
          "id": "94912924-196d-4592-96ba-d40e7055e959",
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
              "id": "2dd6d5b2-2aec-4f51-beef-80c2c802581d"
            }
          ]
        }
      ]
    },
    {
      "name": "Trading",
      "item": [
        {
          "id": "4e55c8fd-0a4b-4ec6-a163-cad19f2c7b21",
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
              "id": "11ffe5f4-cdf9-4953-8b58-eaad4bb727fb"
            }
          ]
        },
        {
          "id": "2caba89a-22fc-4aa5-9a8c-177da119a6b1",
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
              "id": "1f2a5c3b-3813-43be-a366-b8b05ee3a8f7"
            }
          ]
        }
      ]
    },
    {
      "name": "Historical",
      "item": [
        {
          "id": "28602c71-365e-4d63-aa93-311374d5fb6f",
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
              "id": "06c95aba-5078-4c58-98d7-222b11e67eca"
            }
          ]
        },
        {
          "id": "128ed94e-1ddd-459d-b48d-7048e617d221",
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
              "id": "66955636-bb8f-4daa-b5a4-d28d867ce0f1"
            }
          ]
        },
        {
          "id": "0d82a340-d653-4358-a883-545409df3e01",
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
              "id": "15ebe451-d00c-42d8-9119-27db3a1701e1"
            }
          ]
        }
      ]
    },
    {
      "name": "Main",
      "item": [
        {
          "id": "fec8bc5d-2c25-4ba1-bb00-887ffa3faaf1",
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
              "id": "8f625625-d79c-4b21-9e3b-cfc3239987df"
            }
          ]
        }
      ]
    },
    {
      "name": "Account",
      "item": [
        {
          "id": "83e103f1-87ff-4716-98ee-f19807c66609",
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
              "id": "169cd7ae-8aa2-46f3-9059-583342d5b8a7"
            }
          ]
        },
        {
          "id": "7b456c7b-aa23-4b20-9dc4-41829c67d0f7",
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
              "id": "9ea101c0-d579-41b3-907d-d50a9ec45358"
            }
          ]
        }
      ]
    },
    {
      "name": "Withdraw",
      "item": [
        {
          "id": "847861b1-4d7b-4784-883a-00431b0616c5",
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
              "id": "f884ce09-e44e-4d3b-8088-825adbe324cf"
            }
          ]
        }
      ]
    },
    {
      "name": "Commit",
      "item": [
        {
          "id": "ddc9fd70-c1bd-49e2-b7e0-37d1e62a6395",
          "name": "putAccountCryptoWithdraw",
          "request": {
            "url": {
              "host": "{{default}}",
              "path": [
                "account/crypto/withdraw/:id"
              ],
              "variable": [
                {
                  "id": "id",
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
              "mode": "raw"
            },
            "description": "Commit withdraw crypro."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b2188540-0b6c-4967-9c37-75d94b8069ef"
            }
          ]
        }
      ]
    },
    {
      "name": "Rollback",
      "item": [
        {
          "id": "00070872-5a8d-462e-8a63-e781e27bdea2",
          "name": "deleteAccountCryptoWithdraw",
          "request": {
            "url": {
              "host": "{{default}}",
              "path": [
                "account/crypto/withdraw/:id"
              ],
              "variable": [
                {
                  "id": "id",
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
            "description": "Rollback withdraw crypro."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bd718058-d88f-4735-b649-46af8151d3bc"
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