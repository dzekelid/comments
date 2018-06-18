{
  "info": {
    "name": "500px Post Blogs Comments",
    "_postman_id": "ad372fa8-2944-4868-b724-15386ace10ff",
    "description": "Creates a comment for the Story.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Blogs",
      "item": [
        {
          "id": "09b1a06e-68df-4c83-9627-c1ee09314b4a",
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
              "id": "215e4285-96d7-4273-bc71-7eeeeb68b0ea"
            }
          ]
        },
        {
          "id": "88aa0de0-f9e0-432b-88ed-ba381a2a280f",
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
              "id": "3979bb23-0a05-419f-8488-722017d92a0f"
            }
          ]
        },
        {
          "id": "70829cf2-23cf-40fb-891e-5e288d20b4a0",
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
              "id": "e6c67ea7-4098-4755-8dd2-a527eeccf037"
            }
          ]
        },
        {
          "id": "8c66920b-f05d-41d1-a21c-c12b8821e987",
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
              "id": "62263ace-b8a8-4609-8c02-3257bbd2c447"
            }
          ]
        },
        {
          "id": "26261129-2e0c-496c-8cb1-df08c742b7b6",
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
              "id": "d6c21bc6-156a-45ea-b562-daec629daf65"
            }
          ]
        },
        {
          "id": "0af60110-42b0-44c7-9cd6-294ba85beeac",
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
              "id": "3ceb0a86-ab15-4b74-9ad3-5735f4a6cc1c"
            }
          ]
        },
        {
          "id": "2c688048-7c1e-43fe-afe7-947479b8d917",
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
              "id": "35fc9956-adcc-4326-972c-f9b59f45576a"
            }
          ]
        },
        {
          "id": "b194e889-db21-4389-97a6-f3f8d402d39c",
          "name": "getBlogs",
          "request": {
            "url": "http://api.500px.com/v1/blogs?feature=%7B%7D&page=%7B%7D&rpp=%7B%7D&username=%7B%7D&user_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a listing of five recent (blogs) stories (maximum 100 per page)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "58c951df-9a88-4041-81c1-a09d38fda67e"
            }
          ]
        },
        {
          "id": "da4d1282-aba7-4799-ad59-d83bcfb0f7e3",
          "name": "postBlogs",
          "request": {
            "url": "http://api.500px.com/v1/blogs?body=%7B%7D&latitude=%7B%7D&longitude=%7B%7D&photo_ids=%7B%7D&tags=%7B%7D&title=%7B%7D",
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
              "id": "8a3a6c74-ef2d-40fb-a6b0-3b31ecf04c1e"
            }
          ]
        },
        {
          "id": "a385a0ab-2680-4062-a2e1-2aca02e90234",
          "name": "getBlogs",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.500px.com",
              "path": [
                "v1",
                "blogs/:id"
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
              "id": "39408b4c-238d-413e-aeb4-4685f0af4cf6"
            }
          ]
        },
        {
          "id": "ce89e8d3-ac52-4d43-8d6a-83632077b77f",
          "name": "putBlogs",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.500px.com",
              "path": [
                "v1",
                "blogs/:id"
              ],
              "query": [
                {
                  "key": "body",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "latitude",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "longitude",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "photo_ids",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "tags",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "title",
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
            "method": "PUT",
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
              "id": "2f02f5ca-0b3d-4648-b2e0-2f28282423b6"
            }
          ]
        },
        {
          "id": "079457a7-6b07-4142-8a9c-2bdfcd94b44d",
          "name": "deleteBlogs",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.500px.com",
              "path": [
                "v1",
                "blogs/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
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
              "id": "fc092170-7b93-4827-b406-87bf354e45a5"
            }
          ]
        },
        {
          "id": "3ad3ab62-849c-44e7-8fc3-e1ca128058a4",
          "name": "getBlogsComments",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.500px.com",
              "path": [
                "v1",
                "blogs/:id/comments"
              ],
              "query": [
                {
                  "key": "page",
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
              "id": "19c8db93-2050-48bd-80f3-c161267d9269"
            }
          ]
        },
        {
          "id": "e4063332-6191-44ff-be52-4c83969c28ea",
          "name": "postBlogsComments",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.500px.com",
              "path": [
                "v1",
                "blogs/:id/comments"
              ],
              "query": [
                {
                  "key": "body",
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
              "id": "695508c2-bc6a-4a10-af33-34ba0229e7fa"
            }
          ]
        }
      ]
    },
    {
      "name": "Collections",
      "item": [
        {
          "id": "3515c72b-c9a3-4684-9394-0a02c098e175",
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
              "id": "b49c60a0-e9e0-4698-a364-af5d3db51619"
            }
          ]
        },
        {
          "id": "a2aed4c0-2424-4925-9c32-86f6c4874dee",
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
              "id": "462507e9-46a2-48a7-be90-d9cb695d12f9"
            }
          ]
        },
        {
          "id": "5633e885-0089-401e-b10c-9ef1517b02a3",
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
              "id": "2d134acd-e6b1-40c7-978a-0014ab9fabf2"
            }
          ]
        },
        {
          "id": "d5fc1fa5-d3a8-47f6-81e0-5cea138ab61f",
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
              "id": "f4080b48-186d-4a16-8355-8ae1751dcbca"
            }
          ]
        },
        {
          "id": "f8eea958-10bf-41c6-b7d0-a6a56f1cb3dc",
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
              "id": "d836ada0-fe8b-468a-91e6-bcf402d0f473"
            }
          ]
        }
      ]
    },
    {
      "name": "Comments",
      "item": [
        {
          "id": "8839954f-e2d5-4ef6-891f-8dca9e1f9e34",
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
              "id": "63917fb7-7a70-463c-9114-f8223f9f88df"
            }
          ]
        }
      ]
    },
    {
      "name": "Photos",
      "item": [
        {
          "id": "0ed88413-bea3-4ddd-8fbf-90d69ad208ab",
          "name": "getPhotos",
          "request": {
            "url": "http://api.500px.com/v1/photos?exclude=%7B%7D&feature=%7B%7D&image_size=%7B%7D&include_states=%7B%7D&include_store=%7B%7D&only=%7B%7D&page=%7B%7D&rpp=%7B%7D&sort=%7B%7D&sort_direction=%7B%7D&tags=%7B%7D&username=%7B%7D&user_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a listing of twenty (up to one hundred) photos for a specified photo stream."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e8fbbdbd-1945-4590-8b90-6ab83db2b9a7"
            }
          ]
        },
        {
          "id": "a7b3965d-6b54-41a0-8577-008af497ca6a",
          "name": "postPhotos",
          "request": {
            "url": "http://api.500px.com/v1/photos?aperture=%7B%7D&camera=%7B%7D&category=%7B%7D&description=%7B%7D&focal_length=%7B%7D&iso=%7B%7D&latitude=%7B%7D&lens=%7B%7D&longitude=%7B%7D&name=%7B%7D&privacy=%7B%7D&shutter_speed=%7B%7D&tags=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Create a new photo on behalf of the user, and receive an upload key in exchange."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9618d046-9135-4e18-96c7-8620ff919d64"
            }
          ]
        },
        {
          "id": "a06296c0-e4e4-4416-aed1-69c7aa42ff93",
          "name": "getPhotos",
          "request": {
            "url": "http://api.500px.com/v1/photos/:id?comments=%7B%7D&comments_page=%7B%7D&image_size=%7B%7D&tags=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns detailed information of a single photo."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a66a0106-3ebc-4df6-874d-d206430d7274"
            }
          ]
        },
        {
          "id": "493c2937-9482-4b1a-970e-63799ebfc0ab",
          "name": "putPhotos",
          "request": {
            "url": "http://api.500px.com/v1/photos/:id?add_tags: Comma-separated list of tags to add to this photos existing tags.=%7B%7D&aperture: Aperture value value for the photo, internally stored as string.=%7B%7D&camera: Make and model of the camera used to take this photo.=%7B%7D&category: Integer number of the category of the photo. See category mapping for exact values.=%7B%7D&crop: A hash containing keys x, x2, y, y2 and representing coordinates within which the thumbnail must be cropped. The crop is made using the top left corner as the origin. The points must be given relative to image size 4, an image of at most 900px=%7B%7D&description: Text description of the photo, up to 65535 characters in length.=%7B%7D&focal_length: Focal length value for the photo, internally stored as string.=%7B%7D&iso: Integer ISO value for the photo.=%7B%7D&latitude: Latitude of the location this photo was taken at represented by a decimal number.=%7B%7D&lens: Information about the lens used to take this photo.=%7B%7D&license_type: Integer number of the license type chosen for this photo. See license type mapping for exact values.=%7B%7D&longitude: Longitude of the location this photo was taken at represented by a decimal number.=%7B%7D&name: Title of the photo, up to 255 characters in length.=%7B%7D&nsfw: Boolean value indicating that the photo may contain not-safe-for-work content or content not suitable for minors.=%7B%7D&privacy: Integer value indicating that the photo should be shown (0) or hidden (1) on the users profile.=%7B%7D&remove_tags: Comma-separated list of tags to remove from this photos existing tags.=%7B%7D&shutter_speed: Shutter speed value for the photo, internally stored as string.=%7B%7D&tags: Comma-separated list of tags applicable to this photo.=%7B%7D",
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Allows the client application to update user-editable information on a photo.nnnResource URLnnhttps://api.500px.com/v1/photos/:idnnnnAuthenticationnnRequired; OAuth. The client application must use the OAuth access token issued for the owner of the photo to access this resouce.nnnParametersnnThe application must provide the ID of the photo to update in the URL of the request. The following parameters are recognized when included in the query string or POST body:nnnnname: Title of the photo, up to 255 characters in length.nndescription: Text description of the photo, up to 65535 characters in length.nncategory: Integer number of the category of the photo. See category mapping for exact values.nntags: Comma-separated list of tags applicable to this photo.nnadd_tags: Comma-separated list of tags to add to this photos existing tags.nnremove_tags: Comma-separated list of tags to remove from this photos existing tags.nnshutter_speed: Shutter speed value for the photo, internally stored as string.nnfocal_length: Focal length value for the photo, internally stored as string.nnaperture: Aperture value value for the photo, internally stored as string.nniso: Integer ISO value for the photo.nncamera: Make and model of the camera used to take this photo.nnlens: Information about the lens used to take this photo.nnlatitude: Latitude of the location this photo was taken at represented by a decimal number.nnlongitude: Longitude of the location this photo was taken at represented by a decimal number.nnnsfw: Boolean value indicating that the photo may contain not-safe-for-work content or content not suitable for minors.nnlicense_type: Integer number of the license type chosen for this photo. See license type mapping for exact values.nnprivacy: Integer value indicating that the photo should be shown (0) or hidden (1) on the users profile.nncrop: A hash containing keys x, x2, y, y2 and representing coordinates within which the thumbnail must be cropped. The crop is made using the top left corner as the origin. The points must be given relative to image size 4, an image of at most 900px on the larger side. The client application may skip this if the user does not wish to change photo thumbnail.nnnnImplementation detailsnnA parameter missing from the request will not be updated.  A parameter set to an empty string or null value will be interpreted as the user wishing to reset the value of the field to its default value.nnYou can use the add_tags and remove_tags parameters to manupulate a photos tags without having to send the complete list of tags in the request.nnnReturn formatnnA JSON object containing key photo, where photo is a Photo object in full format.nnnErrorsnnAll known errors cause the resource to return HTTP error code header together with a JSON array containing at least status and error keys describing the source of error.nnnn401: Invalid OAuth request: The request was refused because the OAuth signature is incorrect.nn404: Photo with ID not found: The photo ID provided is not known to the system.nn404: Photo with ID has been deleted: The photo has been deleted and can not be edited.nn404: Photo with ID belongs to a deactivated user: The photo belongs to a user that is no longer active and can not be edited.nn400: Bad photo category: An unrecognized photo category value has been provided.nn400: Bad license type: An unrecognized license type value has been provided."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8fb485ba-22c2-44aa-bed5-354fa82a35d3"
            }
          ]
        },
        {
          "id": "6710ff25-c802-49fe-90b6-a189f9cab204",
          "name": "deletePhotos",
          "request": {
            "url": "http://api.500px.com/v1/photos/:id?id (required)=%7B%7D",
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the photo from the Users library."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9b5c551a-3ac4-4564-9538-6d6d4814d26d"
            }
          ]
        },
        {
          "id": "e445a8f1-6770-4156-8e58-4e5bddb53367",
          "name": "getPhotosComments",
          "request": {
            "url": "http://api.500px.com/v1/photos/:id/comments?id (required)=%7B%7D&nested - Include this parameter to return the comments in nested format.=%7B%7D&page=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a listing of twenty comments for the photo."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3a69ccef-32fe-4bd8-b941-2d7f05cd7461"
            }
          ]
        },
        {
          "id": "dfdfcb6b-5058-46e4-8e2a-a3c18f44c78b",
          "name": "postPhotosComments",
          "request": {
            "url": "http://api.500px.com/v1/photos/:id/comments?body (required)=%7B%7D&id (required)=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new comment for the photo."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "215d2939-b7d7-4f9f-811e-4eed233e9c5d"
            }
          ]
        },
        {
          "id": "9387b6f3-30fe-4da6-92ac-5536eb13462f",
          "name": "postPhotosFavorite",
          "request": {
            "url": "http://api.500px.com/v1/photos/:id/favorite?id (required)=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Adds the photo to users list of favorites."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ab5d18d8-a943-4911-b16f-3553a4c0bd6f"
            }
          ]
        },
        {
          "id": "d1c7be85-7268-4a04-af35-5d4f27e7c80c",
          "name": "deletePhotosFavorite",
          "request": {
            "url": "http://api.500px.com/v1/photos/:id/favorite?id (required)=%7B%7D",
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Removes the photo to users list of favorites."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "693405ea-485f-4010-9344-0e71cc5df568"
            }
          ]
        },
        {
          "id": "7eed1e18-c1dc-48ed-b3d9-6e9c61a79f49",
          "name": "getPhotosFavorites",
          "request": {
            "url": "http://api.500px.com/v1/photos/:id/favorites?page=%7B%7D&rpp=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns all users that had favorite that photo."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "510cad80-2add-458b-a8e8-4358bc8b4023"
            }
          ]
        },
        {
          "id": "70c268af-8e9d-4cc1-95a3-0d34763a619b",
          "name": "postPhotosReport",
          "request": {
            "url": "http://api.500px.com/v1/photos/:id/report?id (required)=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Allows to report a photo."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cd59410f-040c-48e6-94ec-c9bb1269fb96"
            }
          ]
        },
        {
          "id": "599caf97-748a-46ed-9c3f-d237ee50990c",
          "name": "postPhotosTags",
          "request": {
            "url": "http://api.500px.com/v1/photos/:id/tags?id (required)=%7B%7D&tags (required)=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Adds tags to the photo. Accepts one or multiple coma separated tags."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7c7b672c-089c-48a0-979f-47c14654c31a"
            }
          ]
        },
        {
          "id": "9f3661d7-4584-43a1-9508-fb5be247e94e",
          "name": "deletePhotosTags",
          "request": {
            "url": "http://api.500px.com/v1/photos/:id/tags?id (required)=%7B%7D&tags (required)=%7B%7D",
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Removes tags from the photo. Accepts one or multiple coma separated tags."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "61751cf1-fb4e-4ca1-95ec-81f6c5f3d518"
            }
          ]
        },
        {
          "id": "32690567-282e-4dcb-87bf-a4a63710e7c3",
          "name": "postPhotosVote",
          "request": {
            "url": "http://api.500px.com/v1/photos/:id/vote?id (required)=%7B%7D&vote (required)=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Allows the user to vote for a photo."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f89ce422-9184-49f5-80a4-57c5e732c409"
            }
          ]
        },
        {
          "id": "4133ebab-915f-468f-92f4-97cb941a262a",
          "name": "getPhotosVotes",
          "request": {
            "url": "http://api.500px.com/v1/photos/:id/votes?page=%7B%7D&rpp=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns all users that had liked this photo."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5f7ffc8c-06f5-48a1-aadf-6457789f002e"
            }
          ]
        },
        {
          "id": "7200d5e7-9f85-4b21-bae3-2c4ebfb1a09f",
          "name": "getPhotosSearch",
          "request": {
            "url": "http://api.500px.com/v1/photos/search?comments_count u2014u00a0Sort by the number of comments, most commented first.=%7B%7D&created_at=%7B%7D&exclude=%7B%7D&favorites_count=%7B%7D&geo=%7B%7D&highest_rating=%7B%7D&image_size=%7B%7D&license_type -- Restrict the results to one or more license types.  Multiple types can be separated with a comma: license_type=1,4.=%7B%7D&only=%7B%7D&page=%7B%7D&rating=%7B%7D&rpp=%7B%7D&sort u2014u00a0Sort photos in the specified order. The following values are recognized:nnnn_score=%7B%7D&tag=%7B%7D&tags=%7B%7D&taken_at u2014u00a0Sort by the original date of the image extracted from metadata, most recent first (might not be available for all images).=%7B%7D&term=%7B%7D&times_viewed u2014u00a0Sort by the number of views, most viewed first.=%7B%7D&votes_count u2013 Sort by the number of votes, most voted on first.=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a listing of twenty (up to one hundred) photos from search results for a specified tag, keyword, or location."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c2f91b3f-4b8a-4978-8552-fad6b83f7f27"
            }
          ]
        },
        {
          "id": "ccb4a327-0b27-4427-869d-0c683162b3c3",
          "name": "postPhotosUpload",
          "request": {
            "url": "http://api.500px.com/v1/photos/upload?aperture=%7B%7D&camera=%7B%7D&category=%7B%7D&description=%7B%7D&file=%7B%7D&file (required)  - Photo filename in JPG/JPEG, passed along with multipart/form-data.=%7B%7D&focal_length=%7B%7D&iso=%7B%7D&latitude=%7B%7D&lens=%7B%7D&longitude=%7B%7D&name=%7B%7D&privacy=%7B%7D&shutter_speed=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "This is a new photo upload endpoint. It is currently in beta.nCreate a new photo on behalf of the user and upload a file.nfile parameter is passed in multipart/form-data, other parameters are passed as query parametrs or multipart/form-data."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ce657480-95cf-4228-9320-cb870ed58f2c"
            }
          ]
        },
        {
          "id": "6fdd6e09-01d0-443b-8ee2-0da899161e73",
          "name": "getPhotos",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.500px.com",
              "path": [
                "v1",
                "photos/:id"
              ],
              "query": [
                {
                  "key": "comments",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "comments_page",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "image_size",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "tags",
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
            "body": {
              "mode": "raw"
            },
            "description": "Returns detailed information of a single photo."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a7333d89-e4d9-499f-8d84-93ecfdd49ba8"
            }
          ]
        },
        {
          "id": "05f9adad-d059-4725-b73e-cc1723208f2f",
          "name": "putPhotos",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.500px.com",
              "path": [
                "v1",
                "photos/:id"
              ],
              "query": [
                {
                  "key": "description",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "name",
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
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Updates a photo."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e340d685-df23-4bd2-8362-37fa30240a92"
            }
          ]
        },
        {
          "id": "aed58b6e-932e-4405-8b64-a33a5223f592",
          "name": "deletePhotos",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.500px.com",
              "path": [
                "v1",
                "photos/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the photo from the User's library."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9bf1e476-959a-4a51-b27b-e0f5a4bb5aca"
            }
          ]
        },
        {
          "id": "2476eee1-f89c-4fac-a243-45a7ffc3dc2e",
          "name": "getPhotosComments",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.500px.com",
              "path": [
                "v1",
                "photos/:id/comments"
              ],
              "query": [
                {
                  "key": "page",
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
            "body": {
              "mode": "raw"
            },
            "description": "Returns a listing of twenty comments for the photo."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "78e5ab32-f024-4d04-86f2-30ebbcd4c46d"
            }
          ]
        },
        {
          "id": "a9622a89-3172-406e-ba9b-c1ef312d0eea",
          "name": "postPhotosComments",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.500px.com",
              "path": [
                "v1",
                "photos/:id/comments"
              ],
              "query": [
                {
                  "key": "body",
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
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new comment for the photo."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "79a362bd-1036-4429-949d-219530e61c8c"
            }
          ]
        },
        {
          "id": "27e46059-820b-4655-9b16-7258c0262c84",
          "name": "getPhotosFavorite",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.500px.com",
              "path": [
                "v1",
                "photos/:id/favorite"
              ],
              "query": [
                {
                  "key": "page",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "rpp",
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
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the photo from User's favorite list."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "869b880e-46ec-4346-9fe9-1922b7f75aa8"
            }
          ]
        },
        {
          "id": "7fa152ac-8597-4123-aefb-75fc7c3cf0fa",
          "name": "postPhotosFavorite",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.500px.com",
              "path": [
                "v1",
                "photos/:id/favorite"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Adds the photo to user's list of favorites."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "933ceef5-703f-4ff9-8860-a2cbac86d69b"
            }
          ]
        },
        {
          "id": "a2813130-e69f-464f-aafb-d690de6c3371",
          "name": "deletePhotosFavorite",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.500px.com",
              "path": [
                "v1",
                "photos/:id/favorite"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Removes the photo to user's list of favorites."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fad1ecc4-5583-47ed-b5bd-b5cd41feaf81"
            }
          ]
        },
        {
          "id": "f08ff1a8-43bb-4fae-9198-857dcb8b3181",
          "name": "getPhotosVotes",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.500px.com",
              "path": [
                "v1",
                "photos/:id/votes"
              ],
              "query": [
                {
                  "key": "page",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "rpp",
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
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the photo from User's favorite list."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c1be31b1-18e8-403b-ad72-d2933723179a"
            }
          ]
        },
        {
          "id": "12568623-10d3-4b68-a8b4-1a9ffde13b58",
          "name": "postPhotosVote",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.500px.com",
              "path": [
                "v1",
                "photos/:id/vote"
              ],
              "query": [
                {
                  "key": "vote",
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
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Allows the user to vote for a photo."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "85d959b1-bc1f-4438-b25e-a72581a57c74"
            }
          ]
        },
        {
          "id": "55349f42-8811-444f-864b-f7efe65d518d",
          "name": "postPhotosTags",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.500px.com",
              "path": [
                "v1",
                "photos/:id/tags"
              ],
              "query": [
                {
                  "key": "tags",
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
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Adds tags to the photo. Accepts one or multiple coma separated tags."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c70639ae-bcef-45d9-a1a7-2143438f5f23"
            }
          ]
        },
        {
          "id": "9f48384a-4143-4d5d-bdb0-7538eadc1f4d",
          "name": "deletePhotosTags",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.500px.com",
              "path": [
                "v1",
                "photos/:id/tags"
              ],
              "query": [
                {
                  "key": "tags",
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
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Removes tags from the photo. Accepts one or multiple coma separated tags."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dbf949cb-5bda-44cd-a4d9-342bcf4dd408"
            }
          ]
        }
      ]
    },
    {
      "name": "Upload",
      "item": [
        {
          "id": "e8427503-4ceb-4fb5-a3e9-d874d9c8dbae",
          "name": "postUpload",
          "request": {
            "url": "http://api.500px.com/v1/upload?access_key=%7B%7D&consumer_key=%7B%7D&file=%7B%7D&photo_id=%7B%7D&upload_key=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Allows an application to upload the photo file.nnNote that this endpoint is at the upload.500px.com domain, not the api.500px.com domain."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "50a5c823-5b39-4c05-88a7-e46eca077037"
            }
          ]
        }
      ]
    },
    {
      "name": "Users",
      "item": [
        {
          "id": "22f242b3-d339-4d02-89aa-fbee98bc3c6e",
          "name": "getUsers",
          "request": {
            "url": "http://api.500px.com/v1/users",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the profile information for the current user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0958e769-f0f4-4872-a0cc-cf50b4bd1295"
            }
          ]
        },
        {
          "id": "4f7f2efa-ac4a-494e-87a9-26343cd4dbb6",
          "name": "getUsersFollowers",
          "request": {
            "url": "http://api.500px.com/v1/users/:id/followers?id (required)=%7B%7D&page=%7B%7D&rpp=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of users who follow the specified user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c6a4a1e5-1642-46c2-8403-28cda8c683df"
            }
          ]
        },
        {
          "id": "d202ef80-1326-4b83-9cdd-0dd58c6f8883",
          "name": "getUsersFriends",
          "request": {
            "url": "http://api.500px.com/v1/users/:id/friends?id (required)=%7B%7D&page=%7B%7D&rpp=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of friends for the specified user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f685e0cd-fb64-4027-9ff2-c9ce6053f007"
            }
          ]
        },
        {
          "id": "b09da1a7-9de9-4fac-8e5e-06ed5c976d53",
          "name": "postUsersFriends",
          "request": {
            "url": "http://api.500px.com/v1/users/:id/friends?id (required)=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Add the user to the list of followers."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cd5959d9-1261-4d6b-a5ce-c3ea33b4b469"
            }
          ]
        },
        {
          "id": "b1ab012f-b5b3-4591-b40c-1e8f2403fd8a",
          "name": "deleteUsersFriends",
          "request": {
            "url": "http://api.500px.com/v1/users/:id/friends?id (required)=%7B%7D",
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Removes the user from the list of followers."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f468985e-a4a5-4cb1-8b8a-dd3598da7010"
            }
          ]
        },
        {
          "id": "d9b2948d-dbb3-4c89-bfcf-f75690f9eac2",
          "name": "getUsersSearch",
          "request": {
            "url": "http://api.500px.com/v1/users/search?page=%7B%7D&rpp=%7B%7D&term=%7B%7D&term (required)=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Return listing of ten (up to one hundred) users from search results for a specified search term."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6dc862c4-96b6-4d32-873f-e2ff33b61e65"
            }
          ]
        },
        {
          "id": "a5d92c57-e1e6-4275-b990-a475f151090c",
          "name": "getUsersShow",
          "request": {
            "url": "http://api.500px.com/v1/users/show?email=%7B%7D&id=%7B%7D&username=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the profile information for a specified user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "99054290-1548-421e-9df8-bf655406791c"
            }
          ]
        },
        {
          "id": "8f63ae3c-d043-40f6-939d-1adcf0ef276b",
          "name": "getUsersFriends",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.500px.com",
              "path": [
                "v1",
                "users/:id/friends"
              ],
              "query": [
                {
                  "key": "page",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "rpp",
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
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of friends for the specified user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dc587caf-72eb-48d7-88ca-f33f3f57dca5"
            }
          ]
        },
        {
          "id": "013c23b8-1111-4c4e-922d-f7b5464583da",
          "name": "postUsersFriends",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.500px.com",
              "path": [
                "v1",
                "users/:id/friends"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Add the user to the list of followers."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d89291a7-a8fa-49b2-b4db-53ed1b0f64dd"
            }
          ]
        },
        {
          "id": "712a76ba-052e-40f0-93b6-305f984689bf",
          "name": "deleteUsersFriends",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.500px.com",
              "path": [
                "v1",
                "users/:id/friends"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Removes the user from the list of followers."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e9481a02-1026-4a56-8c97-4b462eaff907"
            }
          ]
        },
        {
          "id": "c717d744-f1d9-40d0-b46f-a87d08f745cb",
          "name": "getUsersFollowers",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.500px.com",
              "path": [
                "v1",
                "users/:id/followers"
              ],
              "query": [
                {
                  "key": "page",
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
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of users who follow the specified user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cd57e77e-dced-40e1-90b7-10d5d351710d"
            }
          ]
        }
      ]
    }
  ]
}