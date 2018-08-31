{
  "info": {
    "name": "HitBTC Get Account Transaction By Id",
    "_postman_id": "0c3341f9-ba80-4529-8e16-e5f19477e127",
    "description": "Get account transaction by id.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Account",
      "item": [
        {
          "id": "6e12c318-8578-49b0-bc8d-71397b4ea84b",
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
              "id": "d6fcef94-d1c8-4e54-968d-98a7bc4e4b0e"
            }
          ]
        },
        {
          "id": "a9df0ae4-d219-4288-8c06-c1b654958412",
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
              "id": "95a3d05a-2fcc-4e6d-98dd-c7e9e9144feb"
            }
          ]
        }
      ]
    },
    {
      "name": "Main",
      "item": [
        {
          "id": "9e83edf5-be67-4342-9134-5bd42a930cb7",
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
              "id": "5929e796-b34e-4fbc-a79f-564fb9bd440e"
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