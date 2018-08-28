---
swagger: "2.0"
x-collection-name: Twilio
x-complete: 0
info:
  title: Twilio Delete Incoming Phone Number
  description: Release this phone number from your account. Twilio will no longer
    answerncalls to this number, and you will stop being billed the monthly phonennumber
    fee. The phone number will eventually be recycled and potentiallyngiven to another
    customer, so use with care. If you make a mistake, contacnus. We may be able to
    give you the number back.n
  termsOfService: https://www.twilio.com/legal/tos
  version: v1
host: api.twilio.com
basePath: /2010-04-01/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /Accounts/{AccountSid}/IncomingPhoneNumbers/{IncomingPhoneNumberSid}.{format}:
    delete:
      summary: Delete Incoming Phone Number
      description: Release this phone number from your account. Twilio will no longer
        answerncalls to this number, and you will stop being billed the monthly phonennumber
        fee. The phone number will eventually be recycled and potentiallyngiven to
        another customer, so use with care. If you make a mistake, contacnus. We may
        be able to give you the number back.n
      operationId: release-this-phone-number-from-your-account-twilio-will-no-longer-answercalls-to-this-number-and-you
      x-api-path-slug: accountsaccountsidincomingphonenumbersincomingphonenumbersid-format-delete
      parameters:
      - in: path
        name: AccountSid
        description: The ID for the Twilio account
      - in: path
        name: format
        description: By default, Twilios REST API returns XML
        type: string
        format: string
      - in: path
        name: IncomingPhoneNumberSid
        description: A 34 character string that uniquely identifies the incoming phone
          number
      responses:
        200:
          description: OK
      tags:
      - Incoming Phone Numbers
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