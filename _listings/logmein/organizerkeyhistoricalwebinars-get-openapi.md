---
swagger: "2.0"
x-collection-name: LogMeIn
x-complete: 0
info:
  title: GoToWebinar Historical Webinars
  description: "Returns details for completed webinars for the specified organizer
    and completed webinars of other organizers where the specified organizer is a
    co-organizer.\n\nParameters:\n- organizerkey \n- fromTime\n- toTime"
  version: 1.0.0
host: api.getgo.com
basePath: /G2W/rest/organizers
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{organizerKey}/webinars/{webinarKey}/panelists:
    get:
      summary: Get webinar panelists
      description: Get webinar panelists.
      operationId: WebinarsPanelistsByOrganizerKeyAndWebinarKeyGet
      x-api-path-slug: organizerkeywebinarswebinarkeypanelists-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: organizerKey
      - in: path
        name: webinarKey
      responses:
        200:
          description: OK
      tags:
      - Webinar
      - Panelists
    post:
      summary: Create Panelists
      description: Create panelists.
      operationId: WebinarsPanelistsByOrganizerKeyAndWebinarKeyPost
      x-api-path-slug: organizerkeywebinarswebinarkeypanelists-post
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
        name: webinarKey
      responses:
        200:
          description: OK
      tags:
      - Panelists
  /{organizerkey}/webinars:
    post:
      summary: Create Webinar
      description: Create webinar.
      operationId: WebinarsByOrganizerkeyPost
      x-api-path-slug: organizerkeywebinars-post
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
        name: organizerkey
      responses:
        200:
          description: OK
      tags:
      - Webinar
  /{organizerKey}/webinars/{webinarKey}/sessions/{sessionKey}/attendees/{registrantKey}:
    get:
      summary: Get attendee
      description: Get attendee.
      operationId: WebinarsSessionsSessionKeyAttendeesRegistrantKeyByOrganizerKeyAndWebinarKeyGet
      x-api-path-slug: organizerkeywebinarswebinarkeysessionssessionkeyattendeesregistrantkey-get
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
        name: sessionKey
      - in: path
        name: webinarKey
      responses:
        200:
          description: OK
      tags:
      - Attendee
  /{organizerKey}/webinars/{webinarKey}:
    get:
      summary: Get Webinar
      description: Get webinar.
      operationId: WebinarsByOrganizerKeyAndWebinarKeyGet
      x-api-path-slug: organizerkeywebinarswebinarkey-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: organizerKey
      - in: path
        name: webinarKey
      responses:
        200:
          description: OK
      tags:
      - Webinar
    put:
      summary: Update webinar
      description: Update webinar.
      operationId: WebinarsByOrganizerKeyAndWebinarKeyPut
      x-api-path-slug: organizerkeywebinarswebinarkey-put
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
        name: webinarKey
      responses:
        200:
          description: OK
      tags:
      - Webinar
    delete:
      summary: Cancel Webinar
      description: Cancel webinar.
      operationId: WebinarsByOrganizerKeyAndWebinarKeyDelete
      x-api-path-slug: organizerkeywebinarswebinarkey-delete
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
      - in: query
        name: sendCancellationEmails
      - in: path
        name: webinarKey
      responses:
        200:
          description: OK
      tags:
      - Cancel
      - Webinar
  /{organizerKey}/webinars/{webinarKey}/sessions/{sessionKey}/attendees/{registrantKey}/questions:
    get:
      summary: Get attendee questions
      description: Get attendee questions.
      operationId: WebinarsSessionsSessionKeyAttendeesRegistrantKeyQuestionsByOrganizerKeyAndWebinarKeyGet
      x-api-path-slug: organizerkeywebinarswebinarkeysessionssessionkeyattendeesregistrantkeyquestions-get
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
        name: sessionKey
      - in: path
        name: webinarKey
      responses:
        200:
          description: OK
      tags:
      - Attendee
      - Questions
  /{organizerKey}/webinars/{webinarKey}/sessions/{sessionKey}/surveys:
    get:
      summary: Get session surveys
      description: Get session surveys.
      operationId: WebinarsSessionsSessionKeySurveysByOrganizerKeyAndWebinarKeyGet
      x-api-path-slug: organizerkeywebinarswebinarkeysessionssessionkeysurveys-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: organizerKey
      - in: path
        name: sessionKey
      - in: path
        name: webinarKey
      responses:
        200:
          description: OK
      tags:
      - Session
      - Surveys
  /{organizerKey}/webinars/{webinarKey}/registrants/{registrantKey}:
    get:
      summary: Get Registrant
      description: Get registrant.
      operationId: WebinarsRegistrantsRegistrantKeyByOrganizerKeyAndWebinarKeyGet
      x-api-path-slug: organizerkeywebinarswebinarkeyregistrantsregistrantkey-get
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
        name: webinarKey
      responses:
        200:
          description: OK
      tags:
      - Registrant
    delete:
      summary: Delete Registrant
      description: Delete registrant.
      operationId: WebinarsRegistrantsRegistrantKeyByOrganizerKeyAndWebinarKeyDelete
      x-api-path-slug: organizerkeywebinarswebinarkeyregistrantsregistrantkey-delete
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
        name: webinarKey
      responses:
        200:
          description: OK
      tags:
      - Registrant
  /{organizerKey}/webinars/{webinarKey}/meetingtimes:
    get:
      summary: Get webinar meeting times
      description: Get webinar meeting times.
      operationId: WebinarsMeetingtimesByOrganizerKeyAndWebinarKeyGet
      x-api-path-slug: organizerkeywebinarswebinarkeymeetingtimes-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: organizerKey
      - in: path
        name: webinarKey
      responses:
        200:
          description: OK
      tags:
      - Webinar
      - Meeting
      - Times
  /{organizerKey}/historicalWebinars:
    get:
      summary: Historical Webinars
      description: "Returns details for completed webinars for the specified organizer
        and completed webinars of other organizers where the specified organizer is
        a co-organizer.\n\nParameters:\n- organizerkey \n- fromTime\n- toTime"
      operationId: HistoricalWebinarsByOrganizerKeyGet
      x-api-path-slug: organizerkeyhistoricalwebinars-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: query
        name: fromTime
      - in: path
        name: organizerKey
      - in: query
        name: toTime
      responses:
        200:
          description: OK
      tags:
      - Historical
      - Webinars
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