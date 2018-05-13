{
  "info": {
    "name": "BetterDoctor Doctor search",
    "_postman_id": "7d8ec872-b7f4-460e-aa33-b0fc2688b2e2",
    "description": "Doctor search",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "doctor",
      "item": [
        {
          "id": "0352433a-1a8c-4ca0-a080-5e60145b3a5a",
          "name": "doctor-search",
          "request": {
            "url": "http://api.betterdoctor.com/2016-03-01/doctors?fields=%7B%7D&first_name=%7B%7D&gender=%7B%7D&insurance_uid=%7B%7D&last_name=%7B%7D&limit=%7B%7D&location=%7B%7D&name=%7B%7D&practice_uid=%7B%7D&query=%7B%7D&skip=%7B%7D&sort=%7B%7D&specialty_uid=%7B%7D&user_key=%7B%7D&user_location=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Doctor search"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7c3b5e47-9514-4297-8ae9-1ec15e58bda1"
            }
          ]
        }
      ]
    }
  ]
}