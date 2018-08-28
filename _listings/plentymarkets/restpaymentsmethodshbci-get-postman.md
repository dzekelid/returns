{
  "info": {
    "name": "Plentymarkets Returns the HBCI-Account count",
    "_postman_id": "4ff7ce1a-a826-4382-bef1-7f542180f9b1",
    "description": "Returns the hbci-account count.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Returns",
      "item": [
        {
          "id": "7e640513-377a-47ea-8edf-5bdbb07df97a",
          "name": "getRestPaymentsMethodsHbci",
          "request": {
            "url": "http://example.com/rest/payments/methods/hbci",
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
            "description": "Returns the hbci-account count."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "764ed1ae-be45-4238-b390-7ad08749edad"
            }
          ]
        }
      ]
    }
  ]
}