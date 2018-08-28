{
  "info": {
    "name": "Plentymarkets Search variations",
    "_postman_id": "e8c77d3f-70f7-4be2-a85d-2da72246f10d",
    "description": "Search variations by different filters",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Search",
      "item": [
        {
          "id": "52b7c9b8-5931-41db-a36d-64025bb55d67",
          "name": "getRestItemsVariations",
          "request": {
            "url": "http://example.com/rest/items/variations?barcode=%7B%7D&categoryId=%7B%7D&createdBetween=%7B%7D&flagOne=%7B%7D&flagTwo=%7B%7D&id=%7B%7D&isActive=%7B%7D&isBundle=%7B%7D&isMain=%7B%7D&itemId=%7B%7D&itemName=%7B%7D&itemsPerPage=%7B%7D&itemTagId=%7B%7D&lang=%7B%7D&manufacturerId=%7B%7D&numberExact=%7B%7D&numberFuzzy=%7B%7D&page=%7B%7D&plentyId=%7B%7D&relatedUpdatedBetween=%7B%7D&sku=%7B%7D&storeSpecial=%7B%7D&supplierNumber=%7B%7D&updatedBetween=%7B%7D&with=%7B%7D",
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
            "description": "Search variations by different filters"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0254471e-8b5b-4025-a5fe-3319d93a936d"
            }
          ]
        }
      ]
    }
  ]
}