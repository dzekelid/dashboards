swagger: "2.0"
x-collection-name: Tumblr
x-complete: 1
info:
  title: Tumblr
  description: ntshare-photos-mobile-apps-and-social-network-using-tumblrs-apis-n----
  version: 1.0.0
host: api.tumblr.com
basePath: /v2/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /user/dashboard:
    get:
      summary: Get User Dashboard
      description: Use this method to retrieve the dashboard that matches the OAuth
        credentials submitted with the request.
      operationId: user.dashboard.get
      x-api-path-slug: userdashboard-get
      parameters:
      - in: query
        name: limit
        description: 'The number of results to return: 1???20, inclusive'
      - in: query
        name: offset
        description: Post number to start at
      - in: query
        name: since_id
        description: Return posts that have appeared after this ID
      - in: query
        name: type
        description: The type of post to return
      responses:
        200:
          description: OK
      tags:
      - User
      - Dashboard