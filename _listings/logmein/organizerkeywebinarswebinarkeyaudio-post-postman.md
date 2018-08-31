{
  "info": {
    "name": "GoToWebinar Update audio information",
    "_postman_id": "0627ae0e-c207-436b-be10-d93e4c49abbe",
    "description": "Update audio information.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Audio",
      "item": [
        {
          "id": "6f98da38-68a5-4010-a451-1664b93e2a50",
          "name": "WebinarsAudioByOrganizerKeyAndWebinarKeyGet",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.getgo.com",
              "path": [
                "G2W",
                "rest",
                "organizers",
                ":organizerKey/webinars/:webinarKey/audio"
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
            "description": "Get audio information."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c5a58d5a-10c1-48e0-b011-2f567e2cb56e"
            }
          ]
        },
        {
          "id": "8163081e-aa96-44c2-a606-5b77876f4e84",
          "name": "WebinarsAudioByOrganizerKeyAndWebinarKeyPost",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.getgo.com",
              "path": [
                "G2W",
                "rest",
                "organizers",
                ":organizerKey/webinars/:webinarKey/audio"
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
            "method": "POST",
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
            "description": "Update audio information."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ad35961b-fb19-4c37-969a-debdc355f8eb"
            }
          ]
        }
      ]
    }
  ]
}