---
product-area: requests
navigation-topic: create-requests
title: 尋找已提交的請求
description: 瞭解Adobe Workfront的區域，您可在這裡找到您或其他人提交的請求，或您從未提交且已儲存為草稿的請求。
author: Alina
feature: Work Management
exl-id: cfa2383a-9594-4867-9b48-11b8ea281486
source-git-commit: cd059c445d86ed5581e8b2cb01507f18b97954f3
workflow-type: tm+mt
source-wordcount: '869'
ht-degree: 1%

---

# 尋找已提交的請求

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment.</span> -->

您可以找到您或其他人提交的下列請求型別，或是您已開始但您從未完成提交的請求。 您可以在Adobe Workfront的下列區域中找到這些請求：

* **已提交區段**：您或其他人提交且您至少有權存取檢視的所有請求。
* **草稿區段** ：所有您已開始但未完成且未提交的請求。 如需草稿請求的詳細資訊，請參閱 [建立並提交Adobe Workfront請求](../../../manage-work/requests/create-requests/create-submit-requests.md).

  >[!TIP]
  >
  >您只能檢視自己的草稿請求。

## 存取需求

您必須具備下列專案才能執行本文所述的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>任何 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權概觀*</td> 
   <td> <p>要求或以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>編輯問題的存取權</p> <p><b>附註</b>

如果您仍然沒有存取權，請詢問您的Workfront管理員是否對您的存取層級設定了其他限制。 如需有關Workfront管理員如何修改您的存取層級的資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>檢視要求或以上版本的許可權</p> <p>如需請求其他存取許可權的詳細資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">要求物件的存取權 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*若要瞭解您擁有的計畫、授權型別或存取權，請聯絡Workfront管理員。

## 尋找已提交的請求

若要尋找您或其他使用者已提交的請求：

1. 按一下 **主要功能表** 圖示 ![](assets/main-menu-icon.png) Adobe Workfront右上角。
1. 按一下 **已提交** 以檢視所有已提交的請求。

   您最多可以檢視2000個請求，且這些請求可顯示在多個頁面上。

   >[!TIP]
   >
   >您無法自訂已提交請求清單中的欄。

   ![](assets/nwe-submitted-requests-new-list-350x57.png)

   <!--update the shot above when we release the new Copy button to preview - for or after the 23.3 release-->

1. 預設會顯示下列欄：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">名稱</td> 
      <td> <p>要求的名稱。</p> <p>按一下要求的名稱以開啟。 </p> <p><b>秘訣</b>

   如果問題在轉換為任務或專案時未保留，則問題的名稱會變暗且無法再按一下。 如需轉換問題的相關資訊，請參閱 <a href="../../../manage-work/issues/convert-issues/convert-issues.md" class="MCXref xref">在Adobe Workfront中轉換問題的概觀</a>. </p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">轉換為</td> 
      <td> <p>解析物件的名稱，可以是請求已轉換為的任務或專案。 </p> <p>按一下任務或專案名稱以開啟。 </p> <p>如果未轉換請求，則此欄位為空白。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">路徑</td> 
      <td>最初提交請求的請求佇列、主題群組和佇列主題的名稱。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">狀態</td> 
      <td>請求或解析物件（任務或專案）的目前狀態</td> 
     </tr> 
     <tr> 
      <td role="rowheader">輸入日期</td> 
      <td>提交請求的日期或解決物件的建立日期（如果請求在轉換時被刪除）。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">上次更新日期</td> 
      <td> <p>上次更新請求的日期。</p> <p>依預設，已提交的請求清單會依此欄位排序。 </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. （選用）按一下欄的標題可依其排序。

   >[!TIP]
   >
   >當您離開已提交的請求清單時，所選的排序選項會保留。

1. （選用）在清單中選取請求，然後按一下 **開啟摘要** 圖示 ![](assets/open-summary-with-text-nwe.png) 若要開啟「摘要」面板並顯示請求的其他資訊，請新增註釋、檔案或將其指派。 如需「摘要」面板的相關資訊，請參閱 [摘要概觀](../../../workfront-basics/the-new-workfront-experience/summary-overview.md).

   >[!TIP]
   >
   >如果「摘要」面板已開啟，「開啟摘要」圖示會變更為「關閉摘要」。

1. （選擇性和條件性）按一下 **X** 圖示或右上角的「 」 **關閉摘要** 圖示 ![](assets/close-summary-with-text-nwe.png) 以關閉「摘要」面板。

   如果問題轉換為任務或專案，並且該問題在轉換過程中被刪除，則「摘要」面板為空白。 如需轉換問題的相關資訊，請參閱 [在Adobe Workfront中轉換問題的概觀](../../../manage-work/issues/convert-issues/convert-issues.md).

1. 從 **篩選圖示** ![](assets/filter-nwepng.png) 在清單的右上方，選取下表所列的任何篩選器。

   >[!TIP]
   >
   >您無法修改請求區域的已提交區段中的篩選器。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">全部</td> 
      <td>所有已提交的請求，無論狀態或提交者為何。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">開啟</td> 
      <td> <p>目前未完成的所有已提交請求，無論提交者為何。 只有您至少擁有檢視許可權的請求才會顯示在這裡（如果您未親自提交）。 </p> <p>沒有實際完成日期或其解析物件沒有實際完成日期的請求會列在「開啟」子頁標中。</p> <p><b>秘訣</b>

   處於不等於「已關閉」之任何狀態的請求會視為未完成。</p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">我的請求</td> 
      <td>您提交的請求，無論其狀態為何。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">我的未完成請求</td> 
      <td> <p>您提交的請求仍然未完成。 </p> <p>沒有實際完成日期或其解析物件沒有實際完成日期的請求會列在「我的未結請求」子頁標中。 </p> <p><b>秘訣</b>

   未處於已關閉狀態的請求會被視為未完成。</p> </td>
   </tr> 
    </tbody> 
   </table>

1. （可選）按一下 **篩選頁面** 圖示 ![](assets/search-icon.png) 位於清單頂端，依名稱搜尋請求。 清單會隨著符合搜尋條件的結果而更新。

   <!--
   <li value="9" data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>Click the&nbsp;<strong>Complete</strong> subtab to view requests that have been completed.</p> <p>(NOTE: this step will stay drafted even after release. We can't see Completed at this time!) <br>Requests with an Actual Completion Date or whose resolving object has an Actual Completion Date are listed in the Complete subtab.<br>Once a request receives an Actual Completion Date, it stays in the Recently Completed area for 10 business days. After that, it is moved to the Completed area. <br>For information about resolving and resolvable objects, see the article <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Overview of Resolving and Resolvable Objects </a>.</p> </li>
   -->

   <!--
   <li value="10" data-mc-conditions="QuicksilverOrClassic.Draft mode">(Optional) Select an option from the <strong>Sort by</strong> drop-down menu to sort the requests by the following criteria:&nbsp; &nbsp;(NOTE:&nbsp;this step will stay drafted even after release. We can't see Completed at this time!) &nbsp;
   <ul>
   <li><strong>Assigned To</strong>: Requests are sorted alphabetically by the name of the assignee using the following criteria:&nbsp;
   <ul>
   <li>All requests assigned to users are sorted first, in the order of the users' names.</li>
   <li>Requests assigned to job roles are sorted secondly, in the order of the job roles' names and are listed after all the requests assigned to users.</li>
   <li>Requests that are assigned to teams are sorted last, in the order of the teams' names and are listed after all the requests assigned to users and those assigned to job roles.</li>
   <li>All unassigned requests are listed last, in the order of their Entry Date. </li>
   </ul></li>
   <li><strong>Submitted On</strong>: Requests are sorted chronologically by the date when they were submitted.</li>
   <li><strong>Recently Updated</strong> (this is the default): Requests are sorted chronologically by the date of their last update.</li>
   <li><strong>Name</strong>: Requests are sorted alphabetically by name.&nbsp;</li>
   <li><strong>Priority</strong>: Requests are sorted in the order of their priority.</li>
   <li><strong>Queue</strong>: Requests are sorted alphabetically by the name of the requests queue where they were submitted.&nbsp;</li>
   <li><strong>Status</strong>: Requests are sorted alphabetically by their status.&nbsp;</li>
   </ul></li>
   -->

1. 按一下 **草稿** 以檢視所有草擬的請求。 Workfront會為此資料夾中的每個請求佇列儲存不限數量的草稿。 當您為已有草稿的佇列主題輸入新請求時，系統會提示您使用現有的草稿。 如需詳細資訊，請參閱 [從草稿建立請求](../../../manage-work/requests/create-requests/create-requests-from-drafts.md).

 

 

 
