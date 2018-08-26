---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 1
info:
  title: Dezrez.Rezi.Client.Api
  version: 1.0.0
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
  /api/dashboard/available:
    get:
      summary: Get all available dashboards
      description: Get all available dashboards.
      operationId: Dashboard_AvailableDashboards
      x-api-path-slug: apidashboardavailable-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Available
      - Dashboards
  /api/dashboard/create:
    post:
      summary: Create/Update dashboard
      description: Create/update dashboard.
      operationId: Dashboard_SetDashboardBydataContract
      x-api-path-slug: apidashboardcreate-post
      parameters:
      - in: body
        name: dataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Dashboard
  /api/dashboard/{id}/delete:
    delete:
      summary: Delete dashboard
      description: Delete dashboard.
      operationId: Dashboard_DeleteDashboardByid
      x-api-path-slug: apidashboardiddelete-delete
      parameters:
      - in: path
        name: id
        description: Dashboard Id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Dashboard
  /api/dashboard/{id}/removewidgets:
    put:
      summary: Remove widgets from a dashboard
      description: Remove widgets from a dashboard.
      operationId: Dashboard_RemoveWidgetsFromDashboardByid
      x-api-path-slug: apidashboardidremovewidgets-put
      parameters:
      - in: path
        name: id
        description: Dashboard Id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Widgets
      - From
      - Dashboard
  /api/dashboard/{id}/share:
    put:
      summary: Share dashboard
      description: Share dashboard.
      operationId: Dashboard_ShareDashboardByidBydataContract
      x-api-path-slug: apidashboardidshare-put
      parameters:
      - in: body
        name: dataContract
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: Dashboard Id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Share
      - Dashboard
  /api/dashboard/{id}/setwidget:
    put:
      summary: Add widget to dashboard
      description: Add widget to dashboard.
      operationId: Dashboard_SetWidgetByidBydataContract
      x-api-path-slug: apidashboardidsetwidget-put
      parameters:
      - in: body
        name: dataContract
        description: Widget to be added to dashboard
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: Dashboard Id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Widget
      - To
      - Dashboard
  /api/dashboard/{id}/deletewidget/{widgetId}:
    delete:
      summary: Delete widget on dashboard
      description: Delete widget on dashboard.
      operationId: Dashboard_DeleteWidgetByidBywidgetId
      x-api-path-slug: apidashboardiddeletewidgetwidgetid-delete
      parameters:
      - in: path
        name: id
        description: Dashboard Id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: path
        name: widgetId
        description: Widget Id to be deleted
      responses:
        200:
          description: OK
      tags:
      - Widget
      - "On"
      - Dashboard
  /api/dashboard/movewidget:
    put:
      summary: Move widget onto another dashboard
      description: Move widget onto another dashboard.
      operationId: Dashboard_MoveWidgetBydataContract
      x-api-path-slug: apidashboardmovewidget-put
      parameters:
      - in: body
        name: dataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Move
      - Widget
      - Onto
      - Another
      - Dashboard
  /api/dashboard/{id}/addnegotiator:
    put:
      summary: Add negotiator to dashboard id
      description: Add negotiator to dashboard id.
      operationId: Dashboard_AddNegotiatorToDashboardByid
      x-api-path-slug: apidashboardidaddnegotiator-put
      parameters:
      - in: path
        name: id
        description: Dashboard Id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Negotiator
      - To
      - Dashboard
      - Id
  /api/negotiator/my/properties/{roleType}:
    get:
      summary: Used for the Property Sales Dashboard to return a list of the negotiator's
        properties.
      description: Used for the property sales dashboard to return a list of the negotiator's
        properties..
      operationId: Negotiator_PropertiesByroleTypeBypageSizeBypageNumber
      x-api-path-slug: apinegotiatormypropertiesroletype-get
      parameters:
      - in: query
        name: pageNumber
        description: which page number of results to choose
      - in: query
        name: pageSize
        description: how many properties to return (default 10)
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: path
        name: roleType
        description: the PropertyMarketingRole type
      responses:
        200:
          description: OK
      tags:
      - Usedthe
      - Property
      - Sales
      - Dashboard
      - To
      - Return
      - List
      - Of
      - Negotiators
      - Properties
---