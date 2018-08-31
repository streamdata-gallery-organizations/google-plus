{
  "info": {
    "name": "Google Plus Get Person",
    "_postman_id": "e9ef43cf-fe47-48b2-8e9e-78554eb8fe51",
    "description": "Get a person's profile. If your app uses scope https://www.googleapis.com/auth/plus.login, this method is guaranteed to return ageRange and language.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Activity",
      "item": [
        {
          "id": "4da1eb1b-a1ec-4545-b406-645d77ea4c4a",
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
              "id": "fa22dd8c-398e-45e8-9561-ef6613523195"
            }
          ]
        },
        {
          "id": "47eb0ebc-f4d9-4931-940d-4e9f53d40646",
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
              "id": "0ae62199-5e6e-4506-a2d6-8381abc0a72a"
            }
          ]
        }
      ]
    },
    {
      "name": "Comment",
      "item": [
        {
          "id": "a0f2322d-be75-44b6-a306-d1e7ae5a0c2f",
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
              "id": "bc3de757-5183-4523-8f18-9a2e8b167b2b"
            }
          ]
        },
        {
          "id": "1b3d7224-2aea-4151-94f7-f653a8aa7ed8",
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
              "id": "8122c50f-2ad5-4d0e-8f13-c7f1fa2b87a8"
            }
          ]
        }
      ]
    },
    {
      "name": "Person",
      "item": [
        {
          "id": "fc98bc53-e2d1-4a60-8f72-75d7afa7acda",
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
              "id": "6bac44e9-0c2b-4b79-8d2b-5eb10905117d"
            }
          ]
        },
        {
          "id": "d77af909-a1f8-445b-abc2-bebc13e9d97c",
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
              "id": "e46be7cd-c875-4e8d-931a-f46614fa1656"
            }
          ]
        },
        {
          "id": "be0b5ee4-5b51-4c3d-9383-6db43a0531f3",
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
              "id": "7eda55c8-94d4-4a18-a933-7bce72659ed3"
            }
          ]
        }
      ]
    }
  ]
}