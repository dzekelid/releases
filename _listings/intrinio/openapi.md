---
swagger: "2.0"
x-collection-name: Intrinio
x-complete: 1
info:
  title: Intrinio
  description: through-our-intrinio-data-marketplace-we-offer-a-wide-selection-of-financial-data-feeds-sourced-by-our-own-proprietary-processes-as-well-as-from-many-data-vendors--the-primary-application-of-the-intrinio-api-is-for-use-in-thirdparty-applications-and-integrations-or-for-endusers-utilizing-the-excel-addin-and-google-sheets-addon--the-intrinio-api-uses-https-verbs-and-a-restful-endpoint-structure-which-makes-it-easy-to-request-data-from-intrinio--basic-authentication-is-administered-over-https--responses-are-delivered-in-json-format-
  version: 1.0.0
host: api.intrinio.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /press_releases:
    get:
      summary: Press Releases
      description: Returns the most recent press releases by Nasdaq GlobeNewsire for
        a company.
      operationId: press-releases
      x-api-path-slug: press-releases-get
      parameters:
      - in: query
        name: identifier
        description: the stock market ticker symbol associated with the company&rsquo;s
          common stock
        type: string
      - in: query
        name: page_number
        description: an integer greater than or equal to 1 for specifying the page
          number for the return values
        type: string
      - in: query
        name: page_size
        description: an integer greater than 1 for specifying the number of results
          on each page
        type: string
      - in: query
        name: related
        description: 'filter whether the list returned includes all press releases
          where a company is the subject or only press releases issued by the company:
          all | false | true'
        type: string
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Press Releases
---