swagger: "2.0"
x-collection-name: Kaltura
x-complete: 1
info:
  title: Kaltura VPaaS
  description: building-video-experiences-consists-of-ingesting-media-files-playing-back-videos-and-reviewing-usage-and-engagement-analytics--in-between-there-is-a-world-of-nuances-required-for-your-unique-usecase-and-application--kaltura-vpaas-is-built-on-the-principles-of-atomic-services-sdks-and-tools-that-allow-you-full-control-and-flexibility-over-every-element-and-process-in-your-medias-life-cycle-
  version: 3.3.0
host: www.kaltura.com
basePath: /api_v3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /service/captionsearch_captionassetitem/action/search:
    get:
      summary: Get Service Captionsearch Captionassetitem Action Search
      description: Search caption asset items by filter, pager and free text
      operationId: captionAssetItem.search
      x-api-path-slug: servicecaptionsearch-captionassetitemactionsearch-get
      parameters:
      - in: query
        name: captionAssetItemFilter[advancedSearch][attribute]
        description: 'Enum Type: `KalturaBaseEntryCompareAttribute`'
      - in: query
        name: captionAssetItemFilter[advancedSearch][categoriesMatchOr]
      - in: query
        name: captionAssetItemFilter[advancedSearch][categoryEntryStatusIn]
      - in: query
        name: captionAssetItemFilter[advancedSearch][categoryIdEqual]
      - in: query
        name: captionAssetItemFilter[advancedSearch][comparison]
        description: 'Enum Type: `KalturaSearchConditionComparison`'
      - in: query
        name: captionAssetItemFilter[advancedSearch][contentLike]
      - in: query
        name: captionAssetItemFilter[advancedSearch][contentMultiLikeAnd]
      - in: query
        name: captionAssetItemFilter[advancedSearch][contentMultiLikeOr]
      - in: query
        name: captionAssetItemFilter[advancedSearch][cuePointsFreeText]
      - in: query
        name: captionAssetItemFilter[advancedSearch][cuePointSubTypeEqual]
      - in: query
        name: captionAssetItemFilter[advancedSearch][cuePointTypeIn]
      - in: query
        name: captionAssetItemFilter[advancedSearch][depthGreaterThanEqual]
      - in: query
        name: captionAssetItemFilter[advancedSearch][distributionProfileId]
      - in: query
        name: captionAssetItemFilter[advancedSearch][distributionSunStatus]
        description: 'Enum Type: `KalturaEntryDistributionSunStatus`'
      - in: query
        name: captionAssetItemFilter[advancedSearch][entryDistributionFlag]
        description: 'Enum Type: `KalturaEntryDistributionFlag`'
      - in: query
        name: captionAssetItemFilter[advancedSearch][entryDistributionStatus]
        description: 'Enum Type: `KalturaEntryDistributionStatus`'
      - in: query
        name: captionAssetItemFilter[advancedSearch][entryDistributionValidationErrors]
        description: Comma seperated validation error types
      - in: query
        name: captionAssetItemFilter[advancedSearch][extendedStatusEqual]
        description: 'Enum Type: `KalturaUserEntryExtendedStatus`'
      - in: query
        name: captionAssetItemFilter[advancedSearch][extendedStatusIn]
      - in: query
        name: captionAssetItemFilter[advancedSearch][field]
      - in: query
        name: captionAssetItemFilter[advancedSearch][hasEntryDistributionValidationErrors]
      - in: query
        name: captionAssetItemFilter[advancedSearch][idEqual]
      - in: query
        name: captionAssetItemFilter[advancedSearch][idIn]
      - in: query
        name: captionAssetItemFilter[advancedSearch][indexIdGreaterThan]
      - in: query
        name: captionAssetItemFilter[advancedSearch][isQuiz]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: captionAssetItemFilter[advancedSearch][items]
      - in: query
        name: captionAssetItemFilter[advancedSearch][memberIdEq]
      - in: query
        name: captionAssetItemFilter[advancedSearch][memberIdIn]
      - in: query
        name: captionAssetItemFilter[advancedSearch][memberPermissionsMatchAnd]
      - in: query
        name: captionAssetItemFilter[advancedSearch][memberPermissionsMatchOr]
      - in: query
        name: captionAssetItemFilter[advancedSearch][metadataProfileId]
      - in: query
        name: captionAssetItemFilter[advancedSearch][noDistributionProfiles]
      - in: query
        name: captionAssetItemFilter[advancedSearch][not]
      - in: query
        name: captionAssetItemFilter[advancedSearch][objectType]
      - in: query
        name: captionAssetItemFilter[advancedSearch][orderBy]
        description: 'Enum Type: `KalturaCategoryEntryAdvancedOrderBy`'
      - in: query
        name: captionAssetItemFilter[advancedSearch][type]
        description: 'Enum Type: `KalturaSearchOperatorType`'
      - in: query
        name: captionAssetItemFilter[advancedSearch][updatedAtGreaterThanOrEqual]
      - in: query
        name: captionAssetItemFilter[advancedSearch][updatedAtLessThanOrEqual]
      - in: query
        name: captionAssetItemFilter[advancedSearch][userIdEqual]
      - in: query
        name: captionAssetItemFilter[advancedSearch][userIdIn]
      - in: query
        name: captionAssetItemFilter[advancedSearch][value]
      - in: query
        name: captionAssetItemFilter[advancedSearch][watermarkId]
      - in: query
        name: captionAssetItemFilter[captionParamsIdEqual]
      - in: query
        name: captionAssetItemFilter[captionParamsIdIn]
      - in: query
        name: captionAssetItemFilter[contentLike]
      - in: query
        name: captionAssetItemFilter[contentMultiLikeAnd]
      - in: query
        name: captionAssetItemFilter[contentMultiLikeOr]
      - in: query
        name: captionAssetItemFilter[createdAtGreaterThanOrEqual]
      - in: query
        name: captionAssetItemFilter[createdAtLessThanOrEqual]
      - in: query
        name: captionAssetItemFilter[deletedAtGreaterThanOrEqual]
      - in: query
        name: captionAssetItemFilter[deletedAtLessThanOrEqual]
      - in: query
        name: captionAssetItemFilter[endTimeGreaterThanOrEqual]
      - in: query
        name: captionAssetItemFilter[endTimeLessThanOrEqual]
      - in: query
        name: captionAssetItemFilter[entryIdEqual]
      - in: query
        name: captionAssetItemFilter[entryIdIn]
      - in: query
        name: captionAssetItemFilter[formatEqual]
        description: 'Enum Type: `KalturaCaptionType`'
      - in: query
        name: captionAssetItemFilter[formatIn]
      - in: query
        name: captionAssetItemFilter[idEqual]
      - in: query
        name: captionAssetItemFilter[idIn]
      - in: query
        name: captionAssetItemFilter[labelEqual]
      - in: query
        name: captionAssetItemFilter[labelIn]
      - in: query
        name: captionAssetItemFilter[languageEqual]
        description: 'Enum Type: `KalturaLanguage`'
      - in: query
        name: captionAssetItemFilter[languageIn]
      - in: query
        name: captionAssetItemFilter[orderBy]
      - in: query
        name: captionAssetItemFilter[partnerDescriptionLike]
      - in: query
        name: captionAssetItemFilter[partnerDescriptionMultiLikeAnd]
      - in: query
        name: captionAssetItemFilter[partnerDescriptionMultiLikeOr]
      - in: query
        name: captionAssetItemFilter[partnerIdEqual]
      - in: query
        name: captionAssetItemFilter[partnerIdIn]
      - in: query
        name: captionAssetItemFilter[sizeGreaterThanOrEqual]
      - in: query
        name: captionAssetItemFilter[sizeLessThanOrEqual]
      - in: query
        name: captionAssetItemFilter[startTimeGreaterThanOrEqual]
      - in: query
        name: captionAssetItemFilter[startTimeLessThanOrEqual]
      - in: query
        name: captionAssetItemFilter[statusEqual]
        description: 'Enum Type: `KalturaCaptionAssetStatus`'
      - in: query
        name: captionAssetItemFilter[statusIn]
      - in: query
        name: captionAssetItemFilter[statusNotIn]
      - in: query
        name: captionAssetItemFilter[tagsLike]
      - in: query
        name: captionAssetItemFilter[tagsMultiLikeAnd]
      - in: query
        name: captionAssetItemFilter[tagsMultiLikeOr]
      - in: query
        name: captionAssetItemFilter[typeIn]
      - in: query
        name: captionAssetItemFilter[updatedAtGreaterThanOrEqual]
      - in: query
        name: captionAssetItemFilter[updatedAtLessThanOrEqual]
      - in: query
        name: captionAssetItemPager[pageIndex]
        description: The page number for which {pageSize} of objects should be retrieved
          (Default is 1)
      - in: query
        name: captionAssetItemPager[pageSize]
        description: The number of objects to retrieve
      - in: query
        name: entryFilter[accessControlIdEqual]
      - in: query
        name: entryFilter[accessControlIdIn]
      - in: query
        name: entryFilter[adminTagsLike]
        description: This filter should be in use for retrieving specific entries
      - in: query
        name: entryFilter[adminTagsMultiLikeAnd]
        description: This filter should be in use for retrieving specific entries
      - in: query
        name: entryFilter[adminTagsMultiLikeOr]
        description: This filter should be in use for retrieving specific entries
      - in: query
        name: entryFilter[advancedSearch][attribute]
        description: 'Enum Type: `KalturaBaseEntryCompareAttribute`'
      - in: query
        name: entryFilter[advancedSearch][categoriesMatchOr]
      - in: query
        name: entryFilter[advancedSearch][categoryEntryStatusIn]
      - in: query
        name: entryFilter[advancedSearch][categoryIdEqual]
      - in: query
        name: entryFilter[advancedSearch][comparison]
        description: 'Enum Type: `KalturaSearchConditionComparison`'
      - in: query
        name: entryFilter[advancedSearch][contentLike]
      - in: query
        name: entryFilter[advancedSearch][contentMultiLikeAnd]
      - in: query
        name: entryFilter[advancedSearch][contentMultiLikeOr]
      - in: query
        name: entryFilter[advancedSearch][cuePointsFreeText]
      - in: query
        name: entryFilter[advancedSearch][cuePointSubTypeEqual]
      - in: query
        name: entryFilter[advancedSearch][cuePointTypeIn]
      - in: query
        name: entryFilter[advancedSearch][depthGreaterThanEqual]
      - in: query
        name: entryFilter[advancedSearch][distributionProfileId]
      - in: query
        name: entryFilter[advancedSearch][distributionSunStatus]
        description: 'Enum Type: `KalturaEntryDistributionSunStatus`'
      - in: query
        name: entryFilter[advancedSearch][entryDistributionFlag]
        description: 'Enum Type: `KalturaEntryDistributionFlag`'
      - in: query
        name: entryFilter[advancedSearch][entryDistributionStatus]
        description: 'Enum Type: `KalturaEntryDistributionStatus`'
      - in: query
        name: entryFilter[advancedSearch][entryDistributionValidationErrors]
        description: Comma seperated validation error types
      - in: query
        name: entryFilter[advancedSearch][extendedStatusEqual]
        description: 'Enum Type: `KalturaUserEntryExtendedStatus`'
      - in: query
        name: entryFilter[advancedSearch][extendedStatusIn]
      - in: query
        name: entryFilter[advancedSearch][field]
      - in: query
        name: entryFilter[advancedSearch][hasEntryDistributionValidationErrors]
      - in: query
        name: entryFilter[advancedSearch][idEqual]
      - in: query
        name: entryFilter[advancedSearch][idIn]
      - in: query
        name: entryFilter[advancedSearch][indexIdGreaterThan]
      - in: query
        name: entryFilter[advancedSearch][isQuiz]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: entryFilter[advancedSearch][items]
      - in: query
        name: entryFilter[advancedSearch][memberIdEq]
      - in: query
        name: entryFilter[advancedSearch][memberIdIn]
      - in: query
        name: entryFilter[advancedSearch][memberPermissionsMatchAnd]
      - in: query
        name: entryFilter[advancedSearch][memberPermissionsMatchOr]
      - in: query
        name: entryFilter[advancedSearch][metadataProfileId]
      - in: query
        name: entryFilter[advancedSearch][noDistributionProfiles]
      - in: query
        name: entryFilter[advancedSearch][not]
      - in: query
        name: entryFilter[advancedSearch][objectType]
      - in: query
        name: entryFilter[advancedSearch][orderBy]
        description: 'Enum Type: `KalturaCategoryEntryAdvancedOrderBy`'
      - in: query
        name: entryFilter[advancedSearch][type]
        description: 'Enum Type: `KalturaSearchOperatorType`'
      - in: query
        name: entryFilter[advancedSearch][updatedAtGreaterThanOrEqual]
      - in: query
        name: entryFilter[advancedSearch][updatedAtLessThanOrEqual]
      - in: query
        name: entryFilter[advancedSearch][userIdEqual]
      - in: query
        name: entryFilter[advancedSearch][userIdIn]
      - in: query
        name: entryFilter[advancedSearch][value]
      - in: query
        name: entryFilter[advancedSearch][watermarkId]
      - in: query
        name: entryFilter[assetParamsIdsMatchAnd]
      - in: query
        name: entryFilter[assetParamsIdsMatchOr]
      - in: query
        name: entryFilter[categoriesFullNameIn]
      - in: query
        name: entryFilter[categoriesIdsEmpty]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: entryFilter[categoriesIdsMatchAnd]
      - in: query
        name: entryFilter[categoriesIdsMatchOr]
        description: All entries of the categories, excluding their child categories
      - in: query
        name: entryFilter[categoriesIdsNotContains]
      - in: query
        name: entryFilter[categoriesMatchAnd]
      - in: query
        name: entryFilter[categoriesMatchOr]
        description: All entries within these categories or their child categories
      - in: query
        name: entryFilter[categoriesNotContains]
      - in: query
        name: entryFilter[categoryAncestorIdIn]
        description: All entries within this categoy or in child categories
      - in: query
        name: entryFilter[createdAtGreaterThanOrEqual]
        description: This filter parameter should be in use for retrieving only entries
          which were created at Kaltura system after a specific time/date (standard
          timestamp format)
      - in: query
        name: entryFilter[createdAtLessThanOrEqual]
        description: This filter parameter should be in use for retrieving only entries
          which were created at Kaltura system before a specific time/date (standard
          timestamp format)
      - in: query
        name: entryFilter[creatorIdEqual]
      - in: query
        name: entryFilter[documentTypeEqual]
        description: 'Enum Type: `KalturaDocumentType`'
      - in: query
        name: entryFilter[documentTypeIn]
      - in: query
        name: entryFilter[durationGreaterThanOrEqual]
      - in: query
        name: entryFilter[durationGreaterThan]
      - in: query
        name: entryFilter[durationLessThanOrEqual]
      - in: query
        name: entryFilter[durationLessThan]
      - in: query
        name: entryFilter[durationTypeMatchOr]
      - in: query
        name: entryFilter[endDateGreaterThanOrEqualOrNull]
      - in: query
        name: entryFilter[endDateGreaterThanOrEqual]
      - in: query
        name: entryFilter[endDateLessThanOrEqualOrNull]
      - in: query
        name: entryFilter[endDateLessThanOrEqual]
      - in: query
        name: entryFilter[entitledUsersEditMatchAnd]
      - in: query
        name: entryFilter[entitledUsersEditMatchOr]
      - in: query
        name: entryFilter[entitledUsersPublishMatchAnd]
      - in: query
        name: entryFilter[entitledUsersPublishMatchOr]
      - in: query
        name: entryFilter[externalSourceTypeEqual]
        description: 'Enum Type: `KalturaExternalMediaSourceType`'
      - in: query
        name: entryFilter[externalSourceTypeIn]
      - in: query
        name: entryFilter[flavorParamsIdsMatchAnd]
      - in: query
        name: entryFilter[flavorParamsIdsMatchOr]
      - in: query
        name: entryFilter[freeText]
      - in: query
        name: entryFilter[groupIdEqual]
      - in: query
        name: entryFilter[hasMediaServerHostname]
      - in: query
        name: entryFilter[idEqual]
        description: This filter should be in use for retrieving only a specific entry
          (identified by its entryId)
      - in: query
        name: entryFilter[idIn]
        description: This filter should be in use for retrieving few specific entries
          (string should include comma separated list of entryId strings)
      - in: query
        name: entryFilter[idNotIn]
      - in: query
        name: entryFilter[isLive]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: entryFilter[isRecordedEntryIdEmpty]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: entryFilter[isRoot]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: entryFilter[lastPlayedAtGreaterThanOrEqual]
      - in: query
        name: entryFilter[lastPlayedAtLessThanOrEqual]
      - in: query
        name: entryFilter[limit]
      - in: query
        name: entryFilter[mediaDateGreaterThanOrEqual]
      - in: query
        name: entryFilter[mediaDateLessThanOrEqual]
      - in: query
        name: entryFilter[mediaTypeEqual]
        description: 'Enum Type: `KalturaMediaType`'
      - in: query
        name: entryFilter[mediaTypeIn]
      - in: query
        name: entryFilter[moderationStatusEqual]
        description: 'Enum Type: `KalturaEntryModerationStatus`'
      - in: query
        name: entryFilter[moderationStatusIn]
      - in: query
        name: entryFilter[moderationStatusNotEqual]
        description: 'Enum Type: `KalturaEntryModerationStatus`'
      - in: query
        name: entryFilter[moderationStatusNotIn]
      - in: query
        name: entryFilter[nameEqual]
        description: This filter should be in use for retrieving entries with a specific
          name
      - in: query
        name: entryFilter[nameLike]
        description: This filter should be in use for retrieving specific entries
      - in: query
        name: entryFilter[nameMultiLikeAnd]
        description: This filter should be in use for retrieving specific entries
      - in: query
        name: entryFilter[nameMultiLikeOr]
        description: This filter should be in use for retrieving specific entries
      - in: query
        name: entryFilter[objectType]
      - in: query
        name: entryFilter[orderBy]
      - in: query
        name: entryFilter[parentEntryIdEqual]
      - in: query
        name: entryFilter[partnerIdEqual]
        description: This filter should be in use for retrieving only entries which
          were uploaded by/assigned to users of a specific Kaltura Partner (identified
          by Partner ID)
      - in: query
        name: entryFilter[partnerIdIn]
        description: This filter should be in use for retrieving only entries within
          Kaltura network which were uploaded by/assigned to users of few Kaltura
          Partners  (string should include comma separated list of PartnerIDs)
      - in: query
        name: entryFilter[partnerSortValueGreaterThanOrEqual]
      - in: query
        name: entryFilter[partnerSortValueLessThanOrEqual]
      - in: query
        name: entryFilter[redirectFromEntryId]
        description: The id of the original entry
      - in: query
        name: entryFilter[referenceIdEqual]
      - in: query
        name: entryFilter[referenceIdIn]
      - in: query
        name: entryFilter[replacedEntryIdEqual]
      - in: query
        name: entryFilter[replacedEntryIdIn]
      - in: query
        name: entryFilter[replacementStatusEqual]
        description: 'Enum Type: `KalturaEntryReplacementStatus`'
      - in: query
        name: entryFilter[replacementStatusIn]
      - in: query
        name: entryFilter[replacingEntryIdEqual]
      - in: query
        name: entryFilter[replacingEntryIdIn]
      - in: query
        name: entryFilter[rootEntryIdEqual]
      - in: query
        name: entryFilter[rootEntryIdIn]
      - in: query
        name: entryFilter[searchTextMatchAnd]
        description: 'This filter should be in use for retrieving specific entries
          while search match the input string within all of the following metadata
          attributes: name, description, tags, adminTags'
      - in: query
        name: entryFilter[searchTextMatchOr]
        description: 'This filter should be in use for retrieving specific entries
          while search match the input string within at least one of the following
          metadata attributes: name, description, tags, adminTags'
      - in: query
        name: entryFilter[sourceTypeEqual]
        description: 'Enum Type: `KalturaSourceType`'
      - in: query
        name: entryFilter[sourceTypeIn]
      - in: query
        name: entryFilter[sourceTypeNotEqual]
        description: 'Enum Type: `KalturaSourceType`'
      - in: query
        name: entryFilter[sourceTypeNotIn]
      - in: query
        name: entryFilter[startDateGreaterThanOrEqualOrNull]
      - in: query
        name: entryFilter[startDateGreaterThanOrEqual]
      - in: query
        name: entryFilter[startDateLessThanOrEqualOrNull]
      - in: query
        name: entryFilter[startDateLessThanOrEqual]
      - in: query
        name: entryFilter[statusEqual]
        description: 'Enum Type: `KalturaEntryStatus`This filter should be in use
          for retrieving only entries, at a specific {'
      - in: query
        name: entryFilter[statusIn]
        description: This filter should be in use for retrieving only entries, at
          few specific {
      - in: query
        name: entryFilter[statusNotEqual]
        description: 'Enum Type: `KalturaEntryStatus`This filter should be in use
          for retrieving only entries, not at a specific {'
      - in: query
        name: entryFilter[statusNotIn]
        description: This filter should be in use for retrieving only entries, not
          at few specific {
      - in: query
        name: entryFilter[tagsAdminTagsMultiLikeAnd]
      - in: query
        name: entryFilter[tagsAdminTagsMultiLikeOr]
      - in: query
        name: entryFilter[tagsAdminTagsNameMultiLikeAnd]
      - in: query
        name: entryFilter[tagsAdminTagsNameMultiLikeOr]
      - in: query
        name: entryFilter[tagsLike]
        description: This filter should be in use for retrieving specific entries
      - in: query
        name: entryFilter[tagsMultiLikeAnd]
        description: This filter should be in use for retrieving specific entries
      - in: query
        name: entryFilter[tagsMultiLikeOr]
        description: This filter should be in use for retrieving specific entries
      - in: query
        name: entryFilter[tagsNameMultiLikeAnd]
      - in: query
        name: entryFilter[tagsNameMultiLikeOr]
      - in: query
        name: entryFilter[totalRankGreaterThanOrEqual]
      - in: query
        name: entryFilter[totalRankLessThanOrEqual]
      - in: query
        name: entryFilter[typeEqual]
        description: 'Enum Type: `KalturaEntryType`'
      - in: query
        name: entryFilter[typeIn]
        description: This filter should be in use for retrieving entries of few {
      - in: query
        name: entryFilter[updatedAtGreaterThanOrEqual]
      - in: query
        name: entryFilter[updatedAtLessThanOrEqual]
      - in: query
        name: entryFilter[userIdEqual]
        description: This filter parameter should be in use for retrieving only entries,
          uploaded by/assigned to a specific user (identified by user Id)
      - in: query
        name: entryFilter[userIdIn]
      - in: query
        name: entryFilter[userIdNotIn]
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Captionsearch
      - Captionassetitem
      - Action
      - Search