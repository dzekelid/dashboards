---
swagger: "2.0"
x-collection-name: Starred
x-complete: 0
info:
  title: Starred Dashboard Summary
  description: "Retrieve segment summary from your account. This summary includes
    your NPS score and detailed breakdown.\n\n**Request Parameters**\n\n| Parameter
    | Required | Description |\n| ------ | ------ | ------ |\n| `form` | Required
    | ID of the form that will be sent out |\n| `segment` | Optional | Group ID to
    get summary data for (defaults to 0) |\n\nNote: Segment is an alias for Groups
    in Starred Platform. You can retrieve Segment ID on Groups page in Starred Platform.
    [Groups in Starred](https://app.starred.com/segments/overview)\n\n#### Steps to
    retrieve Segment ID\n1. Login to Starred Platform\n2. Go to Clients tab\n3. Click
    on a Group you want to get data for. \n4. In Group detail view copy the Segment
    ID from URL\n\n![Starred API Key][starred-segment-id]\n[See Full Image](http://www.starred.com/wp-content/uploads/2018/05/starred-segment-id.png)\n[starred-segment-id]:
    http://www.starred.com/wp-content/uploads/2018/05/starred-segment-id.png"
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /segment/summary:
    get:
      summary: Dashboard Summary
      description: "Retrieve segment summary from your account. This summary includes
        your NPS score and detailed breakdown.\n\n**Request Parameters**\n\n| Parameter
        | Required | Description |\n| ------ | ------ | ------ |\n| `form` | Required
        | ID of the form that will be sent out |\n| `segment` | Optional | Group ID
        to get summary data for (defaults to 0) |\n\nNote: Segment is an alias for
        Groups in Starred Platform. You can retrieve Segment ID on Groups page in
        Starred Platform. [Groups in Starred](https://app.starred.com/segments/overview)\n\n####
        Steps to retrieve Segment ID\n1. Login to Starred Platform\n2. Go to Clients
        tab\n3. Click on a Group you want to get data for. \n4. In Group detail view
        copy the Segment ID from URL\n\n![Starred API Key][starred-segment-id]\n[See
        Full Image](http://www.starred.com/wp-content/uploads/2018/05/starred-segment-id.png)\n[starred-segment-id]:
        http://www.starred.com/wp-content/uploads/2018/05/starred-segment-id.png"
      operationId: SegmentSummaryGet
      x-api-path-slug: segmentsummary-get
      responses:
        200:
          description: OK
      tags:
      - Dashboard
      - Summary
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