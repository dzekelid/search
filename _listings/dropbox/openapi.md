swagger: "2.0"
x-collection-name: Dropbox
x-complete: 1
info:
  title: Dropbox Notify Appendix API v1
  description: the-dropbox-notify--is-a-part-of-dropbox-core-ap-with-a-separate-endpoint-for-notification-call-
  termsOfService: https://www.dropbox.com/developers/reference/tos
  contact:
    name: Dropbox
    url: https://www.dropbox.com/developers
  version: 1.0.0
host: api-notify.dropbox.com
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
  /search:
    get:
      summary: Search
      description: /search
      operationId: search
      x-api-path-slug: search-get
      parameters:
      - in: query
        name: file_limit
        description: The maximum and default value is 1,000
      - in: query
        name: include_deleted
        description: If this parameter is set to true, then files and folders that
          have been deleted will also be included in the search
      - in: query
        name: include_membership
        description: If true, metadata for a shared folder will include a list of
          the members of the shared folder
      - in: query
        name: locale
        description: The metadata returned will have its size field translated based
          on the given locale
      - in: query
        name: query
        description: The search string
      responses:
        200:
          description: OK
      tags:
      - Search