{
  "info": {
    "name": "GoToWebinar Get audio information",
    "_postman_id": "18ac7f21-8b6f-4e1a-abb9-65bd0f988009",
    "description": "Get audio information.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Audio",
      "item": [
        {
          "id": "0fefc09e-9076-448f-9f26-2d1ed4e68b36",
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
              "id": "f0646d93-1af4-41f5-af30-f3b02e33afc2"
            }
          ]
        }
      ]
    }
  ]
}