---
swagger: "2.0"
x-collection-name: Server Density
x-complete: 0
info:
  title: Dashboards API Deleting a dashboard
  description: Deleting a dashboard.
  version: 1.0.0
host: api.serverdensity.io.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /users/dashboards/dashboardId:
    "":
      summary: Deleting a dashboard
      description: Deleting a dashboard.
      operationId: deleting-a-dashboard
      x-api-path-slug: usersdashboardsdashboardid-
      parameters:
      - in: path
        name: dashboardId
        description: ID of the dashboard to delete
        type: string
      - in: path
        name: layout
        description: Dictionary with the ids of the widgets from this dashboard as
          keys
        type: string
      - in: body
        name: layout
        description: Dictionary with the ids of the widgets from this dashboard as
          keys
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: name
        description: Name of the dashboard
        type: string
      - in: body
        name: name
        description: Name of the dashboard
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: token
        description: Your API token
        type: string
      - in: body
        name: token
        description: Your API token
        schema:
          $ref: '#/definitions/holder'
      responses:
        apps:
          description: app_allow
        devices:
          description: device_link
        members:
          description: member_invite
        passwords:
          description: tfa_enable
        sharing:
          description: shmodel_create
        team_admin_actions:
          description: sf_external_accept_allow
      tags:
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