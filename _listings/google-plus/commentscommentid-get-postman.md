{
  "info": {
    "name": "Google Plus Get Comments",
    "_postman_id": "f94810a2-2321-42d1-8b99-59e9a6ee0aea",
    "description": "Get a comment.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Activity",
      "item": [
        {
          "id": "0653685f-b010-45fb-9da3-7fe8b77f463b",
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
              "id": "59d84ef8-2a46-4ee1-acf5-332ed8e03337"
            }
          ]
        },
        {
          "id": "33301e57-f816-47d1-b433-8103b1513d11",
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
              "id": "7788f4e5-8b71-47c2-bd35-a855d881e180"
            }
          ]
        }
      ]
    },
    {
      "name": "Comment",
      "item": [
        {
          "id": "578146f0-7dc2-4aeb-a256-e71865a73a2c",
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
              "id": "dc17f1a9-6877-4d62-be0c-e9c609840e52"
            }
          ]
        },
        {
          "id": "896421e5-c311-439a-90a7-a7773d01e090",
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
              "id": "bb7e3002-702b-40e1-b716-664389cc23c0"
            }
          ]
        }
      ]
    },
    {
      "name": "Person",
      "item": [
        {
          "id": "160f6bb6-76d0-43f6-8c55-37f6ced6f5a2",
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
              "id": "1f342ced-7f3e-4dba-a8b9-6c6101553890"
            }
          ]
        }
      ]
    }
  ]
}