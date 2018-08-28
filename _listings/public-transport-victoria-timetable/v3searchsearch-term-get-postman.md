{
  "info": {
    "name": "PTV Timetable API - Version 3 Get V3 Search Search Term",
    "_postman_id": "29e4ce55-b6a1-415e-8c9d-cfca9eb65eae",
    "description": "View stops, routes and myki ticket outlets that match the search term.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Departures",
      "item": [
        {
          "id": "a99cc3e0-8669-410f-b8dd-609806770c9d",
          "name": "Departures_GetForStop",
          "request": {
            "url": {
              "protocol": "http",
              "host": "timetableapi.ptv.vic.gov.au",
              "path": [
                "v3/departures/route_type/:route_type/stop/:stop_id"
              ],
              "query": [
                {
                  "key": "date_utc",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "devid",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "direction_id",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "expand",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "gtfs",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "include_cancelled",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "max_results",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "platform_numbers",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "signature",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "token",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "route_type",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "stop_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "View departures for all routes from a stop."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "786f601d-db1c-4b1e-a961-8d3f9129a801"
            }
          ]
        },
        {
          "id": "312328a3-89aa-4b37-b9af-750ceae4d17f",
          "name": "Departures_GetForStopAndRoute",
          "request": {
            "url": {
              "protocol": "http",
              "host": "timetableapi.ptv.vic.gov.au",
              "path": [
                "v3/departures/route_type/:route_type/stop/:stop_id/route/:route_id"
              ],
              "query": [
                {
                  "key": "date_utc",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "devid",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "direction_id",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "expand",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "gtfs",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "include_cancelled",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "max_results",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "signature",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "token",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "route_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "route_type",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "stop_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "View departures for a specific route from a stop."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9eb80f2b-8e4c-4c22-bb1f-e013a46ca115"
            }
          ]
        }
      ]
    },
    {
      "name": "Directions",
      "item": [
        {
          "id": "d3f40c6e-f407-4c6a-a300-2901eebb3f42",
          "name": "Directions_ForRoute",
          "request": {
            "url": {
              "protocol": "http",
              "host": "timetableapi.ptv.vic.gov.au",
              "path": [
                "v3/directions/route/:route_id"
              ],
              "query": [
                {
                  "key": "devid",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "signature",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "token",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "route_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "View directions that a route travels in."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "33b326dc-d885-46c6-b26d-fa1edd739b25"
            }
          ]
        },
        {
          "id": "3622cb68-d5f5-4696-b3aa-58748d70e895",
          "name": "Directions_ForDirection",
          "request": {
            "url": {
              "protocol": "http",
              "host": "timetableapi.ptv.vic.gov.au",
              "path": [
                "v3/directions/:direction_id"
              ],
              "query": [
                {
                  "key": "devid",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "signature",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "token",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "direction_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "View all routes for a direction of travel."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3e5d85c1-80ae-4b1d-9e3b-98d02ee1065d"
            }
          ]
        },
        {
          "id": "1053b5fd-43a6-4014-9919-1965438ae291",
          "name": "Directions_ForDirectionAndType",
          "request": {
            "url": {
              "protocol": "http",
              "host": "timetableapi.ptv.vic.gov.au",
              "path": [
                "v3/directions/:direction_id/route_type/:route_type"
              ],
              "query": [
                {
                  "key": "devid",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "signature",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "token",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "direction_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "route_type",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "View all routes of a particular type for a direction of travel."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "880477ad-991a-4c04-8dea-c48b706cdc9a"
            }
          ]
        }
      ]
    },
    {
      "name": "Disruptions",
      "item": [
        {
          "id": "b930c2c8-4184-46c9-92c9-33027f6bff93",
          "name": "Disruptions_GetAllDisruptions",
          "request": {
            "url": "http://timetableapi.ptv.vic.gov.au/v3/disruptions?devid=%7B%7D&disruption_status=%7B%7D&route_types=%7B%7D&signature=%7B%7D&token=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "View all disruptions for all route types."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6cfe5255-85a1-415c-b3dc-d19ec567a265"
            }
          ]
        },
        {
          "id": "09194e11-0dca-49c3-9b97-875ba706ebce",
          "name": "Disruptions_GetDisruptionsByRoute",
          "request": {
            "url": {
              "protocol": "http",
              "host": "timetableapi.ptv.vic.gov.au",
              "path": [
                "v3/disruptions/route/:route_id"
              ],
              "query": [
                {
                  "key": "devid",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "disruption_status",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "signature",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "token",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "route_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "View all disruptions for a particular route."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b3c4485f-6f7b-4dc0-93cb-1fcd9abcbefe"
            }
          ]
        },
        {
          "id": "6b0bbd30-3389-48c4-86f3-23c9ed24fe68",
          "name": "Disruptions_GetDisruptionById",
          "request": {
            "url": {
              "protocol": "http",
              "host": "timetableapi.ptv.vic.gov.au",
              "path": [
                "v3/disruptions/:disruption_id"
              ],
              "query": [
                {
                  "key": "devid",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "signature",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "token",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "disruption_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "View a specific disruption."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d631a1bb-4043-408b-b7a8-7a619ba78732"
            }
          ]
        }
      ]
    },
    {
      "name": "Pattern",
      "item": [
        {
          "id": "83ed4086-4079-46a7-b7b2-7e5953aa43ae",
          "name": "Patterns_GetPatternByRun",
          "request": {
            "url": {
              "protocol": "http",
              "host": "timetableapi.ptv.vic.gov.au",
              "path": [
                "v3/pattern/run/:run_id/route_type/:route_type"
              ],
              "query": [
                {
                  "key": "date_utc",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "devid",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "signature",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "stop_id",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "token",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "route_type",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "run_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "View the stopping pattern for a specific trip/service run."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "44d072cf-ff74-4d9a-a2d5-5b9c55cd65e7"
            }
          ]
        }
      ]
    },
    {
      "name": "Route",
      "item": [
        {
          "id": "795a9b21-b361-45b1-a9dc-0d1e25d2e628",
          "name": "RouteTypes_GetRouteTypes",
          "request": {
            "url": "http://timetableapi.ptv.vic.gov.au/v3/route_types?devid=%7B%7D&signature=%7B%7D&token=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "View all route types and their names."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3e5297d2-bad5-450a-8bf6-0bec8550bead"
            }
          ]
        }
      ]
    },
    {
      "name": "Routes",
      "item": [
        {
          "id": "1dcda52d-43c3-4ff1-99a0-c8d1157b6528",
          "name": "Routes_OneOrMoreRoutes",
          "request": {
            "url": "http://timetableapi.ptv.vic.gov.au/v3/routes?devid=%7B%7D&route_name=%7B%7D&route_types=%7B%7D&signature=%7B%7D&token=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "View route names and numbers for all routes."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b694d695-1c0f-4c4a-af3e-6c57c83961b7"
            }
          ]
        },
        {
          "id": "28861b10-5f65-4d38-9c75-c9257252d53f",
          "name": "Routes_RouteFromId",
          "request": {
            "url": {
              "protocol": "http",
              "host": "timetableapi.ptv.vic.gov.au",
              "path": [
                "v3/routes/:route_id"
              ],
              "query": [
                {
                  "key": "devid",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "signature",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "token",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "route_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "View route name and number for specific route id."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1ae63e64-53e1-4c38-903b-2ea3d26ccf11"
            }
          ]
        }
      ]
    },
    {
      "name": "Runs",
      "item": [
        {
          "id": "d9c068c6-7ff8-4de3-a3fd-99abe7c9f46d",
          "name": "Runs_ForRoute",
          "request": {
            "url": {
              "protocol": "http",
              "host": "timetableapi.ptv.vic.gov.au",
              "path": [
                "v3/runs/route/:route_id"
              ],
              "query": [
                {
                  "key": "devid",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "signature",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "token",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "route_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "View all trip/service runs for a specific route id."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "af9dc667-d407-4e74-afc7-ca3b7588d022"
            }
          ]
        },
        {
          "id": "ac55bce3-143a-4ca6-9258-15988847f655",
          "name": "Runs_ForRouteAndRouteType",
          "request": {
            "url": {
              "protocol": "http",
              "host": "timetableapi.ptv.vic.gov.au",
              "path": [
                "v3/runs/route/:route_id/route_type/:route_type"
              ],
              "query": [
                {
                  "key": "devid",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "signature",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "token",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "route_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "route_type",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "View all trip/service runs for a specific route id and route type."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "489fb3f4-64fc-486c-afc2-e6ad4f8e6d73"
            }
          ]
        },
        {
          "id": "784c0d4c-cdc1-469f-a4ad-1827cec0cca6",
          "name": "Runs_ForRun",
          "request": {
            "url": {
              "protocol": "http",
              "host": "timetableapi.ptv.vic.gov.au",
              "path": [
                "v3/runs/:run_id"
              ],
              "query": [
                {
                  "key": "devid",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "signature",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "token",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "run_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "View all trip/service runs for a specific run id."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6b0c0bed-27c3-4430-9d16-35b76811ebf2"
            }
          ]
        },
        {
          "id": "2dc4563c-0dae-4ea7-8c60-b6ffab302730",
          "name": "Runs_ForRunAndRouteType",
          "request": {
            "url": {
              "protocol": "http",
              "host": "timetableapi.ptv.vic.gov.au",
              "path": [
                "v3/runs/:run_id/route_type/:route_type"
              ],
              "query": [
                {
                  "key": "devid",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "signature",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "token",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "route_type",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "run_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "View the trip/service run for a specific run id and route type."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6d62492c-e339-4aaa-9ce5-280b3b430db8"
            }
          ]
        }
      ]
    },
    {
      "name": "Search",
      "item": [
        {
          "id": "5efe6a21-fb4f-4417-b5ee-08e8189631d1",
          "name": "Search_Search",
          "request": {
            "url": {
              "protocol": "http",
              "host": "timetableapi.ptv.vic.gov.au",
              "path": [
                "v3/search/:search_term"
              ],
              "query": [
                {
                  "key": "devid",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "include_addresses",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "include_outlets",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "latitude",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "longitude",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "max_distance",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "route_types",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "signature",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "token",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "search_term",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "View stops, routes and myki ticket outlets that match the search term."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ad7b9426-a512-4206-bbc6-fdbc4fc3db7c"
            }
          ]
        }
      ]
    }
  ]
}