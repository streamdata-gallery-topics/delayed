---
swagger: "2.0"
x-collection-name: Xignite
x-complete: 0
info:
  title: Xignite Futures Get Delayed Future
  description: Returns a delayed quote for a future contract.
  version: 1.0.0
host: www.xignite.com
basePath: xFutures.json/XigniteFutures
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /GetDelayedSwap:
    get:
      summary: Get Delayed Swap
      description: Returns a delayed quote for a NYMEX swap contract.
      operationId: postGetdelayedswap
      x-api-path-slug: getdelayedswap-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Delayed
      - Swap
  /GetDelayedFuture:
    get:
      summary: Get Delayed Future
      description: Returns a delayed quote for a future contract.
      operationId: postGetdelayedfuture
      x-api-path-slug: getdelayedfuture-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Delayed
      - Future
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