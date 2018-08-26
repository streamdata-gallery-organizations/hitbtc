{
  "info": {
    "name": "HitBTC Get Trading Fee Rate",
    "_postman_id": "31c75fbf-802e-4195-b635-7d381799ae9a",
    "description": "Get trading fee rate.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Trading",
      "item": [
        {
          "id": "79e67dfe-9246-476c-92a9-d0f468b48896",
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
              "id": "20e1cf7a-d85a-49a1-900d-57b3b832131f"
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