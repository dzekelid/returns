{
  "info": {
    "name": "Capital One DevExchange Get all withdrawals",
    "_postman_id": "1eb9b347-0caa-4f5c-af4a-d695427158cc",
    "description": "Returns the withdrawals that you are involved in.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "banks",
      "item": [
        {
          "id": "cc8aa32b-9696-4ce9-8dc0-c8bf36b03150",
          "name": "returns-the-withdrawals-that-you-are-involved-in",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.reimaginebanking.com",
              "path": [
                "accounts/:id/withdrawals"
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
            "body": {
              "mode": "raw"
            },
            "description": "Returns the withdrawals that you are involved in"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "73a35a25-22eb-4043-bfab-015dccfb6473"
            }
          ]
        }
      ]
    }
  ]
}