{
  "info": {
    "name": "Dezrez Returns GeoAggregations of all searching groups",
    "_postman_id": "d99ec836-0a39-4344-ab22-9a1b677d46ad",
    "description": "Returns geoaggregations of all searching groups.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Returns",
      "item": [
        {
          "id": "9f6de2ec-cbfd-45e6-9671-26ac7f91d06a",
          "name": "Group_GeoAggregationByzoom",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.dezrez.com",
              "path": [
                "api/group/geoaggregation/:zoom"
              ],
              "variable": [
                {
                  "id": "zoom",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "header": [
              {
                "key": "Rezi-Api-Version",
                "value": "{}",
                "description": "Specifies which version of the API to call",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Returns geoaggregations of all searching groups."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9c2f4156-89b5-4367-bc5c-6b5f547a291d"
            }
          ]
        },
        {
          "id": "51a3a1ca-94ac-4f18-bcd8-7cbbbe7f36e7",
          "name": "Property_GeoAggregationByzoom",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.dezrez.com",
              "path": [
                "api/property/geoaggregation/:zoom"
              ],
              "variable": [
                {
                  "id": "zoom",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "header": [
              {
                "key": "Rezi-Api-Version",
                "value": "{}",
                "description": "Specifies which version of the API to call",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Returns geoaggregations of all properties."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "26d309e7-511a-463e-b833-e30ba1eb16cc"
            }
          ]
        }
      ]
    }
  ]
}