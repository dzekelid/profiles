{
  "info": {
    "name": "Azure CDN API Profiles Get",
    "_postman_id": "18d801b7-ffc8-46f1-abf7-c429c390e223",
    "description": "Gets a CDN profile with the specified profile name under the specified subscription and resource group.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "cdn",
      "item": [
        {
          "id": "5506676f-1c12-4b3f-b34a-fe65e4d6f94d",
          "name": "Profiles_Get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.Cdn/profiles/:profileName"
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
                  "id": "profileName",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "subscriptionId",
                  "value": "subscriptionId",
                  "type": "string"
                },
                {
                  "id": "resourceGroupName",
                  "value": "resourceGroupName",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets a CDN profile with the specified profile name under the specified subscription and resource group"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "33953999-805d-4f9b-9703-984da290bfc9"
            }
          ]
        }
      ]
    }
  ]
}