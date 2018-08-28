{
  "info": {
    "name": "HealthCare.gov Get Blog",
    "_postman_id": "bab2bab3-4bd5-4ffc-8a0d-2b74df8e8671",
    "description": "Returns pages content.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Articles",
      "item": [
        {
          "id": "2a767096-c3d9-4696-a76c-d626bd08c6aa",
          "name": "getApiArticlesMediatypeextension",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.healthcare.gov",
              "path": [
                "api/articles:mediaTypeExtension"
              ],
              "variable": [
                {
                  "id": "mediaTypeExtension",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns pages content."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "acdfa840-7650-462d-9291-f0a2c3c7f4b6"
            }
          ]
        }
      ]
    },
    {
      "name": "Blog",
      "item": [
        {
          "id": "85f6a2e7-43ee-48fd-a54f-182d6650c4d8",
          "name": "getApiBlogMediatypeextension",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.healthcare.gov",
              "path": [
                "api/blog:mediaTypeExtension"
              ],
              "variable": [
                {
                  "id": "mediaTypeExtension",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns pages content."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5dcc829e-b112-46e4-8910-25a5a4fd09ca"
            }
          ]
        }
      ]
    }
  ]
}