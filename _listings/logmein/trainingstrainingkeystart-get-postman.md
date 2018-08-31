{
  "info": {
    "name": "GoToTraining Start Training",
    "_postman_id": "7caf351b-bed0-4034-9fde-11eed219fd0b",
    "description": "Start training.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Start",
      "item": [
        {
          "id": "23c4a250-b265-44ea-bbf8-fbab476e44b5",
          "name": "TrainingsStartByTrainingKeyGet",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.getgo.com",
              "path": [
                "G2T",
                "rest",
                "trainings/:trainingKey/start"
              ],
              "variable": [
                {
                  "id": "trainingKey",
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
            "description": "Start training."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "89ee3869-ec9f-46ba-a8fb-7aadb53f9418"
            }
          ]
        },
        {
          "id": "5c054c5f-9aa8-4b24-ab3f-d353c1920868",
          "name": "OrganizersTrainingsStartUrlByOrganizerKeyAndTrainingKeyGet",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.getgo.com",
              "path": [
                "G2T",
                "rest",
                "organizers/:organizerKey/trainings/:trainingKey/startUrl"
              ],
              "variable": [
                {
                  "id": "organizerKey",
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
            "description": "Get start url."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ce81a128-3a0c-4f17-91ec-70e2622a034a"
            }
          ]
        }
      ]
    }
  ]
}