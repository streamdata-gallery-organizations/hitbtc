{
  "info": {
    "name": "HitBTC Cancel Order",
    "_postman_id": "546e506d-6fc0-470e-87a6-5b82d70d2d7a",
    "description": "Cancel order.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Cancel",
      "item": [
        {
          "id": "bc96b5ba-2c0f-428a-8ec6-166a69f52db8",
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
              "id": "055f5fa9-3bb6-45a2-8a24-d8b190cd1d15"
            }
          ]
        },
        {
          "id": "fc2d35d6-ff35-4e8e-b8a3-c9fd2c07759e",
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
              "id": "f9e1827b-004b-4366-bf22-2c730426ef9d"
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