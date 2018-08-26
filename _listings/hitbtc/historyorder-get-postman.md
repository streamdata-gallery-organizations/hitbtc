{
  "info": {
    "name": "HitBTC Get Historical Orders",
    "_postman_id": "0f65ae48-fb01-4c2f-8764-36ada621b4fc",
    "description": "Get historical orders.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Historical",
      "item": [
        {
          "id": "fbb9707a-c227-44d7-8183-0acdebdf821f",
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
              "id": "26e01857-ff6b-4802-ae2f-9ac0705a528c"
            }
          ]
        },
        {
          "id": "62c8f09a-6c5e-41e5-95d0-28560ef75b9f",
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
              "id": "227b0d61-298b-4873-87bd-f9e0506ddcdc"
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