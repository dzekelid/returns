---
name: Neblio
x-slug: neblio
description: Neblio was born out of the need for simple and intuitive tools and solutions
  to drive the adoption of blockchain technology in the enterprise space. We are working
  on tools, services, and APIs that will simplify and revolutionize the way that businesses
  deploy next-generation applications on the Neblio Blockchain Platform.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/26754-neblio.jpg
x-kinRank: "7"
x-alexaRank: "350300"
tags: Returns
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/neblio/apis.md
specificationVersion: "0.14"
apis:
- name: Neblio REST API Suite - Returns the tokenId representing a token
  x-api-slug: ntp1tokenidtokensymbol-get
  description: Translates a token symbol to a tokenId if a token exists with that
    symbol on the network
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/26754-neblio.jpg
  humanURL: https://nebl.io
  baseURL: https://ntp1node.nebl.io//
  tags: Enterprise, Technology, SaaS, Blockchain, Profiles, Networks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/neblio/ntp1tokenidtokensymbol-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/neblio/ntp1tokenidtokensymbol-get-openapi.md
- name: Neblio REST API Suite - Returns information regarding a Neblio block
  x-api-slug: insblockblockhash-get
  description: Returns blockchain data for a given block based upon the block hash
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/26754-neblio.jpg
  humanURL: https://nebl.io
  baseURL: https://ntp1node.nebl.io//
  tags: Enterprise, Technology, SaaS, Blockchain, Profiles, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/neblio/insblockblockhash-get-openapi.md
- name: Neblio REST API Suite - Returns block hash of block
  x-api-slug: insblockindexblockindex-get
  description: Returns the block hash of a block at a given block index
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/26754-neblio.jpg
  humanURL: https://nebl.io
  baseURL: https://ntp1node.nebl.io//
  tags: Enterprise, Technology, SaaS, Blockchain, Profiles, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/neblio/insblockindexblockindex-get-openapi.md
- name: Neblio REST API Suite - Returns transaction object
  x-api-slug: instxtxid-get
  description: Returns NEBL transaction object representing a NEBL transaction
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/26754-neblio.jpg
  humanURL: https://nebl.io
  baseURL: https://ntp1node.nebl.io//
  tags: Enterprise, Technology, SaaS, Blockchain, Profiles, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/neblio/instxtxid-get-openapi.md
- name: Neblio REST API Suite - Returns raw transaction hex
  x-api-slug: insrawtxtxid-get
  description: Returns raw transaction hex representing a NEBL transaction
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/26754-neblio.jpg
  humanURL: https://nebl.io
  baseURL: https://ntp1node.nebl.io//
  tags: Enterprise, Technology, SaaS, Blockchain, Profiles, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/neblio/insrawtxtxid-get-openapi.md
- name: Neblio REST API Suite - Returns address object
  x-api-slug: insaddraddress-get
  description: Returns NEBL address object containing information on a specific address
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/26754-neblio.jpg
  humanURL: https://nebl.io
  baseURL: https://ntp1node.nebl.io//
  tags: Enterprise, Technology, SaaS, Blockchain, Profiles, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/neblio/insaddraddress-get-openapi.md
- name: Neblio REST API Suite - Returns address balance in sats
  x-api-slug: insaddraddressbalance-get
  description: Returns NEBL address balance in satoshis
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/26754-neblio.jpg
  humanURL: https://nebl.io
  baseURL: https://ntp1node.nebl.io//
  tags: Enterprise, Technology, SaaS, Blockchain, Profiles, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/neblio/insaddraddressbalance-get-openapi.md
- name: Neblio REST API Suite - Returns address unconfirmed balance in sats
  x-api-slug: insaddraddressunconfirmedbalance-get
  description: Returns NEBL address unconfirmed balance in satoshis
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/26754-neblio.jpg
  humanURL: https://nebl.io
  baseURL: https://ntp1node.nebl.io//
  tags: Enterprise, Technology, SaaS, Blockchain, Profiles, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/neblio/insaddraddressunconfirmedbalance-get-openapi.md
- name: Neblio REST API Suite - Returns total received by address in sats
  x-api-slug: insaddraddresstotalreceived-get
  description: Returns total NEBL received by address in satoshis
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/26754-neblio.jpg
  humanURL: https://nebl.io
  baseURL: https://ntp1node.nebl.io//
  tags: Enterprise, Technology, SaaS, Blockchain, Profiles, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/neblio/insaddraddresstotalreceived-get-openapi.md
- name: Neblio REST API Suite - Returns all UTXOs at a given address
  x-api-slug: insaddraddressutxo-get
  description: Returns information on each Unspent Transaction Output contained at
    an address
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/26754-neblio.jpg
  humanURL: https://nebl.io
  baseURL: https://ntp1node.nebl.io//
  tags: Enterprise, Technology, SaaS, Blockchain, Profiles, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/neblio/insaddraddressutxo-get-openapi.md
- name: Neblio REST API Suite - Returns total sent by address in sats
  x-api-slug: insaddraddresstotalsent-get
  description: Returns total NEBL sent by address in satoshis
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/26754-neblio.jpg
  humanURL: https://nebl.io
  baseURL: https://ntp1node.nebl.io//
  tags: Enterprise, Technology, SaaS, Blockchain, Profiles, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/neblio/insaddraddresstotalsent-get-openapi.md
- name: Neblio REST API Suite - Returns information regarding a Neblio block
  x-api-slug: testnetinsblockblockhash-get
  description: Returns blockchain data for a given block based upon the block hash
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/26754-neblio.jpg
  humanURL: https://nebl.io
  baseURL: https://ntp1node.nebl.io//
  tags: Enterprise, Technology, SaaS, Blockchain, Profiles, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/neblio/testnetinsblockblockhash-get-openapi.md
- name: Neblio REST API Suite - Returns block hash of block
  x-api-slug: testnetinsblockindexblockindex-get
  description: Returns the block hash of a block at a given block index
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/26754-neblio.jpg
  humanURL: https://nebl.io
  baseURL: https://ntp1node.nebl.io//
  tags: Enterprise, Technology, SaaS, Blockchain, Profiles, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/neblio/testnetinsblockindexblockindex-get-openapi.md
- name: Neblio REST API Suite - Returns transaction object
  x-api-slug: testnetinstxtxid-get
  description: Returns NEBL transaction object representing a NEBL transaction
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/26754-neblio.jpg
  humanURL: https://nebl.io
  baseURL: https://ntp1node.nebl.io//
  tags: Enterprise, Technology, SaaS, Blockchain, Profiles, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/neblio/testnetinstxtxid-get-openapi.md
- name: Neblio REST API Suite - Returns raw transaction hex
  x-api-slug: testnetinsrawtxtxid-get
  description: Returns raw transaction hex representing a NEBL transaction
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/26754-neblio.jpg
  humanURL: https://nebl.io
  baseURL: https://ntp1node.nebl.io//
  tags: Enterprise, Technology, SaaS, Blockchain, Profiles, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/neblio/testnetinsrawtxtxid-get-openapi.md
- name: Neblio REST API Suite - Returns address object
  x-api-slug: testnetinsaddraddress-get
  description: Returns NEBL address object containing information on a specific address
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/26754-neblio.jpg
  humanURL: https://nebl.io
  baseURL: https://ntp1node.nebl.io//
  tags: Enterprise, Technology, SaaS, Blockchain, Profiles, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/neblio/testnetinsaddraddress-get-openapi.md
- name: Neblio REST API Suite - Returns address balance in sats
  x-api-slug: testnetinsaddraddressbalance-get
  description: Returns NEBL address balance in satoshis
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/26754-neblio.jpg
  humanURL: https://nebl.io
  baseURL: https://ntp1node.nebl.io//
  tags: Enterprise, Technology, SaaS, Blockchain, Profiles, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/neblio/testnetinsaddraddressbalance-get-openapi.md
- name: Neblio REST API Suite - Returns address unconfirmed balance in sats
  x-api-slug: testnetinsaddraddressunconfirmedbalance-get
  description: Returns NEBL address unconfirmed balance in satoshis
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/26754-neblio.jpg
  humanURL: https://nebl.io
  baseURL: https://ntp1node.nebl.io//
  tags: Enterprise, Technology, SaaS, Blockchain, Profiles, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/neblio/testnetinsaddraddressunconfirmedbalance-get-openapi.md
- name: Neblio REST API Suite - Returns total received by address in sats
  x-api-slug: testnetinsaddraddresstotalreceived-get
  description: Returns total NEBL received by address in satoshis
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/26754-neblio.jpg
  humanURL: https://nebl.io
  baseURL: https://ntp1node.nebl.io//
  tags: Enterprise, Technology, SaaS, Blockchain, Profiles, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/neblio/testnetinsaddraddresstotalreceived-get-openapi.md
- name: Neblio REST API Suite - Returns all UTXOs at a given address
  x-api-slug: testnetinsaddraddressutxo-get
  description: Returns information on each Unspent Transaction Output contained at
    an address
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/26754-neblio.jpg
  humanURL: https://nebl.io
  baseURL: https://ntp1node.nebl.io//
  tags: Enterprise, Technology, SaaS, Blockchain, Profiles, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/neblio/testnetinsaddraddressutxo-get-openapi.md
- name: Neblio REST API Suite - Returns total sent by address in sats
  x-api-slug: testnetinsaddraddresstotalsent-get
  description: Returns total NEBL sent by address in satoshis
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/26754-neblio.jpg
  humanURL: https://nebl.io
  baseURL: https://ntp1node.nebl.io//
  tags: Enterprise, Technology, SaaS, Blockchain, Profiles, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/neblio/testnetinsaddraddresstotalsent-get-openapi.md
- name: Neblio REST API Suite - Returns the tokenId representing a token
  x-api-slug: testnetntp1tokenidtokensymbol-get
  description: Translates a token symbol to a tokenId if a token exists with that
    symbol on the network
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/26754-neblio.jpg
  humanURL: https://nebl.io
  baseURL: https://ntp1node.nebl.io//
  tags: Enterprise, Technology, SaaS, Blockchain, Profiles, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/neblio/testnetntp1tokenidtokensymbol-get-openapi.md
x-common:
- type: x-blog-rss
  url: https://nebl.io/feed/
- type: x-documentation
  url: https://nebl.io/apidocs/index.html
- type: x-github
  url: http://github.com/NeblioTeam
- type: x-openapi
  url: https://raw.githubusercontent.com/NeblioTeam/neblio-api-swagger-docs/master/swagger.json
- type: x-api-gallery
  url: http://moltin.api.gallery.streamdata.io
- type: x-blog
  url: https://nebl.io/blog/
- type: x-twitter
  url: https://twitter.com/NeblioTeam
- type: x-website
  url: https://nebl.io
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---