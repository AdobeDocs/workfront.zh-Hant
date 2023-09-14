---
title: 記錄型別和分類概觀
description: 記錄型別是Maestro工作區的建置組塊。
hidefromtoc: true
hide: true
source-git-commit: f058c369bdb3b991910d3a820895de73ea4709f0
workflow-type: tm+mt
source-wordcount: '526'
ht-degree: 0%

---


<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# 記錄型別和分類概觀

>[!IMPORTANT]
>
>目前，Adobe大師是測試版計畫的一部分，向有限數量的客戶開放。
>
>如需加入Maestro測試版計畫的詳細資訊，請聯絡您的客戶代表。
>
>如需詳細資訊，請參閱 [Adobe大師概觀](../maestro-overview.md).

與Workfront預先定義物件型別不同，在Adobe製作中，您可以建立自己的物件型別。 例如，在Workfront中，已建立方案、Portfolio、專案、任務或問題的物件型別。

Maestro物件型別稱為「記錄型別」。 記錄型別是Maestro工作區的建置組塊。 如需有關工作區的資訊，請參閱 [建立工作區](../architecture-and-fields/create-workspaces.md).

## 記錄型別概觀

在Maestro中，您可以建立符合組織需求的自訂記錄型別。

* 以下是Maestro記錄型別：

   * [作業記錄型別](#operational-record-type)：代表策略性計畫、方案或計畫工作的記錄型別。 例如，促銷活動、活動、策略、機會可以是營運記錄型別。
   * [分類法](#taxonomy)：擷取操作記錄型別相關屬性的記錄型別。 例如，地區、地址、對象可以是分類。

* 建立記錄型別時，組織中的所有人都可以檢視、編輯或刪除它。 <!--this will change with access levels and permissions-->
* 您必須先建立工作區，才能為工作區建立記錄型別。
* 在一個工作區中總共可以有1,000種作業記錄型別和分類。 這包括從頭建立或從其他系統匯入的記錄型別或分類。

### 作業記錄型別{#operational-record-type}

作業記錄型別是代表工作相關物件的Maestro記錄型別。

![](assets/operational-record-type-blank.png)

如需操作記錄型別的詳細資訊，包括如何建立它們，請參閱 [建立記錄型別](../architecture-and-fields/create-record-types.md).

### 分類法{#taxonomy}

分類法是一種記錄型別，可擷取有關作業記錄型別的屬性。

![](assets/taxonomy-record-type-blank.png)

如需分類記錄型別的詳細資訊，請參閱 [建立分類法](../architecture-and-fields/create-a-taxonomy.md).

雖然建立分類與建立作業記錄型別相同，但Maestro在概念上區分作業記錄型別和分類記錄型別。 分類法的用途是增強作業記錄型別。 分類不應該直接代表工作物件。  <!--this is no longer true, but might be later?!: A taxonomy is a record without dates, like a static list of attributes.-->

<!--mimic what you did above for operational record types to say that we can also import taxonomies from other applications too - this will be possible later; for example Team would be a taxonomy record type, etc -->

例如，「對象」、「區域」或「地址」可以是分類型別的記錄型別。

如需詳細資訊，請參閱 [建立分類法](../architecture-and-fields/create-a-taxonomy.md).

## 營運記錄型別與分類之間的異同

下表說明作業記錄型別與分類之間的一些異同：

| 記錄型別和特性 | 作業記錄型別 | 分類記錄型別 |
|-------------------------------------------------------------|:-----------------------:|:--------------------:|
| 它們是工作區的一部分 | ✓ (A) | ✓ |
| 您可以從工作區範本自動建立範本 | ✓ | ✓ |
| 您可以從頭開始手動建立 | ✓ | ✓ |
| 您可以從外部檔案或清單複製並貼上資訊，以建立它們 | ✓ | ✓ |
| 您可以透過匯入Excel或CSV檔案來建立 | ✓ |                     |
| 您可以透過從其他應用程式連線到物件型別來建立唯讀記錄型別 | ✓ |                     |
| 它們代表與工作相關的物件 | ✓ |                      |
| 它們代表工作相關物件的屬性 |                         | ✓ |
| 您可以從頭開始建立 | ✓ | ✓ |
| 您可以透過匯入Excel或CSV檔案來建立 | ✓ |                      |
| 您可以將記錄型別連線到第三方應用程式的物件 | ✓ |                      |
| 您可以連線到其他主要記錄型別 | ✓ |                    |
| 您可以在表格檢視中檢視其關聯記錄 | ✓ | ✓ |
| 您可以在時間表檢視中檢視其關聯記錄 | ✓ | ✓ |
