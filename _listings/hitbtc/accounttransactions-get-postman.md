{
  "info": {
    "name": "HitBTC Get Account Transactions",
    "_postman_id": "cfed5bfd-07cb-4551-9199-0417a6534fda",
    "description": "Get account transactions.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Account",
      "item": [
        {
          "id": "0ba9b101-eb20-49ea-ae83-b382a167e680",
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
              "id": "9908ac67-47e3-46f9-8fe6-4bbef5ed3ced"
            }
          ]
        },
        {
          "id": "93c462cf-9114-4c95-9de0-eb2ec0554e44",
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
              "id": "dfc81d83-676f-406d-98b1-0c50c107878a"
            }
          ]
        }
      ]
    },
    {
      "name": "Main",
      "item": [
        {
          "id": "2c4efeae-cb73-4ff8-ab8c-767d62a899e9",
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
              "id": "cb38e0a5-faa8-47d9-87ad-e1cdfa528161"
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