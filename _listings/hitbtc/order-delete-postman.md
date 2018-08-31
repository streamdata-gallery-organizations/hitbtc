{
  "info": {
    "name": "HitBTC Cancel All Open Orders",
    "_postman_id": "1d4d938d-b8a3-4c77-a163-6482532214fa",
    "description": "Cancel all open orders.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Cancel",
      "item": [
        {
          "id": "89f749ea-7e61-4f92-bf55-2dd58530ba37",
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
              "id": "094238f5-c8b3-418d-855d-699ff12c7329"
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