---
swagger: "2.0"
info:
  title: Google Plus
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /people/{userId}/people/{collection}:
    get:
      summary: Get People In Collection
      description: List all of the people in the specified collection
      operationId: plusDomains.people.list
      parameters:
      - in: path
        name: collection
        description: The collection of people to list
      - in: query
        name: maxResults
        description: The maximum number of people to include in the response, which
          is used for paging
      - in: query
        name: orderBy
        description: The order to return people in
      - in: query
        name: pageToken
        description: The continuation token, which is used to page through large result
          sets
      - in: path
        name: userId
        description: Get the collection of people for the person identified
      responses:
        200:
          description: OK
      tags:
      - person
definitions: []
x-collection-name: Google Plus
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---