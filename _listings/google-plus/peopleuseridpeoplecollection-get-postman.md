{
  "info": {
    "name": "Google Plus Get Collection of People",
    "_postman_id": "c26c8184-1905-4d14-93da-393a7c116610",
    "description": "List all of the people in the specified collection.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Activity",
      "item": [
        {
          "id": "796780eb-2f65-45c4-9a7d-c4dc2b4d062c",
          "name": "plus.activities.search",
          "request": {
            "url": "http://example.com/api/activities?language=%7B%7D&maxResults=%7B%7D&orderBy=%7B%7D&pageToken=%7B%7D&query=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Search public activities."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5f45b1af-6779-4acf-9b1a-0ab05b974c08"
            }
          ]
        },
        {
          "id": "83f56e67-f9a5-4c6e-811c-b092e2da97ed",
          "name": "plus.activities.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "api",
                "activities/:activityId"
              ],
              "variable": [
                {
                  "id": "activityId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get an activity."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a8ad2ebc-890f-4713-af6c-c1cfdeeec6b4"
            }
          ]
        },
        {
          "id": "8a38b9b2-11f0-4fc7-83c6-0c43b47f4b9e",
          "name": "plus.activities.list",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "api",
                "people/:userId/activities/:collection"
              ],
              "query": [
                {
                  "key": "maxResults",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "pageToken",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "collection",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "userId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List all of the activities in the specified collection for a particular user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6c523e20-44e5-4563-bbc5-b843170f08a3"
            }
          ]
        }
      ]
    },
    {
      "name": "Comment",
      "item": [
        {
          "id": "d66f30d8-dc38-4e7d-8c7d-fef10880bc20",
          "name": "plus.comments.list",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "api",
                "activities/:activityId/comments"
              ],
              "query": [
                {
                  "key": "maxResults",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "pageToken",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "sortOrder",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "activityId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List all of the comments for an activity."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7c549f34-89ff-4057-a748-97f23636f38c"
            }
          ]
        },
        {
          "id": "d4ab7e13-54ea-42ef-9df1-8f07032da135",
          "name": "plus.comments.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "api",
                "comments/:commentId"
              ],
              "variable": [
                {
                  "id": "commentId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a comment."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "02259f7f-e7f1-454f-889b-e76d5f4d7873"
            }
          ]
        }
      ]
    },
    {
      "name": "Person",
      "item": [
        {
          "id": "bcab50b5-03cc-4932-a523-47fcd244c387",
          "name": "plus.people.listByActivity",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "api",
                "activities/:activityId/people/:collection"
              ],
              "query": [
                {
                  "key": "maxResults",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "pageToken",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "activityId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "collection",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List all of the people in the specified collection for a particular activity."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "155b73ff-8eeb-4d2a-85c6-45563a6683fc"
            }
          ]
        },
        {
          "id": "8a36c9e4-729a-4982-a8e3-2a0bd644addd",
          "name": "plus.people.search",
          "request": {
            "url": "http://example.com/api/people?language=%7B%7D&maxResults=%7B%7D&pageToken=%7B%7D&query=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Search all public profiles."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "706006f7-4b9c-4929-bf69-f796bfc3bd85"
            }
          ]
        },
        {
          "id": "bbe38e7e-6fcf-45ea-94de-fe675443ae7e",
          "name": "plus.people.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "api",
                "people/:userId"
              ],
              "variable": [
                {
                  "id": "userId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a person's profile. If your app uses scope https://www.googleapis.com/auth/plus.login, this method is guaranteed to return ageRange and language."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c98b3a80-5f85-4a69-ba33-9a87c144707f"
            }
          ]
        },
        {
          "id": "9b805f57-77ee-4bd7-9712-b2f7ba83b023",
          "name": "plus.people.list",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "api",
                "people/:userId/people/:collection"
              ],
              "query": [
                {
                  "key": "maxResults",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "orderBy",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "pageToken",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "collection",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "userId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List all of the people in the specified collection."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b80cb48d-06b7-4a05-ad68-ea7c1c2703ed"
            }
          ]
        }
      ]
    }
  ]
}