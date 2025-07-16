---
product-area: requests
navigation-topic: create-requests
title: 找出已提交的請求
description: 瞭解Adobe Workfront的區域，您可在此找到您或其他人提交的請求，或您從未提交且已儲存為草稿的請求。
author: Alina
feature: Requests
topic: Collaboration
role: User
exl-id: cfa2383a-9594-4867-9b48-11b8ea281486
source-git-commit: b27b01e1efacc3fc459cec0a53b2c11cbe5e132b
workflow-type: tm+mt
source-wordcount: '1022'
ht-degree: 1%

---

# 找出已提交的請求

<span class="preview">本頁醒目提示的資訊指出尚未普遍可用的功能。 它僅在預覽環境中可供所有客戶使用。 每月發行至生產環境後，生產環境中為啟用快速發行的客戶也提供相同的功能。</span>

<span class="preview">如需快速發行資訊，請參閱[為您的組織啟用或停用快速發行](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>

您可以找到以下您或其他人提交的請求型別，或您已開始但您從未完成提交的請求。 您可以在Adobe Workfront的下列區域中找到這些請求：

* Workfront中「請求」區域的&#x200B;**Workfront**&#x200B;索引標籤：在下列區段中找出提交至Workfront請求佇列的請求：
   * **已提交區段**：您或其他人已提交且您至少有權存取檢視的所有要求。
   * **草稿區段** ：所有您已開始但您未完成且您未提交的請求。 如需草稿要求的詳細資訊，請參閱[建立並提交Adobe Workfront要求](../../../manage-work/requests/create-requests/create-submit-requests.md)。

  >[!TIP]
  >
  >您只能檢視自己的草稿要求。

* Workfront中請求區域的&#x200B;**規劃**&#x200B;標籤：找出提交至Workfront規劃請求表單的請求。 貴組織必須購買Workfront Planning套件。 如需詳細資訊，請參閱下列文章：

   * [在Adobe Workfront Planning中建立和管理請求表單](/help/quicksilver/planning/requests/create-request-form.md)
   * [提交Adobe Workfront Planning請求以建立記錄](/help/quicksilver/planning/requests/submit-requests.md)


## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td> <p>任何 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td> <p>新增：投稿人或更高版本</p>
   或
   <p>目前：要求或以上</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td><p>編輯問題的存取權</p></td> 
  </tr>
  <tr>
   <td role="rowheader">物件許可權</td> 
   <td><p>檢視請求上的許可權或更高的許可權</p></td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 找出已提交的請求

若要尋找您或其他使用者已提交的請求：

{{step1-to-requests}}

1. （視條件而定）如果您的組織已購買Workfront Planning套件，請按一下&#x200B;**Workfront**&#x200B;標籤以檢視Workfront請求。
1. 按一下左側面板中的&#x200B;**已提交**&#x200B;以檢視所有已提交的請求。

   您最多可檢視2000個請求，且這些請求可顯示在多個頁面上。

   >[!TIP]
   >
   >您無法自訂已提交請求清單中的欄。

   ![](assets/nwe-submitted-requests-new-list-350x57.png)


1. 預設會顯示下列欄：

   <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
      <tr> 
         <td role="rowheader">姓名</td> 
         <td> <p>要求的名稱。</p> <p>按一下請求的名稱以開啟。 </p> <p><b>秘訣</b>

   如果問題在轉換為任務或專案時未保留，則問題的名稱會變暗且無法再按一下。 如需轉換問題的相關資訊，請參閱<a href="../../../manage-work/issues/convert-issues/convert-issues.md" class="MCXref xref">在Adobe Workfront中轉換問題的概述</a>。 </p> </td>
   </tr> 
      <tr> 
         <td role="rowheader">轉換為</td> 
         <td> <p>解析物件的名稱，可以是請求已轉換為的任務或專案。 </p> <p>按一下任務或專案的名稱以開啟。 </p> <p>如果未轉換請求，則此欄位為空白。 </p> </td> 
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
         <td>提交請求的日期或解析物件的建立日期（如果請求在轉換時被刪除）。 </td> 
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
   >當您離開提交的請求清單時，所選的排序選項會保留。

1. （選擇性）在清單中選取要求，然後按一下&#x200B;**開啟摘要**&#x200B;圖示![](assets/open-summary-with-text-nwe.png)以開啟「摘要」面板，並顯示要求、新增註解、檔案或指派的其他相關資訊。 如需「摘要」面板的相關資訊，請參閱[摘要概觀](../../../workfront-basics/the-new-workfront-experience/summary-overview.md)。

   >[!TIP]
   >
   >如果「摘要」面板已經開啟，則「開啟摘要」圖示會變更為「關閉摘要」。

1. （選擇性和條件性）按一下右上角的&#x200B;**X**&#x200B;圖示或&#x200B;**關閉摘要**&#x200B;圖示![](assets/close-summary-with-text-nwe.png)以關閉摘要面板。

   如果問題轉換為任務或專案，且在轉換過程中已刪除問題，則「摘要」面板為空白。 如需轉換問題的相關資訊，請參閱[在Adobe Workfront中轉換問題的概述](../../../manage-work/issues/convert-issues/convert-issues.md)。

1. 從清單右上方的&#x200B;**篩選器圖示** ![](assets/filter-nwepng.png)中，選取下表所列的任何篩選器。

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
      <td> <p>目前未完成的所有已提交請求，不論提交者為何。 只有您至少有許可權檢視的要求，才會顯示在這裡（如果您未自行提交）。 </p> <p>沒有實際完成日期或解析物件沒有實際完成日期的請求會列在「開啟」子頁簽中。</p> <p><b>秘訣</b>

   處於任何不等於「已關閉」狀態的請求會視為未完成。</p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">我的請求</td> 
      <td>無論狀態為何，您皆已提交請求。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">我的待處理請求</td> 
      <td> <p>您提交的請求仍未完成。 </p> <p>沒有實際完成日期或解析物件沒有實際完成日期的請求會列在「我的未結請求」子頁標中。 </p> <p><b>秘訣</b>

   未處於已關閉狀態的請求會視為未完成。</p> </td>
   </tr> 
    </tbody> 
   </table>

1. （選擇性）按一下清單頂端的&#x200B;**篩選頁面**&#x200B;圖示![](assets/search-icon.png)，依名稱搜尋請求。 清單會以符合搜尋條件的結果更新。

   <!--
   <li value="9" data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>Click the <strong>Complete</strong> subtab to view requests that have been completed.</p> <p>(NOTE: this step will stay drafted even after release. We can't see Completed at this time!) <br>Requests with an Actual Completion Date or whose resolving object has an Actual Completion Date are listed in the Complete subtab.<br>Once a request receives an Actual Completion Date, it stays in the Recently Completed area for 10 business days. After that, it is moved to the Completed area. <br>For information about resolving and resolvable objects, see the article <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Overview of Resolving and Resolvable Objects </a>.</p> </li>
   -->

   <!--
   <li value="10" data-mc-conditions="QuicksilverOrClassic.Draft mode">(Optional) Select an option from the <strong>Sort by</strong> drop-down menu to sort the requests by the following criteria:   (NOTE: this step will stay drafted even after release. We can't see Completed at this time!)  
   <ul>
   <li><strong>Assigned To</strong>: Requests are sorted alphabetically by the name of the assignee using the following criteria: 
   <ul>
   <li>All requests assigned to users are sorted first, in the order of the users' names.</li>
   <li>Requests assigned to job roles are sorted secondly, in the order of the job roles' names and are listed after all the requests assigned to users.</li>
   <li>Requests that are assigned to teams are sorted last, in the order of the teams' names and are listed after all the requests assigned to users and those assigned to job roles.</li>
   <li>All unassigned requests are listed last, in the order of their Entry Date. </li>
   </ul></li>
   <li><strong>Submitted On</strong>: Requests are sorted chronologically by the date when they were submitted.</li>
   <li><strong>Recently Updated</strong> (this is the default): Requests are sorted chronologically by the date of their last update.</li>
   <li><strong>Name</strong>: Requests are sorted alphabetically by name. </li>
   <li><strong>Priority</strong>: Requests are sorted in the order of their priority.</li>
   <li><strong>Queue</strong>: Requests are sorted alphabetically by the name of the requests queue where they were submitted. </li>
   <li><strong>Status</strong>: Requests are sorted alphabetically by their status. </li>
   </ul></li>
   -->

1. 按一下&#x200B;**草稿**&#x200B;以檢視所有草擬的請求。 Workfront會針對此資料夾中的每個請求佇列儲存不限數量的草稿。 當您為已有草稿的佇列主題輸入新請求時，系統會提示您使用現有的草稿。 如需詳細資訊，請參閱[從草稿建立請求](../../../manage-work/requests/create-requests/create-requests-from-drafts.md)。

1. （選擇性和條件性）如果您的組織購買了Workfront計畫套件，請按一下&#x200B;**計畫**&#x200B;標籤，然後按一下左側面板中的&#x200B;**已提交**，以檢視Workfront計畫請求。

   使用&#x200B;**篩選器**&#x200B;和&#x200B;**資料行**&#x200B;來更新Planning要求清單中的資訊。

   ![](assets/workfront-planning-tab-submitted-section-in-requests-area.png)

   如需詳細資訊，請參閱[提交Adobe Workfront Planning要求以建立記錄](/help/quicksilver/planning/requests/submit-requests.md)。


