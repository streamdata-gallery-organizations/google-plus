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
  /people/{userId}/audiences:
    get:
      summary: Get Audience
      description: List all of the audiences to which a user can share
      operationId: plusDomains.audiences.list
      parameters:
      - in: query
        name: maxResults
        description: The maximum number of circles to include in the response, which
          is used for paging
      - in: query
        name: pageToken
        description: The continuation token, which is used to page through large result
          sets
      - in: path
        name: userId
        description: The ID of the user to get audiences for
      responses:
        200:
          description: OK
      tags:
      - audience
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