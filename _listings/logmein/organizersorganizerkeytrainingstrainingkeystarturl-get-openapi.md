---
swagger: "2.0"
x-collection-name: LogMeIn
x-complete: 0
info:
  title: GoToTraining Get Start Url
  description: Get start url.
  version: 1.0.0
host: api.getgo.com
basePath: /G2T/rest
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /trainings/{trainingKey}/start:
    get:
      summary: Start Training
      description: Start training.
      operationId: TrainingsStartByTrainingKeyGet
      x-api-path-slug: trainingstrainingkeystart-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: trainingKey
      responses:
        200:
          description: OK
      tags:
      - Start
      - Training
  /organizers/{organizerKey}/trainings/{trainingKey}/startUrl:
    get:
      summary: Get Start Url
      description: Get start url.
      operationId: OrganizersTrainingsStartUrlByOrganizerKeyAndTrainingKeyGet
      x-api-path-slug: organizersorganizerkeytrainingstrainingkeystarturl-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: organizerKey
      - in: path
        name: trainingKey
      responses:
        200:
          description: OK
      tags:
      - Start
      - Url
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