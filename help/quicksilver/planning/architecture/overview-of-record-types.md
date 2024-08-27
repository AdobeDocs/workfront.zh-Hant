---
title: 記錄型別概觀
description: 記錄型別是Adobe Workfront Planning工作區的建置組塊。
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 1de095b3-78d9-44df-a678-51f4238deb91
source-git-commit: 83c716dea3815ed9a2ce4c3d0598ef42b128de87
workflow-type: tm+mt
source-wordcount: '274'
ht-degree: 0%

---


# 記錄型別概觀

{{planning-important-intro}}

與Workfront預先定義物件型別不同，在Adobe Workfront Planning中，您可以建立自己的物件型別。 例如，在Workfront中，已建立方案、Portfolio、專案、任務或問題的物件型別。

Workfront Planning物件型別稱為「記錄型別」，只有在使用者建立時，它們才會存在。 記錄型別是Workfront Planning工作區的建置組塊。 如需有關工作區的資訊，請參閱[建立工作區](/help/quicksilver/planning/architecture/create-workspaces.md)。

## 記錄型別概觀

在Workfront Planning中，您可以建立符合組織需求的自訂記錄型別。

如需有關建立記錄型別的資訊，請參閱[建立記錄型別](/help/quicksilver/planning/architecture/create-record-types.md)。

* 從範本建立工作區時，會在下列工作區區段中建立記錄型別：

   * **作業記錄型別**：代表策略性計畫、方案或計畫工作的記錄型別。 例如，行銷活動、活動、策略、機會是營運記錄型別。
   * **分類**：擷取有關作業記錄型別的屬性的記錄型別。 例如，地區、地址、對象是分類。

* 當您在從頭開始建立的工作區中建立記錄型別時，可以將記錄型別置於您在工作區中建立的任何區段中。
* 當您建立記錄型別時，只有您和您授予存取工作區許可權的人可以檢視記錄型別。
* 您必須先建立工作區，才能為工作區建立記錄型別。
* 一個工作區中總共可有1,000種記錄型別，無論工作區有多少區段皆然。 這包括您從頭建立的記錄型別，或使用範本時建立的記錄型別。


<!--

### Operational Record Type{#operational-record-type}

An operational record type is a Wrorkfront Planning record type that represents work-related objects.  

(***********insert screen shot**************)
For more information about operational record types including how to create them, see [Create record types](/help/quicksilver/planning/architecture/create-record-types.md). 

### Taxonomy{#taxonomy}

A taxonomy is a record type that captures attributes about an operational record type. 

(**********add screen shot**********)

Although creating taxonomies is identical to creating operational record types, Workfront Planning distinguishes conceptually between an operational record type and a taxonomy record type. The purpose of taxonomies is to enhance operational record types. Taxonomies should not directly represent work objects.  (***********this is no longer true, but might be later?!: A taxonomy is a record without dates, like a static list of attributes.***********) 

(********mimic what you did above for operational record types to say that we can also import taxonomies from other applications too - this will be possible later; for example Team would be a taxonomy record type, etc*************)

For example, Audience, Region, or Address can be taxonomy-type record types.  

## Similarities and differences between operational record types and taxonomies

The following table illustrates some of the similarities and differences between operational record types and taxonomies: 

| Record type and characteristic                              | Operational Record Type | Taxonomy Record Type |
|-------------------------------------------------------------|:-----------------------:|:--------------------:|
| They are part of a workspace                                |            ✓            |           ✓          |
| You can create them automatically, from a workspace template                    |            ✓            |           ✓          |
| You can create them manually, from scratch                    |            ✓            |           ✓          |
| You can create them by copying and pasting information from an external file or list                   |            ✓            |           ✓          |
| You can create by importing an Excel or CSV file                    |            ✓            |                     |
| You can create read-only record types by connecting to object types from other applications                    |            ✓            |                     |
| They represent work-related objects                         |            ✓            |                      |
| They represent attributes about work-related objects        |                         |           ✓          |
| You can create from scratch                                 |            ✓            |           ✓          |
| You can create by importing an Excel or CSV file            |            ✓            |                      |
| You can connect the record type to an object from another application|            ✓            |                      |
| You can connect to other record types               |            ✓            |                    |
| You can view their associated records in a table view       |            ✓            |           ✓          |
| You can view their associated records in a timeline view    |            ✓            |           ✓          |

-->