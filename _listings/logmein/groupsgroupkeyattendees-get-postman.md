{
  "info": {
    "name": "GoToMeeting Attendees by group",
    "_postman_id": "71c9f29e-e90b-46ae-ad21-151a39b3f4a7",
    "description": "Returns all attendees for all meetings within specified date range held by organizers within the specified group. This API call is only available to users with the admin role. This API call can be used only for groups with maximum 50 organizers.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Attendees",
      "item": [
        {
          "id": "d6a14f32-64bc-4593-8ce5-f37dda14c210",
          "name": "MeetingsAttendeesByMeetingInstanceKeyGet",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.getgo.com",
              "path": [
                "G2M",
                "rest",
                "meetings/:meetingInstanceKey/attendees"
              ],
              "variable": [
                {
                  "id": "meetingInstanceKey",
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
            "description": "List all attendees for specified meetingId of historical meeting. The historical meetings can be fetched using 'Get historical meetings', 'Get historical meetings by organizer', and 'Get historical meetings by group'. For users with the admin role this call returns attendees for any meeting. For any other user the call will return attendees for meetings on which the user is a valid organizer."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7b531fac-2aca-48c6-ae21-8612c9f68572"
            }
          ]
        },
        {
          "id": "4292fb4e-7d9f-4fe4-9e2c-7c4a3ca37c9c",
          "name": "OrganizersAttendeesByOrganizerKeyGet",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.getgo.com",
              "path": [
                "G2M",
                "rest",
                "organizers/:organizerKey/attendees"
              ],
              "query": [
                {
                  "key": "endDate",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "starttime",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "organizerKey",
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
            "description": "Lists all attendees for all meetings within a specified date range for a specified organizer. This API call is only available to users with the admin role."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "aaa87bd5-0d5a-46eb-8c5e-e0adeb77e11c"
            }
          ]
        },
        {
          "id": "f6f3c514-2edb-4d3c-bb7f-091fd34630ef",
          "name": "GroupsAttendeesByGroupkeyGet",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.getgo.com",
              "path": [
                "G2M",
                "rest",
                "groups/:groupkey/attendees"
              ],
              "query": [
                {
                  "key": "endDate",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "startDate",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "groupkey",
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
            "description": "Returns all attendees for all meetings within specified date range held by organizers within the specified group. This API call is only available to users with the admin role. This API call can be used only for groups with maximum 50 organizers."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8825a1a2-0788-425b-9447-f93091a6345c"
            }
          ]
        }
      ]
    }
  ]
}