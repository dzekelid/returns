{
  "info": {
    "name": "Capital One DevExchange Get all bills for a specific account",
    "_postman_id": "49d54858-35ea-49f6-9094-1f891727912d",
    "description": "Returns the bills that are tied to the specific account.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "banks",
      "item": [
        {
          "id": "d296f83d-8d19-4d02-9fbe-a1aff0c22a8f",
          "name": "returns-the-bills-that-are-tied-to-the-specific-account",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.reimaginebanking.com",
              "path": [
                "accounts/:id/bills"
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
            "description": "Returns the bills that are tied to the specific account"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "df43dba1-1df9-494b-b7cb-5872b5db71c7"
            }
          ]
        }
      ]
    }
  ]
}