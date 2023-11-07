---
content-type: api
navigation-topic: api-navigation-topic
title: API第9版的新增功能（續）
description: 此清單是大型清單的第二個部分。 上半部分位於API 9版的新增功能。 如需版本9的更新清單，請前往API 9更新。
author: Becky
feature: Workfront API
role: Developer
exl-id: 0af97c16-e6a7-4796-92e0-4c2d9751c845
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '145'
ht-degree: 25%

---

# API第9版的新增功能（續）

此清單是大型清單的第二個部分。 上半部分可以位於 [API 9版的新增功能](../../wf-api/api/new-api-version-9.md). 如需第9版的更新清單，請前往 [API第9版的更新](../../wf-api/api/new-api-version-9-updates.md).

## PortalSection

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
| `accessorIDs` | `customer` | `accessRules` | `accessLevelMM` | `exportFusionChartToPDF` |  | `ADD` |
| `appGlobalID` | `enteredBy` | `lastViewers` | `displayDescription` | `getPK` |  | `COPY` |
| `controllerClass` | `filter` | `linkedRoles` | `displayName` | `getReportFromCache` |  | `COUNT` |
| `currency` | `groupBy` | `linkedTeams` | `groupIDs` | `isReportFilterable` |  | `DELETE` |
| `customerID` | `lastUpdatedBy` | `linkedUsers` | `linkedCustomersMM` | `linkCustomer` |  | `EDIT` |
| `dashboards` | `publicRunAsUser` | `portalTabSections` | `linkedPortalTabsMM` | `migratePortalSectionsPPMToAnaconda` |  | `GET` |
| `defaultTab` | `reportFolder` | `scheduledReports` | `linkedRoleIDs` | `unlinkCustomer` |  | `REPORT` |
| `definition` | `runAsUser` |  | `linkedTeamIDs` |  |  | `SEARCH` |
| `description` | `scheduledReport` |  | `linkedUsersMM` |   |   |   |
| `descriptionKey` | `statisticInfo` |  | `portalTabsMM`  |   |   |   |
| `enablePromptSecurity` | `view` |  | `scheduledReportsOM`  |   |   |   |
| `enteredByID`  |   |   |   |   |   |   |
| `extRefID`  |   |   |   |   |   |   |
| `filterControl`  |   |   |   |   |   |   |
| `filterID`  |   |   |   |   |   |   |
| `folderName`  |   |   |   |   |   |   |
| `forceLoad`  |   |   |   |   |   |   |
| `ganttOpen`  |   |   |   |   |   |   |
| `globalUIKey`  |   |   |   |   |   |   |
| `groupByID`  |   |   |   |   |   |   |
| `groupControl`  |   |   |   |   |   |   |
| `ID`  |   |   |   |   |   |   |
| `isAppGlobalCopiable`  |   |   |   |   |   |   |
| `isAppGlobalEditable`  |   |   |   |   |   |   |
| `isNewFormat` |   |   |   |   |   |   |
| `isPublic`  |   |   |   |   |   |   |
| `isReport`  |   |   |   |   |   |   |
| `isStandalone`  |   |   |   |   |   |   |
| `lastUpdateDate`  |   |   |   |   |   |   |
| `lastUpdatedByID`  |   |   |   |   |   |   |
| `maxResults`  |   |   |   |   |   |   |
| `methodName`  |   |   |   |   |   |   |
| `modDate`  |   |   |   |   |   |   |
| `name` |   |   |   |   |   |   |
| `nameKey`  |   |   |   |   |   |   |
| `objID`  |   |   |   |   |   |   |
| `objInterface` |   |   |   |   |   |   |
| `objObjCode` |   |   |   |   |   |   |
| `preferenceID` |   |   |   |   |   |   |
| `publicRunAsUserID` |   |   |   |   |   |   |
| `publicToken` |   |   |   |   |   |   |
| `reportFolderID`  |   |   |   |   |   |   |
| `reportType` |   |   |   |   |   |   |
| `runAsUserID`  |   |   |   |   |   |   |
| `scheduledReportID`  |   |   |   |   |   |   |
| `securityAncestorsDisabled`  |   |   |   |   |   |   |
| `securityRootID`  |   |   |   |   |   |   |
| `securityRootObjCode`  |   |   |   |   |   |   |
| `showPrompts`  |   |   |   |   |   |   |
| `sortBy`  |   |   |   |   |   |   |
| `sortBy2` |   |   |   |   |   |   |
| `sortBy3`  |   |   |   |   |   |   |
| `sortType`  |   |   |   |   |   |   |
| `sortType2` |   |   |   |   |   |   |
| `sortType3` |   |   |   |   |   |   |
| `specialView` |   |   |   |   |   |   |
| `toolBar` |   |   |   |   |   |   |
| `uiObjCode`  |   |   |   |   |   |   |
| `viewControl` |   |   |   |   |   |   |
| `viewID` |   |   |   |   |   |   |
| `width` |   |   |   |   |   |   |

{style="table-layout:auto"}

## PortalSectionLastViewer

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
| creationDate | `customer` |  |  |  |  | `COUNT` |
| `customerID` | `report` |  |  |  |  | `GET` |
| `ID` | `viewer` |  |  |  |  | `REPORT` |
| `reportID` |  |  |  |  |  | `SEARCH` |
| viewerID |   |   |   |   |   |   |

{style="table-layout:auto"}

## PortalSectionStatisticInfo

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
| `allViews` | `customer` |  |  |  |  | `COUNT` |
| `customerID` | `report` |  |  |  |  | `GET` |
| `ID` |  |  |  |  |  | `REPORT` |
| `lastUpdatedDate` |  |  |  |  |  | `SEARCH` |
| `reportID`  |   |   |   |   |   |   |
| `viewsLastMonth`  |   |   |   |   |   |   |
| `viewsLastQuarter` |   |   |   |   |   |   |
| `viewsLastYear` |   |   |   |   |   |   |
| `viewsThisMonth`  |   |   |   |   |   |   |
| `viewsThisQuarter`  |   |   |   |   |   |   |
| `viewsThisYear`  |   |   |   |   |   |   |

{style="table-layout:auto"}

## Portaltab

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
| `accessorIDs` | `customer` | `accessRules` | `linkedRoleIDs` | `advancedCopy` |  | `ADD` |
| `customerID` | `lastUpdatedBy` | `linkedRoles` | `linkedTeamIDs` | `exportDashboard` |  | `COPY` |
| `description` | `user` | `linkedTeams` | `linkedUsersMM` | `migrateCustomTabUserPrefs` |  | `COUNT` |
| `displayOrder` |  | `linkedUsers` |  |  |  | `DELETE` |
| `docID` |  | `portalTabSections` |  |  |  | `EDIT` |
| `extRefID` |  |  |  |  |  | `GET` |
| `ID` |  |  |  |  |  | `REPORT` |
| `isPublic` |  |  |  |  |  | `SEARCH` |
| `lastUpdateDate`  |   |   |   |   |   |   |
| `lastUpdatedByID`  |   |   |   |   |   |   |
| `name` |   |   |   |   |   |   |
| `nameKey`  |   |   |   |   |   |   |
| `portalProfileID`  |   |   |   |   |   |   |
| `tabname` |   |   |   |   |   |   |
| `userID`  |   |   |   |   |   |   |

{style="table-layout:auto"}

## PortalTabSection

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
| `area` | `calendarPortalSection`  |   |   |   |   |   |
| `calendarPortalSectionID` | `customer`  |   |   |   |   |   |
| `customerID` | `externalSection`  |   |   |   |   |   |
| `displayOrder` | `internalSection`  |   |   |   |   |   |
| `externalSectionID` | `portalTab` |   |   |   |   |   |
| ID |   |   |   |   |   |   |
| `internalSectionID` |   |   |   |   |   |   |
| `portalSectionObjCode`  |   |   |   |   |   |   |
| `portalSectionObjID`  |   |   |   |   |   |   |
| `portalTabID` |   |   |   |   |   |   |

{style="table-layout:auto"}

## 報告資料夾

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
| customerID | `customer` |   |   |   |   |   |
| `ID`  |   |   |   |   |   |   |
| 名稱 |   |   |   |   |   |   |

{style="table-layout:auto"}

## 排程報表

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
| `customerID` | `customer` | `groups` | `accessLevelMM` | `sendReportDeliveryNow` |  | `ADD` |
| `description` | `enteredBy` | `roles` |  |  |  | `COPY` |
| `enteredByID` | `portalSection` | `teams` |  |  |  | `COUNT` |
| `externalEmails` | `runAsUser` | `users` |  |  |  | `DELETE` |
| `format` |  |  |  |  |  | `EDIT` |
| `groupIDs` |  |  |  |  |  | `GET` |
| `ID` |  |  |  |  |  | `REPORT` |
| `isExcelHyperlinksEnabled` |  |  |  |  |  | `SEARCH` |
| `lastRuntimeMilliseconds` |   |   |   |   |   |   |
| `lastSentDate` |   |   |   |   |   |   |
| `name`  |   |   |   |   |   |   |
| `pageSize`  |   |   |   |   |   |   |
| `portalSectionID`  |   |   |   |   |   |   |
| `recipients`  |   |   |   |   |   |   |
| `recurrenceRule` |   |   |   |   |   |   |
| `roleIDs` |   |   |   |   |   |   |
| `runAsUserID` |   |   |   |   |   |   |
| `runAsUserTypeAhead` |   |   |   |   |   |   |
| `schedTime`  |   |   |   |   |   |   |
| `schedule` |   |   |   |   |   |   |
| `scheduleStart`  |   |   |   |   |   |   |
| `startDate`  |   |   |   |   |   |   |
| `teamIDs` |   |   |   |   |   |   |
| `uiObjCode`  |   |   |   |   |   |   |
| `uiObjID`  |   |   |   |   |   |   |
| `userIDs`  |   |   |   |   |   |   |
