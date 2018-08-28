{
  "info": {
    "name": "IDX Broker Get Mls Search Field Values Approved MLS",
    "_postman_id": "d2243072-c79f-47e6-af98-367ad3c1b701",
    "description": "Field values in a given MLS that are currently allowed to be searched according to MLS guidelines.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Approved",
      "item": [
        {
          "id": "15aef551-5871-453a-967c-c131250ae123",
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
              "id": "cbf3a0be-af7e-4187-85b8-5d5aa2e135b8"
            }
          ]
        }
      ]
    },
    {
      "name": "Mls",
      "item": [
        {
          "id": "68640b7d-dc4e-41f1-a406-9245c62fd99f",
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
              "id": "80f7854b-3058-4f8d-b583-add1e71b2877"
            }
          ]
        },
        {
          "id": "7e78ca94-6651-4751-bf2f-f9ff0e860282",
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
              "id": "969a45c5-22c4-4a7a-a25e-d60aeaaeb271"
            }
          ]
        },
        {
          "id": "beb7d033-7ce2-4cb2-b198-4bb4dc24fd43",
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
              "id": "d5db7441-4c81-453a-b92b-bea7f0a6c239"
            }
          ]
        },
        {
          "id": "ba1eb73b-6aad-4c56-9847-d90145f419b0",
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
              "id": "17b99bf6-9b92-451f-8f1b-d9240ec8fa3f"
            }
          ]
        },
        {
          "id": "36026bf6-0787-490d-a174-783b8d2835a9",
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
              "id": "db4f4d67-ec3b-40af-92c3-51c5016d3156"
            }
          ]
        },
        {
          "id": "0ddc84b4-7ce2-4272-a178-7d955da0ef7d",
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
              "id": "cac8c8d6-dafa-45c3-bdb6-3ccb3a166041"
            }
          ]
        },
        {
          "id": "8462e1e9-795c-4c20-abd7-2f5c6b28cf9a",
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
              "id": "1a2460e8-4034-42e1-a947-c19007e7653a"
            }
          ]
        },
        {
          "id": "43083df8-1548-4860-8320-5ee617dabd3f",
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
              "id": "9dcd4156-9440-4c5a-868b-34d3607a9719"
            }
          ]
        },
        {
          "id": "3a38f697-27f6-4642-b7a4-ebe7c8487368",
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
              "id": "42f2ccb0-46bc-46c0-bc23-cf434e443a6f"
            }
          ]
        }
      ]
    },
    {
      "name": "List",
      "item": [
        {
          "id": "93ab7a1f-8960-4b92-a8eb-8d3d15a8e506",
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
              "id": "2d796567-b032-4baf-8ea0-3eac10c5260e"
            }
          ]
        }
      ]
    },
    {
      "name": "Listing",
      "item": [
        {
          "id": "60c8bd6f-4005-41de-9dd2-755d6d45d6fc",
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
              "id": "62b8d52c-ccc1-40bb-94da-cf56576a37b2"
            }
          ]
        }
      ]
    }
  ]
}