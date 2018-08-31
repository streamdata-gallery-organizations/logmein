{
  "info": {
    "name": "GoToMeeting Historical meetings",
    "_postman_id": "763e8c32-c385-444f-a419-8cf825a5dda1",
    "description": "Get historical meetings for the currently authenticated organizer that started within the specified date/time range. Remark: Meetings which are still ongoing at the time of the request are NOT contained in the result array.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Historical",
      "item": [
        {
          "id": "77610e36-9705-4441-a863-e11f1ab6b1c4",
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
              "id": "5f71199d-27d0-4051-bd3f-338dd4425a80"
            }
          ]
        }
      ]
    }
  ]
}