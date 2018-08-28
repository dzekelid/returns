{
  "info": {
    "name": "Capital One DevExchange Get all loans",
    "_postman_id": "8e8a55d0-ddc9-4327-b29b-9fd15f175e2b",
    "description": "Returns the loans that you are involved in.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "banks",
      "item": [
        {
          "id": "673b2104-01c6-4c14-ac10-088bdd9bd08b",
          "name": "returns-the-loans-that-you-are-involved-in",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.reimaginebanking.com",
              "path": [
                "accounts/:id/loans"
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
            "description": "Returns the loans that you are involved in"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "64050dc4-5d19-468a-bd8d-83e4d2d05d24"
            }
          ]
        }
      ]
    }
  ]
}