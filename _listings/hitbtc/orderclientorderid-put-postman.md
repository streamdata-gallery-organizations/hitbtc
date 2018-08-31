{
  "info": {
    "name": "HitBTC Create New Order",
    "_postman_id": "b25a9bea-7a8c-422d-8a33-502b62d6f94d",
    "description": "Create new order.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "New",
      "item": [
        {
          "id": "2b5a57ee-0bd2-4dc1-9b81-94b006f7c141",
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
              "id": "ca868c80-5e35-4aa9-94d8-720b59100ff1"
            }
          ]
        },
        {
          "id": "0784118e-1f13-4fe3-95d9-acb418b3023b",
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
              "id": "e32218e8-5f6e-4f2b-acee-f44447834f31"
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