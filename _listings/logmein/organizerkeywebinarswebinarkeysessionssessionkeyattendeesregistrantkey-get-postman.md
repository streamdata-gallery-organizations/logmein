{
  "info": {
    "name": "GoToWebinar Get attendee",
    "_postman_id": "8735a673-a28c-4800-975d-bc71f62b7f2c",
    "description": "Get attendee.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Session",
      "item": [
        {
          "id": "3e2c3631-fa53-4b77-8f17-7a3da5b866e8",
          "name": "WebinarsSessionsSessionKeyAttendeesByOrganizerKeyAndWebinarKeyGet",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.getgo.com",
              "path": [
                "G2W",
                "rest",
                "organizers",
                ":organizerKey/webinars/:webinarKey/sessions/:sessionKey/attendees"
              ],
              "variable": [
                {
                  "id": "organizerKey",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "sessionKey",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "webinarKey",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get session attendees."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b7996723-c4ad-4c9b-a85d-55707639f1f9"
            }
          ]
        }
      ]
    },
    {
      "name": "Attendees",
      "item": [
        {
          "id": "5e929cb1-1156-463c-9d71-e95250747be5",
          "name": "WebinarsAttendeesByOrganizerKeyAndWebinarKeyGet",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.getgo.com",
              "path": [
                "G2W",
                "rest",
                "organizers",
                ":organizerKey/webinars/:webinarKey/attendees"
              ],
              "variable": [
                {
                  "id": "organizerKey",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "webinarKey",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get attendees for all webinar sessions."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9e01496b-7c5b-4b36-8a30-12d3e1f1c85e"
            }
          ]
        }
      ]
    },
    {
      "name": "Attendee",
      "item": [
        {
          "id": "aa1c6011-ed67-4025-a27e-e83253a816ce",
          "name": "WebinarsSessionsSessionKeyAttendeesRegistrantKeyByOrganizerKeyAndWebinarKeyGet",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.getgo.com",
              "path": [
                "G2W",
                "rest",
                "organizers",
                ":organizerKey/webinars/:webinarKey/sessions/:sessionKey/attendees/:registrantKey"
              ],
              "variable": [
                {
                  "id": "organizerKey",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "registrantKey",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "sessionKey",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "webinarKey",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get attendee."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cb0abc12-dd54-49f3-875d-4a1d13f85a84"
            }
          ]
        },
        {
          "id": "20cfe4a9-9dec-4a21-92d3-469271e6e5c7",
          "name": "WebinarsSessionsSessionKeyAttendeesRegistrantKeyQuestionsByOrganizerKeyAndWebinarKeyGet",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.getgo.com",
              "path": [
                "G2W",
                "rest",
                "organizers",
                ":organizerKey/webinars/:webinarKey/sessions/:sessionKey/attendees/:registrantKey/questions"
              ],
              "variable": [
                {
                  "id": "organizerKey",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "registrantKey",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "sessionKey",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "webinarKey",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get attendee questions."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3ccb1db5-625e-4fed-a475-efb81e3b4764"
            }
          ]
        },
        {
          "id": "5b5cf5b6-38ae-4dd4-863d-69a0e5571387",
          "name": "WebinarsSessionsSessionKeyAttendeesRegistrantKeySurveysByOrganizerKeyAndWebinarKeyGet",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.getgo.com",
              "path": [
                "G2W",
                "rest",
                "organizers",
                ":organizerKey/webinars/:webinarKey/sessions/:sessionKey/attendees/:registrantKey/surveys"
              ],
              "variable": [
                {
                  "id": "organizerKey",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "registrantKey",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "sessionKey",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "webinarKey",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get attendee survey answers."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "20caff3f-9f82-49ca-ac50-1e6cd76a5564"
            }
          ]
        },
        {
          "id": "e564fc9c-953a-4fba-b7c7-bfb55f5cd575",
          "name": "WebinarsSessionsSessionKeyAttendeesRegistrantKeyPollsByOrganizerKeyAndWebinarKeyGet",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.getgo.com",
              "path": [
                "G2W",
                "rest",
                "organizers",
                ":organizerKey/webinars/:webinarKey/sessions/:sessionKey/attendees/:registrantKey/polls"
              ],
              "variable": [
                {
                  "id": "organizerKey",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "registrantKey",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "sessionKey",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "webinarKey",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get attendee poll answers."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2f0d923c-6fb2-4cd9-8af5-4a2e23da2f8e"
            }
          ]
        }
      ]
    }
  ]
}