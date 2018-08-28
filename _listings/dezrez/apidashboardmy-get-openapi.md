---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Get all shared dashboards
  version: 1.0.0
  description: Get all shared dashboards.
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/dashboard/{id}/setlayout:
    put:
      summary: Set widget layout on dashboards
      description: Set widget layout on dashboards.
      operationId: Dashboard_SetWidgetLayoutByidBylayouts
      x-api-path-slug: apidashboardidsetlayout-put
      parameters:
      - in: path
        name: id
        description: Dashboard Id
      - in: body
        name: layouts
        description: Array of layout objects
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Set
      - Widget
      - Layout
      - "On"
      - Dashboards
  /api/dashboard/getshared:
    get:
      summary: Get all shared dashboards
      description: Get all shared dashboards.
      operationId: Dashboard_AllDashboards
      x-api-path-slug: apidashboardgetshared-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Shared
      - Dashboards
  /api/dashboard/my:
    get:
      summary: Get all shared dashboards
      description: Get all shared dashboards.
      operationId: Dashboard_MyDashboards
      x-api-path-slug: apidashboardmy-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Shared
      - Dashboards
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