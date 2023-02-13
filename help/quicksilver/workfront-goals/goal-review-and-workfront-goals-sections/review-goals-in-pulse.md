---
product-previous: workfront-goals
navigation-topic: goal-review-and-sections
title: 在Adobe Workfront Goals Pulse區段中檢閱目標
description: 您可以檢視組織中的所有目標，無論擁有者是誰。 如需建立目標的相關資訊，請參閱在Adobe Workfront目標中建立目標。
author: Alina
feature: Workfront Goals
exl-id: 33873797-183d-4efc-9099-26eb907ca799
source-git-commit: 1d221d10e5845e477dff825f853330b9b4df0adf
workflow-type: tm+mt
source-wordcount: '911'
ht-degree: 1%

---

# 在Adobe Workfront Goals Pulse區段中檢閱目標

>[!IMPORTANT]
> 
>自23.1版開始，本文所述的功能已從Workfront中移除。\
>2023年初，23.1版發行後不久，也將移除本文。 此時，建議您據以更新任何書籤。


您可以檢視組織中的所有目標，無論擁有者是誰。 如需建立目標的相關資訊，請參閱 [在Adobe Workfront目標中建立目標](../../workfront-goals/goal-management/create-goals.md).

您可以使用Adobe Workfront目標的Pulse區段作為協作工具，在此檢閱並參與屬於您、您的團隊、群組或組織之目標的最新資訊流，並確保目標保持最新。 Workfront目標會依目標在Pulse區段中，將進度更新、留言和編輯歷史記錄分組。

## 存取需求

您必須具備下列存取權，才能執行本文所述的動作：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>Pro或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>要求或更高版本</p> <p>如需詳細資訊，請參閱 <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront授權概觀</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td> <p>您必須購買額外的Adobe Workfront目標授權才能存取本文所述的功能。 </p> <p>如需詳細資訊，請參閱 <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">使用Workfront目標的需求</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級*</td> 
   <td> <p>檢視或更高程度地存取目標</p> <p>備註:  <p>如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何變更您的存取層級的詳細資訊，請參閱：</p> 
     <ul> 
      <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a> </p> </li> 
      <li> <p><span href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md"><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md" class="MCXref xref">授予Adobe Workfront目標的存取權</a></span> </p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">物件權限</td> 
   <td> 
    <div> 
     <p>檢視目標的或更高權限</p> 
     <p>如需共用目標的相關資訊，請參閱 <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">在Workfront目標中共用目標</a>. </p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 必要條件

您必須具備下列條件，才能開始：

* 一種佈局模板，在主菜單中包括目標區域。

## 在Pulse區段中管理目標更新和註解 

>[!TIP]
>
>只有已至少簽入一次的目標才會顯示在「脈衝」區段中。

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) > **目標** 在螢幕的右上角。

   這會開啟Workfront目標區域。

   預設會顯示所有目標。

1. 按一下 **脈衝** 中。

   <!--
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
      (NOTE: see the numbering in the procedure)
      </MadCap:conditionalText>
      -->

   目標清單隨即顯示。 清單包含下列各欄，其中包含每個目標的相關資訊：

   <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
      <tr> 
         <td role="rowheader">目標</td> 
         <td>目標名稱。</td> 
      </tr> 
      <tr> 
         <td role="rowheader">所有者</td> 
         <td>目標所有者的名稱。</td> 
      </tr> 
      <tr> 
         <td role="rowheader">期間</td> 
         <td>排程目標的時段。</td> 
      </tr> 
      <tr> 
         <td role="rowheader">進度</td> 
         <td>目標的進度指標，通常為百分比值。</td> 
      </tr> 
      <tr> 
         <td role="rowheader"> <p>狀態（包括對齊表徵圖）</p> <p> <img src="assets/alignment-icon-large.png"> </p> </td> 
         <td> <p>目標的狀態，可以是下列其中一項：</p> 
         <ul> 
         <li>使用中</li> 
         <li>草稿</li> 
         <li>非使用中</li> 
         <li>已關閉</li> 
         </ul> <p>對齊圖示會顯示在與其他目標對齊的目標上。 如需協調目標的相關資訊，請參閱 <a href="../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md" class="MCXref xref">在Adobe Workfront目標中將目標連結起來，以協調目標</a>.</p>

   <p>「狀態」(Status)列還包括對每個結果或活動進行的增量更新，並在目標上進行每次簽入。</p>

   例如，如果目標有一個手動進度列活動，而您簽入目標並將活動更新為50%，則狀態欄會為該目標的活動顯示50%。 稍後，您可將相同的活動更新為60%。 在此情況下，10%的相同活動在相同目標下會顯示新行，因為您剛新增10%至活動進度。
   </td>
   </tr> 
      </tbody> 
      </table>

1. （可選）更新「脈衝」部分右上角的篩選器，以選擇要顯示的資訊類型。

   「脈衝」清單會顯示符合您所選篩選條件的目標及其更新的歷史記錄。

   如需篩選目標的詳細資訊，請參閱 [篩選Adobe Workfront目標中的資訊](../../workfront-goals/goal-management/filter-information-wf-goals.md).

1. 按一下目標名稱左側的右箭頭，以展開目標並檢視有關每個目標更新的其他資訊。

   下列資訊會顯示在每個目標下的「脈衝」區段中：

   * 結果名稱和所有者。 如需結果的相關資訊，請參閱 [將結果新增至Adobe Workfront目標中的目標](../../workfront-goals/results-and-activities/add-results-to-goals.md).
   * 活動名稱和擁有者。 如需活動的相關資訊，請參閱 [將活動新增至Adobe Workfront目標中的目標](../../workfront-goals/results-and-activities/add-activities-to-goals.md).
   * 結果和活動進度條和進度狀態。 如需Workfront目標如何計算目標進度的相關資訊，請參閱 [Adobe Workfront目標中的目標進度和條件概覽](../../workfront-goals/goal-management/calculate-goal-progress.md).

1. 按一下 **添加註釋** 為目標添加註釋，然後按一下 **貼文**. 注釋將顯示在「簽入」區域以及「目標詳細資訊」面板的「更新」頁簽中。 建議您使用「脈衝」區段，對一段時間內未更新的目標加以註解，並要求目標擁有者進行更新。

1. （選用）按一下 **顯示所有更新** 顯示所有目標更新。 這會開啟右側「目標詳細資料」面板中的「更新」標籤。
1. 按一下目標名稱以開啟 **目標詳細資料** 關於右方的小組，並審查關於目標的更多資訊以及管理目標及其成果和活動。 如需檢閱個別目標的相關資訊，請參閱 [更新Adobe Workfront目標中「目標詳細資訊」區段中的目標](../../workfront-goals/goal-management/update-goals-in-goal-details-panel.md).
1. （選用和條件式）按一下 **對齊圖示** ![](assets/align-icon.png) 在「目標對齊」部分中開啟目標（如果目標與其他目標對齊）。

1. （選用）展開 **每頁目標** 下拉式選單中選取，以顯示其他目標：

   * 20. 這是預設選取項目。
   * 50
   * 100


