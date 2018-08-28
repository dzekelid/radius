{
  "info": {
    "name": "Dezrez Get historical prices within a radius of a location",
    "_postman_id": "f5f593dc-54f6-48d7-9bd5-053be8b3e448",
    "description": "Get historical prices within a radius of a location.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Historical",
      "item": [
        {
          "id": "a4e255b2-f758-4bc0-9884-681de9c70739",
          "name": "HistoricalPrice_GetByPropertyIdByidBypageNumberBypageSize",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.dezrez.com",
              "path": [
                "api/property/:id/historicalprices"
              ],
              "query": [
                {
                  "key": "pageNumber",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "pageSize",
                  "value": "%7B%7D",
                  "disabled": false
                }
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
            "description": "Get historical prices for a property by its id."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3562f8f1-a774-4229-9a7c-08cce2c1e395"
            }
          ]
        },
        {
          "id": "162212fe-c036-4ea9-81c2-615fb5530296",
          "name": "HistoricalPrice_GetByPostcodeBypostcodeBypropertyTypeBystyleTypeByleaseTypeBypageNumberBypageSize",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.dezrez.com",
              "path": [
                "api/property/historicalprices/postcode/:postcode"
              ],
              "query": [
                {
                  "key": "leaseType",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "pageNumber",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "pageSize",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "propertyType",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "styleType",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "postcode",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
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
            "description": "Get historical prices for a property by its id."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d4f61f15-f217-4cbf-aceb-6a5ee6245d38"
            }
          ]
        },
        {
          "id": "46835c93-f2a0-4d41-bbdd-e9f93d555886",
          "name": "HistoricalPrice_GetWithinRadiusOfLocationBypropertyIdBylatitudeBylongitudeBymileRadiusBypropertyType",
          "request": {
            "url": "http://api.dezrez.com/api/property/historicalprices/radius?latitude=%7B%7D&leaseType=%7B%7D&longitude=%7B%7D&mileRadius=%7B%7D&pageNumber=%7B%7D&pageSize=%7B%7D&propertyId=%7B%7D&propertyType=%7B%7D&styleType=%7B%7D",
            "method": "GET",
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
            "description": "Get historical prices within a radius of a location."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5822c378-e52c-481b-92ee-4e755facfd8a"
            }
          ]
        }
      ]
    }
  ]
}