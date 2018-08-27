swagger: "2.0"
x-collection-name: Broadleaf Commerce
x-complete: 1
info:
  title: Broadleaf Commerce API
  description: the-default-broadleaf-commerce-apis
  version: 1.0.0
host: demo.broadleafcommerce.org
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /cart/checkout:
    post:
      summary: Post Cart Checkout
      description: Post cart checkout.
      operationId: postCartCheckout
      x-api-path-slug: cartcheckout-post
      parameters:
      - in: query
        name: cartId
        description: cartId
      responses:
        200:
          description: OK
      tags:
      - Cart
      - Checkout
  /cart/checkout/payment:
    post:
      summary: Post Cart Checkout Payment
      description: Post cart checkout payment.
      operationId: postCartCheckoutPayment
      x-api-path-slug: cartcheckoutpayment-post
      parameters:
      - in: query
        name: cartId
        description: cartId
      - in: body
        name: wrapper
        description: wrapper
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Cart
      - Checkout
      - Payment
  /cart/checkout/payment/{customerPaymentId}:
    post:
      summary: Post Cart Checkout Payment Customerpaymentid
      description: Post cart checkout payment customerpaymentid.
      operationId: postCartCheckoutPaymentCustomerpayment
      x-api-path-slug: cartcheckoutpaymentcustomerpaymentid-post
      parameters:
      - in: query
        name: amount
        description: amount
      - in: query
        name: cartId
        description: cartId
      - in: query
        name: currency
        description: currency
      - in: path
        name: customerPaymentId
        description: customerPaymentId
      responses:
        200:
          description: OK
      tags:
      - Cart
      - Checkout
      - Payment
      - Customerpaymentid
  /cart/checkout/payment/{paymentId}:
    delete:
      summary: Delete Cart Checkout Payment Paymentid
      description: Delete cart checkout payment paymentid.
      operationId: deleteCartCheckoutPaymentPayment
      x-api-path-slug: cartcheckoutpaymentpaymentid-delete
      parameters:
      - in: query
        name: cartId
        description: cartId
      - in: path
        name: paymentId
        description: paymentId
      responses:
        200:
          description: OK
      tags:
      - Cart
      - Checkout
      - Payment
      - Paymentid
  /cart/checkout/payment/{paymentId}/transaction:
    put:
      summary: Put Cart Checkout Payment Paymentid Transaction
      description: Put cart checkout payment paymentid transaction.
      operationId: putCartCheckoutPaymentPaymentTransaction
      x-api-path-slug: cartcheckoutpaymentpaymentidtransaction-put
      parameters:
      - in: query
        name: cartId
        description: cartId
      - in: path
        name: paymentId
        description: paymentId
      - in: body
        name: wrapper
        description: wrapper
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Cart
      - Checkout
      - Payment
      - Paymentid
      - Transaction
  /cart/checkout/payments:
    get:
      summary: Get Cart Checkout Payments
      description: Get cart checkout payments.
      operationId: getCartCheckoutPayments
      x-api-path-slug: cartcheckoutpayments-get
      parameters:
      - in: query
        name: cartId
        description: cartId
      responses:
        200:
          description: OK
      tags:
      - Cart
      - Checkout
      - Payments