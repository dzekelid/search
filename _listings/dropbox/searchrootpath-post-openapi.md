---
swagger: "2.0"
x-collection-name: Dropbox
x-complete: 0
info:
  title: Dropbox Core Search for files and folders by name.
  description: |-
    Returns metadata for all files and folders whose filename contains the given search string as a substring.

    Searches are limited to the folder path and its sub-folder hierarchy provided in the call.

    **Note:** Recent changes may not immediately be reflected in search results due to a short delay in indexing.
  termsOfService: https://www.dropbox.com/developers/reference/tos
  contact:
    name: Dropbox
    url: https://www.dropbox.com/developers
  version: 1.0.0
host: api.dropbox.com
basePath: /1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /search/{root}/{path}:
    get:
      summary: Search for files and folders by name.
      description: |-
        Returns metadata for all files and folders whose filename contains the given search string as a substring.

        Searches are limited to the folder path and its sub-folder hierarchy provided in the call.

        **Note:** Recent changes may not immediately be reflected in search results due to a short delay in indexing.
      operationId: returns-metadata-for-all-files-and-folders-whose-filename-contains-the-given-search-string-as-a-subs
      x-api-path-slug: searchrootpath-get
      parameters:
      - in: query
        name: file_limit
        description: The maximum and default value is 1,000
      - in: query
        name: include_deleted
        description: If this parameter is set to `true`, then files and folders that
          have been deleted will also be includedin the search
      - in: query
        name: include_membership
        description: If `true`, metadata for a shared folder will include a list of
          members and a list of groups
      - in: query
        name: locale
        description: The metadata returned will have its `size` field translated based
          on the given `locale`
      - in: path
        name: path
        description: The path to the folder you want to search from
      - in: query
        name: query
        description: The search string
      - in: path
        name: root
        description: 'Root folder: `auto` - automatically determines the appropriate
          root folder using your apps permissionlevel (recommended); `sandbox` - the
          codename for app folder level; `dropbox` - full dropbox access'
      responses:
        200:
          description: OK
      tags:
      - Storage
      - Documents
      - Search
      - Root
      - Path
    post:
      summary: Search for files and folders by name.
      description: |-
        Returns metadata for all files and folders whose filename contains the given search string as a substring.

        Searches are limited to the folder path and its sub-folder hierarchy provided in the call.

        **Note:** Recent changes may not immediately be reflected in search results due to a short delay in indexing.
      operationId: returns-metadata-for-all-files-and-folders-whose-filename-contains-the-given-search-string-as-a-subs
      x-api-path-slug: searchrootpath-post
      parameters:
      - in: formData
        name: file_limit
        description: The maximum and default value is 1,000
      - in: formData
        name: include_deleted
        description: If this parameter is set to `true`, then files and folders that
          have been deleted will also be includedin the search
      - in: formData
        name: include_membership
        description: If `true`, metadata for a shared folder will include a list of
          members and a list of groups
      - in: formData
        name: locale
        description: The metadata returned will have its `size` field translated based
          on the given `locale`
      - in: path
        name: path
        description: The path to the folder you want to search from
      - in: formData
        name: query
        description: The search string
      - in: path
        name: root
        description: 'Root folder: `auto` - automatically determines the appropriate
          root folder using your apps permissionlevel (recommended); `sandbox` - the
          codename for app folder level; `dropbox` - full dropbox access'
      responses:
        200:
          description: OK
      tags:
      - Storage
      - Documents
      - Search
      - Root
      - Path
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