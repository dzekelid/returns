swagger: "2.0"
x-collection-name: AWS EC2
x-complete: 1
info:
  title: AWS EC2 API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=GetReservedInstancesExchangeQuote:
    get:
      summary: Get Reserved Instances Exchange Quote
      description: Returns details about the values and term of your specified Convertible
        Reserved Instances.
      operationId: getreservedinstancesexchangequote
      x-api-path-slug: actiongetreservedinstancesexchangequote-get
      parameters:
      - in: query
        name: ClientToken
        description: A unique, case-sensitive token you provide to ensure idempotency
          of your modification request
        type: string
      - in: query
        name: ReservedInstancesConfigurationSetItemType.N
        description: The configuration settings for the Reserved Instances to modify
        type: string
      - in: query
        name: ReservedInstancesId.N
        description: The IDs of the Reserved Instances to modify
        type: string
      responses:
        200:
          description: OK
      tags:
      - Reserved Instances