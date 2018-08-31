{
  "info": {
    "name": "GoToMeeting Upcoming meetings",
    "_postman_id": "7cdace32-fe65-45ea-9f11-7ff5d8b9cfd3",
    "description": "Gets upcoming meetings for the current authenticated organizer.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Upcoming",
      "item": [
        {
          "id": "fc57db19-8c07-4358-9c4d-85aaa4b14cc8",
          "name": "GroupsUpcomingMeetingsByGroupKeyGet",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.getgo.com",
              "path": [
                "G2M",
                "rest",
                "groups/:groupKey/upcomingMeetings"
              ],
              "variable": [
                {
                  "id": "groupKey",
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
            "description": "Get upcoming meetings for a specified group. This API call is only available to users with the admin role. This API call can be used only for groups with maximum 50 organizers."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5f77187d-f173-49b3-b616-987abf88f2bd"
            }
          ]
        },
        {
          "id": "e7b709cd-e95e-496d-ac45-26be921af9ed",
          "name": "UpcomingMeetingsGet",
          "request": {
            "url": "http://api.getgo.com/G2M/rest/upcomingMeetings",
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
            "description": "Gets upcoming meetings for the current authenticated organizer."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fc832345-50f9-44fc-836e-e272ecd811b2"
            }
          ]
        }
      ]
    },
    {
      "name": "Historical",
      "item": [
        {
          "id": "c16fff7b-5239-481f-b52f-29abac52b19e",
          "name": "HistoricalMeetingsGet",
          "request": {
            "url": "http://api.getgo.com/G2M/rest/historicalMeetings?endDate=%7B%7D&startDate=%7B%7D",
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
            "description": "Get historical meetings for the currently authenticated organizer that started within the specified date/time range. Remark: Meetings which are still ongoing at the time of the request are NOT contained in the result array."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "683b27c0-30f8-418c-8047-1c42b894455d"
            }
          ]
        }
      ]
    }
  ]
}