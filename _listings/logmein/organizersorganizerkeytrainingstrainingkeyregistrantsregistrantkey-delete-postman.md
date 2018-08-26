{
  "info": {
    "name": "GoToTraining Cancel Registration",
    "_postman_id": "737820d5-660b-4514-b19c-97e8fb8e0a04",
    "description": "Cancel registration.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Cancel",
      "item": [
        {
          "id": "1f2efcbb-8fa5-4c87-b572-c25c68ca7d8c",
          "name": "OrganizersTrainingsRegistrantsRegistrantKeyByOrganizerKeyAndTrainingKeyDelete",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.getgo.com",
              "path": [
                "G2T",
                "rest",
                "organizers/:organizerKey/trainings/:trainingKey/registrants/:registrantKey"
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
                  "id": "trainingKey",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
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
            "description": "Cancel registration."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "eb656786-ef47-41c4-9a92-ec3df76dbf5a"
            }
          ]
        }
      ]
    }
  ]
}