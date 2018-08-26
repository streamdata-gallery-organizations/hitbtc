{
  "info": {
    "name": "HitBTC Get Trading Balance",
    "_postman_id": "9c99b30d-d197-4275-b5d8-6634f0d9b539",
    "description": "Get trading balance.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Trading",
      "item": [
        {
          "id": "dd99be88-e727-403c-872f-4055ac368404",
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
              "id": "b7363804-00f0-4a6e-ab72-26554c4ea3d3"
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