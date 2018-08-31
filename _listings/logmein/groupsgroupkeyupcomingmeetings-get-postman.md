{
  "info": {
    "name": "GoToMeeting Upcoming meetings by group",
    "_postman_id": "b85e02a9-05fc-49a1-bd89-0d0466c1a7e0",
    "description": "Get upcoming meetings for a specified group. This API call is only available to users with the admin role. This API call can be used only for groups with maximum 50 organizers.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Upcoming",
      "item": [
        {
          "id": "3e51226d-cab6-41f8-8154-11e214baf8ba",
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
              "id": "045e952a-4d8b-4877-b604-ab2e8c1392a1"
            }
          ]
        }
      ]
    }
  ]
}