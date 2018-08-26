{
  "info": {
    "name": "GoToTraining Get Start Url",
    "_postman_id": "0672a52f-39b7-4e61-afa2-c0d4ff791a12",
    "description": "Get start url.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Start",
      "item": [
        {
          "id": "58ed1f81-bacd-4d07-a5bc-33c2360f7108",
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
              "id": "fbf35499-281a-47d5-bdd0-d842c254cc7a"
            }
          ]
        },
        {
          "id": "775a8cd1-9573-44c1-8b90-89e837d82976",
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
              "id": "72168d78-07eb-4e49-8137-29071754e919"
            }
          ]
        }
      ]
    }
  ]
}