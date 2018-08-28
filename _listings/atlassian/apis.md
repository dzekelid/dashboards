---
name: Atlassian
x-slug: atlassian
description: Millions of users globally rely on Atlassian products every day for improving
  software development, project management, collaboration, and code quality.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
x-kinRank: "8"
x-alexaRank: "1656"
tags: Dashboards
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/dashboards/master/_listings/atlassian/apis.md
specificationVersion: "0.14"
apis:
- name: Jira Cloud REST API - Get all dashboards
  x-api-slug: api2dashboard-get
  description: "Returns a list of dashboards owned by or shared with the user. The
    list may be filtered to include only favorite or owned dashboards.  \n  \n**[Permissions](https://confluence.atlassian.com/x/FQiiLQ)
    required:** Permission to access Jira."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/dashboards/master/_listings/atlassian/api2dashboard-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/dashboards/master/_listings/atlassian/api2dashboard-get-openapi.md
- name: Jira Cloud REST API - Get dashboard item property keys
  x-api-slug: api2dashboarddashboardiditemsitemidproperties-get
  description: "Returns the keys of all properties for a dashboard item.  \n  \n**[Permissions](https://confluence.atlassian.com/x/FQiiLQ)
    required:** Permission to access Jira. However, to get the property keys the user
    must be the owner of the dashboard or be shared the dashboard. Note, users with
    the _Administer Jira_ [global permission](href=) are considered owners of the
    System dashboard. The System dashboard is considered to be shared with all other
    users."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/dashboards/master/_listings/atlassian/api2dashboarddashboardiditemsitemidproperties-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/dashboards/master/_listings/atlassian/api2dashboarddashboardiditemsitemidproperties-get-openapi.md
- name: Jira Cloud REST API - Get dashboard item property
  x-api-slug: api2dashboarddashboardiditemsitemidpropertiespropertykey-get
  description: "Returns the key and value of a dashboard item property.  \n  \nA dashboard
    item enables an app to add user-specific information to a user dashboard. Dashboard
    items are exposed to users as gadgets that users can add to their dashboards.
    For more information on how users do this, see [Adding and customizing gadgets](https://confluence.atlassian.com/x/7AeiLQ).
    \ \n  \nWhen an app creates a dashboard item it registers a callback to receive
    the dashboard item ID. The callback fires whenever the item is rendered or, where
    the item is configurable, the user edits the item. The app then uses this resource
    to store the item's content or configuration details. For more information on
    working with dashboard items, see [Building a dashboard item for a JIRA Connect
    add-on](https://developer.atlassian.com/server/jira/platform/guide-building-a-dashboard-item-for-a-jira-connect-add-on-33746254/)
    and the [Dashboard Item](https://developer.atlassian.com/cloud/jira/platform/modules/dashboard-item/)
    documentation.  \n  \nThere is no resource to set or get dashboard items.  \n
    \ \n**[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** Permission
    to access Jira. However, to get a dashboard item property the user must be the
    owner of the dashboard or be shared the dashboard. Note, users with the _Administer
    Jira_ [global permission](href=) are considered owners of the System dashboard.
    The System dashboard is considered to be shared with all other users."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/dashboards/master/_listings/atlassian/api2dashboarddashboardiditemsitemidpropertiespropertykey-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/dashboards/master/_listings/atlassian/api2dashboarddashboardiditemsitemidpropertiespropertykey-get-openapi.md
- name: Jira Cloud REST API - Set dashboard item property
  x-api-slug: api2dashboarddashboardiditemsitemidpropertiespropertykey-put
  description: "Sets the value of a dashboard item property. Use this resource in
    apps to store custom data against a dashboard item.  \n  \nA dashboard item enables
    an app to add user-specific information to a user dashboard. Dashboard items are
    exposed to users as gadgets that users can add to their dashboards. For more information
    on how users do this, see [Adding and customizing gadgets](https://confluence.atlassian.com/x/7AeiLQ).
    \ \n  \nWhen an app creates a dashboard item it registers a callback to receive
    the dashboard item ID. The callback fires whenever the item is rendered or, where
    the item is configurable, the user edits the item. The app then uses this resource
    to store the item's content or configuration details. For more information on
    working with dashboard items, see [Building a dashboard item for a JIRA Connect
    add-on](https://developer.atlassian.com/server/jira/platform/guide-building-a-dashboard-item-for-a-jira-connect-add-on-33746254/)
    and the [Dashboard Item](https://developer.atlassian.com/cloud/jira/platform/modules/dashboard-item/)
    documentation.  \n  \nThere is no resource to set or get dashboard items.  \n
    \ \n**[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** Permission
    to access Jira. However, to set a dashboard item property the user must be the
    owner of the dashboard. Note, users with the _Administer Jira_ [global permission](href=)
    are considered owners of the System dashboard.  \n  \nThe value of the request
    body must be a [valid](http://tools.ietf.org/html/rfc4627), non-empty JSON blob.
    The maximum length is 32768 bytes."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/dashboards/master/_listings/atlassian/api2dashboarddashboardiditemsitemidpropertiespropertykey-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/dashboards/master/_listings/atlassian/api2dashboarddashboardiditemsitemidpropertiespropertykey-put-openapi.md
- name: Jira Cloud REST API - Delete dashboard item property
  x-api-slug: api2dashboarddashboardiditemsitemidpropertiespropertykey-delete
  description: "Deletes a dashboard item property.  \n  \n**[Permissions](https://confluence.atlassian.com/x/FQiiLQ)
    required:** Permission to access Jira. However, to delete a dashboard item property
    the user must be the owner of the dashboard. Note, users with the _Administer
    Jira_ [global permission](href=) are considered owners of the System dashboard."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/dashboards/master/_listings/atlassian/api2dashboarddashboardiditemsitemidpropertiespropertykey-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/dashboards/master/_listings/atlassian/api2dashboarddashboardiditemsitemidpropertiespropertykey-delete-openapi.md
- name: Jira Cloud REST API - Get dashboard
  x-api-slug: api2dashboardid-get
  description: "Returns a dashboard.  \n  \n**[Permissions](https://confluence.atlassian.com/x/FQiiLQ)
    required:** Permission to access Jira. However, to get a dashboard, the dashboard
    must be shared with the user or the user must own it. Note, users with the _Administer
    Jira_ [global permission](href=) are considered owners of the System dashboard.
    The System dashboard is considered to be shared with all other users."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/dashboards/master/_listings/atlassian/api2dashboardid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/dashboards/master/_listings/atlassian/api2dashboardid-get-openapi.md
- name: Jira Cloud REST API - Get dashboard item property keys
  x-api-slug: api2dashboarddashboardiditemsitemidproperties-get
  description: "Returns the keys of all properties for a dashboard item.  \n  \n**[Permissions](https://confluence.atlassian.com/x/FQiiLQ)
    required:** Permission to access Jira. However, to get the property keys the user
    must be the owner of the dashboard or be shared the dashboard. Note, users with
    the _Administer Jira_ [global permission](href=) are considered owners of the
    System dashboard. The System dashboard is considered to be shared with all other
    users."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/dashboards/master/_listings/atlassian/api2dashboarddashboardiditemsitemidproperties-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/dashboards/master/_listings/atlassian/api2dashboarddashboardiditemsitemidproperties-get-openapi.md
- name: Jira Cloud REST API - Get dashboard item property keys
  x-api-slug: api2dashboarddashboardiditemsitemidproperties-get
  description: "Returns the keys of all properties for a dashboard item.  \n  \n**[Permissions](https://confluence.atlassian.com/x/FQiiLQ)
    required:** Permission to access Jira. However, to get the property keys the user
    must be the owner of the dashboard or be shared the dashboard. Note, users with
    the _Administer Jira_ [global permission](href=) are considered owners of the
    System dashboard. The System dashboard is considered to be shared with all other
    users."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/dashboards/master/_listings/atlassian/api2dashboarddashboardiditemsitemidproperties-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/dashboards/master/_listings/atlassian/api2dashboarddashboardiditemsitemidproperties-get-openapi.md
- name: Jira Cloud REST API - Get dashboard item property
  x-api-slug: api2dashboarddashboardiditemsitemidpropertiespropertykey-get
  description: "Returns the key and value of a dashboard item property.  \n  \nA dashboard
    item enables an app to add user-specific information to a user dashboard. Dashboard
    items are exposed to users as gadgets that users can add to their dashboards.
    For more information on how users do this, see [Adding and customizing gadgets](https://confluence.atlassian.com/x/7AeiLQ).
    \ \n  \nWhen an app creates a dashboard item it registers a callback to receive
    the dashboard item ID. The callback fires whenever the item is rendered or, where
    the item is configurable, the user edits the item. The app then uses this resource
    to store the item's content or configuration details. For more information on
    working with dashboard items, see [Building a dashboard item for a JIRA Connect
    add-on](https://developer.atlassian.com/server/jira/platform/guide-building-a-dashboard-item-for-a-jira-connect-add-on-33746254/)
    and the [Dashboard Item](https://developer.atlassian.com/cloud/jira/platform/modules/dashboard-item/)
    documentation.  \n  \nThere is no resource to set or get dashboard items.  \n
    \ \n**[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** Permission
    to access Jira. However, to get a dashboard item property the user must be the
    owner of the dashboard or be shared the dashboard. Note, users with the _Administer
    Jira_ [global permission](href=) are considered owners of the System dashboard.
    The System dashboard is considered to be shared with all other users."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/dashboards/master/_listings/atlassian/api2dashboarddashboardiditemsitemidpropertiespropertykey-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/dashboards/master/_listings/atlassian/api2dashboarddashboardiditemsitemidpropertiespropertykey-get-openapi.md
- name: Jira Cloud REST API - Get dashboard item property
  x-api-slug: api2dashboarddashboardiditemsitemidpropertiespropertykey-get
  description: "Returns the key and value of a dashboard item property.  \n  \nA dashboard
    item enables an app to add user-specific information to a user dashboard. Dashboard
    items are exposed to users as gadgets that users can add to their dashboards.
    For more information on how users do this, see [Adding and customizing gadgets](https://confluence.atlassian.com/x/7AeiLQ).
    \ \n  \nWhen an app creates a dashboard item it registers a callback to receive
    the dashboard item ID. The callback fires whenever the item is rendered or, where
    the item is configurable, the user edits the item. The app then uses this resource
    to store the item's content or configuration details. For more information on
    working with dashboard items, see [Building a dashboard item for a JIRA Connect
    add-on](https://developer.atlassian.com/server/jira/platform/guide-building-a-dashboard-item-for-a-jira-connect-add-on-33746254/)
    and the [Dashboard Item](https://developer.atlassian.com/cloud/jira/platform/modules/dashboard-item/)
    documentation.  \n  \nThere is no resource to set or get dashboard items.  \n
    \ \n**[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** Permission
    to access Jira. However, to get a dashboard item property the user must be the
    owner of the dashboard or be shared the dashboard. Note, users with the _Administer
    Jira_ [global permission](href=) are considered owners of the System dashboard.
    The System dashboard is considered to be shared with all other users."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/dashboards/master/_listings/atlassian/api2dashboarddashboardiditemsitemidpropertiespropertykey-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/dashboards/master/_listings/atlassian/api2dashboarddashboardiditemsitemidpropertiespropertykey-get-openapi.md
- name: Jira Cloud REST API - Set dashboard item property
  x-api-slug: api2dashboarddashboardiditemsitemidpropertiespropertykey-put
  description: "Sets the value of a dashboard item property. Use this resource in
    apps to store custom data against a dashboard item.  \n  \nA dashboard item enables
    an app to add user-specific information to a user dashboard. Dashboard items are
    exposed to users as gadgets that users can add to their dashboards. For more information
    on how users do this, see [Adding and customizing gadgets](https://confluence.atlassian.com/x/7AeiLQ).
    \ \n  \nWhen an app creates a dashboard item it registers a callback to receive
    the dashboard item ID. The callback fires whenever the item is rendered or, where
    the item is configurable, the user edits the item. The app then uses this resource
    to store the item's content or configuration details. For more information on
    working with dashboard items, see [Building a dashboard item for a JIRA Connect
    add-on](https://developer.atlassian.com/server/jira/platform/guide-building-a-dashboard-item-for-a-jira-connect-add-on-33746254/)
    and the [Dashboard Item](https://developer.atlassian.com/cloud/jira/platform/modules/dashboard-item/)
    documentation.  \n  \nThere is no resource to set or get dashboard items.  \n
    \ \n**[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** Permission
    to access Jira. However, to set a dashboard item property the user must be the
    owner of the dashboard. Note, users with the _Administer Jira_ [global permission](href=)
    are considered owners of the System dashboard.  \n  \nThe value of the request
    body must be a [valid](http://tools.ietf.org/html/rfc4627), non-empty JSON blob.
    The maximum length is 32768 bytes."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/dashboards/master/_listings/atlassian/api2dashboarddashboardiditemsitemidpropertiespropertykey-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/dashboards/master/_listings/atlassian/api2dashboarddashboardiditemsitemidpropertiespropertykey-put-openapi.md
- name: Jira Cloud REST API - Set dashboard item property
  x-api-slug: api2dashboarddashboardiditemsitemidpropertiespropertykey-put
  description: "Sets the value of a dashboard item property. Use this resource in
    apps to store custom data against a dashboard item.  \n  \nA dashboard item enables
    an app to add user-specific information to a user dashboard. Dashboard items are
    exposed to users as gadgets that users can add to their dashboards. For more information
    on how users do this, see [Adding and customizing gadgets](https://confluence.atlassian.com/x/7AeiLQ).
    \ \n  \nWhen an app creates a dashboard item it registers a callback to receive
    the dashboard item ID. The callback fires whenever the item is rendered or, where
    the item is configurable, the user edits the item. The app then uses this resource
    to store the item's content or configuration details. For more information on
    working with dashboard items, see [Building a dashboard item for a JIRA Connect
    add-on](https://developer.atlassian.com/server/jira/platform/guide-building-a-dashboard-item-for-a-jira-connect-add-on-33746254/)
    and the [Dashboard Item](https://developer.atlassian.com/cloud/jira/platform/modules/dashboard-item/)
    documentation.  \n  \nThere is no resource to set or get dashboard items.  \n
    \ \n**[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** Permission
    to access Jira. However, to set a dashboard item property the user must be the
    owner of the dashboard. Note, users with the _Administer Jira_ [global permission](href=)
    are considered owners of the System dashboard.  \n  \nThe value of the request
    body must be a [valid](http://tools.ietf.org/html/rfc4627), non-empty JSON blob.
    The maximum length is 32768 bytes."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/dashboards/master/_listings/atlassian/api2dashboarddashboardiditemsitemidpropertiespropertykey-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/dashboards/master/_listings/atlassian/api2dashboarddashboardiditemsitemidpropertiespropertykey-put-openapi.md
- name: Jira Cloud REST API - Delete dashboard item property
  x-api-slug: api2dashboarddashboardiditemsitemidpropertiespropertykey-delete
  description: "Deletes a dashboard item property.  \n  \n**[Permissions](https://confluence.atlassian.com/x/FQiiLQ)
    required:** Permission to access Jira. However, to delete a dashboard item property
    the user must be the owner of the dashboard. Note, users with the _Administer
    Jira_ [global permission](href=) are considered owners of the System dashboard."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/dashboards/master/_listings/atlassian/api2dashboarddashboardiditemsitemidpropertiespropertykey-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/dashboards/master/_listings/atlassian/api2dashboarddashboardiditemsitemidpropertiespropertykey-delete-openapi.md
- name: Jira Cloud REST API - Delete dashboard item property
  x-api-slug: api2dashboarddashboardiditemsitemidpropertiespropertykey-delete
  description: "Deletes a dashboard item property.  \n  \n**[Permissions](https://confluence.atlassian.com/x/FQiiLQ)
    required:** Permission to access Jira. However, to delete a dashboard item property
    the user must be the owner of the dashboard. Note, users with the _Administer
    Jira_ [global permission](href=) are considered owners of the System dashboard."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/dashboards/master/_listings/atlassian/api2dashboarddashboardiditemsitemidpropertiespropertykey-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/dashboards/master/_listings/atlassian/api2dashboarddashboardiditemsitemidpropertiespropertykey-delete-openapi.md
- name: Jira Cloud REST API - Get dashboard
  x-api-slug: api2dashboardid-get
  description: "Returns a dashboard.  \n  \n**[Permissions](https://confluence.atlassian.com/x/FQiiLQ)
    required:** Permission to access Jira. However, to get a dashboard, the dashboard
    must be shared with the user or the user must own it. Note, users with the _Administer
    Jira_ [global permission](href=) are considered owners of the System dashboard.
    The System dashboard is considered to be shared with all other users."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/dashboards/master/_listings/atlassian/api2dashboardid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/dashboards/master/_listings/atlassian/api2dashboardid-get-openapi.md
- name: Jira Cloud REST API - Get dashboard
  x-api-slug: api2dashboardid-get
  description: "Returns a dashboard.  \n  \n**[Permissions](https://confluence.atlassian.com/x/FQiiLQ)
    required:** Permission to access Jira. However, to get a dashboard, the dashboard
    must be shared with the user or the user must own it. Note, users with the _Administer
    Jira_ [global permission](href=) are considered owners of the System dashboard.
    The System dashboard is considered to be shared with all other users."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/dashboards/master/_listings/atlassian/api2dashboardid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/dashboards/master/_listings/atlassian/api2dashboardid-get-openapi.md
- name: Jira Cloud REST API - Get dashboard
  x-api-slug: api2dashboardid-get
  description: "Returns a dashboard.  \n  \n**[Permissions](https://confluence.atlassian.com/x/FQiiLQ)
    required:** Permission to access Jira. However, to get a dashboard, the dashboard
    must be shared with the user or the user must own it. Note, users with the _Administer
    Jira_ [global permission](href=) are considered owners of the System dashboard.
    The System dashboard is considered to be shared with all other users."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/dashboards/master/_listings/atlassian/api2dashboardid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/dashboards/master/_listings/atlassian/api2dashboardid-get-openapi.md
- name: Jira Cloud REST API - Get dashboard
  x-api-slug: api2dashboardid-get
  description: "Returns a dashboard.  \n  \n**[Permissions](https://confluence.atlassian.com/x/FQiiLQ)
    required:** Permission to access Jira. However, to get a dashboard, the dashboard
    must be shared with the user or the user must own it. Note, users with the _Administer
    Jira_ [global permission](href=) are considered owners of the System dashboard.
    The System dashboard is considered to be shared with all other users."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/dashboards/master/_listings/atlassian/api2dashboardid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/dashboards/master/_listings/atlassian/api2dashboardid-get-openapi.md
- name: Jira Cloud REST API - Delete dashboard item property
  x-api-slug: api2dashboarddashboardiditemsitemidpropertiespropertykey-delete
  description: "Deletes a dashboard item property.  \n  \n**[Permissions](https://confluence.atlassian.com/x/FQiiLQ)
    required:** Permission to access Jira. However, to delete a dashboard item property
    the user must be the owner of the dashboard. Note, users with the _Administer
    Jira_ [global permission](href=) are considered owners of the System dashboard."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/dashboards/master/_listings/atlassian/api2dashboarddashboardiditemsitemidpropertiespropertykey-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/dashboards/master/_listings/atlassian/api2dashboarddashboardiditemsitemidpropertiespropertykey-delete-openapi.md
- name: Jira Cloud REST API - Delete dashboard item property
  x-api-slug: api2dashboarddashboardiditemsitemidpropertiespropertykey-delete
  description: "Deletes a dashboard item property.  \n  \n**[Permissions](https://confluence.atlassian.com/x/FQiiLQ)
    required:** Permission to access Jira. However, to delete a dashboard item property
    the user must be the owner of the dashboard. Note, users with the _Administer
    Jira_ [global permission](href=) are considered owners of the System dashboard."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/dashboards/master/_listings/atlassian/api2dashboarddashboardiditemsitemidpropertiespropertykey-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/dashboards/master/_listings/atlassian/api2dashboarddashboardiditemsitemidpropertiespropertykey-delete-openapi.md
- name: Jira Cloud REST API - Set dashboard item property
  x-api-slug: api2dashboarddashboardiditemsitemidpropertiespropertykey-put
  description: "Sets the value of a dashboard item property. Use this resource in
    apps to store custom data against a dashboard item.  \n  \nA dashboard item enables
    an app to add user-specific information to a user dashboard. Dashboard items are
    exposed to users as gadgets that users can add to their dashboards. For more information
    on how users do this, see [Adding and customizing gadgets](https://confluence.atlassian.com/x/7AeiLQ).
    \ \n  \nWhen an app creates a dashboard item it registers a callback to receive
    the dashboard item ID. The callback fires whenever the item is rendered or, where
    the item is configurable, the user edits the item. The app then uses this resource
    to store the item's content or configuration details. For more information on
    working with dashboard items, see [Building a dashboard item for a JIRA Connect
    add-on](https://developer.atlassian.com/server/jira/platform/guide-building-a-dashboard-item-for-a-jira-connect-add-on-33746254/)
    and the [Dashboard Item](https://developer.atlassian.com/cloud/jira/platform/modules/dashboard-item/)
    documentation.  \n  \nThere is no resource to set or get dashboard items.  \n
    \ \n**[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** Permission
    to access Jira. However, to set a dashboard item property the user must be the
    owner of the dashboard. Note, users with the _Administer Jira_ [global permission](href=)
    are considered owners of the System dashboard.  \n  \nThe value of the request
    body must be a [valid](http://tools.ietf.org/html/rfc4627), non-empty JSON blob.
    The maximum length is 32768 bytes."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/dashboards/master/_listings/atlassian/api2dashboarddashboardiditemsitemidpropertiespropertykey-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/dashboards/master/_listings/atlassian/api2dashboarddashboardiditemsitemidpropertiespropertykey-put-openapi.md
- name: Jira Cloud REST API - Set dashboard item property
  x-api-slug: api2dashboarddashboardiditemsitemidpropertiespropertykey-put
  description: "Sets the value of a dashboard item property. Use this resource in
    apps to store custom data against a dashboard item.  \n  \nA dashboard item enables
    an app to add user-specific information to a user dashboard. Dashboard items are
    exposed to users as gadgets that users can add to their dashboards. For more information
    on how users do this, see [Adding and customizing gadgets](https://confluence.atlassian.com/x/7AeiLQ).
    \ \n  \nWhen an app creates a dashboard item it registers a callback to receive
    the dashboard item ID. The callback fires whenever the item is rendered or, where
    the item is configurable, the user edits the item. The app then uses this resource
    to store the item's content or configuration details. For more information on
    working with dashboard items, see [Building a dashboard item for a JIRA Connect
    add-on](https://developer.atlassian.com/server/jira/platform/guide-building-a-dashboard-item-for-a-jira-connect-add-on-33746254/)
    and the [Dashboard Item](https://developer.atlassian.com/cloud/jira/platform/modules/dashboard-item/)
    documentation.  \n  \nThere is no resource to set or get dashboard items.  \n
    \ \n**[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** Permission
    to access Jira. However, to set a dashboard item property the user must be the
    owner of the dashboard. Note, users with the _Administer Jira_ [global permission](href=)
    are considered owners of the System dashboard.  \n  \nThe value of the request
    body must be a [valid](http://tools.ietf.org/html/rfc4627), non-empty JSON blob.
    The maximum length is 32768 bytes."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/dashboards/master/_listings/atlassian/api2dashboarddashboardiditemsitemidpropertiespropertykey-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/dashboards/master/_listings/atlassian/api2dashboarddashboardiditemsitemidpropertiespropertykey-put-openapi.md
- name: Jira Cloud REST API - Get dashboard item property
  x-api-slug: api2dashboarddashboardiditemsitemidpropertiespropertykey-get
  description: "Returns the key and value of a dashboard item property.  \n  \nA dashboard
    item enables an app to add user-specific information to a user dashboard. Dashboard
    items are exposed to users as gadgets that users can add to their dashboards.
    For more information on how users do this, see [Adding and customizing gadgets](https://confluence.atlassian.com/x/7AeiLQ).
    \ \n  \nWhen an app creates a dashboard item it registers a callback to receive
    the dashboard item ID. The callback fires whenever the item is rendered or, where
    the item is configurable, the user edits the item. The app then uses this resource
    to store the item's content or configuration details. For more information on
    working with dashboard items, see [Building a dashboard item for a JIRA Connect
    add-on](https://developer.atlassian.com/server/jira/platform/guide-building-a-dashboard-item-for-a-jira-connect-add-on-33746254/)
    and the [Dashboard Item](https://developer.atlassian.com/cloud/jira/platform/modules/dashboard-item/)
    documentation.  \n  \nThere is no resource to set or get dashboard items.  \n
    \ \n**[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** Permission
    to access Jira. However, to get a dashboard item property the user must be the
    owner of the dashboard or be shared the dashboard. Note, users with the _Administer
    Jira_ [global permission](href=) are considered owners of the System dashboard.
    The System dashboard is considered to be shared with all other users."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/dashboards/master/_listings/atlassian/api2dashboarddashboardiditemsitemidpropertiespropertykey-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/dashboards/master/_listings/atlassian/api2dashboarddashboardiditemsitemidpropertiespropertykey-get-openapi.md
- name: Jira Cloud REST API - Get dashboard item property
  x-api-slug: api2dashboarddashboardiditemsitemidpropertiespropertykey-get
  description: "Returns the key and value of a dashboard item property.  \n  \nA dashboard
    item enables an app to add user-specific information to a user dashboard. Dashboard
    items are exposed to users as gadgets that users can add to their dashboards.
    For more information on how users do this, see [Adding and customizing gadgets](https://confluence.atlassian.com/x/7AeiLQ).
    \ \n  \nWhen an app creates a dashboard item it registers a callback to receive
    the dashboard item ID. The callback fires whenever the item is rendered or, where
    the item is configurable, the user edits the item. The app then uses this resource
    to store the item's content or configuration details. For more information on
    working with dashboard items, see [Building a dashboard item for a JIRA Connect
    add-on](https://developer.atlassian.com/server/jira/platform/guide-building-a-dashboard-item-for-a-jira-connect-add-on-33746254/)
    and the [Dashboard Item](https://developer.atlassian.com/cloud/jira/platform/modules/dashboard-item/)
    documentation.  \n  \nThere is no resource to set or get dashboard items.  \n
    \ \n**[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** Permission
    to access Jira. However, to get a dashboard item property the user must be the
    owner of the dashboard or be shared the dashboard. Note, users with the _Administer
    Jira_ [global permission](href=) are considered owners of the System dashboard.
    The System dashboard is considered to be shared with all other users."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/dashboards/master/_listings/atlassian/api2dashboarddashboardiditemsitemidpropertiespropertykey-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/dashboards/master/_listings/atlassian/api2dashboarddashboardiditemsitemidpropertiespropertykey-get-openapi.md
- name: Jira Cloud REST API - Get dashboard item property keys
  x-api-slug: api2dashboarddashboardiditemsitemidproperties-get
  description: "Returns the keys of all properties for a dashboard item.  \n  \n**[Permissions](https://confluence.atlassian.com/x/FQiiLQ)
    required:** Permission to access Jira. However, to get the property keys the user
    must be the owner of the dashboard or be shared the dashboard. Note, users with
    the _Administer Jira_ [global permission](href=) are considered owners of the
    System dashboard. The System dashboard is considered to be shared with all other
    users."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/dashboards/master/_listings/atlassian/api2dashboarddashboardiditemsitemidproperties-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/dashboards/master/_listings/atlassian/api2dashboarddashboardiditemsitemidproperties-get-openapi.md
- name: Jira Cloud REST API - Get dashboard item property keys
  x-api-slug: api2dashboarddashboardiditemsitemidproperties-get
  description: "Returns the keys of all properties for a dashboard item.  \n  \n**[Permissions](https://confluence.atlassian.com/x/FQiiLQ)
    required:** Permission to access Jira. However, to get the property keys the user
    must be the owner of the dashboard or be shared the dashboard. Note, users with
    the _Administer Jira_ [global permission](href=) are considered owners of the
    System dashboard. The System dashboard is considered to be shared with all other
    users."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/dashboards/master/_listings/atlassian/api2dashboarddashboardiditemsitemidproperties-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/dashboards/master/_listings/atlassian/api2dashboarddashboardiditemsitemidproperties-get-openapi.md
x-common:
- type: x-openapi
  url: https://developer.atlassian.com/cloud/jira/platform/swagger.v3.json
- type: x-openapi
  url: https://developer.atlassian.com/cloud/confluence/swagger.v3.json
- type: x-openapi
  url: https://developer.atlassian.com/cloud/jira/software/swagger.v3.json
- type: x-openapi
  url: https://developer.atlassian.com/cloud/jira/service-desk/swagger.v3.json
- type: x-website
  url: http://atlassian.com/
- type: x-website
  url: http://www.atlassian.com
- type: x-api-gallery
  url: http://att.dev.program.api.gallery.streamdata.io
- type: x-api-stack
  url: http://atlassian.stack.network
- type: x-blog
  url: http://blogs.atlassian.com/
- type: x-crunchbase
  url: https://crunchbase.com/organization/atlassian
- type: x-crunchbase
  url: http://www.crunchbase.com/company/atlassian
- type: x-email
  url: copyright@atlassian.com
- type: x-email
  url: trademarks@atlassian.com
- type: x-email
  url: sales@atlassian.com
- type: x-email
  url: ar_enterprise@atlassian.com
- type: x-email
  url: privacy@atlassian.com
- type: x-email
  url: eudatarep@atlassian.com
- type: x-email
  url: experts@atlassian.com
- type: x-email
  url: remittance@atlassian.com
- type: x-email
  url: ap@atlassian.com
- type: x-email
  url: procurement@atlassian.com
- type: x-github
  url: https://github.com/atlassian
- type: x-privacy-policy
  url: https://www.atlassian.com/legal/privacy-policy?_ga=2.188884514.868776184.1519225620-845241124.1519225620
- type: x-twitter
  url: https://twitter.com/atlassian
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---