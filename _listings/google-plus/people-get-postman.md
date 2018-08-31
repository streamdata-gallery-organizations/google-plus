{
  "info": {
    "name": "Google Plus Get People",
    "_postman_id": "9b1bf8d8-bfd8-4e37-8d69-f9a15b3ce386",
    "description": "Search all public profiles.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Activity",
      "item": [
        {
          "id": "d9c056c9-7d25-40d7-8774-a64af6c6e3ba",
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
              "id": "c0de935c-ecd6-4fbc-9eea-6fd71df42e30"
            }
          ]
        },
        {
          "id": "2167a6be-0653-4197-a8e7-bb1204ea8aa9",
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
              "id": "44a4c381-6482-4b04-a448-5160e38a75f6"
            }
          ]
        }
      ]
    },
    {
      "name": "Comment",
      "item": [
        {
          "id": "4fab38e8-e42d-43eb-a245-11bdc09d3016",
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
              "id": "44fe0f8a-9743-46e5-a1b0-bd18e60a2911"
            }
          ]
        },
        {
          "id": "1f588c66-47c7-4eda-9ece-4303607e6da7",
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
              "id": "85024b18-7e07-406d-962f-ba126a6b515d"
            }
          ]
        }
      ]
    },
    {
      "name": "Person",
      "item": [
        {
          "id": "c1b0674a-f858-4559-b641-6e4444fabf3e",
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
              "id": "71aee453-294e-4607-9d40-7f7247327975"
            }
          ]
        },
        {
          "id": "71e1566d-22e7-4d18-a594-f8fc6d4044e3",
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
              "id": "ad451966-394d-451d-8fb1-f47158b1f1f7"
            }
          ]
        }
      ]
    }
  ]
}