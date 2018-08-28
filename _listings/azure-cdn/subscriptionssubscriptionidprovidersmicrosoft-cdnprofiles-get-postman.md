{
  "info": {
    "name": "Azure CDN API Profiles List",
    "_postman_id": "5280fe8d-1125-4360-be2e-6fe0f2820078",
    "description": "Lists all of the CDN profiles within an Azure subscription.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "cdn",
      "item": [
        {
          "id": "b3c05986-3100-4a48-9fa2-a8a949de7efb",
          "name": "Profiles_List",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/providers/Microsoft.Cdn/profiles"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "subscriptionId",
                  "value": "subscriptionId",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists all of the CDN profiles within an Azure subscription"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a4ef393c-2524-44e8-9675-6f8610131c0d"
            }
          ]
        }
      ]
    }
  ]
}