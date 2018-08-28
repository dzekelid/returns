---
name: Stripe
x-slug: stripe
description: Online payment processing for internet businesses. Stripe is a suite
  of payment APIs that powers commerce for online businesses of all sizes, including
  fraud prevention, and subscription management. Use Stripes payment platform to accept
  and process p...
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
x-kinRank: "10"
x-alexaRank: "1914"
tags: Returns
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/stripe/apis.md
specificationVersion: "0.14"
apis:
- name: Stripe - Get Order Returns
  x-api-slug: order-returns-get
  description: Returns a list of your order returns. The returns are returned sorted
    by creation date, with the most recently created return appearing first.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1/
  tags: Billing, Finance, Payments, Payments, Stripe Stack, Imports, Change Log Example,
    Stack Network, Stack, SaaS, Invoices, Payments, Relative Data, Service API, Relative
    StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/stripe/order-returns-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/stripe/order-returns-get-openapi.md
- name: Stripe - Get Order Returns
  x-api-slug: order-returnsid-get
  description: Retrieves the details of an existing order return. Supply the unique
    order ID from either an order return creation request or the order return list,
    and Stripe will return the corresponding order information.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1/
  tags: Billing, Finance, Payments, Payments, Stripe Stack, Imports, Change Log Example,
    Stack Network, Stack, SaaS, Invoices, Payments, Relative Data, Service API, Relative
    StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/stripe/order-returnsid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/stripe/order-returnsid-get-openapi.md
- name: Stripe - Add Orders  Returns
  x-api-slug: ordersidreturns-post
  description: Return all or part of an order. The order must have a status of paid
    or fulfilled before it can be returned. Once all items have been returned, the
    order will become canceled or returned depending on which status the order started
    in.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1/
  tags: Billing, Finance, Payments, Payments, Stripe Stack, Imports, Change Log Example,
    Stack Network, Stack, SaaS, Invoices, Payments, Relative Data, Service API, Relative
    StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/stripe/ordersidreturns-post-openapi.md
- name: Stripe - Get Accounts
  x-api-slug: accounts-get
  description: Returns a list of accounts connected to your platform via Connect.
    If you???re not a platform, the list is empty.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1/
  tags: Billing, Finance, Payments, Payments, Stripe Stack, Imports, Change Log Example,
    Stack Network, Stack, SaaS, Invoices, Payments, Relative Data, Service API, Relative
    StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/stripe/accounts-get-openapi.md
- name: Stripe - Get Application Fees
  x-api-slug: application-fees-get
  description: Returns a list of application fees you???ve previously collected. The
    application fees are returned in sorted order, with the most recent fees appearing
    first.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1/
  tags: Billing, Finance, Payments, Payments, Stripe Stack, Imports, Change Log Example,
    Stack Network, Stack, SaaS, Invoices, Payments, Relative Data, Service API, Relative
    StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/stripe/application-fees-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/stripe/application-fees-get-openapi.md
- name: Stripe - Get Application Fees
  x-api-slug: application-fees-get
  description: Returns a list of application fees you???ve previously collected. The
    application fees are returned in sorted order, with the most recent fees appearing
    first.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1/
  tags: Billing, Finance, Payments, Payments, Stripe Stack, Imports, Change Log Example,
    Stack Network, Stack, SaaS, Invoices, Payments, Relative Data, Service API, Relative
    StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/stripe/application-fees-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/stripe/application-fees-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://stride.api.gallery.streamdata.io
- type: x-api-stack
  url: http://stripe.stack.network
- type: x-base
  url: https://api.stripe.com/
- type: x-blog
  url: https://stripe.com/blog
- type: x-blog-rss
  url: https://stripe.com/blog/feed.rss
- type: x-change-log
  url: https://stripe.com/docs/upgrades
- type: x-crunchbase
  url: http://www.crunchbase.com/company/stripe
- type: x-crunchbase
  url: https://crunchbase.com/organization/stripe
- type: x-email
  url: info@stripe.com
- type: x-email
  url: privacy@stripe.com
- type: x-email
  url: atlas@stripe.com
- type: x-email
  url: notices@stripe.com
- type: x-email
  url: jane.diaz@stripe.com
- type: x-email
  url: nonprofit@stripe.com
- type: x-email
  url: support@stripe.com
- type: x-email
  url: dpo@stripe.com
- type: x-github
  url: https://github.com/stripe
- type: x-linkedin
  url: https://www.linkedin.com/company/stripe/
- type: x-pricing
  url: https://stripe.com/us/pricing
- type: x-twitter
  url: https://twitter.com/stripe
- type: x-website
  url: https://stripe.com/
- type: x-website
  url: http://stripe.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---