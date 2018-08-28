{
  "info": {
    "name": "Data.gov API Delete Reuses Reuse Badges Badge Kind",
    "_postman_id": "c0c40e19-4b6e-43b4-bf97-4adef339560b",
    "description": "Delete a badge for a given reuse",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "reuses",
      "item": [
        {
          "id": "48ecc936-461d-4cb1-be6e-f935732a359a",
          "name": "deleteReusesReuseBadgesBadgeKind",
          "request": {
            "url": {
              "protocol": "http",
              "host": "catalog.data.gov",
              "path": [
                "api",
                "3",
                "reuses/:reuse/badges/:badge_kind/"
              ],
              "variable": [
                {
                  "id": "badge_kind",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "reuse",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete a badge for a given reuse"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1514816c-d17d-4552-a1cb-aa99bc198dfc"
            }
          ]
        }
      ]
    }
  ]
}