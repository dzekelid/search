---
swagger: "2.0"
info:
  title: BetterDoctor Record search
  description: "The endpoint can be used to identify providers with validation data.
    The search supports BetterDoctor unique provider identifier, National Provider
    Identifier (NPI) or reference uid based provider lookups. BetterDoctor identifiers
    and NPIs for doctors and practices can be discovered using BetterDoctor API\u2019s
    search functionalities. <br><h4 style='margin-bottom: 0px !important;'> Return
    Headers </h4> <div>Last-Modified: Timestamp of the last validation made over the
    matching validations. The value can be used to query changes in the validation
    status for the provider using since parameter in collaboration with HEAD method.</div>"
  version: 1.0.0
host: api.betterdoctor.com
basePath: /2016-03-01
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /validations:
    get:
      summary: Record search
      description: The endpoint can be used to identify providers with validation
        data
      operationId: the-endpoint-can-be-used-to-identify-providers-with-validation-data-the-search-supports-betterdoctor
      parameters:
      - in: query
        name: data_type
        description: Provider type to search validations for
      - in: query
        name: data_uid
        description: Paired with data_type
      - in: query
        name: limit
        description: For paginated list operations; specifies the maximum number of
          items to retrieve
      - in: query
        name: npi
        description: Paired with data_type
      - in: query
        name: ref_uid
        description: Optional to data_type style queries
      - in: query
        name: since
        description: Limits validations returned to the validations after the given
          timestamp value (ISO 8601)
      - in: query
        name: skip
        description: For paginated list operations; specifies the zero-based start
          index of the first item to retrieve
      - in: query
        name: user_key
        description: Your API access key
      - in: query
        name: validation_method
        description: Limits validations returned to a validation method wanted
      responses:
        200:
          description: OK
      tags:
      - record
      - search
      - validations
definitions:
  Info:
    properties:
      status:
        description: This is a default description.
        type: get
      api_version:
        description: This is a default description.
        type: get
      proxy_build_version:
        description: This is a default description.
        type: get
  Metadata:
    properties:
      data_type:
        description: This is a default description.
        type: get
      item_type:
        description: This is a default description.
        type: get
      total:
        description: This is a default description.
        type: get
      count:
        description: This is a default description.
        type: get
      skip:
        description: This is a default description.
        type: get
      limit:
        description: This is a default description.
        type: get
      fields_requested:
        description: This is a default description.
        type: get
      ignored_query_parameters:
        description: This is a default description.
        type: get
  ErrorMeta:
    properties:
      error:
        description: This is a default description.
        type: get
      message:
        description: This is a default description.
        type: get
      error_code:
        description: This is a default description.
        type: get
      http_status_code:
        description: This is a default description.
        type: get
      details:
        description: This is a default description.
        type: get
  ErrorMessage:
    properties: []
  ValidationErrorMeta:
    properties:
      error:
        description: This is a default description.
        type: get
      message:
        description: This is a default description.
        type: get
      error_code:
        description: This is a default description.
        type: get
      error_name:
        description: This is a default description.
        type: get
      http_status_code:
        description: This is a default description.
        type: get
  ValidationErrorDetails:
    properties:
      errors:
        description: This is a default description.
        type: get
  ValidationDetailedError:
    properties:
      code:
        description: This is a default description.
        type: get
      name:
        description: This is a default description.
        type: get
      message:
        description: This is a default description.
        type: get
      path:
        description: This is a default description.
        type: get
  ValidationErrorMessage:
    properties: []
  Doctor:
    properties:
      practices:
        description: This is a default description.
        type: get
      educations:
        description: This is a default description.
        type: get
      ratings:
        description: This is a default description.
        type: get
      insurances:
        description: This is a default description.
        type: get
      specialties:
        description: This is a default description.
        type: get
      hospital_affiliations:
        description: This is a default description.
        type: get
      group_affiliations:
        description: This is a default description.
        type: get
      claims:
        description: This is a default description.
        type: get
      licenses:
        description: This is a default description.
        type: get
      uid:
        description: This is a default description.
        type: get
  Doctor_Single:
    properties: []
  Doctor_List:
    properties:
      data:
        description: This is a default description.
        type: get
  Media:
    properties:
      uid:
        description: This is a default description.
        type: get
      status:
        description: This is a default description.
        type: get
      url:
        description: This is a default description.
        type: get
      tags:
        description: This is a default description.
        type: get
  MediaVersion:
    properties:
      thumbnail:
        description: This is a default description.
        type: get
      thumbnail2x:
        description: This is a default description.
        type: get
      small:
        description: This is a default description.
        type: get
      medium:
        description: This is a default description.
        type: get
      large:
        description: This is a default description.
        type: get
      hero:
        description: This is a default description.
        type: get
  PracticeDoctor:
    properties:
      educations:
        description: This is a default description.
        type: get
      ratings:
        description: This is a default description.
        type: get
      insurances:
        description: This is a default description.
        type: get
      specialties:
        description: This is a default description.
        type: get
      hospital_affiliations:
        description: This is a default description.
        type: get
      group_affiliations:
        description: This is a default description.
        type: get
      claims:
        description: This is a default description.
        type: get
      licenses:
        description: This is a default description.
        type: get
      uid:
        description: This is a default description.
        type: get
      npi:
        description: This is a default description.
        type: get
  Practice:
    properties:
      location_slug:
        description: This is a default description.
        type: get
      within_search_area:
        description: This is a default description.
        type: get
      distance:
        description: This is a default description.
        type: get
      lat:
        description: This is a default description.
        type: get
      lon:
        description: This is a default description.
        type: get
      uid:
        description: This is a default description.
        type: get
      slug:
        description: This is a default description.
        type: get
      name:
        description: This is a default description.
        type: get
      accepts_new_patients:
        description: This is a default description.
        type: get
      image_urls:
        description: This is a default description.
        type: get
  Practice_Single:
    properties: []
  Practice_List:
    properties:
      data:
        description: This is a default description.
        type: get
  Profile:
    properties:
      first_name:
        description: This is a default description.
        type: get
      last_name:
        description: This is a default description.
        type: get
      slug:
        description: This is a default description.
        type: get
      title:
        description: This is a default description.
        type: get
      image_url:
        description: This is a default description.
        type: get
      gender:
        description: This is a default description.
        type: get
      languages:
        description: This is a default description.
        type: get
      bio:
        description: This is a default description.
        type: get
  Profile_Single:
    properties: []
  Profile_List:
    properties:
      data:
        description: This is a default description.
        type: get
  Rating:
    properties:
      active:
        description: This is a default description.
        type: get
      provider:
        description: This is a default description.
        type: get
      provider_uid:
        description: This is a default description.
        type: get
      provider_url:
        description: This is a default description.
        type: get
      rating:
        description: This is a default description.
        type: get
      review_count:
        description: This is a default description.
        type: get
      image_url_small:
        description: This is a default description.
        type: get
      image_url_small_2x:
        description: This is a default description.
        type: get
      image_url_large:
        description: This is a default description.
        type: get
      image_url_large_2x:
        description: This is a default description.
        type: get
  Rating_Single:
    properties: []
  Rating_List:
    properties:
      data:
        description: This is a default description.
        type: get
  Specialty:
    properties:
      uid:
        description: This is a default description.
        type: get
      name:
        description: This is a default description.
        type: get
      category:
        description: This is a default description.
        type: get
      actor:
        description: This is a default description.
        type: get
      actors:
        description: This is a default description.
        type: get
  Specialty_Single:
    properties: []
  Specialty_List:
    properties:
      data:
        description: This is a default description.
        type: get
  StreetAddress:
    properties:
      city:
        description: This is a default description.
        type: get
      lat:
        description: This is a default description.
        type: get
      lon:
        description: This is a default description.
        type: get
      state:
        description: This is a default description.
        type: get
      state_long:
        description: This is a default description.
        type: get
      street:
        description: This is a default description.
        type: get
      street2:
        description: This is a default description.
        type: get
      zip:
        description: This is a default description.
        type: get
  StreetAddress_Single:
    properties: []
  StreetAddress_List:
    properties:
      data:
        description: This is a default description.
        type: get
  PhoneNumber:
    properties:
      number:
        description: This is a default description.
        type: get
      type:
        description: This is a default description.
        type: get
  PhoneNumber_Single:
    properties: []
  PhoneNumber_List:
    properties:
      data:
        description: This is a default description.
        type: get
  Location:
    properties:
      latitude:
        description: This is a default description.
        type: get
      longitude:
        description: This is a default description.
        type: get
      name:
        description: This is a default description.
        type: get
      slug:
        description: This is a default description.
        type: get
      state:
        description: This is a default description.
        type: get
      zoom_level:
        description: This is a default description.
        type: get
      tags:
        description: This is a default description.
        type: get
  Location_Single:
    properties: []
  Location_List:
    properties:
      data:
        description: This is a default description.
        type: get
  Language:
    properties:
      name:
        description: This is a default description.
        type: get
      code:
        description: This is a default description.
        type: get
  Language_Single:
    properties: []
  Language_List:
    properties:
      data:
        description: This is a default description.
        type: get
  Condition:
    properties:
      uid:
        description: This is a default description.
        type: get
      name:
        description: This is a default description.
        type: get
      url:
        description: This is a default description.
        type: get
      active:
        description: This is a default description.
        type: get
  Condition_Single:
    properties: []
  Condition_List:
    properties:
      data:
        description: This is a default description.
        type: get
  InsuranceProviderBase:
    properties:
      uid:
        description: This is a default description.
        type: get
      name:
        description: This is a default description.
        type: get
  InsuranceProviderBase_Single:
    properties: []
  InsuranceProviderBase_List:
    properties:
      data:
        description: This is a default description.
        type: get
  InsuranceProvider:
    properties:
      uid:
        description: This is a default description.
        type: get
      name:
        description: This is a default description.
        type: get
      plans:
        description: This is a default description.
        type: get
  InsuranceProvider_Single:
    properties: []
  InsuranceProvider_List:
    properties:
      data:
        description: This is a default description.
        type: get
  InsurancePlan:
    properties:
      uid:
        description: This is a default description.
        type: get
      name:
        description: This is a default description.
        type: get
      category:
        description: This is a default description.
        type: get
  InsurancePlan_Single:
    properties: []
  InsurancePlan_List:
    properties:
      data:
        description: This is a default description.
        type: get
  DoctorInsurancePlan:
    properties: []
  DoctorInsurancePlan_Single:
    properties: []
  DoctorInsurancePlan_List:
    properties:
      data:
        description: This is a default description.
        type: get
  License:
    properties: []
  License_Single:
    properties: []
  License_List:
    properties:
      data:
        description: This is a default description.
        type: get
  Education:
    properties:
      degree:
        description: This is a default description.
        type: get
  Education_Single:
    properties: []
  Education_List:
    properties:
      data:
        description: This is a default description.
        type: get
  Claim:
    properties:
      hcpcs:
        description: This is a default description.
        type: get
      hcpcs_description:
        description: This is a default description.
        type: get
      service_cnt:
        description: This is a default description.
        type: get
      bene_uniq_cnt:
        description: This is a default description.
        type: get
      avg_allowed_amt:
        description: This is a default description.
        type: get
      avg_charge_amt:
        description: This is a default description.
        type: get
      avg_payment_amt:
        description: This is a default description.
        type: get
  Claim_Single:
    properties: []
  Claim_List:
    properties:
      data:
        description: This is a default description.
        type: get
  HospitalAffiliation:
    properties:
      uid:
        description: This is a default description.
        type: get
      name:
        description: This is a default description.
        type: get
      type:
        description: This is a default description.
        type: get
  HospitalAffiliation_Single:
    properties: []
  HospitalAffiliation_List:
    properties:
      data:
        description: This is a default description.
        type: get
  GroupAffiliation:
    properties:
      uid:
        description: This is a default description.
        type: get
      name:
        description: This is a default description.
        type: get
      type:
        description: This is a default description.
        type: get
  GroupAffiliation_Single:
    properties: []
  GroupAffiliation_List:
    properties:
      data:
        description: This is a default description.
        type: get
  Highlight:
    properties:
      type:
        description: This is a default description.
        type: get
      description:
        description: This is a default description.
        type: get
  Highlight_Single:
    properties: []
  Highlight_List:
    properties:
      data:
        description: This is a default description.
        type: get
  ServiceStatus:
    properties:
      status:
        description: This is a default description.
        type: get
      api_version:
        description: This is a default description.
        type: get
      proxy_build_version:
        description: This is a default description.
        type: get
  ServiceStatus_Single:
    properties: []
  ServiceStatus_List:
    properties:
      data:
        description: This is a default description.
        type: get
  Validation:
    properties:
      data:
        description: This is a default description.
        type: get
      original_data:
        description: This is a default description.
        type: get
  ValidationMeta:
    properties:
      data_type:
        description: This is a default description.
        type: get
      data_uid:
        description: This is a default description.
        type: get
  ValidationOrigin:
    properties: []
  ValidationSource:
    properties:
      org:
        description: This is a default description.
        type: get
      created_at:
        description: This is a default description.
        type: get
      contexts:
        description: This is a default description.
        type: get
  ValidationSourceAuthor:
    properties:
      account_id:
        description: This is a default description.
        type: get
      name:
        description: This is a default description.
        type: get
      email:
        description: This is a default description.
        type: get
  ValidationSourceContext:
    properties:
      type:
        description: This is a default description.
        type: get
      validated_at:
        description: This is a default description.
        type: get
      status:
        description: This is a default description.
        type: get
      notes:
        description: This is a default description.
        type: get
      ref_uid:
        description: This is a default description.
        type: get
      validation_method:
        description: This is a default description.
        type: get
      tags:
        description: This is a default description.
        type: get
      ref_source:
        description: This is a default description.
        type: get
      ref_url:
        description: This is a default description.
        type: get
  ValidationList:
    properties:
      data:
        description: This is a default description.
        type: get
  ValidationListData:
    properties:
      value:
        description: This is a default description.
        type: get
x-collection-name: BetterDoctor
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