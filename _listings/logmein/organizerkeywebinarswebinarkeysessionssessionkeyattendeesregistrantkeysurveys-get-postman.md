{
  "info": {
    "name": "GoToWebinar Get attendee survey answers",
    "_postman_id": "a7dc6c7d-f961-4b73-b05a-42c9b795e6ba",
    "description": "Get attendee survey answers.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Attendee",
      "item": [
        {
          "id": "4a160ab2-4e2f-44ae-aa3a-e897f9621098",
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
              "id": "beb2dfd5-0207-493e-9d1e-be85b2c92701"
            }
          ]
        }
      ]
    }
  ]
}