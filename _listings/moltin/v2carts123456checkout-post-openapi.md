---
swagger: "2.0"
x-collection-name: moltin
x-complete: 0
info:
  title: Moltin API Checkout using customer id
  description: |-
    Converts a cart to an incomplete order. The original cart will remain and can be modified and checked out again if required.

    The new order will be returned and `data.meta.payment_gateways` will contain an array of the available payment gateways for this order.
  version: 1.0.0
host: api.moltin.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v2/carts/123456/checkout:
    post:
      summary: Checkout using customer id
      description: |-
        Converts a cart to an incomplete order. The original cart will remain and can be modified and checked out again if required.

        The new order will be returned and `data.meta.payment_gateways` will contain an array of the available payment gateways for this order.
      operationId: V2Carts123456CheckoutPost2
      x-api-path-slug: v2carts123456checkout-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Checkout
      - Using
      - Customer
      - Id
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---