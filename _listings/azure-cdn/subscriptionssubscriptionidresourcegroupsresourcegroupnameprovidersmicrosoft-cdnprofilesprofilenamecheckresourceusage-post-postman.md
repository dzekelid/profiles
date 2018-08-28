{
  "info": {
    "name": "Azure CDN API Profiles List Resource Usage",
    "_postman_id": "2a9a4e36-99f7-459d-9a48-07e397a76cee",
    "description": "Checks the quota and actual usage of endpoints under the given CDN profile.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "cdn",
      "item": [
        {
          "id": "b90851ee-d93e-49f6-b5e6-134670cf8050",
          "name": "Profiles_ListResourceUsage",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.Cdn/profiles/:profileName/checkResourceUsage"
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
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Checks the quota and actual usage of endpoints under the given CDN profile"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9a3f3a66-77d9-425a-8b30-aabeecff5caa"
            }
          ]
        }
      ]
    }
  ]
}