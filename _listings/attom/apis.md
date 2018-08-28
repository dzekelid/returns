---
name: ATTOM
x-slug: attom
description: 'Search public property records including real estate data: sale, ownership,
  tax, and more - for more than 150 million U.S. properties. ATTOM Data Solutions
  is the curator of ATTOM, a multi-sourced national property data warehouse that contains
  tax, deed, mortgage, foreclosure, environmental risk, natural hazard, health hazard,
  neighborhood characteristic and property characteristic data for over 155 million
  U.S. properties, delivering actionable data to clients and powering consumer websites
  owned by ATTOM Data Solutions: RealtyTrac.com, Homefacts.com, and HomeDisclosure.com.'
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28881-api-developer-attomdata-com.jpg
x-kinRank: "7"
x-alexaRank: "359677"
tags: Returns
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/attom/apis.md
specificationVersion: "0.14"
apis:
- name: Attom Data Solutions API - Returns a list of properties that fit a criteria.
  x-api-slug: propertyid-get
  description: Get a list of property IDs within a specific geography that have a
    specific number of beds. Use orderby to choose how you want your results sorted.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28881-api-developer-attomdata-com.jpg
  humanURL: https://api.developer.attomdata.com
  baseURL: https://search.onboard-apis.com//communityapi/v2.0.0
  tags: SaaS, Technology, Enterprise, Real Estate, Places, Schools, Properties, General
    Data, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/attom/propertyid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/attom/propertyid-get-openapi.md
- name: Attom Data Solutions API - Returns property details based on an ID.
  x-api-slug: propertydetail-get
  description: Get property details based on its Onboard property ID.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28881-api-developer-attomdata-com.jpg
  humanURL: https://api.developer.attomdata.com
  baseURL: https://search.onboard-apis.com//communityapi/v2.0.0
  tags: SaaS, Technology, Enterprise, Real Estate, Places, Schools, Properties, General
    Data, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/attom/propertydetail-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/attom/propertydetail-get-openapi.md
- name: Attom Data Solutions API - Returns properties within a zip code.
  x-api-slug: propertyaddress-get
  description: Get a list of properties within a zip code. Use propertytype and order
    by to narrow down your results.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28881-api-developer-attomdata-com.jpg
  humanURL: https://api.developer.attomdata.com
  baseURL: https://search.onboard-apis.com//communityapi/v2.0.0
  tags: SaaS, Technology, Enterprise, Real Estate, Places, Schools, Properties, General
    Data, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/attom/propertyaddress-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/attom/propertyaddress-get-openapi.md
- name: Attom Data Solutions API - Returns properties and their characteristics that
    fit a criteria.
  x-api-slug: propertysnapshot-get
  description: Get a list of property snapshots within a specific city that are within
    a desired size range and a specific property type.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28881-api-developer-attomdata-com.jpg
  humanURL: https://api.developer.attomdata.com
  baseURL: https://search.onboard-apis.com//communityapi/v2.0.0
  tags: SaaS, Technology, Enterprise, Real Estate, Places, Schools, Properties, General
    Data, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/attom/propertysnapshot-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/attom/propertysnapshot-get-openapi.md
- name: Attom Data Solutions API - Returns basic property information and most recent
    transaction and taxes.
  x-api-slug: propertybasicprofile-get
  description: Get basic property information and most recent transaction and taxes
    for a specific attom id.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28881-api-developer-attomdata-com.jpg
  humanURL: https://api.developer.attomdata.com
  baseURL: https://search.onboard-apis.com//communityapi/v2.0.0
  tags: SaaS, Technology, Enterprise, Real Estate, Places, Schools, Properties, General
    Data, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/attom/propertybasicprofile-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/attom/propertybasicprofile-get-openapi.md
- name: Attom Data Solutions API - Returns detailed property information and most
    recent transaction and taxes.
  x-api-slug: propertyexpandedprofile-get
  description: Get a detailed property information and most recent transaction and
    taxes for a specific address.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28881-api-developer-attomdata-com.jpg
  humanURL: https://api.developer.attomdata.com
  baseURL: https://search.onboard-apis.com//communityapi/v2.0.0
  tags: SaaS, Technology, Enterprise, Real Estate, Places, Schools, Properties, General
    Data, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/attom/propertyexpandedprofile-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/attom/propertyexpandedprofile-get-openapi.md
- name: Attom Data Solutions API - Returns all the events that have occurred on a
    specific address.
  x-api-slug: alleventsdetail-get
  description: Get a detail of all the events on a specific property based on its
    address.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28881-api-developer-attomdata-com.jpg
  humanURL: https://api.developer.attomdata.com
  baseURL: https://search.onboard-apis.com//communityapi/v2.0.0
  tags: SaaS, Technology, Enterprise, Real Estate, Places, Schools, Properties, General
    Data, Historical Data API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/attom/alleventsdetail-get-openapi.md
- name: Attom Data Solutions API - Returns property details mortgage based on ID.
  x-api-slug: propertydetailmortgage-get
  description: Get property details mortgage based on its Onboard property ID.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28881-api-developer-attomdata-com.jpg
  humanURL: https://api.developer.attomdata.com
  baseURL: https://search.onboard-apis.com//communityapi/v2.0.0
  tags: SaaS, Technology, Enterprise, Real Estate, Places, Schools, Properties, General
    Data, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/attom/propertydetailmortgage-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/attom/propertydetailmortgage-get-openapi.md
- name: Attom Data Solutions API - Returns property details owner based on an ID.
  x-api-slug: propertydetailowner-get
  description: Get property details owner based on its Onboard property ID.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28881-api-developer-attomdata-com.jpg
  humanURL: https://api.developer.attomdata.com
  baseURL: https://search.onboard-apis.com//communityapi/v2.0.0
  tags: SaaS, Technology, Enterprise, Real Estate, Places, Schools, Properties, General
    Data, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/attom/propertydetailowner-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/attom/propertydetailowner-get-openapi.md
- name: Attom Data Solutions API - Returns property details mortgageowner based on
    an ID.
  x-api-slug: propertydetailmortgageowner-get
  description: Get property details mortgageowner based on its Onboard property ID.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28881-api-developer-attomdata-com.jpg
  humanURL: https://api.developer.attomdata.com
  baseURL: https://search.onboard-apis.com//communityapi/v2.0.0
  tags: SaaS, Technology, Enterprise, Real Estate, Places, Schools, Properties, General
    Data, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/attom/propertydetailmortgageowner-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/attom/propertydetailmortgageowner-get-openapi.md
- name: Attom Data Solutions API - Returns assessment details for properties within
    a radius.
  x-api-slug: assessmentsnapshot-get
  description: Get snapshots of the properties within a radius of a property that
    have a total market value within a specified range.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28881-api-developer-attomdata-com.jpg
  humanURL: https://api.developer.attomdata.com
  baseURL: https://search.onboard-apis.com//communityapi/v2.0.0
  tags: SaaS, Technology, Enterprise, Real Estate, Places, Schools, Properties, General
    Data, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/attom/assessmentsnapshot-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/attom/assessmentsnapshot-get-openapi.md
- name: Attom Data Solutions API - Returns assessment details for properties within
    a zip code.
  x-api-slug: assessmentdetail-get
  description: Get assessment details for properties within a zip code. Use propertytpe
    to select a specific property type for your search.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28881-api-developer-attomdata-com.jpg
  humanURL: https://api.developer.attomdata.com
  baseURL: https://search.onboard-apis.com//communityapi/v2.0.0
  tags: SaaS, Technology, Enterprise, Real Estate, Places, Schools, Properties, General
    Data, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/attom/assessmentdetail-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/attom/assessmentdetail-get-openapi.md
- name: Attom Data Solutions API - Returns assessment history and property details.
  x-api-slug: assessmenthistorydetail-get
  description: Get a full detail of property characteristics and assessment history
    information for a specific property.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28881-api-developer-attomdata-com.jpg
  humanURL: https://api.developer.attomdata.com
  baseURL: https://search.onboard-apis.com//communityapi/v2.0.0
  tags: SaaS, Technology, Enterprise, Real Estate, Places, Schools, Properties, General
    Data, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/attom/assessmenthistorydetail-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/attom/assessmenthistorydetail-get-openapi.md
- name: Attom Data Solutions API - Returns AVM details within a geography.
  x-api-slug: avmsnapshot-get
  description: Get a list of AVM snapshot records that fall within an Onboard GeoID
    with a specific value range. Use propertytpe to select a specific property type
    for your search.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28881-api-developer-attomdata-com.jpg
  humanURL: https://api.developer.attomdata.com
  baseURL: https://search.onboard-apis.com//communityapi/v2.0.0
  tags: SaaS, Technology, Enterprise, Real Estate, Places, Schools, Properties, General
    Data, Historical Data API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/attom/avmsnapshot-get-openapi.md
- name: Attom Data Solutions API - Returns AVM details for a property.
  x-api-slug: avmdetail-get
  description: Get AVM details for a specific address.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28881-api-developer-attomdata-com.jpg
  humanURL: https://api.developer.attomdata.com
  baseURL: https://search.onboard-apis.com//communityapi/v2.0.0
  tags: SaaS, Technology, Enterprise, Real Estate, Places, Schools, Properties, General
    Data, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/attom/avmdetail-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/attom/avmdetail-get-openapi.md
- name: Attom Data Solutions API - Returns the Attomized AVM and other property details
    .
  x-api-slug: attomavmdetail-get
  description: Get Attomized AVM and other property details for a specific address.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28881-api-developer-attomdata-com.jpg
  humanURL: https://api.developer.attomdata.com
  baseURL: https://search.onboard-apis.com//communityapi/v2.0.0
  tags: SaaS, Technology, Enterprise, Real Estate, Places, Schools, Properties, General
    Data, Historical Data API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/attom/attomavmdetail-get-openapi.md
- name: Attom Data Solutions API - Returns home sale information for properties within
    a geography.
  x-api-slug: salesnapshot-get
  description: Get a list of home sale snapshots within a Onboard GeoID that sold
    within a date range and specified sale amount.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28881-api-developer-attomdata-com.jpg
  humanURL: https://api.developer.attomdata.com
  baseURL: https://search.onboard-apis.com//communityapi/v2.0.0
  tags: SaaS, Technology, Enterprise, Real Estate, Places, Schools, Properties, General
    Data, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/attom/salesnapshot-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/attom/salesnapshot-get-openapi.md
- name: Attom Data Solutions API - Returns sale information for a property.
  x-api-slug: saledetail-get
  description: Get sales information for a specific address.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28881-api-developer-attomdata-com.jpg
  humanURL: https://api.developer.attomdata.com
  baseURL: https://search.onboard-apis.com//communityapi/v2.0.0
  tags: SaaS, Technology, Enterprise, Real Estate, Places, Schools, Properties, General
    Data, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/attom/saledetail-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/attom/saledetail-get-openapi.md
- name: Attom Data Solutions API - Returns sales history for a property.
  x-api-slug: saleshistorysnapshot-get
  description: Get a sales history snapshot of a property based on an Onboard property
    ID.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28881-api-developer-attomdata-com.jpg
  humanURL: https://api.developer.attomdata.com
  baseURL: https://search.onboard-apis.com//communityapi/v2.0.0
  tags: SaaS, Technology, Enterprise, Real Estate, Places, Schools, Properties, General
    Data, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/attom/saleshistorysnapshot-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/attom/saleshistorysnapshot-get-openapi.md
- name: Attom Data Solutions API - Returns basic transaction and loan history on a
    property.
  x-api-slug: saleshistorybasichistory-get
  description: Get the basic transaction and loan history on a property for a specific
    address.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28881-api-developer-attomdata-com.jpg
  humanURL: https://api.developer.attomdata.com
  baseURL: https://search.onboard-apis.com//communityapi/v2.0.0
  tags: SaaS, Technology, Enterprise, Real Estate, Places, Schools, Properties, General
    Data, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/attom/saleshistorybasichistory-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/attom/saleshistorybasichistory-get-openapi.md
- name: Attom Data Solutions API - Returns detailed transaction, pre-foreclosure and
    loan history on a property.
  x-api-slug: saleshistoryexpandedhistory-get
  description: Get the detailed transaction, pre-foreclosure and loan history on a
    property for a specific address.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28881-api-developer-attomdata-com.jpg
  humanURL: https://api.developer.attomdata.com
  baseURL: https://search.onboard-apis.com//communityapi/v2.0.0
  tags: SaaS, Technology, Enterprise, Real Estate, Places, Schools, Properties, General
    Data, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/attom/saleshistoryexpandedhistory-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/attom/saleshistoryexpandedhistory-get-openapi.md
- name: Attom Data Solutions API - Returns sales history for a property.
  x-api-slug: saleshistorydetail-get
  description: Get a sales history snapshot of a property based on an address.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28881-api-developer-attomdata-com.jpg
  humanURL: https://api.developer.attomdata.com
  baseURL: https://search.onboard-apis.com//communityapi/v2.0.0
  tags: SaaS, Technology, Enterprise, Real Estate, Places, Schools, Properties, General
    Data, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/attom/saleshistorydetail-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/attom/saleshistorydetail-get-openapi.md
- name: Attom Data Solutions API - Returns sales trends for a given zip code in yearly
    intervals
  x-api-slug: salestrendsnapshot-get
  description: Get the average sale price, median sale price, and count of sales for
    the past 2 years in yearly intervals.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28881-api-developer-attomdata-com.jpg
  humanURL: https://api.developer.attomdata.com
  baseURL: https://search.onboard-apis.com//communityapi/v2.0.0
  tags: SaaS, Technology, Enterprise, Real Estate, Places, Schools, Properties, General
    Data, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/attom/salestrendsnapshot-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/attom/salestrendsnapshot-get-openapi.md
- name: Attom Data Solutions API - Returns all boundaries a point falls within.
  x-api-slug: hierarchylookup-get
  description: This method allows you to pass a latitude and longitude point and geo
    type to retrieve a list of geographies that point falls within. Required input
    is a valid WKT (Well Known Text) point.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28881-api-developer-attomdata-com.jpg
  humanURL: https://api.developer.attomdata.com
  baseURL: https://search.onboard-apis.com//communityapi/v2.0.0
  tags: SaaS, Technology, Enterprise, Real Estate, Places, Schools, Properties, General
    Data, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/attom/hierarchylookup-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/attom/hierarchylookup-get-openapi.md
- name: Attom Data Solutions API - Returns POIs based on zip code.
  x-api-slug: poigeography-get
  description: This search returns a list of Points of Interest in proximity to the
    centroid of a zip code.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28881-api-developer-attomdata-com.jpg
  humanURL: https://api.developer.attomdata.com
  baseURL: https://search.onboard-apis.com//communityapi/v2.0.0
  tags: SaaS, Technology, Enterprise, Real Estate, Places, Schools, Properties, General
    Data, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/attom/poigeography-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/attom/poigeography-get-openapi.md
- name: Attom Data Solutions API - Returns POIs based on point.
  x-api-slug: poipoint-get
  description: This search returns a list of POI in proximity to a latitude/longitude.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28881-api-developer-attomdata-com.jpg
  humanURL: https://api.developer.attomdata.com
  baseURL: https://search.onboard-apis.com//communityapi/v2.0.0
  tags: SaaS, Technology, Enterprise, Real Estate, Places, Schools, Properties, General
    Data, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/attom/poipoint-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/attom/poipoint-get-openapi.md
- name: Attom Data Solutions API - Returns POIs based on an address.
  x-api-slug: poistreetaddress-get
  description: This search returns a list of POI in proximity to an address.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28881-api-developer-attomdata-com.jpg
  humanURL: https://api.developer.attomdata.com
  baseURL: https://search.onboard-apis.com//communityapi/v2.0.0
  tags: SaaS, Technology, Enterprise, Real Estate, Places, Schools, Properties, General
    Data, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/attom/poistreetaddress-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/attom/poistreetaddress-get-openapi.md
- name: Attom Data Solutions API - Returns business categories.
  x-api-slug: businesscategorylookup-get
  description: This lookup is used to obtain a full list of Business Categories.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28881-api-developer-attomdata-com.jpg
  humanURL: https://api.developer.attomdata.com
  baseURL: https://search.onboard-apis.com//communityapi/v2.0.0
  tags: SaaS, Technology, Enterprise, Real Estate, Places, Schools, Properties, General
    Data, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/attom/businesscategorylookup-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/attom/businesscategorylookup-get-openapi.md
- name: Attom Data Solutions API - Returns lines of business categories.
  x-api-slug: loblookup-get
  description: This lookup can be used to show the full list of Lines of Businesses
    (LOB), and which categories they belong to.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28881-api-developer-attomdata-com.jpg
  humanURL: https://api.developer.attomdata.com
  baseURL: https://search.onboard-apis.com//communityapi/v2.0.0
  tags: SaaS, Technology, Enterprise, Real Estate, Places, Schools, Properties, General
    Data, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/attom/loblookup-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/attom/loblookup-get-openapi.md
- name: Attom Data Solutions API - Returns community information.
  x-api-slug: areafull-get
  description: This search returns community information for a specific geography.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28881-api-developer-attomdata-com.jpg
  humanURL: https://api.developer.attomdata.com
  baseURL: https://search.onboard-apis.com//communityapi/v2.0.0
  tags: SaaS, Technology, Enterprise, Real Estate, Places, Schools, Properties, General
    Data, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/attom/areafull-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/attom/areafull-get-openapi.md
- name: Attom Data Solutions API - Returns available data fields.
  x-api-slug: attributelookup-get
  description: This lookup returns the full list of over 375 data fields that are
    available in the Community API.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28881-api-developer-attomdata-com.jpg
  humanURL: https://api.developer.attomdata.com
  baseURL: https://search.onboard-apis.com//communityapi/v2.0.0
  tags: SaaS, Technology, Enterprise, Real Estate, Places, Schools, Properties, General
    Data, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/attom/attributelookup-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/attom/attributelookup-get-openapi.md
- name: Attom Data Solutions API - Return schools within the attendance boundary of
    a property.
  x-api-slug: propertydetailwithschools-get
  description: Search for a property to have the property details returned, along
    with the schools in the associated attendance zones.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28881-api-developer-attomdata-com.jpg
  humanURL: https://api.developer.attomdata.com
  baseURL: https://search.onboard-apis.com//communityapi/v2.0.0
  tags: SaaS, Technology, Enterprise, Real Estate, Places, Schools, Properties, General
    Data, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/attom/propertydetailwithschools-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/attom/propertydetailwithschools-get-openapi.md
- name: Attom Data Solutions API - Return all schools within a defined radius from
    a point.
  x-api-slug: schoolsnapshot-get
  description: Search for all schools that are located within a given radius around
    a given latitude and longitude.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28881-api-developer-attomdata-com.jpg
  humanURL: https://api.developer.attomdata.com
  baseURL: https://search.onboard-apis.com//communityapi/v2.0.0
  tags: SaaS, Technology, Enterprise, Real Estate, Places, Schools, Properties, General
    Data, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/attom/schoolsnapshot-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/attom/schoolsnapshot-get-openapi.md
- name: Attom Data Solutions API - Return details about a particular school.
  x-api-slug: schooldetail-get
  description: Search by school ID to return all of the available details about a
    school
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28881-api-developer-attomdata-com.jpg
  humanURL: https://api.developer.attomdata.com
  baseURL: https://search.onboard-apis.com//communityapi/v2.0.0
  tags: SaaS, Technology, Enterprise, Real Estate, Places, Schools, Properties, General
    Data, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/attom/schooldetail-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/attom/schooldetail-get-openapi.md
- name: Attom Data Solutions API - Return details about a particular school district.
  x-api-slug: schooldistrictdetail-get
  description: Search by district number to return all of the available details about
    a school district
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28881-api-developer-attomdata-com.jpg
  humanURL: https://api.developer.attomdata.com
  baseURL: https://search.onboard-apis.com//communityapi/v2.0.0
  tags: SaaS, Technology, Enterprise, Real Estate, Places, Schools, Properties, General
    Data, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/attom/schooldistrictdetail-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/attom/schooldistrictdetail-get-openapi.md
- name: Attom Data Solutions API - Return schools within the attendance boundary of
    a property.
  x-api-slug: propertydetailwithschools-get
  description: Search for a property to have the property details returned, along
    with the schools in the associated attendance zones.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28881-api-developer-attomdata-com.jpg
  humanURL: https://api.developer.attomdata.com
  baseURL: https://search.onboard-apis.com//communityapi/v2.0.0
  tags: SaaS, Technology, Enterprise, Real Estate, Places, Schools, Properties, General
    Data, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/attom/propertydetailwithschools-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/attom/propertydetailwithschools-get-openapi.md
- name: Attom Data Solutions API - Return all schools within a defined radius from
    a point.
  x-api-slug: schoolsnapshot-get
  description: Search for all schools that are located within a given radius around
    a given latitude and longitude.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28881-api-developer-attomdata-com.jpg
  humanURL: https://api.developer.attomdata.com
  baseURL: https://search.onboard-apis.com//communityapi/v2.0.0
  tags: SaaS, Technology, Enterprise, Real Estate, Places, Schools, Properties, General
    Data, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/attom/schoolsnapshot-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/attom/schoolsnapshot-get-openapi.md
- name: Attom Data Solutions API - Return details about a particular school.
  x-api-slug: schooldetail-get
  description: Search by school ID to return all of the available details about a
    school
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28881-api-developer-attomdata-com.jpg
  humanURL: https://api.developer.attomdata.com
  baseURL: https://search.onboard-apis.com//communityapi/v2.0.0
  tags: SaaS, Technology, Enterprise, Real Estate, Places, Schools, Properties, General
    Data, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/attom/schooldetail-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/attom/schooldetail-get-openapi.md
- name: Attom Data Solutions API - Return details about a particular school district.
  x-api-slug: schooldistrictdetail-get
  description: Search by district number to return all of the available details about
    a school district
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28881-api-developer-attomdata-com.jpg
  humanURL: https://api.developer.attomdata.com
  baseURL: https://search.onboard-apis.com//communityapi/v2.0.0
  tags: SaaS, Technology, Enterprise, Real Estate, Places, Schools, Properties, General
    Data, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/attom/schooldistrictdetail-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/attom/schooldistrictdetail-get-openapi.md
- name: Attom Data Solutions API - Returns all the events that have occurred on a
    specific address.
  x-api-slug: alleventsdetail-get
  description: Get a detail of all the events on a specific property based on its
    address.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28881-api-developer-attomdata-com.jpg
  humanURL: https://api.developer.attomdata.com
  baseURL: https://search.onboard-apis.com//communityapi/v2.0.0
  tags: SaaS, Technology, Enterprise, Real Estate, Places, Schools, Properties, General
    Data, Historical Data API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/attom/alleventsdetail-get-openapi.md
- name: Attom Data Solutions API - Returns all the events that have occurred on a
    specific address.
  x-api-slug: alleventsdetail-get
  description: Get a detail of all the events on a specific property based on its
    address.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28881-api-developer-attomdata-com.jpg
  humanURL: https://api.developer.attomdata.com
  baseURL: https://search.onboard-apis.com//communityapi/v2.0.0
  tags: SaaS, Technology, Enterprise, Real Estate, Places, Schools, Properties, General
    Data, Historical Data API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/attom/alleventsdetail-get-openapi.md
- name: Attom Data Solutions API - Returns community information.
  x-api-slug: areafull-get
  description: This search returns community information for a specific geography.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28881-api-developer-attomdata-com.jpg
  humanURL: https://api.developer.attomdata.com
  baseURL: https://search.onboard-apis.com//communityapi/v2.0.0
  tags: SaaS, Technology, Enterprise, Real Estate, Places, Schools, Properties, General
    Data, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/attom/areafull-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/attom/areafull-get-openapi.md
- name: Attom Data Solutions API - Returns community information.
  x-api-slug: areafull-get
  description: This search returns community information for a specific geography.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28881-api-developer-attomdata-com.jpg
  humanURL: https://api.developer.attomdata.com
  baseURL: https://search.onboard-apis.com//communityapi/v2.0.0
  tags: SaaS, Technology, Enterprise, Real Estate, Places, Schools, Properties, General
    Data, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/attom/areafull-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/attom/areafull-get-openapi.md
- name: Attom Data Solutions API - Return details about a particular school district.
  x-api-slug: schooldistrictdetail-get
  description: Search by district number to return all of the available details about
    a school district
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28881-api-developer-attomdata-com.jpg
  humanURL: https://api.developer.attomdata.com
  baseURL: https://search.onboard-apis.com//communityapi/v2.0.0
  tags: SaaS, Technology, Enterprise, Real Estate, Places, Schools, Properties, General
    Data, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/attom/schooldistrictdetail-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/attom/schooldistrictdetail-get-openapi.md
- name: Attom Data Solutions API - Return details about a particular school.
  x-api-slug: schooldetail-get
  description: Search by school ID to return all of the available details about a
    school
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28881-api-developer-attomdata-com.jpg
  humanURL: https://api.developer.attomdata.com
  baseURL: https://search.onboard-apis.com//communityapi/v2.0.0
  tags: SaaS, Technology, Enterprise, Real Estate, Places, Schools, Properties, General
    Data, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/attom/schooldetail-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/attom/schooldetail-get-openapi.md
- name: Attom Data Solutions API - Return all schools within a defined radius from
    a point.
  x-api-slug: schoolsnapshot-get
  description: Search for all schools that are located within a given radius around
    a given latitude and longitude.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28881-api-developer-attomdata-com.jpg
  humanURL: https://api.developer.attomdata.com
  baseURL: https://search.onboard-apis.com//communityapi/v2.0.0
  tags: SaaS, Technology, Enterprise, Real Estate, Places, Schools, Properties, General
    Data, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/attom/schoolsnapshot-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/attom/schoolsnapshot-get-openapi.md
- name: Attom Data Solutions API - Return schools within the attendance boundary of
    a property.
  x-api-slug: propertydetailwithschools-get
  description: Search for a property to have the property details returned, along
    with the schools in the associated attendance zones.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28881-api-developer-attomdata-com.jpg
  humanURL: https://api.developer.attomdata.com
  baseURL: https://search.onboard-apis.com//communityapi/v2.0.0
  tags: SaaS, Technology, Enterprise, Real Estate, Places, Schools, Properties, General
    Data, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/attom/propertydetailwithschools-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/returns/master/_listings/attom/propertydetailwithschools-get-openapi.md
x-common:
- type: x-openapi
  url: https://api.developer.attomdata.com/swagger/spec/propertyapi_property.json
- type: x-api-gallery
  url: http://atlassian.api.gallery.streamdata.io
- type: x-api-stack
  url: http://attom.stack.network
- type: x-email
  url: privacy@attomdata.com
- type: x-twitter
  url: https://twitter.com/Attomdata
- type: x-website
  url: https://api.developer.attomdata.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---