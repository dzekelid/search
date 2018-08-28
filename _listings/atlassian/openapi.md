swagger: "2.0"
x-collection-name: Atlassian
x-complete: 1
info:
  title: Stride API
  description: this-service-provides-public-api-for-the-stride-
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /content/search:
    get:
      summary: Search content by CQL
      description: "Returns the list of content that matches a Confluence Query Language
        \n(CQL) query. For information on CQL, see: \n[Advanced searching using CQL](https://developer.atlassian.com/cloud/confluence/advanced-searching-using-cql/).\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
        required**: \nPermission to access the Confluence site ('Can use' global permission).
        \nOnly content that the user has permission to view will be returned."
      operationId: com.atlassian.confluence.plugins.restapi.resources.ContentResource.searchContentByCQL_get
      x-api-path-slug: contentsearch-get
      parameters:
      - in: query
        name: cql
        description: The CQL string that is used to find the requested content
      - in: query
        name: cqlcontext
        description: The space, content, and content status to execute the search
          against
      - in: query
        name: expand
        description: A multi-value parameter indicating which properties of the content
          to expand
      - in: query
        name: limit
        description: The maximum number of content objects to return per page
      - in: query
        name: start
        description: The starting index of the returned content
      responses:
        200:
          description: OK
      tags:
      - Search
      - Content
      - By
      - CQL
  /search:
    get:
      summary: Search
      description: "Searches for content using the \n[Confluence Query Language (CQL)](https://developer.atlassian.com/cloud/confluence/advanced-searching-using-cql/)\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
        required**: \nPermission to view the entities. Note, only entities that the
        user has \npermission to view will be returned."
      operationId: com.atlassian.confluence.plugins.restapi.resources.SearchResource.search_get
      x-api-path-slug: search-get
      parameters:
      - in: query
        name: cql
        description: The CQL query to be used for the search
      - in: query
        name: cqlcontext
        description: The space, content, and content status to execute the searchagainst
      - in: query
        name: includeArchivedSpaces
        description: Include content from archived spaces in the results
      - in: query
        name: limit
        description: The maximum number of content objects to return per page
      - in: query
        name: start
        description: The starting index of the returned content
      responses:
        200:
          description: OK
      tags:
      - Search
  /api/2/project/search:
    get:
      summary: search
      description: Returns all projects visible to the currently logged in user, i.e.
        all projects the user has permission defined by the {@code action} parameter.
        If no user is logged in, all projects visible to anonymous users are returned.
      operationId: com.atlassian.jira.rest.v2.issue.ProjectResource.searchProjects_get
      x-api-path-slug: api2projectsearch-get
      parameters:
      - in: query
        name: action
        description: Type of the project action
      - in: query
        name: categoryId
        description: Project category filter
      - in: query
        name: expand
        description: Use [expand](https://developer
      - in: query
        name: maxResults
        description: Maximum number of items to return per page
      - in: query
        name: orderBy
        description: Ordering of the results by a given field from the following:*   `name`*   `key`*   `type`*   `category`*   `owner`Prefix
          it with + for ascending and - for descending order
      - in: query
        name: query
        description: A string used to filter the results; only projects with key or
          name containing the string will be returned (case insensitive)
      - in: query
        name: startAt
        description: Page offset, i
      - in: query
        name: typeKey
        description: Projects type key filter
      responses:
        200:
          description: OK
      tags:
      - Search