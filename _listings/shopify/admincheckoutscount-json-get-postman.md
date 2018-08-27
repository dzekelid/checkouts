{
  "info": {
    "name": "Shopify Get a count of checkouts",
    "_postman_id": "0f0711d5-386b-4670-a5cf-3d1cf9655ea8",
    "description": "Get a count of checkouts.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Commerce",
      "item": [
        {
          "id": "38a22b93-89a3-4561-b5d8-b6609def58a7",
          "name": "getAdminCheckouts.json",
          "request": {
            "url": "http://DefaultParameterValue:DefaultParameterValue@DefaultParameterValue.myshopify.com/admin/checkouts.json",
            "method": "GET",
            "header": [
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "",
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
            "description": "List all abandoned checkouts."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "20fe90d6-a28e-4c18-8f34-6867ce4b8557"
            }
          ]
        },
        {
          "id": "15c09291-6611-4d5b-8856-426e146cca20",
          "name": "getAdminCheckoutsCount.json",
          "request": {
            "url": "http://DefaultParameterValue:DefaultParameterValue@DefaultParameterValue.myshopify.com/admin/checkouts/count.json",
            "method": "GET",
            "header": [
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "",
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
            "description": "Get a count of checkouts."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "27becf06-d9d8-4822-bf86-8519b7715f49"
            }
          ]
        }
      ]
    }
  ]
}