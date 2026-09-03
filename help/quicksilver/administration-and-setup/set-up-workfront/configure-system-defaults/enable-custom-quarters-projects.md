---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: 啟用自訂季度
description: 若您組織的季度是根據行事曆日期以外的特定條件（例如營業日或購物日），基於報表目的，您可能會想要建立自訂季度。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 0f643d36-6235-4fd3-b6d3-54fbd03c9b33
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/8kRfZ17zcgN0-hlc16wh328YGRjTlzuI3LAe-Yjj25s
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 6f64c3e6ebb8407c38ad3a1d46b2fc63b534879e
workflow-type: tm+mt
source-wordcount: 902
ht-degree: 2%

---

# 啟用自訂季度

<!--Audited: 03/2026-->

<!--remove Production and Preview references at release-->

<span class="preview">本頁醒目提示的資訊指出尚未普遍可用的功能。 它僅在預覽環境中可供所有客戶使用。 每月發行至生產環境後，生產環境中為啟用快速發行的客戶也提供相同的功能。</span>

<span class="preview">如需快速發行資訊，請參閱[為您的組織啟用或停用快速發行](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>


若您組織的季度是根據行事曆日期以外的特定條件（例如營業日或購物日），基於報表目的，您可能會想要建立自訂季度。

根據貴公司已購買的產品，您可以在Workfront設定區域中設定下列季度數：

* 僅購買[!DNL Workfront]的客戶，最多可以為其[!DNL Adobe Workfront]系統設定8個自訂季度。
* 購買[!DNL Workfront]和[!DNL Workfront Planning]的客戶可以為其[!DNL Workfront]系統設定最多100個季度，這些季度也可在[!DNL Planning]中使用。

<div class="preview">

* 購買[!DNL Workfront]和[!DNL Workfront Planning]的客戶可設定每個自訂季度的自訂周數。 自訂周數會顯示在[!DNL Planning]個時間軸檢視中。

</div>

## 存取權要求

+++ 展開以檢視這篇文章中所述功能的存取權要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] 封裝</td> 
   <td><p>任何</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] 授權</td> 
   <td><p>[！UICONTROL Workflow Standard]或[！UICONTROL Workfront Plan]授權</p>
       <p></p></td>
  </tr> 
  <tr> 
   <td>存取層級設定</td> 
   <td>[！UICONTROL系統管理員]</td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

<!--
When we release fiscal weeks, replace the table above with this:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] package</td> 
   <td>
   <ul>
   <li><p>To configure custom quarters:</p>
   <p>Any Workfront or Workflow package</p></li>
   <li>
   <div class="preview">
   <p>To configure custom weeks:</p>
   <p>Any Planning package, including Planning as a standalone product</p>
   </div>
   </li>
   </ul>
   </td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] license</td> 
   <td>
   
   <ul>
   <li><p>To configure custom quarters:</p>
   <p>[!UICONTROL Workflow Standard] or [!UICONTROL Workfront Plan] license</p></li>
   <li>
   <div class="preview">
   <p>To configure custom weeks:</p>
   <p>A [!UICONTROL Planning Standard] license, in addition to a Workfront or a Workflow license</p>
   </div>
   </li>
   </ul>
    </td>
  </tr> 
  <tr> 
   <td>Access level configurations</td> 
   <td>[!UICONTROL System Administrator]</td> 
  </tr> 
 </tbody> 
</table>

-->


## 為您的[!DNL Workfront]系統設定自訂季度

設定自訂季度會依您使用的環境而有所不同。

### 在生產環境中為您的[!DNL Workfront]系統設定自訂季度

{{step-1-to-setup}}

1. 按一下&#x200B;**[!UICONTROL 自訂季度]**。

1. 選取&#x200B;**[!UICONTROL 啟用自訂季度]**。

1. 輸入自訂季度的名稱，例如「2021年第一財政年度」。
1. 選取自訂季度的開始和結束日期。

   ![自訂季度](assets/custom-quarters-nwe.png)

1. （選擇性）按一下&#x200B;**[!UICONTROL 新增自訂季度]**&#x200B;以新增其他自訂季度至系統。

   >[!IMPORTANT]
   >
   > 如果貴公司已購買[!DNL Workfront Planning]，如果季度之間存在間隔或重疊，則您無法儲存自訂季度。
   >![自訂季度有重疊警告](assets/custom-quarters-with-overlap-warning.png)
   >只有[!DNL Workfront]個客戶才允許季之間的間隔和重疊。

1. （選擇性和條件性）如果貴公司只購買了[!DNL Workfront]，而沒有購買[!DNL Workfront Planning]，請建立參考會計季的報表元素。

   **範例：**&#x200B;為[!UICONTROL 專案]清單建立篩選器，並包含參考自訂季度的專案計畫完成日期。

   ![包含自訂季數的專案篩選器](assets/example-of-project-filter-with-custom-quarters.png)

   「本季」、「下一季」和「上一季」的參考資料會取代為自訂季度的新參考資料。

   如需有關報告元素的資訊，請參閱[報告元素：篩選器、檢視和群組](../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md)。

   如需建立篩選的詳細資訊，請參閱[在 [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md)中建立或編輯篩選。
1. （選擇性和條件性）如果貴公司已購買Workfront Planning，而您擁有[!DNL Workfront Planning]的存取權，請移至記錄型別頁面並開啟時間表檢視。 檢視會顯示新的自訂季度。
如需詳細資訊，請參閱[管理時間表檢視](/help/quicksilver/planning/views/manage-the-timeline-view.md)。

<div class="preview">

### 在預覽環境中設定[!DNL Workfront]系統的自訂季度

>[!NOTE]
>
>如果您的組織購買了Planning套件以及Workflow套件，或者如果他們購買了Workfront Planning作為獨立套件，則除了自訂季度之外，您還可以設定自訂周數。
> 
>自訂周不適用於Workfront報表和清單。

{{step-1-to-setup}}

1. 按一下&#x200B;**[!UICONTROL 自訂季度]**。

1. 選取&#x200B;**[!UICONTROL 啟用自訂季度]**。

1. 輸入自訂季度的名稱。 例如，「2021年第一財政年度」。
1. 選取自訂季度的開始和結束日期。

1. （選擇性）選取&#x200B;**開始新的自訂周順序**&#x200B;選項。

   選取後，此選項會在Planning時間表檢視中，將自訂季的開始設定為該季的第一個自訂周的開始。
1. （選擇性）在&#x200B;**自訂周標籤格式**&#x200B;區域，選擇自訂周標籤的&#x200B;**格式**。 從下列選項中選擇:

   * **W1、W2、W3 ...** 。 這是預設格式。
   * **FW1， FW2， FW3 ...**
   * **第1週、第2週、第3週……**
   * **自訂**

1. （視條件而定）如果您為&#x200B;**格式**&#x200B;欄位選取&#x200B;**自訂**，請輸入&#x200B;**自訂標籤**&#x200B;以識別自訂周數。

   自訂週會顯示在Planning時間表檢視中。

   >[!TIP]
   >
   >新增自訂標籤時，您最多可以輸入100個字元。
   >
   >您可以指定第一週的名稱，而接下來的幾週將使用相同的標籤，後面接著一個序號。
   >
   >例如，「會計週」的&#x200B;**自訂標籤**&#x200B;將新增「會計周1、會計周2、會計周3...」的標籤 到序列中的其餘周。

1. （選擇性）按一下&#x200B;**[!UICONTROL 新增自訂季度]**&#x200B;以新增其他自訂季度至系統。

   >[!IMPORTANT]
   >
   > 如果貴公司已購買[!DNL Workfront Planning]，如果季度之間存在間隔或重疊，則您無法儲存自訂季度。
   >![自訂季度有重疊警告](assets/custom-quarters-with-overlap-warning-red-outline.png)
   >只有[!DNL Workfront]個客戶才允許季之間的間隔和重疊。

1. （選擇性和條件性）若要在Workfront中檢視自訂季度，請建立參考自訂季度的報表元素。

   **範例：**&#x200B;為[!UICONTROL 專案]清單建立篩選器，並包含參考自訂季度的專案計畫完成日期。

   ![包含自訂季數的專案篩選器](assets/example-of-project-filter-with-custom-quarters.png)

   「本季」、「下一季」和「上一季」的參考資料會取代為自訂季度的新參考資料。

   如需有關報告元素的資訊，請參閱[報告元素：篩選器、檢視和群組](../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md)。

   如需建立篩選的詳細資訊，請參閱[在 [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md)中建立或編輯篩選。
1. （選擇性和條件性）若要在Workfront Planning中檢視自訂季度和周，請移至記錄型別頁面並開啟時間軸檢視。 檢視會顯示新的自訂季度和周。

如需詳細資訊，請參閱[管理時間表檢視](/help/quicksilver/planning/views/manage-the-timeline-view.md)。

</div>
