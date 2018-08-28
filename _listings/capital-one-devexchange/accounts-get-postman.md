{
  "info": {
    "name": "Capital One DevExchange Get all accounts",
    "_postman_id": "71c15464-afb6-46e5-9547-c0b742db8e19",
    "description": "Returns the accounts that have been assigned to you.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "banks",
      "item": [
        {
          "id": "27391bb4-f403-46ab-9045-b01e1378a9b2",
          "name": "returns-the-accounts-that-have-been-assigned-to-you",
          "request": {
            "url": "http://api.reimaginebanking.com/accounts?type=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the accounts that have been assigned to you"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "00a9db3e-57c4-4648-8c31-95d892e439bc"
            }
          ]
        }
      ]
    }
  ]
}