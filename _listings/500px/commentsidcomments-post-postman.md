{
  "info": {
    "name": "500px Post Comments Comments",
    "_postman_id": "62f8f36c-3c85-4e64-ad57-e43f3e19bee6",
    "description": "Creates a reply to an existing comment. Comments can only be nested one level deep, you cannot reply to a reply of a comment. If a comment has a non-null parent_id value then it cannot be replied to.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Blogs",
      "item": [
        {
          "id": "0f4a09ef-0c7c-401c-9b5c-c946ac66487d",
          "name": "getBlogs",
          "request": {
            "url": "http://api.500px.com/v1/blogs/?feature=%7B%7D&feature (required)=%7B%7D&page=%7B%7D&rpp=%7B%7D&user=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a listing of five recent stories (maximum 100 per page)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ffe818e0-1d0d-431e-9547-69a1adaee4d6"
            }
          ]
        },
        {
          "id": "0318e2ff-750f-41ae-9bba-e10004c6fad3",
          "name": "postBlogs",
          "request": {
            "url": "http://api.500px.com/v1/blogs/?body (required)=%7B%7D&latitude=%7B%7D&longitude=%7B%7D&photo_ids=%7B%7D&tags=%7B%7D&title (required)=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new Story."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "925b5006-9b12-4dfd-958d-84de75fe6983"
            }
          ]
        },
        {
          "id": "4042ad07-73ab-4bba-83d5-70995c6d67f6",
          "name": "getBlogs",
          "request": {
            "url": "http://api.500px.com/v1/blogs/:id?id (required) - Return information for the specific story.=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns detailed information of a single story."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d563c2a7-add9-47ba-9931-8b91a064cec5"
            }
          ]
        },
        {
          "id": "7210a01a-d05e-4f91-beb3-7007b3fc7d0d",
          "name": "putBlogs",
          "request": {
            "url": "http://api.500px.com/v1/blogs/:id?body=%7B%7D&id (required)=%7B%7D&latitude=%7B%7D&longitude=%7B%7D&photo_ids=%7B%7D&tags=%7B%7D&title=%7B%7D",
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Updates the Story."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7f002783-df0b-4a19-b1a2-6936a739dd7a"
            }
          ]
        },
        {
          "id": "f070dc44-c83f-4763-aa47-6a31addd0a8e",
          "name": "deleteBlogs",
          "request": {
            "url": "http://api.500px.com/v1/blogs/:id?id (required)=%7B%7D",
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the story."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "02648a40-7e0f-46df-b12a-9f67dfe924ec"
            }
          ]
        },
        {
          "id": "a7108ddf-86c1-45f1-88e5-7e56ef709d12",
          "name": "getBlogsComments",
          "request": {
            "url": "http://api.500px.com/v1/blogs/:id/comments?id (required)=%7B%7D&page=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a listing of twenty comments for a specific Story."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0604a79c-79d4-4652-8cdd-bcfed37b050b"
            }
          ]
        },
        {
          "id": "0a2aa4be-4b7a-452a-8df5-639f92a65ea1",
          "name": "postBlogsComments",
          "request": {
            "url": "http://api.500px.com/v1/blogs/:id/comments?body (required)=%7B%7D&id (required)=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a comment for the Story."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6b26bbb0-5298-4417-968b-cf654e566bf6"
            }
          ]
        }
      ]
    },
    {
      "name": "Collections",
      "item": [
        {
          "id": "889eb630-d1c7-480d-af0b-c05326e108aa",
          "name": "getCollections",
          "request": {
            "url": "http://api.500px.com/v1/collections?photos_per_collection_limit=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a listing of all Users collections and sets."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9f90d258-4f49-4a29-9949-6c47367b6cef"
            }
          ]
        },
        {
          "id": "c8ef99a5-cc4b-406e-a531-e09bd7eebfca",
          "name": "postCollections",
          "request": {
            "url": "http://api.500px.com/v1/collections?kind=%7B%7D&path=%7B%7D&path (required)=%7B%7D&photo_ids=%7B%7D&position=%7B%7D&title=%7B%7D&title (required)=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Creates new a collection."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d4f4ec88-1a98-44da-aae9-0829d41cd9bc"
            }
          ]
        },
        {
          "id": "825e64a5-72ee-4a5b-a5b3-51035f045a26",
          "name": "getCollections",
          "request": {
            "url": "http://api.500px.com/v1/collections/:id?image_size - Numerical size of the image to link to, 1 being the smallest and 4 being the largest. Multiple image sizes may be specified as image_size[]=2&amp;image_size[]=4.=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a collection."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bd47634c-6be0-44c3-9546-b0e5b508cf5c"
            }
          ]
        },
        {
          "id": "ae7b6d60-34d3-46a8-ba79-c2ae2ad9db52",
          "name": "putCollections",
          "request": {
            "url": "http://api.500px.com/v1/collections/:id?id (required)=%7B%7D&kind=%7B%7D&path=%7B%7D&photo_ids=%7B%7D&position=%7B%7D&title=%7B%7D",
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Updates collection."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f606d4eb-e627-43cf-82a8-5bafa8ba3e7c"
            }
          ]
        },
        {
          "id": "8b152ce4-d109-4666-9ab2-05dc38f74877",
          "name": "deleteCollections",
          "request": {
            "url": "http://api.500px.com/v1/collections/:id?Forkn      n      n        69=%7B%7D&Starn  nn    n      281=%7B%7D",
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes collection."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9fa522f2-ac66-44d9-87f9-ffff210c06c3"
            }
          ]
        }
      ]
    },
    {
      "name": "Comments",
      "item": [
        {
          "id": "7dcd5869-8d0d-4061-b11b-5ff71eee5be7",
          "name": "postCommentsComments",
          "request": {
            "url": "http://api.500px.com/v1/comments/:id/comments?body (required)=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a reply to an existing comment. Comments can only be nested one level deep, you cannot reply to a reply of a comment. If a comment has a non-null parent_id value then it cannot be replied to."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4a76f709-18eb-492b-92ba-0930159bfb8e"
            }
          ]
        }
      ]
    }
  ]
}