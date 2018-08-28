{
  "info": {
    "name": "IDX Broker Get Search Query",
    "_postman_id": "d8a8d14b-5db0-42ef-ada7-7395861c7b74",
    "description": "Performs search and returns the results.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Approved",
      "item": [
        {
          "id": "219ef705-abc4-456a-8376-5bc23017b729",
          "name": "MlsApprovedmlsGet",
          "request": {
            "url": "http://example.com/mls/approvedmls",
            "method": "GET",
            "header": [
              {
                "key": "accesskey",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "ancillarykey",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "apiversion",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "outputtype",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "This method provides all of the IDX IDs and names for all of the paperwork approved MLSs on the client's account.\n\nNote: This method was previously camelcased as \"approvedMLS\" but was made lower case to fit the API naming convention. Calls to \"approvedMLS\" will be forwarded to \"approvedmls\" and \"approvedMLS\" is listed as deprecated in the method list."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d41a4228-54f5-4659-9f0b-d1ddf1e2e6cc"
            }
          ]
        }
      ]
    },
    {
      "name": "Mls",
      "item": [
        {
          "id": "73b95437-f0fe-4daa-8e2c-c07e0dee556d",
          "name": "MlsAgeByApprovedMLSGet",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "mls/age/:approvedMLS"
              ],
              "variable": [
                {
                  "id": "approvedMLS",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "accesskey",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "ancillarykey",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "apiversion",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "outputtype",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "TODO: Add Description"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f3a6e413-4948-4ad3-9200-f9f7244fc2ab"
            }
          ]
        },
        {
          "id": "58d0f4af-69cc-46de-899d-d48502c1306d",
          "name": "MlsCitiesByApprovedMLSGet",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "mls/cities/:approvedMLS"
              ],
              "variable": [
                {
                  "id": "approvedMLS",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "accesskey",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "ancillarykey",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "apiversion",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "outputtype",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "All cities represented in the current set of MLS data are available from this method."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ca761a77-923f-4790-a702-1f93d0b2396b"
            }
          ]
        },
        {
          "id": "aae9f127-f4f5-457f-b370-bbe9820fa64a",
          "name": "MlsListcomponentsGet",
          "request": {
            "url": "http://example.com/mls/listcomponents",
            "method": "GET",
            "header": [
              {
                "key": "accesskey",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "ancillarykey",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "apiversion",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "outputtype",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "This is a simple, access anywhere, method for getting a list of all API components available."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "794dfb54-df00-4334-a553-8f4e1f23cdce"
            }
          ]
        },
        {
          "id": "42b84c1d-0782-49a7-9c5c-76dc54be3dff",
          "name": "MlsListmethodsGet",
          "request": {
            "url": "http://example.com/mls/listmethods",
            "method": "GET",
            "header": [
              {
                "key": "accesskey",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "ancillarykey",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "apiversion",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "outputtype",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "A simple method for listing all available methods in the current API component. This method will also list which request methods (GET, PUT, POST, or DELETE) are supported by each method in addition to each method status."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f627c497-822e-44ab-8552-1e04878a9c99"
            }
          ]
        },
        {
          "id": "306d3ff6-905a-4f9b-a354-4b44082772cd",
          "name": "MlsPostalcodesByApprovedMLSGet",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "mls/postalcodes/:approvedMLS"
              ],
              "variable": [
                {
                  "id": "approvedMLS",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "accesskey",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "ancillarykey",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "apiversion",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "outputtype",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "All postal codes represented in the current set of MLS data are available from this method."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "72ad3eaf-d0be-480a-9949-2f94a0384aad"
            }
          ]
        },
        {
          "id": "ef4c2fc2-e9b8-4770-8f41-d1ba9992de69",
          "name": "MlsPricesByApprovedMLSGet",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "mls/prices/:approvedMLS"
              ],
              "variable": [
                {
                  "id": "approvedMLS",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "accesskey",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "ancillarykey",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "apiversion",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "outputtype",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "The sum total of properties listed in a given MLS as well as sums for each property type in the MLS."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4e903aaa-744d-4c7c-a627-eb602d616687"
            }
          ]
        },
        {
          "id": "0d461c86-1f86-4d0b-8eab-433ffcbe3e83",
          "name": "MlsPropertycountByApprovedMLSGet",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "mls/propertycount/:approvedMLS"
              ],
              "query": [
                {
                  "key": "countSpecifier",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "countType",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "approvedMLS",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "accesskey",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "ancillarykey",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "apiversion",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "outputtype",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Gives a total number of listings available for a given city, county, or zipcode"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d24834e5-4432-415a-b3ce-014f29fbb31a"
            }
          ]
        },
        {
          "id": "0e570058-2dcc-4eb1-80a6-14eb11d1115d",
          "name": "MlsPropertytypesByApprovedMLSGet",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "mls/propertytypes/:approvedMLS"
              ],
              "variable": [
                {
                  "id": "approvedMLS",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "accesskey",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "ancillarykey",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "apiversion",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "outputtype",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Gives the property type information for all types that are available on a given MLS."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a30f30ba-a4eb-44a8-b572-785c4ee536db"
            }
          ]
        },
        {
          "id": "4021dfe0-d740-485b-9bf5-76c9a9e9a207",
          "name": "MlsSearchfieldsByApprovedMLSGet",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "mls/searchfields/:approvedMLS"
              ],
              "variable": [
                {
                  "id": "approvedMLS",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "accesskey",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "ancillarykey",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "apiversion",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "outputtype",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "All the fields in a given MLS that are currently allowed to be searched according to MLS guidelines."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "83fa9759-1b40-43e0-827b-f0c63816637b"
            }
          ]
        },
        {
          "id": "327a4e86-9d0a-4fc0-886e-39adf24d5ffd",
          "name": "MlsSearchfieldvaluesByApprovedMLSGet",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "mls/searchfieldvalues/:approvedMLS"
              ],
              "query": [
                {
                  "key": "mlsPtID",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "approvedMLS",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "accesskey",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "ancillarykey",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "apiversion",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "outputtype",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Field values in a given MLS that are currently allowed to be searched according to MLS guidelines."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "41fe8dfc-731f-406d-a902-d9449ca006c4"
            }
          ]
        },
        {
          "id": "630397ca-2dd9-4200-a9b5-eefca7a77931",
          "name": "MlsZipcodesByApprovedMLSGet",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "mls/zipcodes/:approvedMLS"
              ],
              "variable": [
                {
                  "id": "approvedMLS",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "accesskey",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "ancillarykey",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "apiversion",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "outputtype",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "All zip codes represented in the current set of MLS data are available from this method."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "31b5f5f9-bb85-47a3-bcc1-d6bf6b267ae1"
            }
          ]
        }
      ]
    },
    {
      "name": "Agents",
      "item": [
        {
          "id": "8290d122-d6f1-463a-aab7-35038ae814f7",
          "name": "ClientsAgentsGet",
          "request": {
            "url": "http://example.com/clients/agents",
            "method": "GET",
            "header": [
              {
                "key": "accesskey",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "ancillarykey",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "apiversion",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "outputtype",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "View agent information on a multi-user account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ed4f6d4b-8b27-425f-8142-496b5b853b63"
            }
          ]
        }
      ]
    },
    {
      "name": "Apiversion",
      "item": [
        {
          "id": "9e7396f7-89e6-46be-8185-dbfc0f4621f9",
          "name": "ClientsApiversionGet",
          "request": {
            "url": "http://example.com/clients/apiversion",
            "method": "GET",
            "header": [
              {
                "key": "accesskey",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "ancillarykey",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "apiversion",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "outputtype",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get the default api version."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "068ac67e-a535-46bf-ac54-fd32d8599127"
            }
          ]
        }
      ]
    },
    {
      "name": "Cities",
      "item": [
        {
          "id": "af73105e-89c3-43c7-99be-cf707a16fab4",
          "name": "ClientsCitiesGet",
          "request": {
            "url": "http://example.com/clients/cities",
            "method": "GET",
            "header": [
              {
                "key": "accesskey",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "ancillarykey",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "apiversion",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "outputtype",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Returns the cities available in each of a client's city lists."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9be6f11a-3bd5-4cdf-aa4c-7b9f5750b2bf"
            }
          ]
        },
        {
          "id": "4a568e96-b252-428f-b7b8-6b65ca360af4",
          "name": "ClientsCitieslistnameGet",
          "request": {
            "url": "http://example.com/clients/citieslistname",
            "method": "GET",
            "header": [
              {
                "key": "accesskey",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "ancillarykey",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "apiversion",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "outputtype",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Returns the IDs and names for each of a client's city lists including MLS city lists."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b57923e0-8c90-495f-83fe-d55d91870318"
            }
          ]
        }
      ]
    },
    {
      "name": "Counties",
      "item": [
        {
          "id": "a19f0d33-1bde-497b-aa41-174dff221f2b",
          "name": "ClientsCountiesGet",
          "request": {
            "url": "http://example.com/clients/counties",
            "method": "GET",
            "header": [
              {
                "key": "accesskey",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "ancillarykey",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "apiversion",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "outputtype",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Returns the counties available in each of a client's county lists."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3a8b6b1a-6d05-44a1-98d6-e1b7c4a71dff"
            }
          ]
        }
      ]
    },
    {
      "name": "Countieslistname",
      "item": [
        {
          "id": "b2c63bae-e026-4b7d-862f-717f8785435d",
          "name": "ClientsCountieslistnameGet",
          "request": {
            "url": "http://example.com/clients/countieslistname",
            "method": "GET",
            "header": [
              {
                "key": "accesskey",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "ancillarykey",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "apiversion",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "outputtype",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Returns the IDs and names for each of a client's counties lists including MLS counties lists."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "37f3ed70-6a18-4367-a2a8-dcee3b14a473"
            }
          ]
        }
      ]
    },
    {
      "name": "Dynamicwrapperurl",
      "item": [
        {
          "id": "fc8b009a-3062-4e7e-a1f1-c0e91eeda847",
          "name": "ClientsDynamicwrapperurlPost",
          "request": {
            "url": "http://example.com/clients/dynamicwrapperurl",
            "method": "POST",
            "header": [
              {
                "key": "accesskey",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "apiversion",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "outputtype",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "dynamicURL",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                }
              ]
            },
            "description": "Set wrapper URL. This is the global url."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f1c045e5-42fd-48b4-baa3-80fdd47aa234"
            }
          ]
        }
      ]
    },
    {
      "name": "Featured",
      "item": [
        {
          "id": "1ea4e0bf-19c4-4441-a42c-f25f938bf1c9",
          "name": "ClientsFeaturedGet",
          "request": {
            "url": "http://example.com/clients/featured",
            "method": "GET",
            "header": [
              {
                "key": "accesskey",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "ancillarykey",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "apiversion",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "outputtype",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Returns a basic set of information for all of the client's featured (active) properties"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "708ecfbb-2d48-4ac9-80d8-638f576f3405"
            }
          ]
        }
      ]
    },
    {
      "name": "List",
      "item": [
        {
          "id": "948a0d58-776b-4622-bea0-2f2fbdd943b0",
          "name": "ClientsListallowedfieldsByApprovedMLSAndFeaturedIdGet",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "clients/listallowedfields/:approvedMLS/:featuredId"
              ],
              "variable": [
                {
                  "id": "approvedMLS",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "featuredId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "accesskey",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "ancillarykey",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "apiversion",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "outputtype",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Returns the allowed returnable fields for a given listingID."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "44cfe4e2-65c8-4b43-ae80-9b176bfcd740"
            }
          ]
        },
        {
          "id": "3351f832-4cdd-46c3-9cab-3326706f5ad4",
          "name": "ClientsListmethodsGet",
          "request": {
            "url": "http://example.com/clients/listmethods",
            "method": "GET",
            "header": [
              {
                "key": "accesskey",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "ancillarykey",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "apiversion",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "outputtype",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "A simple method for listing all available methods in the current API component."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "69c77abc-f3d9-402b-9443-ac33847b054f"
            }
          ]
        }
      ]
    },
    {
      "name": "Listcomponents",
      "item": [
        {
          "id": "988c3ea7-2fa1-4b6d-85e0-1dfad431a150",
          "name": "ClientsListcomponentsGet",
          "request": {
            "url": "http://example.com/clients/listcomponents",
            "method": "GET",
            "header": [
              {
                "key": "accesskey",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "ancillarykey",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "apiversion",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "outputtype",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "This is a simple, access anywhere, method for getting a list of all API components available."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "561b0431-c1f8-4f4e-b038-4819a2b387db"
            }
          ]
        }
      ]
    },
    {
      "name": "Listing",
      "item": [
        {
          "id": "64eda97e-3085-4f4a-be81-8797a58497fa",
          "name": "ClientsListingByApprovedMLSAndFeaturedIdGet",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "clients/listing/:approvedMLS/:featuredId"
              ],
              "variable": [
                {
                  "id": "approvedMLS",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "featuredId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "accesskey",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "ancillarykey",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "apiversion",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "outputtype",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Returns the detailed information for a given listingID."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "73b71c46-dfbb-46ce-9cbb-593c4c48185a"
            }
          ]
        }
      ]
    },
    {
      "name": "Offices",
      "item": [
        {
          "id": "55c6be38-626e-4c6c-8f32-323c90849b70",
          "name": "ClientsOfficesGet",
          "request": {
            "url": "http://example.com/clients/offices",
            "method": "GET",
            "header": [
              {
                "key": "accesskey",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "ancillarykey",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "apiversion",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "outputtype",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "View all offices on a mutli-user account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "041db484-70dc-49a4-8a89-51c8af562aae"
            }
          ]
        }
      ]
    },
    {
      "name": "Alcodes",
      "item": [
        {
          "id": "ee8cff15-2599-4839-8ba6-c0542bff3a29",
          "name": "ClientsPostalcodesGet",
          "request": {
            "url": "http://example.com/clients/postalcodes",
            "method": "GET",
            "header": [
              {
                "key": "accesskey",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "ancillarykey",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "apiversion",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "outputtype",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Returns the postalcodes available in each of a client's postalcode lists."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "64e611c6-e283-4fd2-a3d9-b88d6e0f777a"
            }
          ]
        }
      ]
    },
    {
      "name": "Alcodeslistname",
      "item": [
        {
          "id": "90e66990-2949-477c-893d-e2a3be25bf88",
          "name": "ClientsPostalcodeslistnameGet",
          "request": {
            "url": "http://example.com/clients/postalcodeslistname",
            "method": "GET",
            "header": [
              {
                "key": "accesskey",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "ancillarykey",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "apiversion",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "outputtype",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Returns the IDs and names for each of a client's postalcode lists including MLS postalcode lists."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "59a8a377-dbfb-4883-b477-bc5f70bd8e95"
            }
          ]
        }
      ]
    },
    {
      "name": "Saved",
      "item": [
        {
          "id": "4ca9c729-6441-4263-a666-30ba4705e2df",
          "name": "ClientsSavedlinksGet",
          "request": {
            "url": "http://example.com/clients/savedlinks",
            "method": "GET",
            "header": [
              {
                "key": "accesskey",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "ancillarykey",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "apiversion",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "outputtype",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Getclient saved links"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "06cbc3ed-69ba-49c7-aa02-089f3ec8f9d1"
            }
          ]
        },
        {
          "id": "de47f775-d9fc-40f6-bc69-49cf1f93f89d",
          "name": "ClientsSavedlinksPut",
          "request": {
            "url": "http://example.com/clients/savedlinks",
            "method": "PUT",
            "header": [
              {
                "key": "accesskey",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "ancillarykey",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "apiversion",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "outputtype",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "linkName",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "linkTitle",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "pageTitle",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "queryString[hp]",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "queryString[idxID]",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                }
              ]
            },
            "description": "Create a new client saved link"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0e683d69-d490-4b0c-b35c-ef0375093910"
            }
          ]
        },
        {
          "id": "5bb5a7a3-1c95-4a4f-b836-21d88725dc4b",
          "name": "ClientsSavedlinksBySavedLinkIdPost",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "clients/savedlinks/:savedLinkId"
              ],
              "variable": [
                {
                  "id": "savedLinkId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "header": [
              {
                "key": "accesskey",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "ancillarykey",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "apiversion",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "outputtype",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "linkName",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "linkTitle",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "pageTitle",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "queryString[hp]",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "queryString[idxID]",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                }
              ]
            },
            "description": "Update a client saved link"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "83503aae-4d4c-4b43-a638-d64088de301d"
            }
          ]
        },
        {
          "id": "d99416be-6e69-4c72-ad04-6575e76e63d0",
          "name": "ClientsSavedlinksBySavedLinkIdDelete",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "clients/savedlinks/:savedLinkId"
              ],
              "variable": [
                {
                  "id": "savedLinkId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "header": [
              {
                "key": "accesskey",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "ancillarykey",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "apiversion",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "outputtype",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "linkName",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "linkTitle",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "pageTitle",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "queryString[hp]",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "queryString[idxID]",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                }
              ]
            },
            "description": "Delete a client saved link"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6c60ab1b-f594-4a36-bf1e-c67a96210a7c"
            }
          ]
        }
      ]
    },
    {
      "name": "Properties",
      "item": [
        {
          "id": "4bbf9c11-7b5f-47d2-be57-0be379bb1b29",
          "name": "ClientsPropertiesBySavedLinkIdGet",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "clients/properties/:savedLinkId"
              ],
              "variable": [
                {
                  "id": "savedLinkId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "accesskey",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "ancillarykey",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "apiversion",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "outputtype",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get client saved links results"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0be7cb5c-fe24-4a82-b725-fffc7c713a78"
            }
          ]
        }
      ]
    },
    {
      "name": "Search",
      "item": [
        {
          "id": "28f090e7-b9f4-4fe8-9392-4ab1a8a02596",
          "name": "ClientsSearchqueryGet",
  