{
  "info": {
    "name": "GoToAssist Remote Support Get Tickets",
    "_postman_id": "747a9770-9ed7-4d66-8bb4-8d4a437f67fb",
    "description": "Retrieves a query-able set of tickets for a specific partner system.\n\n                                                         \nRequest Parameters\n                          \n    field      data type      description    \n    userToken      string      The token identifying and authenticating the user in the partner system that this object is being created on behalf of this user.    \n\n\nQuery Parameters (* Optional)\n\n    field      data type      description    \n    q *      string      A query string used to search for objects in the partner system. (It is up to the partner system to determine how the query string is matched. Match against fields like: ticket title, ticket body, requester name, ticket ID, ticket comments, tags, etc. Ideally the matching should be performed using a ‘contains’ type operation and in a case-insensitive way.)                                         \n    limit *      integer      The maximum number of records to be fetched. Default value is 10. Suggested value is less than or equal to 10 for optimal performance.                                         \n    offset *      number      Zero based offset for the first record to return. Default value is 0.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Tickets",
      "item": [
        {
          "id": "aa20fb14-51b4-4fe8-84f5-7acc1ded86d2",
          "name": "UnnammedEndpointGet",
          "request": {
            "url": "http://api.getgo.com/G2A/rest/v1/?limit=%7B%7D&offset=%7B%7D&q=%7B%7D&userToken=%7B%7D",
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
            "description": "Retrieves a query-able set of tickets for a specific partner system.\n\n                                                         \nRequest Parameters\n                          \n    field      data type      description    \n    userToken      string      The token identifying and authenticating the user in the partner system that this object is being created on behalf of this user.    \n\n\nQuery Parameters (* Optional)\n\n    field      data type      description    \n    q *      string      A query string used to search for objects in the partner system. (It is up to the partner system to determine how the query string is matched. Match against fields like: ticket title, ticket body, requester name, ticket ID, ticket comments, tags, etc. Ideally the matching should be performed using a ‘contains’ type operation and in a case-insensitive way.)                                         \n    limit *      integer      The maximum number of records to be fetched. Default value is 10. Suggested value is less than or equal to 10 for optimal performance.                                         \n    offset *      number      Zero based offset for the first record to return. Default value is 0."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8a24dee7-29a9-4a68-8f67-3d0e42e08f38"
            }
          ]
        }
      ]
    }
  ]
}