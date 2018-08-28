{
  "info": {
    "name": "Capital One DevExchange Get account by id",
    "_postman_id": "7fca39ed-649d-44a8-93b2-075a1f2f8e6b",
    "description": "Returns the account with the specific id",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "banks",
      "item": [
        {
          "id": "e979f137-d790-4aac-832d-5a0b5de14401",
          "name": "returns-the-account-with-the-specific-id",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.reimaginebanking.com",
              "path": [
                "accounts/:id"
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
            "description": "Returns the account with the specific id"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3a3cb33e-5e84-4068-aaab-abcac630ee37"
            }
          ]
        }
      ]
    }
  ]
}