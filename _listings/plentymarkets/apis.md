---
name: Plentymarkets
x-slug: plentymarkets
description: plentymarkets is an all-in-one e-commerce ERP solution, which combines
  a comprehensive stock management system with a versatile shop system and effortless
  multichannel sales. Thanks to comprehensive functions and interfaces that include
  all steps of the e-commerce value chain, you can use the cloud based software to
  completely automate all of your e-business processes as well as your companys own
  individual processes.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
x-kinRank: "7"
x-alexaRank: ""
tags: Profiles
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/profiles/master/_listings/plentymarkets/apis.md
specificationVersion: "0.14"
apis:
- name: plentymarkets REST-API - List all shipping profiles of all items
  x-api-slug: restitemsitem-shipping-profiles-get
  description: |-
    Lists all shipping profiles of all items. Results can be filtered by the timestamp of the link between items and shipping profiles (eq, lt, lte, gt, gte, between).
    <ul>
    <li>eq = Equal to</li>
    <li>gte = Greater than or equal to</li>
    <li>gt = Greater than</li>
    <li>lte = Less than or equal to</li>
    <li>lt = Less than</li>
    <li>between = Date range</li>
    </ul>
    Example: updated=gt:2018-04-16 16:00:00 returns all items with shipping profiles that were activated after 4pm on the 16th of April 2018.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/profiles/master/_listings/plentymarkets/restitemsitem-shipping-profiles-get-openapi.md
- name: plentymarkets REST-API - Bulk activate shipping profiles
  x-api-slug: restitemsitem-shipping-profiles-post
  description: Activates up to 50 shipping profiles for items
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/profiles/master/_listings/plentymarkets/restitemsitem-shipping-profiles-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/profiles/master/_listings/plentymarkets/restitemsitem-shipping-profiles-post-openapi.md
- name: plentymarkets REST-API - Deactivate shipping profiles of an item
  x-api-slug: restitemsitemiditem-shipping-profiles-delete
  description: Deactivates all shipping profiles of an item. The ID of the item must
    be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/profiles/master/_listings/plentymarkets/restitemsitemiditem-shipping-profiles-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/profiles/master/_listings/plentymarkets/restitemsitemiditem-shipping-profiles-delete-openapi.md
- name: plentymarkets REST-API - List shipping profiles of an item
  x-api-slug: restitemsitemiditem-shipping-profiles-get
  description: Lists the shipping profiles linked to an item. The ID of the item must
    be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/profiles/master/_listings/plentymarkets/restitemsitemiditem-shipping-profiles-get-openapi.md
- name: plentymarkets REST-API - List listing shipping profiles
  x-api-slug: restlistingsshipping-profiles-get
  description: Lists listing shipping profiles.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/profiles/master/_listings/plentymarkets/restlistingsshipping-profiles-get-openapi.md
- name: plentymarkets REST-API - List shipping profiles
  x-api-slug: restordersshippingpresets-get
  description: List shipping profiles.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/profiles/master/_listings/plentymarkets/restordersshippingpresets-get-openapi.md
- name: plentymarkets REST-API - Activate a shipping profile
  x-api-slug: restitemsitemiditem-shipping-profiles-post
  description: Links a shipping profile to the item. The ID of the item and the ID
    of the shipping profile must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/profiles/master/_listings/plentymarkets/restitemsitemiditem-shipping-profiles-post-openapi.md
- name: plentymarkets REST-API - Deactivate a shipping profile
  x-api-slug: restitemsitemiditem-shipping-profilesid-delete
  description: Unlinks a shipping profile from the item. The ID of the item must be
    specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/profiles/master/_listings/plentymarkets/restitemsitemiditem-shipping-profilesid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/profiles/master/_listings/plentymarkets/restitemsitemiditem-shipping-profilesid-delete-openapi.md
- name: plentymarkets REST-API - Get a shipping profile
  x-api-slug: restlistingsshipping-profilesid-get
  description: Gets a shipping profile by providing its ID.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/profiles/master/_listings/plentymarkets/restlistingsshipping-profilesid-get-openapi.md
- name: plentymarkets REST-API - Get a shipping profile
  x-api-slug: restordersshippingpresetspresetid-get
  description: Gets a shipping profile. The ID of the shipping profile must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/profiles/master/_listings/plentymarkets/restordersshippingpresetspresetid-get-openapi.md
- name: plentymarkets REST-API - Activate a shipping profile
  x-api-slug: restitemsitemiditem-shipping-profiles-post
  description: Links a shipping profile to the item. The ID of the item and the ID
    of the shipping profile must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/profiles/master/_listings/plentymarkets/restitemsitemiditem-shipping-profiles-post-openapi.md
- name: plentymarkets REST-API - Deactivate a shipping profile
  x-api-slug: restitemsitemiditem-shipping-profilesid-delete
  description: Unlinks a shipping profile from the item. The ID of the item must be
    specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/profiles/master/_listings/plentymarkets/restitemsitemiditem-shipping-profilesid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/profiles/master/_listings/plentymarkets/restitemsitemiditem-shipping-profilesid-delete-openapi.md
- name: plentymarkets REST-API - Get a shipping profile
  x-api-slug: restlistingsshipping-profilesid-get
  description: Gets a shipping profile by providing its ID.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/profiles/master/_listings/plentymarkets/restlistingsshipping-profilesid-get-openapi.md
- name: plentymarkets REST-API - Get a shipping profile
  x-api-slug: restordersshippingpresetspresetid-get
  description: Gets a shipping profile. The ID of the shipping profile must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/profiles/master/_listings/plentymarkets/restordersshippingpresetspresetid-get-openapi.md
- name: plentymarkets REST-API - Get a shipping profile
  x-api-slug: restordersshippingpresetspresetid-get
  description: Gets a shipping profile. The ID of the shipping profile must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/profiles/master/_listings/plentymarkets/restordersshippingpresetspresetid-get-openapi.md
- name: plentymarkets REST-API - Get a shipping profile
  x-api-slug: restlistingsshipping-profilesid-get
  description: Gets a shipping profile by providing its ID.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/profiles/master/_listings/plentymarkets/restlistingsshipping-profilesid-get-openapi.md
- name: plentymarkets REST-API - Deactivate a shipping profile
  x-api-slug: restitemsitemiditem-shipping-profilesid-delete
  description: Unlinks a shipping profile from the item. The ID of the item must be
    specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/profiles/master/_listings/plentymarkets/restitemsitemiditem-shipping-profilesid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/profiles/master/_listings/plentymarkets/restitemsitemiditem-shipping-profilesid-delete-openapi.md
- name: plentymarkets REST-API - Activate a shipping profile
  x-api-slug: restitemsitemiditem-shipping-profiles-post
  description: Links a shipping profile to the item. The ID of the item and the ID
    of the shipping profile must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/profiles/master/_listings/plentymarkets/restitemsitemiditem-shipping-profiles-post-openapi.md
x-common:
- type: x-blog-rss
  url: https://www.plentymarkets.co.uk/?ActionCall=WebActionRSS&rrss_id=1
- type: x-github
  url: https://github.com/plentymarkets
- type: x-twitter
  url: https://twitter.com/plentymarketsuk
- type: x-website
  url: http://www.plentymarkets.co.uk
- type: x-api-gallery
  url: http://pivotal.tracker.api.gallery.streamdata.io
- type: x-api-stack
  url: http://plentymarkets.stack.network
- type: x-blog
  url: https://www.plentymarkets.co.uk/blog/
- type: x-pricing
  url: https://www.plentymarkets.co.uk/prices/
- type: x-website
  url: https://www.plentymarkets.co.uk
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---