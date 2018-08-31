---
swagger: "2.0"
x-collection-name: Google Plus
x-complete: 0
info:
  title: Google Plus Update Circle
  version: 1.0.0
  description: Update a circle's description.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /activities:
    get:
      summary: Get Activities
      description: Search public activities.
      operationId: plus.activities.search
      x-api-path-slug: activities-get
      parameters:
      - in: query
        name: language
        description: Specify the preferred language to search with
      - in: query
        name: maxResults
        description: The maximum number of activities to include in the response,
          which is used for paging
      - in: query
        name: orderBy
        description: Specifies how to order search results
      - in: query
        name: pageToken
        description: The continuation token, which is used to page through large result
          sets
      - in: query
        name: query
        description: Full-text search query string
      responses:
        200:
          description: OK
      tags:
      - Activity
  /activities/{activityId}:
    get:
      summary: Get Activity
      description: Get an activity.
      operationId: plusDomains.activities.get
      x-api-path-slug: activitiesactivityid-get
      parameters:
      - in: path
        name: activityId
        description: The ID of the activity to get
      responses:
        200:
          description: OK
      tags:
      - Activity
  /activities/{activityId}/comments:
    get:
      summary: Get Activity Commenets
      description: List all of the comments for an activity.
      operationId: plusDomains.comments.list
      x-api-path-slug: activitiesactivityidcomments-get
      parameters:
      - in: path
        name: activityId
        description: The ID of the activity to get comments for
      - in: query
        name: maxResults
        description: The maximum number of comments to include in the response, which
          is used for paging
      - in: query
        name: pageToken
        description: The continuation token, which is used to page through large result
          sets
      - in: query
        name: sortOrder
        description: The order in which to sort the list of comments
      responses:
        200:
          description: OK
      tags:
      - Activity
    post:
      summary: Create Activity Comment
      description: Create a new comment in reply to an activity.
      operationId: plusDomains.comments.insert
      x-api-path-slug: activitiesactivityidcomments-post
      parameters:
      - in: path
        name: activityId
        description: The ID of the activity to reply to
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Activity
  /activities/{activityId}/people/{collection}:
    get:
      summary: Get People In Collection
      description: List all of the people in the specified collection for a particular
        activity.
      operationId: plusDomains.people.listByActivity
      x-api-path-slug: activitiesactivityidpeoplecollection-get
      parameters:
      - in: path
        name: activityId
        description: The ID of the activity to get the list of people for
      - in: path
        name: collection
        description: The collection of people to list
      - in: query
        name: maxResults
        description: The maximum number of people to include in the response, which
          is used for paging
      - in: query
        name: pageToken
        description: The continuation token, which is used to page through large result
          sets
      responses:
        200:
          description: OK
      tags:
      - Person
  /comments/{commentId}:
    get:
      summary: Get Comments
      description: Get a comment.
      operationId: plus.comments.get
      x-api-path-slug: commentscommentid-get
      parameters:
      - in: path
        name: commentId
        description: The ID of the comment to get
      responses:
        200:
          description: OK
      tags:
      - Comment
  /people:
    get:
      summary: Get People
      description: Search all public profiles.
      operationId: plus.people.search
      x-api-path-slug: people-get
      parameters:
      - in: query
        name: language
        description: Specify the preferred language to search with
      - in: query
        name: maxResults
        description: The maximum number of people to include in the response, which
          is used for paging
      - in: query
        name: pageToken
        description: The continuation token, which is used to page through large result
          sets
      - in: query
        name: query
        description: Specify a query string for full text search of public text in
          all profiles
      responses:
        200:
          description: OK
      tags:
      - Person
  /people/{userId}:
    get:
      summary: Get Person
      description: Get a person's profile. If your app uses scope https://www.googleapis.com/auth/plus.login,
        this method is guaranteed to return ageRange and language.
      operationId: plus.people.get
      x-api-path-slug: peopleuserid-get
      parameters:
      - in: path
        name: userId
        description: The ID of the person to get the profile for
      responses:
        200:
          description: OK
      tags:
      - Person
  /people/{userId}/activities/{collection}:
    get:
      summary: Get Colelction Activities
      description: List all of the activities in the specified collection for a particular
        user.
      operationId: plus.activities.list
      x-api-path-slug: peopleuseridactivitiescollection-get
      parameters:
      - in: path
        name: collection
        description: The collection of activities to list
      - in: query
        name: maxResults
        description: The maximum number of activities to include in the response,
          which is used for paging
      - in: query
        name: pageToken
        description: The continuation token, which is used to page through large result
          sets
      - in: path
        name: userId
        description: The ID of the user to get activities for
      responses:
        200:
          description: OK
      tags:
      - Activity
  /people/{userId}/people/{collection}:
    get:
      summary: Get Collection of People
      description: List all of the people in the specified collection.
      operationId: plus.people.list
      x-api-path-slug: peopleuseridpeoplecollection-get
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
      - Person
  /circles/{circleId}:
    delete:
      summary: Delete Circle
      description: Delete a circle.
      operationId: plusDomains.circles.remove
      x-api-path-slug: circlescircleid-delete
      parameters:
      - in: path
        name: circleId
        description: The ID of the circle to delete
      responses:
        200:
          description: OK
      tags:
      - Circle
    get:
      summary: Get Circle
      description: Get a circle.
      operationId: plusDomains.circles.get
      x-api-path-slug: circlescircleid-get
      parameters:
      - in: path
        name: circleId
        description: The ID of the circle to get
      responses:
        200:
          description: OK
      tags:
      - Circle
    patch:
      summary: Update Circle
      description: Update a circle's description. This method supports patch semantics.
      operationId: plusDomains.circles.patch
      x-api-path-slug: circlescircleid-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: circleId
        description: The ID of the circle to update
      responses:
        200:
          description: OK
      tags:
      - Circle
    put:
      summary: Update Circle
      description: Update a circle's description.
      operationId: plusDomains.circles.update
      x-api-path-slug: circlescircleid-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: circleId
        description: The ID of the circle to update
      responses:
        200:
          description: OK
      tags:
      - Circle
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