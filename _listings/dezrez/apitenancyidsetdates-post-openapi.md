---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: "Dezrez Set start date, terms, end date and notice period for tenancy.\r\nassertions"
  version: 1.0.0
  description: "Set start date, terms, end date and notice period for tenancy.\r\nassertions."
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/progression/lettings/withdrawInstruction:
    post:
      summary: Withdraw a letting at the end of let
      description: Withdraw a letting at the end of let.
      operationId: LettingsProgression_WithdrawInstructionBylettingInstructionCommandData
      x-api-path-slug: apiprogressionlettingswithdrawinstruction-post
      parameters:
      - in: body
        name: lettingInstructionCommandData
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Withdraw
      - Letting
      - At
      - End
      - Of
      - Let
  /api/progression/lettings/completeletting:
    post:
      summary: Withdraw a letting at the end of let
      description: Withdraw a letting at the end of let.
      operationId: LettingsProgression_CompleteLettingBycompleteCommandData
      x-api-path-slug: apiprogressionlettingscompleteletting-post
      parameters:
      - in: body
        name: completeCommandData
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Withdraw
      - Letting
      - At
      - End
      - Of
      - Let
  /api/tenancy/{id}/setdates:
    post:
      summary: "Set start date, terms, end date and notice period for tenancy.\r\nassertions"
      description: "Set start date, terms, end date and notice period for tenancy.\r\nassertions."
      operationId: Tenancy_SetTenancyDatesByidBydatesDataContract
      x-api-path-slug: apitenancyidsetdates-post
      parameters:
      - in: body
        name: datesDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Set
      - Start
      - Date
      - ""
      - Terms
      - ""
      - End
      - Date
      - Notice
      - Periodtenancy
      - Assertions
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