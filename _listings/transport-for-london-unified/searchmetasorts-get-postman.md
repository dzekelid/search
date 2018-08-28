{
  "info": {
    "name": "Transport for London Unified Search  Meta  Sorts",
    "_postman_id": "2d0b822a-830c-4a45-ac84-4e078fdf574b",
    "description": "Gets the available sorting options..",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Accent",
      "item": [
        {
          "id": "fb74a6eb-08fb-4d9e-9772-256b3e840c33",
          "name": "AccidentStats_Get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.tfl.gov.uk",
              "path": [
                "AccidentStats/:year"
              ],
              "variable": [
                {
                  "id": "year",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Gets all accident details for accidents occuring in the specified year."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5afdce3a-137e-4b59-8df8-e23e8f599570"
            }
          ]
        }
      ]
    },
    {
      "name": "Air",
      "item": [
        {
          "id": "8f79ea09-a434-4e53-b555-b5187788ae5a",
          "name": "AirQuality_Get",
          "request": {
            "url": "http://api.tfl.gov.uk/AirQuality",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Gets air quality data feed."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "74fc8c8e-26a0-427b-a525-53cee81030c7"
            }
          ]
        }
      ]
    },
    {
      "name": "Bike",
      "item": [
        {
          "id": "93e1fbe1-f324-4a85-a3de-fbdf4f21e4f1",
          "name": "BikePoint_GetAll",
          "request": {
            "url": "http://api.tfl.gov.uk/BikePoint",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Gets all bike point locations. the place object has an addtionalproperties array which contains the nbbikes, nbdocks and nbspaces\r\n            numbers which give the status of the bikepoint. a mismatch in these numbers i.e. nbdocks - (nbbikes + nbspa."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f0f69128-c0bd-415d-8d5b-3b07dac31da5"
            }
          ]
        },
        {
          "id": "cd5fb08a-8099-4b74-a96c-42e79d6162bf",
          "name": "BikePoint_Search",
          "request": {
            "url": "http://api.tfl.gov.uk/BikePoint/Search?query=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Search for bike stations by their name, a bike point's name often contains information about the name of the street\r\n            or nearby landmarks, for example. note that the search result does not contain the placeproperties i.e. the status\r\n     ."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3ae595ce-5eef-4b2c-a582-38c088384691"
            }
          ]
        },
        {
          "id": "bcf2544d-9603-47ba-a141-f2f4bbfd8344",
          "name": "BikePoint_Get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.tfl.gov.uk",
              "path": [
                "BikePoint/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Gets the bike point with the given id.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "be3790d0-8255-4d81-8761-f01ce3363c67"
            }
          ]
        }
      ]
    },
    {
      "name": "Cabwise",
      "item": [
        {
          "id": "5c0668f7-259f-4d59-ac0d-8b7e6a2f0e49",
          "name": "Cabwise_Get",
          "request": {
            "url": "http://api.tfl.gov.uk/Cabwise/search?forceXml=%7B%7D&lat=%7B%7D&legacyFormat=%7B%7D&lon=%7B%7D&maxResults=%7B%7D&name=%7B%7D&optype=%7B%7D&radius=%7B%7D&twentyFourSevenOnly=%7B%7D&wc=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Gets taxis and minicabs contact information."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2073d6ac-3a7e-4437-8a32-491451e2e931"
            }
          ]
        }
      ]
    },
    {
      "name": "Journey",
      "item": [
        {
          "id": "4cf87498-388a-4e77-952c-53e605aec510",
          "name": "Journey_JourneyResults",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.tfl.gov.uk",
              "path": [
                "Journey/JourneyResults/:from/to/:to"
              ],
              "query": [
                {
                  "key": "accessibilityPreference",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "adjustment",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "alternativeCycle",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "alternativeWalking",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "applyHtmlMarkup",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "bikeProficiency",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "cyclePreference",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "date",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "fromName",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "journeyPreference",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "maxTransferMinutes",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "maxWalkingMinutes",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "mode",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "nationalSearch",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "taxiOnlyTrip",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "time",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "timeIs",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "toName",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "useMultiModalCall",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "via",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "viaName",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "walkingOptimization",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "walkingSpeed",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "from",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "to",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Perform a journey planner search from the parameters specified in simple types."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4294082a-16cc-4b19-a32b-0d9d5b2873f1"
            }
          ]
        },
        {
          "id": "0f233107-4807-47f9-929c-795ea1ab71a4",
          "name": "Journey_Meta",
          "request": {
            "url": "http://api.tfl.gov.uk/Journey/Meta/Modes",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Gets a list of all of the available journey planner modes."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "93574624-a62c-412e-836e-351a9f6adf37"
            }
          ]
        }
      ]
    },
    {
      "name": "Line",
      "item": [
        {
          "id": "bc91f98b-44c2-478f-af58-1852ab14067f",
          "name": "Line_MetaDisruptionCategories",
          "request": {
            "url": "http://api.tfl.gov.uk/Line/Meta/DisruptionCategories",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Gets a list of valid disruption categories."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "34e7e937-97c7-4b6e-8135-037fc9633a89"
            }
          ]
        },
        {
          "id": "665e7b86-53e3-43ed-ab76-631be25c4ac6",
          "name": "Line_MetaModes",
          "request": {
            "url": "http://api.tfl.gov.uk/Line/Meta/Modes",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Gets a list of valid modes."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e182fc74-af69-4580-95ce-45a970b9387e"
            }
          ]
        },
        {
          "id": "262c973a-f3bb-4804-81c1-d3fbb7773f8e",
          "name": "Line_MetaServiceTypes",
          "request": {
            "url": "http://api.tfl.gov.uk/Line/Meta/ServiceTypes",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Gets a list of valid servicetypes to filter on."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "95338561-cacf-4be1-8f18-28a35f90f6ad"
            }
          ]
        },
        {
          "id": "fd18c7d8-ea41-4543-afe4-b34fce60e756",
          "name": "Line_MetaSeverity",
          "request": {
            "url": "http://api.tfl.gov.uk/Line/Meta/Severity",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Gets a list of valid severity codes."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "12ce4f21-f7f6-48e7-b902-0fce3d583d8f"
            }
          ]
        },
        {
          "id": "5beeaba1-f6b9-47d3-ba30-96ebda57d883",
          "name": "Line_GetByMode",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.tfl.gov.uk",
              "path": [
                "Line/Mode/:modes"
              ],
              "variable": [
                {
                  "id": "modes",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Gets lines that serve the given modes.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8ac76fa3-ade4-4a84-94af-dbcc400a70a3"
            }
          ]
        },
        {
          "id": "3518f01e-e9af-46b5-89d0-829c8d6d4774",
          "name": "Line_DisruptionByMode",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.tfl.gov.uk",
              "path": [
                "Line/Mode/:modes/Disruption"
              ],
              "variable": [
                {
                  "id": "modes",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get disruptions for all lines of the given modes.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1bd4fd2c-c718-43ba-b93e-d3e2be451dd5"
            }
          ]
        },
        {
          "id": "a1b446e8-a97a-45cf-8111-5fec1d011dd8",
          "name": "Line_RouteByMode",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.tfl.gov.uk",
              "path": [
                "Line/Mode/:modes/Route"
              ],
              "query": [
                {
                  "key": "serviceTypes",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "modes",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Gets all lines and their valid routes for given modes, including the name and id of the originating and terminating stops for each route."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0af4db97-4485-4219-8866-45208fc3f1b7"
            }
          ]
        },
        {
          "id": "a94cb468-bc61-4b81-a70c-1ddb2fdd6a9d",
          "name": "Line_StatusByMode",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.tfl.gov.uk",
              "path": [
                "Line/Mode/:modes/Status"
              ],
              "query": [
                {
                  "key": "detail",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "modes",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Gets the line status of for all lines for the given modes."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "26c6f2e1-bc5c-4899-98a0-74e0399881d7"
            }
          ]
        },
        {
          "id": "2fdd1ba5-4314-41ae-9acb-578c24bce784",
          "name": "Line_Route",
          "request": {
            "url": "http://api.tfl.gov.uk/Line/Route?serviceTypes=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get all valid routes for all lines, including the name and id of the originating and terminating stops for each route.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "76de1193-7bb1-4818-b745-07fd29ea0f01"
            }
          ]
        },
        {
          "id": "61bde257-433b-4eb6-9d55-b35793823a10",
          "name": "Line_Search",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.tfl.gov.uk",
              "path": [
                "Line/Search/:query"
              ],
              "query": [
                {
                  "key": "modes",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "serviceTypes",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "query",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Search for lines or routes matching the query string."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1020c3e5-bfcc-4634-acc2-36bedf890e7c"
            }
          ]
        },
        {
          "id": "cafde4d1-558c-4769-bb6b-9532f5ef936a",
          "name": "Line_StatusBySeverity",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.tfl.gov.uk",
              "path": [
                "Line/Status/:severity"
              ],
              "variable": [
                {
                  "id": "severity",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Gets the line status for all lines with a given severity\r\n            a list of valid severity codes can be obtained from a call to line/meta/severity."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3baba613-bb40-42e3-bdd7-3b8c88d52166"
            }
          ]
        },
        {
          "id": "9cdd0643-f483-4e2a-ba79-40fdd7e8c057",
          "name": "Line_Get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.tfl.gov.uk",
              "path": [
                "Line/:ids"
              ],
              "variable": [
                {
                  "id": "ids",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Gets lines that match the specified line ids.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "15e8ecf9-3f3e-4f20-ad83-f422010bfa8a"
            }
          ]
        },
        {
          "id": "6fc6ab56-2d6f-4f4b-8f59-4c85b98babce",
          "name": "Line_Arrivals",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.tfl.gov.uk",
              "path": [
                "Line/:ids/Arrivals/:stopPointId"
              ],
              "query": [
                {
                  "key": "destinationStationId",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "direction",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "ids",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "stopPointId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get the list of arrival predictions for given line ids based at the given stop."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e9d9ba19-fe0b-4051-a90c-c6b0d752cc9e"
            }
          ]
        },
        {
          "id": "60598ffb-07fb-4afd-afdb-b47cbe02dfa8",
          "name": "Line_Disruption",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.tfl.gov.uk",
              "path": [
                "Line/:ids/Disruption"
              ],
              "variable": [
                {
                  "id": "ids",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get disruptions for the given line ids."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cbd4f34a-b15d-4a14-a940-bd4c8a6331e7"
            }
          ]
        },
        {
          "id": "1e32bb00-6175-462b-ae2a-2ced38bc6230",
          "name": "Line_LineRoutesByIds",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.tfl.gov.uk",
              "path": [
                "Line/:ids/Route"
              ],
              "query": [
                {
                  "key": "serviceTypes",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "ids",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get all valid routes for given line ids, including the name and id of the originating and terminating stops for each route.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b96a7114-8f4d-481d-9ab5-b5517030d72b"
            }
          ]
        },
        {
          "id": "b76162bb-77b8-4775-9a67-54c2ab7b1e14",
          "name": "Line_StatusByIds",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.tfl.gov.uk",
              "path": [
                "Line/:ids/Status"
              ],
              "query": [
                {
                  "key": "detail",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "ids",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Gets the line status of for given line ids e.g minor delays."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4a6e41c5-1195-48b9-bee2-d00f8796a44b"
            }
          ]
        },
        {
          "id": "d75558d4-b3ee-404e-9e1f-72bdfe2ffa9f",
          "name": "Line_Status",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.tfl.gov.uk",
              "path": [
                "Line/:ids/Status/:StartDate/to/:EndDate"
              ],
              "query": [
                {
                  "key": "dateRange.endDate",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "dateRange.startDate",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "detail",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "EndDate",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "ids",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "StartDate",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "endDate",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "startDate",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Gets the line status for given line ids during the provided dates e.g minor delays."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "94975404-98a7-4d00-94f2-57a8c46bf4ad"
            }
          ]
        },
        {
          "id": "92c64d67-1b0e-44e0-8d69-0ab072cf7737",
          "name": "Line_RouteSequence",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.tfl.gov.uk",
              "path": [
                "Line/:id/Route/Sequence/:direction"
              ],
              "query": [
                {
                  "key": "excludeCrowding",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "serviceTypes",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "direction",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Gets all valid routes for given line id, including the sequence of stops on each route.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "647a91f0-d5f2-4f97-b66d-42642da7f31f"
            }
          ]
        },
        {
          "id": "7307e322-3378-4dff-889c-9d06b1b4c4e6",
          "name": "Line_StopPoints",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.tfl.gov.uk",
              "path": [
                "Line/:id/StopPoints"
              ],
              "query": [
                {
                  "key": "tflOperatedNationalRailStationsOnly",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Gets a list of the stations that serve the given line id."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "847365c3-72cf-4b63-b817-9864ef612b72"
            }
          ]
        },
        {
          "id": "a01657e5-7a5e-4105-9145-57ccbf940c3a",
          "name": "Line_Timetable",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.tfl.gov.uk",
              "path": [
                "Line/:id/Timetable/:fromStopPointId"
              ],
              "variable": [
                {
                  "id": "fromStopPointId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Gets the timetable for a specified station on the give line."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d1f6322b-c772-4a12-961a-a2098b81955d"
            }
          ]
        },
        {
          "id": "60f166fc-13e1-4054-b433-9baae1489393",
          "name": "Line_TimetableTo",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.tfl.gov.uk",
              "path": [
                "Line/:id/Timetable/:fromStopPointId/to/:toStopPointId"
              ],
              "variable": [
                {
                  "id": "fromStopPointId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "toStopPointId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Gets the timetable for a specified station on the give line with specified destination."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ab784fd7-8a1e-4bc4-b033-e3eb050901cb"
            }
          ]
        }
      ]
    },
    {
      "name": "Mode",
      "item": [
        {
          "id": "d030f0b4-ad8a-4a72-be26-aa10d98e9e12",
          "name": "Mode_GetActiveServiceTypes",
          "request": {
            "url": "http://api.tfl.gov.uk/Mode/ActiveServiceTypes",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Returns the service type active for a mode.\r\n            currently only supports tube."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "82ab0930-35e3-4084-900a-c276d1d3b341"
            }
          ]
        },
        {
          "id": "12740139-c6ac-46c1-8ae0-e2c0d3c659aa",
          "name": "Mode_Arrivals",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.tfl.gov.uk",
              "path": [
                "Mode/:mode/Arrivals"
              ],
              "query": [
                {
                  "key": "count",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "mode",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Gets the next arrival predictions for all stops of a given mode."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7ccb32e3-edf9-4f5e-9ad8-558515452e70"
            }
          ]
        }
      ]
    },
    {
      "name": "Occupancy",
      "item": [
        {
          "id": "ef0e6ac0-49b4-45f4-9d68-94933f5f6f10",
          "name": "Occupancy_GetBikePointsOccupancies",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.tfl.gov.uk",
              "path": [
                "Occupancy/BikePoints/:ids"
              ],
              "variable": [
                {
                  "id": "ids",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get the occupancy for bike points.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ff40168d-8a86-4c39-b98b-3bcb553fc92f"
            }
          ]
        },
        {
          "id": "e03da482-a766-44c7-9ef3-bd104c459a06",
          "name": "Occupancy.CarPark.get",
          "request": {
            "url": "http://api.tfl.gov.uk/Occupancy/CarPark",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Gets the occupancy for all car parks that have occupancy data."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b8bdee0d-a31a-4c7f-8cbd-394e156b9491"
            }
          ]
        },
        {
          "id": "b916eef1-4379-4cdd-9966-cdbe8019608b",
          "name": "Occupancy.CarPark.id.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.tfl.gov.uk",
              "path": [
                "Occupancy/CarPark/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Gets the occupancy for a car park with a given id."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "62280725-37ad-4218-bf7a-073d1de0482c"
            }
          ]
        },
        {
          "id": "0686e7ea-0277-4ce9-821c-bb1836da95ac",
          "name": "Occupancy_GetAllChargeConnectorStatus",
          "request": {
            "url": "http://api.tfl.gov.uk/Occupancy/ChargeConnector",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Gets the occupancy for all charge connectors."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "17b10fe3-6726-4f91-8831-d9486ecdca72"
            }
          ]
        },
        {
          "id": "495db5f2-a635-4fcf-8545-8f15ef050da1",
          "name": "Occupancy_GetChargeConnectorStatus",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.tfl.gov.uk",
              "path": [
                "Occupancy/ChargeConnector/:ids"
              ],
              "variable": [
                {
                  "id": "ids",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Gets the occupancy for a charge connectors with a given id (sourcesystemplaceid)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "aea4dfc5-7a4c-4998-b7d3-b2fd4d270674"
            }
          ]
        }
      ]
    },
    {
      "name": "Place",
      "item": [
        {
          "id": "1b23d504-f959-4724-9d14-9539472e6b23",
          "name": "Place_GetByGeoBox",
          "request": {
            "url": "http://api.tfl.gov.uk/Place?activeOnly=%7B%7D&bbBoxpoints.neLat=%7B%7D&bbBoxpoints.neLon=%7B%7D&bbBoxpoints.swLat=%7B%7D&bbBoxpoints.swLon=%7B%7D&categories=%7B%7D&includeChildren=%7B%7D&type=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Gets the places that lie within the bounding box defined by the lat/lon of its north-west and south-east corners. optionally filters\r\n            on type and can strip properties for a smaller payload.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c5c31ba9-6b26-478c-b8c6-ebac59cc511a"
            }
          ]
        },
        {
          "id": "e060993f-0aa0-40ed-8c51-d7cd5130ed39",
          "name": "Place_GetStreetsByPostCode",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.tfl.gov.uk",
              "path": [
                "Place/Address/Streets/:Postcode"
              ],
              "query": [
                {
                  "key": "postcodeInput.postcode",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "Postcode",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "postcode",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Gets the set of streets associated with a post code.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "427600ee-33da-4155-91a8-e4b6df50bc1f"
            }
          ]
        },
        {
          "id": "c438048f-487d-4212-b1ff-4cde5881b1e9",
          "name": "Place_MetaCategories",
          "request": {
            "url": "http://api.tfl.gov.uk/Place/Meta/Categories",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Gets a list of all of the available place property categories and keys.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e47ac531-edbf-4df3-bd6d-e255d6c22d13"
            }
          ]
        },
        {
          "id": "201d740a-ead6-41cc-b99c-cd7ab5ed4b95",
          "name": "Place_MetaPlaceTypes",
          "request": {
            "url": "http://api.tfl.gov.uk/Place/Meta/PlaceTypes",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Gets a list of the available types of place.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b7181752-5973-44ff-8684-8613d8c25802"
            }
          ]
        },
        {
          "id": "ce4160f6-3c10-43a4-b414-dcd505ca8cc8",
          "name": "Place_Search",
          "request": {
            "url": "http://api.tfl.gov.uk/Place/Search?name=%7B%7D&types=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Gets all places that matches the given query."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "143b0d09-9577-40b8-9964-292b61a8104a"
            }
          ]
        },
        {
          "id": "ffb24780-4393-44b0-b11b-8f76bb319019",
          "name": "Place_GetByType",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.tfl.gov.uk",
              "path": [
                "Place/Type/:types"
              ],
              "query": [
                {
                  "key": "activeOnly",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "types",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Gets all places of a given type."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0678ca93-54d8-4cbe-8267-753453929bf8"
            }
          ]
        },
        {
          "id": "656b615c-bb45-4612-bdce-29e1e60167bf",
          "name": "Place_Get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.tfl.gov.uk",
              "path": [
                "Place/:id"
              ],
              "query": [
                {
                  "key": "includeChildren",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Gets the place with the given id.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0ca6031f-8e85-4a44-a004-e714e06a1748"
            }
          ]
        },
        {
          "id": "24d27c96-f0a4-426d-a600-24109ac6389b",
          "name": "Place_GetAt",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.tfl.gov.uk",
              "path": [
                "Place/:type/At/:Lat/:Lon"
              ],
              "query": [
                {
                  "key": "location.lat",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "location.lon",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "Lat",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "Lon",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "type",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "lat",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "lon",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Gets any places of the given type whose geography intersects the given latitude and longitude. in practice this means the place\r\n            must be polygonal e.g. a boroughboundary.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1a1ac524-8b46-451a-bd87-3e24e353a598"
            }
          ]
        },
        {
          "id": "47c4c90c-c758-490b-9978-ac0855f8cd07",
          "name": "Place_GetOverlay",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.tfl.gov.uk",
              "path": [
                "Place/:type/overlay/:z/:Lat/:Lon/:width/:height"
              ],
              "query": [
                {
                  "key": "location.lat",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "location.lon",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "height",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "Lat",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "Lon",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "type",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "width",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "z",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "lat",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "lon",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Gets the place overlay for a given set of co-ordinates and a given width/height.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7ec37193-a6e0-43ed-bfb7-c3ab366a8f6a"
            }
          ]
        }
      ]
    },
    {
      "name": "Road",
      "item": [
        {
          "id": "54cdca10-0b5d-4b08-bdc0-594b26cc72de",
          "name": "Road.get",
          "request": {
            "url": "http://api.tfl.gov.uk/Road",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Gets all roads managed by tfl."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "678765bf-319f-4c1d-aacb-e97dc87b856e"
            }
          ]
        },
        {
          "id": "10f5e368-7c52-4e19-b3f1-417beeb79368",
          "name": "Road_MetaCategories",
          "request": {
            "url": "http://api.tfl.gov.uk/Road/Meta/Categories",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Gets a list of valid roaddisruption categories."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bb1acc0a-fe52-437e-8282-33cdc507885d"
            }
          ]
        },
        {
          "id": "56b7e569-c168-4934-a30f-60bd2da860d7",
          "name": "Road_MetaSeverities",
          "request": {
            "url": "http://api.tfl.gov.uk/Road/Meta/Severities",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Gets a list of valid roaddisruption severity codes."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c320cc00-a1cc-41c6-9a80-9fb06fe4ef32"
            }
          ]
        },
        {
          "id": "150522c3-e98d-48b0-9427-12f898ae9d80",
          "name": "Road_DisruptionById",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.tfl.gov.uk",
              "path": [
                "Road/all/Disruption/:disruptionIds"
              ],
              "query": [
                {
                  "key": "stripContent",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "disruptionIds",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Gets a list of active disruptions filtered by disruption ids.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "19e52f16-d24d-4a7b-85b9-510820f551ba"
            }
          ]
        },
        {
          "id": "ebd60356-7443-4f63-bea7-3623faa38178",
          "name": "Road_DisruptedStreets",
          "request": {
            "url": "http://api.tfl.gov.uk/Road/all/Street/Disruption?endDate=%7B%7D&startDate=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Gets a list of disrupted streets. if no date filters are provided, current disruptions are returned.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f63648ec-483d-4d7b-a76f-f674c6ac1610"
            }
          ]
        },
        {
          "id": "9acd4107-73c1-494b-ba62-6c63d0c287a0",
          "name": "Road.ids.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.tfl.gov.uk",
              "path": [
                "Road/:ids"
              ],
              "variable": [
                {
                  "id": "ids",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Gets the road with the specified id (e.g. a1)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "54a19f0b-ca21-4348-b77e-f16d2dd61a5a"
            }
          ]
        },
        {
          "id": "3d52b10a-666a-4640-aedd-9581dd86bf87",
          "name": "Road_Disruption",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.tfl.gov.uk",
              "path": [
                "Road/:ids/Disruption"
              ],
              "query": [
                {
                  "key": "categories",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "closures",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "severities",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "stripContent",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "ids",
                  "value": "{}",