---
swagger: "2.0"
x-collection-name: LogMeIn
x-complete: 0
info:
  title: GoToTraining Get Trainings
  description: Get trainings.
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
  /organizers/{organizerKey}/trainings/{trainingKey}/organizers:
    put:
      summary: Update Training Organizers
      description: Update training organizers.
      operationId: OrganizersTrainingsOrganizersByOrganizerKeyAndTrainingKeyPut2
      x-api-path-slug: organizersorganizerkeytrainingstrainingkeyorganizers-put
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
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
      - Training
      - Organizers
  /organizers/{organizerKey}/trainings/{trainingKey}/registrants/{registrantKey}:
    get:
      summary: Get Registrant
      description: Get registrant.
      operationId: OrganizersTrainingsRegistrantsRegistrantKeyByOrganizerKeyAndTrainingKeyGet
      x-api-path-slug: organizersorganizerkeytrainingstrainingkeyregistrantsregistrantkey-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: organizerKey
      - in: path
        name: registrantKey
      - in: path
        name: trainingKey
      responses:
        200:
          description: OK
      tags:
      - Registrant
    delete:
      summary: Cancel Registration
      description: Cancel registration.
      operationId: OrganizersTrainingsRegistrantsRegistrantKeyByOrganizerKeyAndTrainingKeyDelete
      x-api-path-slug: organizersorganizerkeytrainingstrainingkeyregistrantsregistrantkey-delete
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: organizerKey
      - in: path
        name: registrantKey
      - in: path
        name: trainingKey
      responses:
        200:
          description: OK
      tags:
      - Cancel
      - Registration
  /reports/organizers/{organizerKey}/trainings/{trainingKey}:
    get:
      summary: Get Sessions by Training
      description: Get sessions by training.
      operationId: ReportsOrganizersTrainingsByOrganizerKeyAndTrainingKeyGet
      x-api-path-slug: reportsorganizersorganizerkeytrainingstrainingkey-get
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
      - Sessions
      - By
      - Training
  /organizers/{organizerKey}/trainings:
    get:
      summary: Get Trainings
      description: Get trainings.
      operationId: OrganizersTrainingsByOrganizerKeyGet
      x-api-path-slug: organizersorganizerkeytrainings-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: organizerKey
      responses:
        200:
          description: OK
      tags:
      - Trainings
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