---
name: Google Plus
x-slug: google-plus
description: Create a more engaging experience and connect with more users by integrating
  social into your web site. Show profile information, and relevant content and connections
  from circles. Let visitors recommend and share your content, and prompt friends
  to take specific actions on your site.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-plus.png
x-kinRank: "9"
x-alexaRank: ""
tags: Google Plus
created: "2018-05-21"
modified: "2018-05-21"
url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-plus/master/_listings/google-plus/apis.md
specificationVersion: "0.14"
apis:
- name: Google Plus Get Activities
  x-api-slug: google-plus
  description: Search public activities.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-plus.png
  humanURL: https://plus.google.com/
  baseURL: https://///activities
  tags: Activity
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-plus/master/_listings/google-plus/activities-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-plus/master/_listings/google-plus/activities-get-openapi.md
- name: Google Plus Get Activity
  x-api-slug: google-plus
  description: Get an activity.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-plus.png
  humanURL: https://plus.google.com/
  baseURL: https://///activities/{activityId}
  tags: Activity
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-plus/master/_listings/google-plus/activitiesactivityid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-plus/master/_listings/google-plus/activitiesactivityid-get-openapi.md
- name: Google Plus Get Activity Comments
  x-api-slug: google-plus
  description: List all of the comments for an activity.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-plus.png
  humanURL: https://plus.google.com/
  baseURL: https://///activities/{activityId}/comments
  tags: Comment
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-plus/master/_listings/google-plus/activitiesactivityidcomments-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-plus/master/_listings/google-plus/activitiesactivityidcomments-get-openapi.md
- name: Google Plus Get Activity People
  x-api-slug: google-plus
  description: List all of the people in the specified collection for a particular
    activity.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-plus.png
  humanURL: https://plus.google.com/
  baseURL: https://///activities/{activityId}/people/{collection}
  tags: Person
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-plus/master/_listings/google-plus/activitiesactivityidpeoplecollection-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-plus/master/_listings/google-plus/activitiesactivityidpeoplecollection-get-openapi.md
- name: Google Plus Get Comments
  x-api-slug: google-plus
  description: Get a comment.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-plus.png
  humanURL: https://plus.google.com/
  baseURL: https://///comments/{commentId}
  tags: Comment
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-plus/master/_listings/google-plus/commentscommentid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-plus/master/_listings/google-plus/commentscommentid-get-openapi.md
- name: Google Plus Get People
  x-api-slug: google-plus
  description: Search all public profiles.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-plus.png
  humanURL: https://plus.google.com/
  baseURL: https://///people
  tags: Person
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-plus/master/_listings/google-plus/people-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-plus/master/_listings/google-plus/people-get-openapi.md
- name: Google Plus Get Person
  x-api-slug: google-plus
  description: Get a person's profile. If your app uses scope https://www.googleapis.com/auth/plus.login,
    this method is guaranteed to return ageRange and language.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-plus.png
  humanURL: https://plus.google.com/
  baseURL: https://///people/{userId}
  tags: Person
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-plus/master/_listings/google-plus/peopleuserid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-plus/master/_listings/google-plus/peopleuserid-get-openapi.md
- name: Google Plus Get Colelction Activities
  x-api-slug: google-plus
  description: List all of the activities in the specified collection for a particular
    user.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-plus.png
  humanURL: https://plus.google.com/
  baseURL: https://///people/{userId}/activities/{collection}
  tags: Activity
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-plus/master/_listings/google-plus/peopleuseridactivitiescollection-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-plus/master/_listings/google-plus/peopleuseridactivitiescollection-get-openapi.md
- name: Google Plus Get Collection of People
  x-api-slug: google-plus
  description: List all of the people in the specified collection.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-plus.png
  humanURL: https://plus.google.com/
  baseURL: https://///people/{userId}/people/{collection}
  tags: Person
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-plus/master/_listings/google-plus/peopleuseridpeoplecollection-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-plus/master/_listings/google-plus/peopleuseridpeoplecollection-get-openapi.md
- name: Google Plus Get Activity
  x-api-slug: google-plus
  description: Get an activity.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-plus.png
  humanURL: https://plus.google.com/
  baseURL: https://///activities/{activityId}
  tags: Activity
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-plus/master/_listings/google-plus/activitiesactivityid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-plus/master/_listings/google-plus/activitiesactivityid-get-openapi.md
- name: Google Plus Get Activity Commenets
  x-api-slug: google-plus
  description: List all of the comments for an activity.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-plus.png
  humanURL: https://plus.google.com/
  baseURL: https://///activities/{activityId}/comments
  tags: Activity
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-plus/master/_listings/google-plus/activitiesactivityidcomments-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-plus/master/_listings/google-plus/activitiesactivityidcomments-get-openapi.md
- name: Google Plus Create Activity Comment
  x-api-slug: google-plus
  description: Create a new comment in reply to an activity.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-plus.png
  humanURL: https://plus.google.com/
  baseURL: https://///activities/{activityId}/comments
  tags: Activity
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-plus/master/_listings/google-plus/activitiesactivityidcomments-post-openapi.md
- name: Google Plus Get People In Collection
  x-api-slug: google-plus
  description: List all of the people in the specified collection for a particular
    activity.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-plus.png
  humanURL: https://plus.google.com/
  baseURL: https://///activities/{activityId}/people/{collection}
  tags: Person
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-plus/master/_listings/google-plus/activitiesactivityidpeoplecollection-get-openapi.md
- name: Google Plus Delete Circle
  x-api-slug: google-plus
  description: Delete a circle.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-plus.png
  humanURL: https://plus.google.com/
  baseURL: https://///circles/{circleId}
  tags: Circle
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-plus/master/_listings/google-plus/circlescircleid-delete-openapi.md
- name: Google Plus Get Circle
  x-api-slug: google-plus
  description: Get a circle.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-plus.png
  humanURL: https://plus.google.com/
  baseURL: https://///circles/{circleId}
  tags: Circle
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-plus/master/_listings/google-plus/circlescircleid-get-openapi.md
- name: Google Plus Update Circle
  x-api-slug: google-plus
  description: Update a circle's description. This method supports patch semantics.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-plus.png
  humanURL: https://plus.google.com/
  baseURL: https://///circles/{circleId}
  tags: Circle
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-plus/master/_listings/google-plus/circlescircleid-patch-openapi.md
- name: Google Plus Update Circle
  x-api-slug: google-plus
  description: Update a circle's description.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-plus.png
  humanURL: https://plus.google.com/
  baseURL: https://///circles/{circleId}
  tags: Circle
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-plus/master/_listings/google-plus/circlescircleid-put-openapi.md
- name: Google Plus Delete Circle
  x-api-slug: google-plus
  description: Remove a person from a circle.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-plus.png
  humanURL: https://plus.google.com/
  baseURL: https://///circles/{circleId}/people
  tags: Circle
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-plus/master/_listings/google-plus/circlescircleidpeople-delete-openapi.md
- name: Google Plus Get People in Circle
  x-api-slug: google-plus
  description: List all of the people who are members of a circle.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-plus.png
  humanURL: https://plus.google.com/
  baseURL: https://///circles/{circleId}/people
  tags: Person
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-plus/master/_listings/google-plus/circlescircleidpeople-get-openapi.md
- name: Google Plus Update People in Circle
  x-api-slug: google-plus
  description: Add a person to a circle. Google+ limits certain circle operations,
    including the number of circle adds. Learn More.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-plus.png
  humanURL: https://plus.google.com/
  baseURL: https://///circles/{circleId}/people
  tags: Person
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-plus/master/_listings/google-plus/circlescircleidpeople-put-openapi.md
- name: Google Plus Get Comment
  x-api-slug: google-plus
  description: Get a comment.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-plus.png
  humanURL: https://plus.google.com/
  baseURL: https://///comments/{commentId}
  tags: Comment
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-plus/master/_listings/google-plus/commentscommentid-get-openapi.md
- name: Google Plus Get Person Profile
  x-api-slug: google-plus
  description: Get a person's profile.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-plus.png
  humanURL: https://plus.google.com/
  baseURL: https://///people/{userId}
  tags: Person
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-plus/master/_listings/google-plus/peopleuserid-get-openapi.md
- name: Google Plus Create Activity
  x-api-slug: google-plus
  description: Create a new activity for the authenticated user.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-plus.png
  humanURL: https://plus.google.com/
  baseURL: https://///people/{userId}/activities
  tags: Activity
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-plus/master/_listings/google-plus/peopleuseridactivities-post-openapi.md
- name: Google Plus Get Activities
  x-api-slug: google-plus
  description: List all of the activities in the specified collection for a particular
    user.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-plus.png
  humanURL: https://plus.google.com/
  baseURL: https://///people/{userId}/activities/{collection}
  tags: Activity
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-plus/master/_listings/google-plus/peopleuseridactivitiescollection-get-openapi.md
- name: Google Plus Get Audience
  x-api-slug: google-plus
  description: List all of the audiences to which a user can share.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-plus.png
  humanURL: https://plus.google.com/
  baseURL: https://///people/{userId}/audiences
  tags: Audience
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-plus/master/_listings/google-plus/peopleuseridaudiences-get-openapi.md
- name: Google Plus Get Circles
  x-api-slug: google-plus
  description: List all of the circles for a user.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-plus.png
  humanURL: https://plus.google.com/
  baseURL: https://///people/{userId}/circles
  tags: Circle
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-plus/master/_listings/google-plus/peopleuseridcircles-get-openapi.md
- name: Google Plus Create New Circle
  x-api-slug: google-plus
  description: Create a new circle for the authenticated user.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-plus.png
  humanURL: https://plus.google.com/
  baseURL: https://///people/{userId}/circles
  tags: Circle
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-plus/master/_listings/google-plus/peopleuseridcircles-post-openapi.md
- name: Google Plus Add Media To Collection
  x-api-slug: google-plus
  description: Add a new media item to an album. The current upload size limitations
    are 36MB for a photo and 1GB for a video. Uploads do not count against quota if
    photos are less than 2048 pixels on their longest side or videos are less than
    15 minutes in length.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-plus.png
  humanURL: https://plus.google.com/
  baseURL: https://///people/{userId}/media/{collection}
  tags: Media
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-plus/master/_listings/google-plus/peopleuseridmediacollection-post-openapi.md
- name: Google Plus Get People In Collection
  x-api-slug: google-plus
  description: List all of the people in the specified collection.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-plus.png
  humanURL: https://plus.google.com/
  baseURL: https://///people/{userId}/people/{collection}
  tags: Person
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-plus/master/_listings/google-plus/peopleuseridpeoplecollection-get-openapi.md
- name: Google Plus
  x-api-slug: google-plus
  description: Create a more engaging experience and connect with more users by integrating
    social into your web site. Show profile information, and relevant content and
    connections from circles. Let visitors recommend and share your content, and prompt
    friends to take specific actions on your site.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-plus.png
  humanURL: https://plus.google.com/
  baseURL: https:///
  tags: Google Plus
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-plus/master/_listings/google-plus/openapi.md
x-common:
- type: x-badges
  url: https://developers.google.com/+/web/badge/
- type: x-buttons
  url: https://developers.google.com/+/web/+1button/
- type: x-change-log
  url: https://developers.google.com/+/web/release-notes
- type: x-code
  url: https://developers.google.com/+/web/samples/javascript
- type: x-developer
  url: https://developers.google.com/+/web/api/rest/
- type: x-documentation
  url: https://developers.google.com/+/web/api/rest/latest/
- type: x-issues
  url: https://code.google.com/p/google-plus-platform/
- type: x-support
  url: https://developers.google.com/+/web/support
- type: x-terms-of-service
  url: https://developers.google.com/+/web/terms
- type: x-website
  url: https://plus.google.com/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---