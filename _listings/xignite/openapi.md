swagger: "2.0"
x-collection-name: Xignite
x-complete: 1
info:
  title: Xignite VWAP
  description: provides-delayed-and-historical-volumeweightedaverage-price-vwap-information-
  version: 1.0.0
host: www.xignite.com
basePath: xVWAP.json/XigniteVWAP
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
  /GetDelayedFrontFuture:
    get:
      summary: Get Delayed Front Future
      description: Returns a delayed quote for a future contract.
      operationId: postGetdelayedfrontfuture
      x-api-path-slug: getdelayedfrontfuture-get
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
      - Front
      - Future
  /GetAllDelayedFutures:
    get:
      summary: Get All Delayed Futures
      description: Returns delayed quotes for all contracts for a commodity.
      operationId: postGetalldelayedfutures
      x-api-path-slug: getalldelayedfutures-get
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
      - Futures
  /GetTopDelayedFutures:
    get:
      summary: Get Top Delayed Futures
      description: Returns delayed quotes for a given number of contract (front-future
        first) for a commodity.
      operationId: postGettopdelayedfutures
      x-api-path-slug: gettopdelayedfutures-get
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
      - Top
      - Delayed
      - Futures
  /GetAllDelayedSwaps:
    get:
      summary: Get All Delayed Swaps
      description: Returns delayed quotes for all contracts for a commodity.
      operationId: postGetalldelayedswaps
      x-api-path-slug: getalldelayedswaps-get
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
      - Swaps
  /GetDelayedFutures:
    get:
      summary: Get Delayed Futures
      description: Returns delayed quotes for multiple future contracts.
      operationId: postGetdelayedfutures
      x-api-path-slug: getdelayedfutures-get
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
      - Futures
  /GetDelayedFutureStrip:
    get:
      summary: Get Delayed Future Strip
      description: Returns a delayed future strip for a commodity.
      operationId: postGetdelayedfuturestrip
      x-api-path-slug: getdelayedfuturestrip-get
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
      - Strip
  /GetDelayedSpot:
    get:
      summary: Get Delayed Spot
      description: Returns a delayed spot quote for a commodity.
      operationId: postGetdelayedspot
      x-api-path-slug: getdelayedspot-get
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
      - Spot
  /GetDelayedSpots:
    get:
      summary: Get Delayed Spots
      description: Returns delayed quotes for multiple commodities.
      operationId: postGetdelayedspots
      x-api-path-slug: getdelayedspots-get
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
      - Spots
  /GetDelayedFutureBySession:
    get:
      summary: Get Delayed Future By Session
      description: Returns a delayed quote for a future contract by exchange session.
      operationId: postGetdelayedfuturebysession
      x-api-path-slug: getdelayedfuturebysession-get
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
      - By
      - Session
  /GetAllDelayedFuturesBySession:
    get:
      summary: Get All Delayed Futures By Session
      description: Returns delayed quotes for all contracts for a commodity by exchange
        session.
      operationId: postGetalldelayedfuturesbysession
      x-api-path-slug: getalldelayedfuturesbysession-get
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
      - Futures
      - By
      - Session
  /GetDelayedFuturesBySession:
    get:
      summary: Get Delayed Futures By Session
      description: Returns delayed quotes for multiple future contracts by exchange
        session.
      operationId: postGetdelayedfuturesbysession
      x-api-path-slug: getdelayedfuturesbysession-get
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
      - Futures
      - By
      - Session
  /GetDelayedIndicesValue:
    get:
      summary: Get Delayed Indices Value
      description: Get delayed indices value.
      operationId: GetDelayedIndicesValue
      x-api-path-slug: getdelayedindicesvalue-get
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
      - Indices
      - Value
  /GetDelayedIndexValue:
    get:
      summary: Get Delayed Index Value
      description: Get delayed index value.
      operationId: GetDelayedIndexValue
      x-api-path-slug: getdelayedindexvalue-get
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
      - Index
      - Value
  /GetDelayedVWAP:
    get:
      summary: Get Delayed VWAP
      description: Returns an intraday VWAP for a security based on all trades for
        the day up to the 15/20 minutes delayed quote.
      operationId: GetDelayedVWAP
      x-api-path-slug: getdelayedvwap-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Delayed
      - VWAP