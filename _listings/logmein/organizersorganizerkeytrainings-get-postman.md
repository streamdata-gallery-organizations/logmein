{
  "info": {
    "name": "GoToTraining Get Trainings",
    "_postman_id": "820a9aa2-7d99-46e0-996e-06fb838b4f57",
    "description": "Get trainings.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Trainings",
      "item": [
        {
          "id": "89215d15-d0d6-4121-8695-e85b308c8662",
          "name": "OrganizersTrainingsByOrganizerKeyGet",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.getgo.com",
              "path": [
                "G2T",
                "rest",
                "organizers/:organizerKey/trainings"
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
            "description": "Get trainings."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e33dbf8a-6c5b-47cc-adb6-b0053ced7905"
            }
          ]
        }
      ]
    }
  ]
}