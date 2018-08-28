---
swagger: "2.0"
x-collection-name: Xibo
x-complete: 0
info:
  title: Xibo API Notification Search
  description: Search this users Notifications
  termsOfService: http://xibo.org.uk/legal
  version: 1.0.0
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /campaign:
    get:
      summary: Search Campaigns
      description: Search all Campaigns this user has access to
      operationId: campaignSearch
      x-api-path-slug: campaign-get
      parameters:
      - in: formData
        name: campaignId
        description: Filter by Campaign Id
      - in: formData
        name: hasLayouts
        description: Filter by has layouts
      - in: formData
        name: isLayoutSpecific
        description: Filter by whether this Campaign is specific to a Layout or User
          added
      - in: formData
        name: name
        description: Filter by Name
      - in: formData
        name: retired
        description: Filter by retired
      - in: formData
        name: tags
        description: Filter by Tags
      - in: formData
        name: totalDuration
        description: Should we total the duration?
      responses:
        200:
          description: OK
      tags:
      - Search
      - Campaigns
  /command:
    get:
      summary: Command Search
      description: Search this users Commands
      operationId: commandSearch
      x-api-path-slug: command-get
      parameters:
      - in: formData
        name: code
        description: Filter by Command Code
      - in: formData
        name: command
        description: Filter by Command Name
      - in: formData
        name: commandId
        description: Filter by Command Id
      responses:
        200:
          description: OK
      tags:
      - Command
      - Search
  /dataset:
    get:
      summary: DataSet Search
      description: Search this users DataSets
      operationId: dataSetSearch
      x-api-path-slug: dataset-get
      parameters:
      - in: formData
        name: code
        description: Filter by DataSet Code
      - in: formData
        name: dataSet
        description: Filter by DataSet Name
      - in: formData
        name: dataSetId
        description: Filter by DataSet Id
      - in: formData
        name: embed
        description: Embed related data such as columns
      responses:
        200:
          description: OK
      tags:
      - DataSet
      - Search
  /dataset/{dataSetId}/column:
    get:
      summary: Search Columns
      description: Search Columns for DataSet
      operationId: dataSetColumnSearch
      x-api-path-slug: datasetdatasetidcolumn-get
      parameters:
      - in: formData
        name: dataSetColumnId
        description: Filter by DataSet ColumnID
      - in: path
        name: dataSetId
        description: The DataSet ID
      responses:
        200:
          description: OK
      tags:
      - Search
      - Columns
  /daypart:
    get:
      summary: Daypart Search
      description: Search dayparts
      operationId: dayPartSearch
      x-api-path-slug: daypart-get
      parameters:
      - in: formData
        name: dayPartId
        description: The dayPart ID to Search
      - in: formData
        name: embed
        description: Embed related data such as exceptions
      - in: formData
        name: name
        description: The name of the dayPart to Search
      responses:
        200:
          description: OK
      tags:
      - Daypart
      - Search
  /display:
    get:
      summary: Display Search
      description: Search Displays for this User
      operationId: displaySearch
      x-api-path-slug: display-get
      parameters:
      - in: formData
        name: authorised
        description: Filter by authorised flag
      - in: formData
        name: clientVersion
        description: Filter by Client Version
      - in: formData
        name: display
        description: Filter by Display Name
      - in: formData
        name: displayGroupId
        description: Filter by DisplayGroup Id
      - in: formData
        name: displayId
        description: Filter by Display Id
      - in: formData
        name: displayProfileId
        description: Filter by Display Profile
      - in: formData
        name: embed
        description: Embed related data, namely displaygroups
      - in: formData
        name: hardwareKey
        description: Filter by Hardware Key
      - in: formData
        name: macAddress
        description: Filter by Mac Address
      responses:
        200:
          description: OK
      tags:
      - Display
      - Search
  /displayprofile:
    get:
      summary: Display Profile Search
      description: Search this users Display Profiles
      operationId: displayProfileSearch
      x-api-path-slug: displayprofile-get
      parameters:
      - in: formData
        name: displayProfile
        description: Filter by DisplayProfile Name
      - in: formData
        name: displayProfileId
        description: Filter by DisplayProfile Id
      - in: formData
        name: type
        description: Filter by DisplayProfile Type (windows|android)
      responses:
        200:
          description: OK
      tags:
      - Display
      - Profile
      - Search
  /layout:
    get:
      summary: Search Layouts
      description: Search for Layouts viewable by this user
      operationId: layoutSearch
      x-api-path-slug: layout-get
      parameters:
      - in: formData
        name: embed
        description: Embed related data such as regions, playlists, tags, etc
      - in: formData
        name: exactTags
        description: A flag indicating whether to treat the tags filter as an exact
          match
      - in: formData
        name: layout
        description: Filter by partial Layout name
      - in: formData
        name: layoutId
        description: Filter by Layout Id
      - in: formData
        name: ownerUserGroupId
        description: Filter by users in this UserGroupId
      - in: formData
        name: retired
        description: Filter by retired flag
      - in: formData
        name: tags
        description: Filter by Tags
      - in: formData
        name: userId
        description: Filter by user Id
      responses:
        200:
          description: OK
      tags:
      - Search
      - Layouts
  /library:
    get:
      summary: Library Search
      description: Search the Library for this user
      operationId: librarySearch
      x-api-path-slug: library-get
      parameters:
      - in: formData
        name: duration
        description: Filter by Duration - a number or less-than,greater-than,less-than-equal
          or great-than-equal followed by a | followed by a number
      - in: formData
        name: exactTags
        description: A flag indicating whether to treat the tags filter as an exact
          match
      - in: formData
        name: fileSize
        description: Filter by File Size - a number or less-than,greater-than,less-than-equal
          or great-than-equal followed by a | followed by a number
      - in: formData
        name: media
        description: Filter by Media Name
      - in: formData
        name: mediaId
        description: Filter by Media Id
      - in: formData
        name: ownerId
        description: Filter by Owner Id
      - in: formData
        name: ownerUserGroupId
        description: Filter by users in this UserGroupId
      - in: formData
        name: retired
        description: Filter by Retired
      - in: formData
        name: tags
        description: Filter by Tags - comma seperated
      - in: formData
        name: type
        description: Filter by Media Type
      responses:
        200:
          description: OK
      tags:
      - Library
      - Search
  /notification:
    get:
      summary: Notification Search
      description: Search this users Notifications
      operationId: notificationSearch
      x-api-path-slug: notification-get
      parameters:
      - in: formData
        name: notificationId
        description: Filter by Notification Id
      - in: formData
        name: subject
        description: Filter by Subject
      responses:
        200:
          description: OK
      tags:
      - Notification
      - Search
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