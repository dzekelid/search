swagger: "2.0"
x-collection-name: EPA Envirofacts
x-complete: 1
info:
  title: U.S. EPA Enforcement and Compliance History Online (ECHO) - Safe Drinking
    Water Act
  description: enforcement-and-compliance-history-online-echo-is-a-tool-developed-and-maintained-by-epas-office-of-enforcement-and-compliance-assurance-for-public-use--echo-provides-integrated-compliance-and-enforcement-information-for-about-800000-regulated-facilities-nationwide-brbrsdw-rest-services-provides-multiple-service-endpoints-each-with-specific-capabilities-to-search-and-retrieve-data-on-public-water-systems-regulated-under-the-safe-drinking-water-act-sdwa--the-returned-results-reflect-data-drawn-from-epas-federal-safe-drinking-water-information-system-sdwis-database-brbrthe-get-systems-get-qid-and-get-download-end-points-are-meant-to-be-used-together-brbrthe-recommended-use-scenario-for-get-systems-get-qid-and-get-downoad-isbrbrb1bnbsp-use-get-systems-to-validate-passed-query-parameters-obtain-summary-statistics-and-to-obtain-a-query-id-qid---qids-are-time-sensitive-and-will-be-valid-for-approximately-30-minutes-brb2bnbsp-use-get-qid-with-the-returned-qid-to-paginate-through-arrays-of-water-system-results-brb3bnbsp-use-get-download-with-the-returned-qid-to-generate-a-comma-separated-value-csv-file-of-water-system-information-that-meets-the-qid-query-criteria-brbruse-the-qcolumns-parameter-to-customize-your-search-results---use-the-metdata-service-endpoint-for-a-list-of-available-output-objects-their-column-ids-and-their-definitions-to-help-you-build-your-customized-output--brbradditional-echo-resourcesnbspnbsp-a-hrefhttpsecho-epa-govtoolswebservicesweb-servicesa-a-hrefhttpsecho-epa-govresourcesechodataaboutthedataabout-echos-dataa-a-hrefhttpsecho-epa-govtoolsdatadownloadsdata-downloadsabr
  contact:
    name: US EPA, OECA Integration, Targeting and Access Branch
  version: 0.0.0
host: ofmpub.epa.gov
basePath: /echo
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /echo_rest_services.get_facility_info:
    get:
      summary: Combined ECHO Facility Enhanced Search Service
      description: Returns either an array of Facilities or an array of Clusters that
        meet the specified search criteria.
      operationId: returns-either-an-array-of-facilities-or-an-array-of-clusters-that-meet-the-specified-search-criteri
      x-api-path-slug: echo-rest-services-get-facility-info-get
      parameters:
      - in: query
        name: No Name
      - in: query
        name: output
        description: Output Format Flag
      - in: query
        name: qcolumns
        description: Used to cutomize service output
      responses:
        200:
          description: OK
      tags:
      - Environment
      - Combined
      - ECHO
      - Facility
      - Enhanced
      - Search
      - Service
  /echo_rest_services.get_facilities:
    get:
      summary: Combined ECHO Facility Search Service
      description: Validates query search parameters and returns query identifier.  Use
        the responseset parameter to set the page size
      operationId: validates-query-search-parameters-and-returns-query-identifier---use-the-responseset-parameter-to-se
      x-api-path-slug: echo-rest-services-get-facilities-get
      parameters:
      - in: query
        name: No Name
      - in: query
        name: output
        description: Output Format Flag
      - in: query
        name: qcolumns
        description: Used to cutomize service output
      responses:
        200:
          description: OK
      tags:
      - Environment
      - Combined
      - ECHO
      - Facility
      - Search
      - Service
  /air_rest_services.get_qid:
    get:
      summary: Clean Air Act Search by Query ID
      description: GET_QID is passed with a query ID corresponding to a previously
        run get_facilities query. It then returns a Facility object containing all
        matching facilities. The main purpose of GET_QID is for large querysets that
        contain multiple pages (responsesets) of output. GET_QID allows for pagination
        and for the selection and sorting of columns.
      operationId: get-qid-is-passed-with-a-query-id-corresponding-to-a-previously-run-get-facilities-query--it-then-re
      x-api-path-slug: air-rest-services-get-qid-get
      parameters:
      - in: query
        name: No Name
      - in: query
        name: output
        description: Output Format Flag
      responses:
        200:
          description: OK
      tags:
      - Environment
      - Clean
      - Air
      - Act
      - Search
      - By
      - Query
      - ID
  /air_rest_services.get_facility_info:
    get:
      summary: Clean Air Act Facility Enhanced Search
      description: Returns either an array of Facilities or an array of Clusters that
        meet the specified search criteria.
      operationId: returns-either-an-array-of-facilities-or-an-array-of-clusters-that-meet-the-specified-search-criteri
      x-api-path-slug: air-rest-services-get-facility-info-get
      parameters:
      - in: query
        name: No Name
      - in: query
        name: output
        description: Output Format Flag
      responses:
        200:
          description: OK
      tags:
      - Environment
      - Clean
      - Air
      - Act
      - Facility
      - Enhanced
      - Search
  /air_rest_services.get_facilities:
    get:
      summary: Clean Air Act Facility Search
      description: Validates query search parameters and returns query identifier.  Use
        the responseset parameter to set the page size
      operationId: validates-query-search-parameters-and-returns-query-identifier---use-the-responseset-parameter-to-se
      x-api-path-slug: air-rest-services-get-facilities-get
      parameters:
      - in: query
        name: No Name
      - in: query
        name: output
        description: Output Format Flag
      responses:
        200:
          description: OK
      tags:
      - Environment
      - Clean
      - Air
      - Act
      - Facility
      - Search
  /cwa_rest_services.get_facility_info:
    get:
      summary: Clean Water Act (CWA) Facility Enhanced Search Service
      description: Returns either an array of Facilities or an array of Clusters that
        meet the specified search criteria.
      operationId: returns-either-an-array-of-facilities-or-an-array-of-clusters-that-meet-the-specified-search-criteri
      x-api-path-slug: cwa-rest-services-get-facility-info-get
      parameters:
      - in: query
        name: No Name
      - in: query
        name: output
        description: Output Format Flag
      - in: query
        name: qcolumns
        description: Used to cutomize service output
      responses:
        200:
          description: OK
      tags:
      - Environment
      - Clean
      - Water
      - Act
      - (CWA)
      - Facility
      - Enhanced
      - Search
      - Service
  /cwa_rest_services.get_facilities:
    get:
      summary: Clean Water Act (CWA) Facility Search Service
      description: Validates query search parameters and returns query identifier.  Use
        the responseset parameter to set the page size
      operationId: validates-query-search-parameters-and-returns-query-identifier---use-the-responseset-parameter-to-se
      x-api-path-slug: cwa-rest-services-get-facilities-get
      parameters:
      - in: query
        name: No Name
      - in: query
        name: output
        description: Output Format Flag
      - in: query
        name: qcolumns
        description: Used to cutomize service output
      responses:
        200:
          description: OK
      tags:
      - Environment
      - Clean
      - Water
      - Act
      - (CWA)
      - Facility
      - Search
      - Service
  /case_rest_services.get_crcase_report:
    get:
      summary: Enforcement Criminal Case Summary Report Search
      description: The get_crcase_report service end point returns a complex object
        of criminal case detials based on the provided criminal case id.
      operationId: the-get-crcase-report-service-end-point-returns-a-complex-object-of-criminal-case-detials-based-on-t
      x-api-path-slug: case-rest-services-get-crcase-report-get
      parameters:
      - in: query
        name: No Name
      - in: query
        name: output
        description: Output Format Flag
      - in: query
        name: p_id
        description: Prosecution Summary Identifier
      responses:
        200:
          description: OK
      tags:
      - Environment
      - Enforcement
      - Criminal
      - Case
      - Summary
      - Report
      - Search
  /case_rest_services.get_cases:
    get:
      summary: Enforcement Case Search
      description: The get_cases service end point searches for civil enforcement
        and criminal cases based on the provided selection criteria.
      operationId: the-get-cases-service-end-point-searches-for-civil-enforcement-and-criminal-cases-based-on-the-provi
      x-api-path-slug: case-rest-services-get-cases-get
      parameters:
      - in: query
        name: No Name
      - in: query
        name: output
        description: Output Format Flag
      responses:
        200:
          description: OK
      tags:
      - Environment
      - Enforcement
      - Case
      - Search
  /case_rest_services.get_case_report:
    get:
      summary: Enforcement Case Summary Report Search
      description: The get_case_report service endpoint returns a complex object of
        civil enforcement case details based on the provided case id.
      operationId: the-get-case-report-service-endpoint-returns-a-complex-object-of-civil-enforcement-case-details-base
      x-api-path-slug: case-rest-services-get-case-report-get
      parameters:
      - in: query
        name: No Name
      - in: query
        name: output
        description: Output Format Flag
      - in: query
        name: p_id
        description: Case Number
      responses:
        200:
          description: OK
      tags:
      - Environment
      - Enforcement
      - Case
      - Summary
      - Report
      - Search
  /rcra_rest_services.get_facility_info:
    get:
      summary: Resource Conservation and Recovery Act (RCRA) Facility Enhanced Search
        Service
      description: Returns either an array of Facilities or an array of Clusters that
        meet the specified search criteria.
      operationId: returns-either-an-array-of-facilities-or-an-array-of-clusters-that-meet-the-specified-search-criteri
      x-api-path-slug: rcra-rest-services-get-facility-info-get
      parameters:
      - in: query
        name: No Name
      - in: query
        name: output
        description: Output Format Flag
      responses:
        200:
          description: OK
      tags:
      - Environment
      - Resource
      - Conservation
      - Recovery
      - Act
      - (RCRA)
      - Facility
      - Enhanced
      - Search
      - Service
  /rcra_rest_services.get_facilities:
    get:
      summary: Resource Conservation and Recovery Act (RCRA) Facility Search Service
      description: Validates query search parameters and returns query identifier.  Use
        the responseset parameter to set the page size
      operationId: validates-query-search-parameters-and-returns-query-identifier---use-the-responseset-parameter-to-se
      x-api-path-slug: rcra-rest-services-get-facilities-get
      parameters:
      - in: query
        name: No Name
      - in: query
        name: output
        description: Output Format Flag
      responses:
        200:
          description: OK
      tags:
      - Environment
      - Resource
      - Conservation
      - Recovery
      - Act
      - (RCRA)
      - Facility
      - Search
      - Service
  /sdw_rest_services.get_systems:
    get:
      summary: Safe Drinking Water Act (SDWA) Systems Search Service
      description: Returns an array of public water systems that meet the specified
        search criteria.
      operationId: returns-an-array-of-public-water-systems-that-meet-the-specified-search-criteria-
      x-api-path-slug: sdw-rest-services-get-systems-get
      parameters:
      - in: query
        name: No Name
      - in: query
        name: output
        description: Output Format Flag
      responses:
        200:
          description: OK
      tags:
      - Environment
      - Safe
      - Drinking
      - Water
      - Act
      - (SDWA)
      - Systems
      - Search
      - Service