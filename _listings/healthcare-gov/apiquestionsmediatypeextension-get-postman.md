{
  "info": {
    "name": "HealthCare.gov Get Questions",
    "_postman_id": "baa72c37-007e-483b-ad2f-ca3ff4dcc54d",
    "description": "Returns pages content.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Articles",
      "item": [
        {
          "id": "b453aac1-3a29-4c11-98fb-565dce8a49aa",
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
              "id": "eabc500f-a0d9-40ca-ab28-ae02bffa80c4"
            }
          ]
        }
      ]
    },
    {
      "name": "Blog",
      "item": [
        {
          "id": "3b35b261-0ad6-42b5-9933-cf390cf714ae",
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
              "id": "6a1db9ef-3fab-4f14-a69d-7d3df3cc11c0"
            }
          ]
        }
      ]
    },
    {
      "name": "Glossary",
      "item": [
        {
          "id": "fdf77511-60a8-49c2-b628-cd4404a21ea2",
          "name": "getApiGlossaryMediatypeextension",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.healthcare.gov",
              "path": [
                "api/glossary:mediaTypeExtension"
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
              "id": "d929e7aa-f4e3-4b69-8491-53e0c11c1116"
            }
          ]
        }
      ]
    },
    {
      "name": "Questions",
      "item": [
        {
          "id": "2b9b737b-07a4-4796-80d8-a80369f2a5b3",
          "name": "getApiQuestionsMediatypeextension",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.healthcare.gov",
              "path": [
                "api/questions:mediaTypeExtension"
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
              "id": "3d4c47ae-fc10-4427-bcaf-7fc808b93338"
            }
          ]
        }
      ]
    }
  ]
}