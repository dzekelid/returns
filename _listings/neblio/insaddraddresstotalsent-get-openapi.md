---
swagger: "2.0"
x-collection-name: Neblio
x-complete: 0
info:
  title: Neblio Returns total sent by address in sats
  description: Returns total NEBL sent by address in satoshis
  version: 1.0.0
host: ntp1node.nebl.io
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /ntp1/tokenid/{tokensymbol}:
    get:
      summary: Returns the tokenId representing a token
      description: Translates a token symbol to a tokenId if a token exists with that
        symbol on the network
      operationId: getTokenId
      x-api-path-slug: ntp1tokenidtokensymbol-get
      parameters:
      - in: path
        name: tokensymbol
        description: Token symbol
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Returns
      - TokenId
      - Representing
      - Token
  /ins/block/{blockhash}:
    get:
      summary: Returns information regarding a Neblio block
      description: Returns blockchain data for a given block based upon the block
        hash
      operationId: getBlock
      x-api-path-slug: insblockblockhash-get
      parameters:
      - in: path
        name: blockhash
        description: Block Hash
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Returns
      - Information
      - Regarding
      - Neblio
      - Block
  /ins/block-index/{blockindex}:
    get:
      summary: Returns block hash of block
      description: Returns the block hash of a block at a given block index
      operationId: getBlockIndex
      x-api-path-slug: insblockindexblockindex-get
      parameters:
      - in: path
        name: blockindex
        description: Block Index
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Returns
      - Block
      - Hash
      - Of
      - Block
  /ins/tx/{txid}:
    get:
      summary: Returns transaction object
      description: Returns NEBL transaction object representing a NEBL transaction
      operationId: getTx
      x-api-path-slug: instxtxid-get
      parameters:
      - in: path
        name: txid
        description: Transaction ID
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Returns
      - Transaction
      - Object
  /ins/rawtx/{txid}:
    get:
      summary: Returns raw transaction hex
      description: Returns raw transaction hex representing a NEBL transaction
      operationId: getRawTx
      x-api-path-slug: insrawtxtxid-get
      parameters:
      - in: path
        name: txid
        description: Transaction ID
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Returns
      - Raw
      - Transaction
      - Hex
  /ins/addr/{address}:
    get:
      summary: Returns address object
      description: Returns NEBL address object containing information on a specific
        address
      operationId: getAddress
      x-api-path-slug: insaddraddress-get
      parameters:
      - in: path
        name: address
        description: Address
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Returns
      - Address
      - Object
  /ins/addr/{address}/balance:
    get:
      summary: Returns address balance in sats
      description: Returns NEBL address balance in satoshis
      operationId: getAddressBalance
      x-api-path-slug: insaddraddressbalance-get
      parameters:
      - in: path
        name: address
        description: Address
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Returns
      - Address
      - Balance
      - In
      - Sats
  /ins/addr/{address}/unconfirmedBalance:
    get:
      summary: Returns address unconfirmed balance in sats
      description: Returns NEBL address unconfirmed balance in satoshis
      operationId: getAddressUnconfirmedBalance
      x-api-path-slug: insaddraddressunconfirmedbalance-get
      parameters:
      - in: path
        name: address
        description: Address
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Returns
      - Address
      - Unconfirmed
      - Balance
      - In
      - Sats
  /ins/addr/{address}/totalReceived:
    get:
      summary: Returns total received by address in sats
      description: Returns total NEBL received by address in satoshis
      operationId: getAddressTotalReceived
      x-api-path-slug: insaddraddresstotalreceived-get
      parameters:
      - in: path
        name: address
        description: Address
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Returns
      - Total
      - Received
      - By
      - Address
      - In
      - Sats
  /ins/addr/{address}/utxo:
    get:
      summary: Returns all UTXOs at a given address
      description: Returns information on each Unspent Transaction Output contained
        at an address
      operationId: getAddressUtxos
      x-api-path-slug: insaddraddressutxo-get
      parameters:
      - in: path
        name: address
        description: Address
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Returns
      - ""
      - UTXOs
      - At
      - Given
      - Address
  /ins/addr/{address}/totalSent:
    get:
      summary: Returns total sent by address in sats
      description: Returns total NEBL sent by address in satoshis
      operationId: getAddressTotalSent
      x-api-path-slug: insaddraddresstotalsent-get
      parameters:
      - in: path
        name: address
        description: Address
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Returns
      - Total
      - Sent
      - By
      - Address
      - In
      - Sats
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