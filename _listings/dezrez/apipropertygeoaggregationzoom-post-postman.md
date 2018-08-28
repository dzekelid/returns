{
  "info": {
    "name": "Dezrez Returns GeoAggregations of all properties",
    "_postman_id": "0f53156f-e4f4-4d47-8fc9-df680214d029",
    "description": "Returns geoaggregations of all properties.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Returns",
      "item": [
        {
          "id": "16ef31cb-d2cf-49cd-aee3-7307084136e0",
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
              "id": "a7945de6-70e5-40fa-8667-27e65e89bfe6"
            }
          ]
        },
        {
          "id": "165ef518-1875-4f8f-90b8-4cedee4a371b",
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
              "id": "8b6e6591-8ee8-4969-a4ed-8f8ea3cb8a82"
            }
          ]
        }
      ]
    }
  ]
}