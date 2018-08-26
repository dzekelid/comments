{
  "info": {
    "name": "Shopify Get a count of all comments",
    "_postman_id": "5a9e82ac-21a9-4332-b07c-112165b15e45",
    "description": "Get a count of all comments.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Commerce",
      "item": [
        {
          "id": "4eee2605-6c7f-4150-9167-c598fc08371d",
          "name": "getAdminComments.json",
          "request": {
            "url": "http://DefaultParameterValue:DefaultParameterValue@DefaultParameterValue.myshopify.com/admin/comments.json",
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
            "description": "Get a list of all comments."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9b4fae59-29c9-4ac6-8405-4865c3771d9a"
            }
          ]
        },
        {
          "id": "51a549a4-8866-48e9-b2d2-f5ab1ea9720e",
          "name": "getAdminCommentsCount.json",
          "request": {
            "url": "http://DefaultParameterValue:DefaultParameterValue@DefaultParameterValue.myshopify.com/admin/comments/count.json",
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
            "description": "Get a count of all comments."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bcab9335-7cfe-4f55-8b87-e7072cb6bc59"
            }
          ]
        }
      ]
    }
  ]
}