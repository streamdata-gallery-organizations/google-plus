{
  "info": {
    "name": "Google Plus Get Activity Commenets",
    "_postman_id": "67563586-9e64-4393-83bc-5ae4fd702011",
    "description": "List all of the comments for an activity.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Activity",
      "item": [
        {
          "id": "f03056dc-4e70-46c8-bc35-dd3090167b9a",
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
              "id": "cae7c8c0-7a57-4ee4-bcbc-e216da13e887"
            }
          ]
        },
        {
          "id": "e5acc025-5a50-4732-a531-1775e746b993",
          "name": "plusDomains.activities.get",
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
              "id": "372bab4d-679c-4497-9cd6-4f66949a325e"
            }
          ]
        },
        {
          "id": "c193dc02-2df6-40bd-b359-cc8943c68c00",
          "name": "plusDomains.comments.list",
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
              "id": "215c4e39-d7f9-4565-8191-4047af02f21a"
            }
          ]
        },
        {
          "id": "a5c45939-80f9-49e7-924a-d22f963ca5eb",
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
              "id": "cdac2245-48f3-4fd6-9400-559f940c00c8"
            }
          ]
        }
      ]
    },
    {
      "name": "Person",
      "item": [
        {
          "id": "f13cf061-b6af-4ad3-87fc-30b7d42b390c",
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
              "id": "ef502e04-2666-4320-8afc-08acdc982915"
            }
          ]
        },
        {
          "id": "4e4dc8ea-167f-43b0-adb1-18053f1459a7",
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
              "id": "aa29230e-e1a7-4541-bae7-1926d7db2846"
            }
          ]
        },
        {
          "id": "beb3d43f-baed-479b-a90a-11e17f252599",
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
              "id": "9f876d84-dd0a-474a-bcae-c1ae5281f425"
            }
          ]
        },
        {
          "id": "d3aee078-3f69-4b73-809d-4854585b1196",
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
              "id": "8adaa25d-6c9d-41f1-aecf-460d77f281ee"
            }
          ]
        }
      ]
    },
    {
      "name": "Comment",
      "item": [
        {
          "id": "97d8ccc9-5206-4813-80ea-b6fdd7f507eb",
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
              "id": "34421cd8-36ad-49bf-9526-c4fdd0514862"
            }
          ]
        }
      ]
    }
  ]
}