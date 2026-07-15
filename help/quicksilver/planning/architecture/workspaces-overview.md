---
title: Workspaces概述
description: 工作區是團隊使用的記錄型別集合，代表團隊的工作生命週期。 您可以在Adobe Workfront Planning中完全自訂工作區，以符合組織單位的工作流程。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: b80d5ccf-4d22-49f2-89b6-bb9678a353c2
TQID: https://experienceleague.adobe.com/Hh1Gh4ex1dLrPhsmqiLv3x5NAU0yKzIwcsV4hEogXTo
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
source-git-commit: 4ac828444e49213cdc4e00a5f92e404899e2225d
workflow-type: tm+mt
source-wordcount: 608
ht-degree: 0%

---

# 工作區概觀

<span class="preview">此頁面上的資訊是指尚未普遍提供的功能。 它僅在預覽環境中可供所有客戶使用。 在「預覽」版發行後，啟用的客戶每月可在「生產」環境中使用相同的功能。</span>

<span class="preview">如需快速發行資訊，請參閱[為您的組織啟用或停用快速發行](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>

{{planning-important-intro}}

工作區是組織單位使用的記錄型別集合，代表單位的工作生命週期與處理。 您可以在Adobe Workfront Planning中完全自訂工作區。

<!--update screenshot with production, it was broken at Preview-->

![工作區登陸頁面管理帳戶](assets/workspaces-landing-page-admin-account.png)

## 關於工作區的考量事項

* 您可以為組織內的特定組織單位建立工作區，以符合每個單位的獨特運作方式。
* Workfront Planning未隨附任何預先設定的工作區。 您必須根據組織的需求來建立這些範本。
* 您可以使用下列方式建立工作區：

   * 從頭開始
   * 使用範本。 範本包含預先設定的記錄型別數及其欄位。
   * 使用AI支援的Planning Designer。 此功能目前在Beta中。
   * 使用多工作區範本套裝。

  如需詳細資訊，請參閱[建立工作區](/help/quicksilver/planning/architecture/create-workspaces.md)。

* 工作區是組織單位（團隊、群組、部門或部門）進行工作的架構。 欄位無法建立關聯。 只有工作區中的記錄型別可以與欄位相關聯。

  如需詳細資訊，請參閱[記錄型別概觀](/help/quicksilver/planning/architecture/overview-of-record-types.md)。
* 工作區會顯示在Planning區域的下列標籤中：

   * **我所在的工作區**：顯示您建立的工作區或與您共用的工作區。
   * **其他工作區**：顯示系統中的所有其他工作區。 這僅供系統管理員使用。
   * <span class="preview">**範例工作區**：顯示內建的最佳實務工作區範例。 您無法編輯工作區、記錄型別，或新增記錄或欄位，但可以新增、編輯檢視並與他人共用檢視。</span>

  >[!NOTE]
  >
  ><span class="preview">我們建議您不要編輯範例工作區，而是使用這些工作區作為建立您自己的工作區的參考。 使用多工作區範本組合來建立與「範例工作區」標籤中所列的工作區相同的工作區。 如需相關資訊，請參閱[建立工作區](/help/quicksilver/planning/architecture/create-workspaces.md)一文中的「使用最佳實務多工作區範本套件組合建立多個工作區」一節。</span>

<!--
No longer the case - they match now: 

* For all other users:

* **Workspaces I'm on**: Workspaces they created (for Standard-license users) and workspaces others shared with them display in the Workspaces area.

<div class="preview"> 

* **Sample workspaces**: Displays built-in examples of best-practice workspaces. You cannot edit the workspaces, record types, or add records, but you can add, edit, and share views with others.

</div>
-->



* 工作區包含的記錄型別應反映工作生命週期和組織單位的概念。

  例如，如果單位的工作物件為行銷活動、產品和區域，則該單位的工作區應包含行銷活動、產品和區域的記錄型別。
* 當您建立工作區時，只有您才有權存取和管理您的工作區。 您必須與其他使用者共用，他們才能在相同空間中與您共同作業。

  如需詳細資訊，請參閱[共用工作區](/help/quicksilver/planning/access/share-workspaces.md)。

  系統管理員可以管理所有工作區，即使是他們未建立的工作區。

<!--make this live with the GA: * There is no limit for how many workspaces you can create in your environment. However, we recommend not to have too many workspaces, as they could become hard to manage and your workflows might be too fragmented.-->

* 您可以在Workfront Planning例項中建立的工作區物件數目有所限制。 如需詳細資訊，請參閱[Adobe Workfront Planning物件限制總覽](/help/quicksilver/planning/general/limitations-overview.md)。

## 全域搜尋概觀

在Planning登陸頁面上，您可以使用全域搜尋方塊來搜尋下列Planning物件：

* 工作區
* 記錄類型
* 檢視

![全域搜尋方塊](assets/global-search-box.png)

關於使用全域搜尋，請考量下列事項：

* 您可以按下列鍵盤組合，從Planning登陸頁面或任何Planning頁面存取搜尋：

   * Windows版CTRL+K
   * 適用於Mac的⌘+K
* 每個物件的最後7個結果都會顯示在搜尋方塊中。
* 您可以執行一般搜尋，或選取物件並搜尋個別清單。


