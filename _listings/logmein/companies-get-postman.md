{
  "info": {
    "name": "GoToAssist Remote Support Get Companies",
    "_postman_id": "6c47c13f-5124-466c-9881-cb1ffcc07efb",
    "description": "This method retrieves information about the companies that the authenticated user has access to.\n\n                    \n  Query Parameters (all are optional)                  \n    q      string      A search query to filter the returned records. Performs a contains check on companyName    \n    limit      integer      The maximum number of records to be fetched. Default limit is 50. Valid range is 1 to 50. Greater than 50 results in bad request.    \n    offset      number      Zero based offset for the first record to return. Default value is 0.    \n    sortField      string      Name of the field to sort by, can be one of companyId, companyName.    \n    sortOrder            Sort order can be specified explicitly. Allowed values are “asc” for ascending order and “desc” for descending order.    \n\n\nStatus Codes              \n              \n    Staus Code      description    \n    200 OK      The information was successfully retrieved    \n    401 Unauthorized      An authentication parameter was passed, but either it was invalid or the technician is not entitled with a Remote Support seat;    \n    403 Forbidden      Access denied. User doesn’t have required roles    \n    404 Not Found      No companies found    \n    405 Method Not Allowed      The method was entered incorrectly (i.e., the technician tried to use POST, PUT etc. instead of GET)    \n    500 Internal Server Error      An unhandled error occurred",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Companies",
      "item": [
        {
          "id": "ff868231-1789-40df-baf0-d3d474732b3f",
          "name": "CompaniesGet",
          "request": {
            "url": "http://api.getgo.com/G2A/rest/v1/companies",
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
            "description": "This method retrieves information about the companies that the authenticated user has access to.\n\n                    \n  Query Parameters (all are optional)                  \n    q      string      A search query to filter the returned records. Performs a contains check on companyName    \n    limit      integer      The maximum number of records to be fetched. Default limit is 50. Valid range is 1 to 50. Greater than 50 results in bad request.    \n    offset      number      Zero based offset for the first record to return. Default value is 0.    \n    sortField      string      Name of the field to sort by, can be one of companyId, companyName.    \n    sortOrder            Sort order can be specified explicitly. Allowed values are “asc” for ascending order and “desc” for descending order.    \n\n\nStatus Codes              \n              \n    Staus Code      description    \n    200 OK      The information was successfully retrieved    \n    401 Unauthorized      An authentication parameter was passed, but either it was invalid or the technician is not entitled with a Remote Support seat;    \n    403 Forbidden      Access denied. User doesn’t have required roles    \n    404 Not Found      No companies found    \n    405 Method Not Allowed      The method was entered incorrectly (i.e., the technician tried to use POST, PUT etc. instead of GET)    \n    500 Internal Server Error      An unhandled error occurred"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9d361bd0-6be1-48eb-bbdd-1dbb19d38164"
            }
          ]
        }
      ]
    }
  ]
}