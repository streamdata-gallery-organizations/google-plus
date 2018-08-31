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
  /people/{userId}:
    get:
      summary: Get Person Profile
      description: Get a person's profile
      operationId: plusDomains.people.get
      parameters:
      - in: path
        name: userId
        description: The ID of the person to get the profile for
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