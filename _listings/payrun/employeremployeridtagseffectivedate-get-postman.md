{
  "info": {
    "name": "Pay Run.IO Get all employer revision tags",
    "_postman_id": "1dbf81c9-bf73-4043-a848-5affb856bcae",
    "description": "Gets all the tags from the employer revision",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Employee",
      "item": [
        {
          "id": "4ea0333f-c0d0-46fb-947f-7e83a747cb40",
          "name": "GetTagsFromEmployee",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.test.payrun.io",
              "path": [
                "Employer/:EmployerId/Employee/:EmployeeId/Tags"
              ],
              "variable": [
                {
                  "id": "EmployeeId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "EmployerId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Api-Version",
                "value": "{}",
                "description": "The version of the api to target",
                "disabled": false
              },
              {
                "key": "Authorization",
                "value": "{}",
                "description": "The OAuth 1 authorization header",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Gets all the tags from the employee"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "986861b9-3821-412c-81d9-1a50bb7cb70f"
            }
          ]
        },
        {
          "id": "ae4028f8-23b0-4c13-b7f0-44eccde0b809",
          "name": "GetTagsFromEmployeeRevision",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.test.payrun.io",
              "path": [
                "Employer/:EmployerId/Employee/:EmployeeId/Tags/:EffectiveDate"
              ],
              "variable": [
                {
                  "id": "EffectiveDate",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "EmployeeId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "EmployerId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Api-Version",
                "value": "{}",
                "description": "The version of the api to target",
                "disabled": false
              },
              {
                "key": "Authorization",
                "value": "{}",
                "description": "The OAuth 1 authorization header",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Gets all the tags from the employee revision"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "628fccd2-3abe-45f6-9bd7-e9a887572f6b"
            }
          ]
        },
        {
          "id": "4062ce57-e1bf-4051-a487-4791e7879a4e",
          "name": "GetAllEmployeeTags",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.test.payrun.io",
              "path": [
                "Employer/:EmployerId/Employees/Tags"
              ],
              "variable": [
                {
                  "id": "EmployerId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Api-Version",
                "value": "{}",
                "description": "The version of the api to target",
                "disabled": false
              },
              {
                "key": "Authorization",
                "value": "{}",
                "description": "The OAuth 1 authorization header",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Gets all the employee tags"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8359cfab-3e6e-4352-9fe9-7f9d81175c75"
            }
          ]
        }
      ]
    },
    {
      "name": "Pay",
      "item": [
        {
          "id": "70f15b87-b1b4-4d8c-b482-426b92d4982e",
          "name": "GetTagsFromPayCode",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.test.payrun.io",
              "path": [
                "Employer/:EmployerId/PayCode/:PayCodeId/Tags"
              ],
              "variable": [
                {
                  "id": "EmployerId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "PayCodeId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Api-Version",
                "value": "{}",
                "description": "The version of the api to target",
                "disabled": false
              },
              {
                "key": "Authorization",
                "value": "{}",
                "description": "The OAuth 1 authorization header",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Gets all the tags from the pay code"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6f567c0d-5c32-4e02-90b6-b85e747c5e9e"
            }
          ]
        },
        {
          "id": "37326f5c-b243-4e49-86b9-867f83006edc",
          "name": "GetAllPayCodeTags",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.test.payrun.io",
              "path": [
                "Employer/:EmployerId/PayCodes/Tags"
              ],
              "variable": [
                {
                  "id": "EmployerId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Api-Version",
                "value": "{}",
                "description": "The version of the api to target",
                "disabled": false
              },
              {
                "key": "Authorization",
                "value": "{}",
                "description": "The OAuth 1 authorization header",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Gets all the pay code tags"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "915b496d-103f-4b72-adc5-5fce20c33941"
            }
          ]
        },
        {
          "id": "8144b4b7-f1d7-4309-a3e3-7fa7571ae29b",
          "name": "GetTagsFromPayRun",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.test.payrun.io",
              "path": [
                "Employer/:EmployerId/PaySchedule/:PayScheduleId/PayRun/:PayRunId/Tags"
              ],
              "variable": [
                {
                  "id": "EmployerId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "PayRunId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "PayScheduleId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Api-Version",
                "value": "{}",
                "description": "The version of the api to target",
                "disabled": false
              },
              {
                "key": "Authorization",
                "value": "{}",
                "description": "The OAuth 1 authorization header",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Gets all the tags from the pay run"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "aaa76c39-e9b4-4648-b5f9-8f7bbe0fff64"
            }
          ]
        },
        {
          "id": "9b6c639b-e634-4e5c-808f-68726e8582b5",
          "name": "GetAllPayRunTags",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.test.payrun.io",
              "path": [
                "Employer/:EmployerId/PaySchedule/:PayScheduleId/PayRuns/Tags"
              ],
              "variable": [
                {
                  "id": "EmployerId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "PayScheduleId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Api-Version",
                "value": "{}",
                "description": "The version of the api to target",
                "disabled": false
              },
              {
                "key": "Authorization",
                "value": "{}",
                "description": "The OAuth 1 authorization header",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Gets all the pay run tags"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "38c21fb7-e64d-4223-a27a-9315335abd5e"
            }
          ]
        },
        {
          "id": "d2c1591a-6e01-4385-8407-dd7149fb066a",
          "name": "GetTagsFromPaySchedule",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.test.payrun.io",
              "path": [
                "Employer/:EmployerId/PaySchedule/:PayScheduleId/Tags"
              ],
              "variable": [
                {
                  "id": "EmployerId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "PayScheduleId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Api-Version",
                "value": "{}",
                "description": "The version of the api to target",
                "disabled": false
              },
              {
                "key": "Authorization",
                "value": "{}",
                "description": "The OAuth 1 authorization header",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Gets all the tags from the pay schedule"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f037480a-3705-4eba-b623-2cd828d1c6bd"
            }
          ]
        },
        {
          "id": "c6b1825a-08ba-47f4-9bf7-f13e45d14b06",
          "name": "GetAllPayScheduleTags",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.test.payrun.io",
              "path": [
                "Employer/:EmployerId/PaySchedules/Tags"
              ],
              "variable": [
                {
                  "id": "EmployerId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Api-Version",
                "value": "{}",
                "description": "The version of the api to target",
                "disabled": false
              },
              {
                "key": "Authorization",
                "value": "{}",
                "description": "The OAuth 1 authorization header",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Gets all the pay schedule tags"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bf155e40-1233-4e90-a66d-3bd1c9c7f914"
            }
          ]
        }
      ]
    },
    {
      "name": "Employer",
      "item": [
        {
          "id": "cf69ae0f-0599-4a28-abbb-46ad0c3be76a",
          "name": "GetTagsFromEmployer",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.test.payrun.io",
              "path": [
                "Employer/:EmployerId/Tags"
              ],
              "variable": [
                {
                  "id": "EmployerId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Api-Version",
                "value": "{}",
                "description": "The version of the api to target",
                "disabled": false
              },
              {
                "key": "Authorization",
                "value": "{}",
                "description": "The OAuth 1 authorization header",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Gets all the tags from the employer"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "44914f5f-cd0d-4b17-8021-17b6d71b6db0"
            }
          ]
        },
        {
          "id": "c8ccceb8-dfee-4fe7-b6d2-40a6ea2a9f6d",
          "name": "GetTagsFromEmployerRevision",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.test.payrun.io",
              "path": [
                "Employer/:EmployerId/Tags/:EffectiveDate"
              ],
              "variable": [
                {
                  "id": "EffectiveDate",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "EmployerId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Api-Version",
                "value": "{}",
                "description": "The version of the api to target",
                "disabled": false
              },
              {
                "key": "Authorization",
                "value": "{}",
                "description": "The OAuth 1 authorization header",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Gets all the tags from the employer revision"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e8433840-1237-4c64-921c-a5fef010d7c9"
            }
          ]
        }
      ]
    }
  ]
}