## 4.0.0
- Remove the `root` property from EntityType definitions ([MODFQMMGR-780](https://folio-org.atlassian.net/browse/MODFQMMGR-780))
- Add support for custom entity types ([FQTM-12](https://folio-org.atlassian.net/browse/FQTM-12), [MODFQMMGR-632](https://folio-org.atlassian.net/browse/MODFQMMGR-632))
- Add the `available-joins` endpoint ([FQTM-14](https://folio-org.atlassian.net/browse/FQTM-14))
- Make the custom entity type definition optional in the `available-joins` endpoint ([FQTM-14](https://folio-org.atlassian.net/browse/FQTM-14))
- Restructure the `available-joins` API to avoid query parameters ([MODFQMMGR-608](https://folio-org.atlassian.net/browse/MODFQMMGR-608))
- Allow nested fields to be hidden from the UI ([MODFQMMGR-739](https://folio-org.atlassian.net/browse/MODFQMMGR-739))
- Add a `deleted` property to entity types ([MODFQMMGR-913](https://folio-org.atlassian.net/browse/MODFQMMGR-913))
- Split handling for `dateType` and `dateTimeType` fields ([MODFQMMGR-918](https://folio-org.atlassian.net/browse/MODFQMMGR-918))
- Remove the `deprecated` annotation from the `sortedIds` endpoint ([FQTM-19](https://folio-org.atlassian.net/browse/FQTM-19))
- Add a `usedBy` property to entity types ([FQTM-20](https://folio-org.atlassian.net/browse/FQTM-20))
- Add an API to update the entity type `usedBy` field ([MODFQMMGR-958](https://folio-org.atlassian.net/browse/MODFQMMGR-958))
- Add descriptions to the `available-joins` endpoint ([MODFQMMGR-972](https://folio-org.atlassian.net/browse/MODFQMMGR-972))
- Make `available-joins` use sources ([MODFQMMGR-988](https://folio-org.atlassian.net/browse/MODFQMMGR-988))
- Update the `available-joins` response ([MODFQMMGR-991](https://folio-org.atlassian.net/browse/MODFQMMGR-991))
- Add a `validated` property to fields ([MODFQMMGR-895](https://folio-org.atlassian.net/browse/MODFQMMGR-895))
- Add a `localizeForExports` property to fields ([MODFQMMGR-999](https://folio-org.atlassian.net/browse/MODFQMMGR-999))
- Add `QUEUED` query status and remove `afterId` from the synchronous query endpoint ([MODFQMMGR-982](https://folio-org.atlassian.net/browse/MODFQMMGR-982), [MODFQMMGR-763](https://folio-org.atlassian.net/browse/MODFQMMGR-763))
- Stop providing default source ordering ([MODFQMMGR-1017](https://folio-org.atlassian.net/browse/MODFQMMGR-1017))
- Standardize API error responses ([MODFQMMGR-1045](https://folio-org.atlassian.net/browse/MODFQMMGR-1045))
- Add the `/entity-types/{entityTypeId}/field-values` API ([MODFQMMGR-1048](https://folio-org.atlassian.net/browse/MODFQMMGR-1048))
- Add `_version` to custom entity types and remove obsolete entity type properties ([MODFQMMGR-1034](https://folio-org.atlassian.net/browse/MODFQMMGR-1034), [MODFQMMGR-1037](https://folio-org.atlassian.net/browse/MODFQMMGR-1037))
- Add support for default values for fields ([MODFQMMGR-628](https://folio-org.atlassian.net/browse/MODFQMMGR-628))
- Spring Boot upgrade to v4.0.2
- Add `maxColumnWidth` to entity type columns ([UIPQB-261](https://folio-org.atlassian.net/browse/UIPQB-261))

## 3.1.2
- Add support for entity-type-level filters ([MODFQMMGR-788](https://folio-org.atlassian.net/browse/MODFQMMGR-788))

## 3.1.1
- Add MAX_SIZE_EXCEEDED query status ([MODFQMMGR-723](https://folio-org.atlassian.net/browse/MODFQMMGR-723))

## 3.1.0
- Add order property to ET sources ([MODFQMMGR-543](https://folio-org.atlassian.net/browse/MODFQMMGR-543))
- New entity type join model ([FQTM-11](https://folio-org.atlassian.net/browse/FQTM-11))
- Update Java to v21 ([FOLIO-4235](https://folio-org.atlassian.net/browse/FOLIO-4235))

## 3.0.2
- Add new jsonbArrayType field type; this should be handled identically to arrayType by FQM consumers ([MODFQMMGR-548](https://folio-org.atlassian.net/browse/MODFQMMGR-548))

## 3.0.1
- Bump to spring-boot-starter-parent v3.3.5 ([FQTM-10](https://folio-org.atlassian.net/browse/FQTM-10))

## 3.0.0
  - Implement object model to support composite entity types [MODFQMMGR-229](https://folio-org.atlassian.net/browse/MODFQMMGR-229)
  - Add support for entity-type-level permissions [MODFQMMGR-268](https://folio-org.atlassian.net/browse/MODFQMMGR-268)
  - Make columns optional in an entity type [MODFMQMGR-313](https://folio-org.atlassian.net/browse/MODFMQMGR-313)
  - Improve support for free text UUIDs [MODFQMMGR-308](https://folio-org.atlassian.net/browse/MODFQMMGR-308)
  - Add ability to mark fields as ECS-only
  - Add ability to hide columns but keep them available for querying [MODFQMMGR-390](https://folio-org.atlassian.net/browse/MODFQMMGR-390)
  - Add ability to mark some columns as "essential" to control when they are inherited [MODFQMMGR-382](https://folio-org.atlassian.net/browse/MODFQMMGR-382)
  - Add options for controlling ECS support in entity types and refactor "special" value sources [MODFQMMGR-378](https://folio-org.atlassian.net/browse/MODFQMMGR-378)
  - Change entityTypeId in field sources from string to UUID [MODFQMMGR-427](https://folio-org.atlassian.net/browse/MODFQMMGR-427)
  - Add crossTenant property to query responses to indicate if the query was cross-tenant [MODFQMMGR-456](https://folio-org.atlassian.net/browse/MODFQMMGR-456)
  - Add support for query migration [MODLISTS-129](https://folio-org.atlassian.net/browse/MODLISTS-129)
  - Add support for query parameters to valueSourceApi settings
  - Add localize parameter to the GET contents endpoint [MODFQMMGR-481](https://folio-org.atlassian.net/browse/MODFQMMGR-481)
  - Mark the sortedIds API endpoint as deprecated [MODFQMMGR-417](https://folio-org.atlassian.net/browse/MODFQMMGR-417)
  - Add new privileged query contents endpoint [MODFQMMGR-563](https://folio-org.atlassian.net/browse/MODFQMMGR-563)

## 2.0.0
  - Add support for composite record IDs ([MODFQMMGR-137](https://folio-org.atlassian.net/browse/MODFQMMGR-137))
  - Add support for nested data types ([FQTM-6](https://folio-org.atlassian.net/browse/FQTM-6))
  - Bumped openapi-generator dependency to v7.3.0 ([FQTM-7](https://folio-org.atlassian.net/browse/FQTM-7))
  - Add queryable flag to entity type fields ([MODFQMMGR-141](https://folio-org.atlassian.net/browse/MODFQMMGR-141))
  - Set a max limit on the number of query results ([MODFQMMGR-172](https://folio-org.atlassian.net/browse/MODFQMMGR-172))

## 1.1.0
  - Change valueGetter type to string in EntityTypeColumn definition
  - Add filterValueGetter field to EntityTypeColumn definition
  - Add valueFunction field to EntityTypeColumn definition
  - Add isCustomField field to EntityTypeColumn definition
  - Add sourceViewExtractor field to EntityTypeColumn definition
  - Add valueSourceApi field to EntityTypeColumn definition
  - Add fromClause field to EntityType definition
  - Add groupByFields field to entityTypeDefinition
  - Add customFieldEntityTypeId field to EntityType definition
  - Add sourceView field to EntityType definition
  - Add nested object types

## 1.0.0
  - Initial module setup
