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
  /circles/{circleId}/people:
    put:
      summary: Update People in Circle
      description: Add a person to a circle
      operationId: plusDomains.circles.addPeople
      parameters:
      - in: path
        name: circleId
        description: The ID of the circle to add the person to
      - in: query
        name: email
        description: Email of the people to add to the circle
      - in: query
        name: userId
        description: IDs of the people to add to the circle
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