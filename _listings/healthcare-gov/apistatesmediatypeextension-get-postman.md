{
  "info": {
    "name": "HealthCare.gov Get States",
    "_postman_id": "a81450e9-c8ec-4ef1-85f1-11b0013986b0",
    "description": "Returns pages content.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Articles",
      "item": [
        {
          "id": "726bd7e7-4171-4622-9672-12c79707b8d1",
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
              "id": "8e501cbe-d713-425a-ac8f-09641aa423d3"
            }
          ]
        }
      ]
    },
    {
      "name": "Blog",
      "item": [
        {
          "id": "74f3886b-41e6-4e13-8822-2bbbf5e21272",
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
              "id": "7a66342a-105d-4bec-977d-d752f2754a4e"
            }
          ]
        }
      ]
    },
    {
      "name": "Glossary",
      "item": [
        {
          "id": "b9927922-506e-4471-9199-1a50ee5138c9",
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
              "id": "e7f2087b-e92c-4d94-be8c-028ead5f1bf8"
            }
          ]
        }
      ]
    },
    {
      "name": "Questions",
      "item": [
        {
          "id": "c6481922-ff11-4225-893d-674e135f5ab8",
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
              "id": "64fa71ac-6045-40be-9799-e2fe61c155f2"
            }
          ]
        }
      ]
    },
    {
      "name": "States",
      "item": [
        {
          "id": "49a4374b-0a67-499b-bf66-0e160e5f7477",
          "name": "getApiStatesMediatypeextension",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.healthcare.gov",
              "path": [
                "api/states:mediaTypeExtension"
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
              "id": "67018d64-bbd0-4d05-b70e-897102bc9d99"
            }
          ]
        }
      ]
    }
  ]
}