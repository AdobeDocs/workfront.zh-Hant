---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: 建立單次使用時程表
description: 如果您想要非週期性時程表，可以手動建立單次使用的時程表。 達到時程表的結束日期而您需要更多時程表時，您必須建立新時程表。
author: Lisa
feature: Timesheets
exl-id: b293dd50-a9b8-448b-afc1-8c7c7c79183b
source-git-commit: cd0214917620e0b147d0da3402ea2d34e28bc9c3
workflow-type: tm+mt
source-wordcount: '1062'
ht-degree: 0%

---

# 建立單次使用時程表

<!--Audited: 6/2025-->

如果您想要非週期性時程表，可以手動建立單次使用的時程表。 達到時程表的結束日期而您需要更多時程表時，您必須建立新時程表。

如需建立時程表設定檔的相關資訊，該設定檔可為您的使用者產生週期性時程表，而不需要您的任何進一步干預（建議），請參閱[建立、編輯和指派時程表設定檔](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md)。

如需有關在系統中為與時程表設定檔相關聯的所有使用者手動產生時程表的資訊，請參閱[手動產生時程表](/help/quicksilver/timesheets/create-and-manage-timesheets/manually-generate-timesheets.md)。

>[!NOTE]
>
>* 無法為群組建立單次使用的時程表。
>* 建立一次性使用時程表時，您無法選取要納入時程表的特定一般時數型別。 在您系統中啟動的所有一般小時型別都會顯示在手動建立的時程表中。
>
>如果您只想選擇某些一般小時型別顯示在您的時程表中，請使用時程表設定檔。 如需週期性時程表的詳細資訊，請參閱[建立、編輯和指派週期性時程表](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md)。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

<table style="table-layout:auto">
 <col> 
 <col>
 <tbody> 
  <tr> 
   <td>Adobe Workfront套件</td> 
   <td><p>任何</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront授權</td> 
   <td>
   <p>標準</p>
   <p>規劃</p></td>
  </tr> 
  <tr> 
   <td>存取層級設定</td> 
   <td><p>對時程表的管理存取權</p> </td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 建立單次使用時程表

{{step1-to-timesheets}}

依預設會選取&#x200B;**全部**&#x200B;篩選器。 這會顯示您有權檢視的所有時間表。

![已選取一個時程表的時程表清單](assets/timesheet-list-one-timesheet-selected-nwe-350x70.png)

1. （選用）執行下列任一項作業，更新時程表清單中的篩選器：

   * 選取頁面右上角的&#x200B;**我的時程表核准**，僅檢視您核准的時程表

     或

     選取&#x200B;**我的時程表**&#x200B;以僅檢視您的時程表。

     這會套用我的時程表核准或我的時程表篩選器到時程表清單。

     ![我的時程表篩選器按鈕在時程表清單頁面上](assets/my-timesheet-approvals-my-timesheets-pills-on-timesheets-list-nwe-350x58.png)

   * 按一下&#x200B;**篩選器**&#x200B;圖示![篩選器圖示](assets/filter-nwepng.png)以套用不同的篩選器，或建立新的篩選器。 如需建立或更新篩選的資訊，請參閱[在Adobe Workfront中建立或編輯篩選器](../../reports-and-dashboards/reports/reporting-elements/create-filters.md)。

   >[!NOTE]
   >
   >如果您的Workfront管理員或群組管理員從「設定」區域的「清單控制項」或您的「版面配置範本」中移除了「我的時程表核准」和「我的時程表」，則「我的時程表核准」和「我的時程表」選項不會顯示在時程表清單頂端或篩選器清單中。 如需詳細資訊，請參閱下列文章：
   > 
   >   * [使用配置範本自訂篩選器、檢視和群組](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)


1. （選擇性）按一下&#x200B;**搜尋**&#x200B;圖示![搜尋圖示](assets/search-icon.png)以輸入關鍵字並搜尋特定時間表。 例如，您可以搜尋擁有者名稱的時程表時間範圍。

1. （選擇性）按一下&#x200B;**檢視** ![檢檢視示](assets/view-icon.png)或&#x200B;**群組** ![群組圖示](assets/grouping.png)圖示，以套用不同的檢視或群組或建立新的檢視或群組。

   如需有關建立篩選器、檢視或群組的資訊，請參閱下列文章：

   * [在Adobe Workfront中建立或編輯篩選器](../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
   * [在Adobe Workfront中建立或編輯檢視](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md)
   * [在Adobe Workfront中建立群組](../../reports-and-dashboards/reports/reporting-elements/create-groupings.md)

1. 按一下時程表清單頂端的&#x200B;**新時程表**。

   指定下列資訊：

   <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
      <tr> 
      <td role="rowheader"><strong>建立</strong>的時程表 </td> 
      <td>開始輸入您為其建立時程表的使用者名稱、工作角色或團隊，然後在清單中顯示時按一下這些專案。</td> 
      </tr> 
      <tr> 
      <td role="rowheader"><strong>開始日期</strong> </td> 
      <td>這是時程表的開始日期。</td> 
      </tr> 
      <tr> 
      <td role="rowheader"><strong>結束日期</strong> </td> 
      <td> 這是時程表的結束日期。</td> 
      </tr> 
      <tr> 
      <td role="rowheader"><strong>核准者</strong> </td> 
      <td>核准者指核准與時程表相關聯之使用者之時程表的使用者。 只有具有時程表管理許可權的使用者才能設定為核准者。 如需時程表管理許可權的詳細資訊，請參閱<a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">授予使用者對特定區域的管理存取權</a>。<br>開始輸入時程表核准者的名稱，並在他們出現在清單中時按一下這些名稱。<br>您可在時程表上擁有多個核准者。 在這種情況下，在核准者核準時程表後，該時程表會被標籤為<strong>已關閉</strong>，並且會從所有剩餘核准者的時程表核准清單中消失。</td> 
      </tr> 
      <tr> 
      <td role="rowheader"><strong>可以編輯時間</strong> </td>

   <td> <p>如果您希望允許核准者編輯時程表上的小時，請選取此選項。</p>

   此選項可與「設定>時程表和時數>偏好設定」區域中的&#x200B;**限制所有者和管理員編輯時程表**&#x200B;設定搭配使用。 如需詳細資訊，請參閱<a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md">設定時程表和小時喜好設定</a>。

   存在下列情況：

   <ul>
      <li>啟用<b>限制所有者和管理員編輯時程表</b>選項時：</li>
   <ul><li>核准者只能核准和拒絕時程表，無論<b>可以編輯時間</b>是否已啟用。 </li>
   <li>時程表所有者的管理員只能檢視其直接報告的時程表。</li></ul>
   <li>當<b>限制所有者和管理員編輯時程表</b>選項停用時：</li>
   <ul><li>當<b>可以編輯時間</b>啟用時，核准者可以提交、重新開啟或關閉時程表，並且可以編輯時間。</li>
   <li>當<b>可以編輯時間</b>停用時，核准者無法提交、重新開啟或關閉時程表，也無法編輯時間。 核准者只能核准或拒絕時程表。 </li>
   <li>時程表所有者的管理員可以提交、撤銷、重新開啟及編輯其直接下屬的時程表。</li></ul>
   </ul>

   <p><b>附註</b>

   一旦您提交時程表進行核准，您就無法再編輯小時。 若要將已提交的時程表傳回至可編輯狀態，請撤回該時程表或讓核准者拒絕該時程表。 如需詳細資訊，請參閱<a href="../../timesheets/create-and-manage-timesheets/submit-timesheet-for-approval.md">提交時程表以供核准</a>和<a href="../../timesheets/create-and-manage-timesheets/timesheet-approvals.md">核準時程表</a>。</p> </p>

   </td> 
      </tr>

   <tr>

   <td role="rowheader"><span style="font-weight: bold;">加班</span> </td> 
      <td>您可以選擇隱藏時程表上的「加班」方塊。 此選項預設為停用。</td> 
      </tr> 
      </tbody> 
   </table>

1. 按一下&#x200B;**建立時間表**。

<!--the content in the table above will need to match the content in the Create timesheet profiles article-->

## 當任務和問題出現在使用者的時程表上時

如果任務或問題符合以下任何條件，則指派給使用者的任務或問題會自動出現在使用者的時程表中：

* 使用者已將時數記錄於任務或問題
* 任務或問題的計畫日期在時程表的日期內
* 任務或問題具有實際開始日期（任務或問題狀態為「進行中」）
* 任務或問題已釘選到時程表
* 計畫完成日期在時程表的日期範圍內，且狀態為進行中

如果取消選取&#x200B;**預先填入具有……**&#x200B;偏好設定的時程表（位於時程表和小時偏好設定中），時程表會顯示狀態為「進行中」的問題和任務。 如需時程表和小時喜好設定的詳細資訊，請參閱[設定時程表和小時喜好設定](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md)。
