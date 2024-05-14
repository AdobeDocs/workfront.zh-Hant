---
title: 記錄型別概觀
description: 記錄型別是Adobe Workfront Planning工作區的建置組塊。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 1de095b3-78d9-44df-a678-51f4238deb91
source-git-commit: b2ec979cf9aa2431c8c908440c227758d9dab521
workflow-type: tm+mt
source-wordcount: '270'
ht-degree: 0%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# 記錄型別概觀

{{maestro-important-intro}}

與Workfront預先定義物件型別不同，在Adobe Workfront Planning中，您可以建立自己的物件型別。 例如，在Workfront中，已建立方案、Portfolio、專案、任務或問題的物件型別。

Workfront Planning物件型別稱為「記錄型別」，您可以建立並自訂所有型別。 記錄型別是Workfront Planning工作區的建置組塊。 如需有關工作區的資訊，請參閱 [建立工作區](../architecture/create-workspaces.md).

## 記錄型別概觀

在Workfront Planning中，您可以建立符合組織需求的自訂記錄型別。

* 從範本建立工作區時，會在下列工作區區段中建立記錄型別：

   * [作業記錄型別](#operational-record-type)：代表策略性計畫、方案或計畫工作的記錄型別。 例如，促銷活動、活動、策略、機會可以是營運記錄型別。
   * [分類](#taxonomy)：擷取操作記錄型別相關屬性的記錄型別。 例如，地區、地址、對象可以是分類。

* 當您在從頭開始建立的工作區中建立記錄型別時，可以將記錄型別置於您在工作區中建立的任何區段中。
* 當您建立記錄型別時，只有您和您授予存取工作區許可權的人可以檢視記錄型別。
* 您必須先建立工作區，才能為工作區建立記錄型別。
* 一個工作區中總共可有1,000種記錄型別，無論工作區有多少區段皆然。 這包括您從頭建立的記錄型別，或使用範本時建立的記錄型別。


<!--

### Operational Record Type{#operational-record-type}

An operational record type is a Maestro record type that represents work-related objects.  

(***********insert screen shot**************)
For more information about operational record types including how to create them, see [Create record types](../architecture/create-record-types.md). 

### Taxonomy{#taxonomy}

A taxonomy is a record type that captures attributes about an operational record type. 

(**********add screen shot**********)

For more information about taxonomy record types, see [Create a taxonomy](../architecture/create-a-taxonomy.md). 

Although creating taxonomies is identical to creating operational record types, Maestro distinguishes conceptually between an operational record type and a taxonomy record type. The purpose of taxonomies is to enhance operational record types. Taxonomies should not directly represent work objects.  (***********this is no longer true, but might be later?!: A taxonomy is a record without dates, like a static list of attributes.***********) 

(********mimic what you did above for operational record types to say that we can also import taxonomies from other applications too - this will be possible later; for example Team would be a taxonomy record type, etc*************)

For example, Audience, Region, or Address can be taxonomy-type record types.  

For more information, see [Create a taxonomy](../architecture/create-a-taxonomy.md). 

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
| You can connect to other Maestro record types               |            ✓            |                    |
| You can view their associated records in a table view       |            ✓            |           ✓          |
| You can view their associated records in a timeline view    |            ✓            |           ✓          |

-->