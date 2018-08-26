{
  "info": {
    "name": "HitBTC Create New Order",
    "_postman_id": "c3ecd829-58ff-4d44-8037-b2988e7cc293",
    "description": "Create new order.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "New",
      "item": [
        {
          "id": "4963afc1-9899-4eac-b40d-bf8eaa76589b",
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
              "id": "b08cccae-a721-4887-9351-cfe2c6ff674c"
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