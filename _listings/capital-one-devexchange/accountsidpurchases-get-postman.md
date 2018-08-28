{
  "info": {
    "name": "Capital One DevExchange Get all purchases",
    "_postman_id": "59d9a4f4-0049-4b27-83cd-d2f11816b200",
    "description": "Returns the purchases that you are involved in.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "banks",
      "item": [
        {
          "id": "d3efc950-7e83-4ac2-9ab5-15ef9f9a83d3",
          "name": "returns-the-purchases-that-you-are-involved-in",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.reimaginebanking.com",
              "path": [
                "accounts/:id/purchases"
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
            "description": "Returns the purchases that you are involved in"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "16a985a6-694a-4b09-9223-1849b3cb28b7"
            }
          ]
        }
      ]
    }
  ]
}