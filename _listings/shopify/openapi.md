swagger: "2.0"
x-collection-name: Shopify
x-complete: 1
info:
  title: Shopify API
  description: todo-add-description
  version: 1.0.0
host: DefaultParameterValue:DefaultParameterValue@DefaultParameterValue.myshopify.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /admin/checkouts.json:
    get:
      summary: List all abandoned checkouts
      description: List all abandoned checkouts.
      operationId: getAdminCheckouts.json
      x-api-path-slug: admincheckouts-json-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - List
      - Abandoned
      - Checkouts
  /admin/checkouts/count.json:
    get:
      summary: Get a count of checkouts
      description: Get a count of checkouts.
      operationId: getAdminCheckoutsCount.json
      x-api-path-slug: admincheckoutscount-json-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Count
      - Checkouts