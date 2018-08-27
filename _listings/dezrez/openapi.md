swagger: "2.0"
x-collection-name: Dezrez
x-complete: 1
info:
  title: Dezrez.Rezi.Client.Api
  version: 1.0.0
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/property/{id}/keys/checkout:
    put:
      summary: Checkout a collection of keys for a property
      description: Checkout a collection of keys for a property.
      operationId: Property_CheckoutKeysByidBycheckoutDetails
      x-api-path-slug: apipropertyidkeyscheckout-put
      parameters:
      - in: body
        name: checkoutDetails
        description: The details of the keys to checkout
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: The property id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Checkout
      - Collection
      - Of
      - Keysa
      - Property