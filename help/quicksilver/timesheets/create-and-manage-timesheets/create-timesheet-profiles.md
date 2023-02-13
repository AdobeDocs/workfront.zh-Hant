---
product-area: timesheets;system-administration
navigation-topic: create-and-manage-timesheets
title: 建立、編輯和分配工時單配置檔案
description: 您可以建立、編輯和分配工時單配置檔案，這些工時單為用戶生成循環工時單，無需您進一步干預。 這樣可節省您的時間，並確保用戶(EDIT ME)之間的以下內容一致。
author: Alina
feature: Timesheets
exl-id: 8f4826bd-82b4-4157-a7d4-a7c94b8fc879
source-git-commit: 7e2a4b02277e8b82ac6ee92a7994250fcdebb0b0
workflow-type: tm+mt
source-wordcount: '1509'
ht-degree: 1%

---

# 建立、編輯和分配工時單配置檔案

您可以建立、編輯和分配工時單配置檔案，這些工時單為用戶生成循環工時單，無需您進一步干預。 這樣可節省時間，並確保使用者之間的下列項目一致：

* 時間表時間範圍
* 核准者
* 一般小時類型

有關手動建立工時單的詳細資訊，請參閱 [建立單次使用的工時單](../../timesheets/create-and-manage-timesheets/create-tmshts.md).

## 存取需求

您必須具備下列條件才能執行本文所述步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td> <p>計劃 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>必須具有對工時單的管理訪問權限。 </p> <p>如需詳細資訊，請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref" data-mc-variable-override="">授予用戶對特定區域的管理訪問權限</a>.</p>  <p><b>附註</b>

如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">建立或修改自訂存取層級</a>.</p> </td>
</tr> 
 </tbody> 
</table>

*若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 建立或編輯工時單配置檔案

<!--
<div style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p style="color: #ff1493;">Alina drafted an Important note under this heading because Tracy/WorkEx said this is not working as designed - the changes WILL take effect the minute to make them for existing timesheets - see this issue - https://hub.workfront.com/issue/5dba59f600c401cca536567c368aa299/overview</p>
<p style="color: #ff1493;">Important: The changes you make to an existing timesheet profile are not automatically applied to timesheets that have already been generated. The changes you make to a timesheet prile are applied only to the timesheets that are&nbsp;generated after the timesheet profiles changes are made. To&nbsp;apply your&nbsp;changes to the timesheet profile for the timesheets that are already generated, you must delete the existing timesheets and manually generate&nbsp;them.For more information about deleting and manually generating timesheets, see&nbsp;Delete and manually generating Timesheets.</p>
</div>
-->

>[!IMPORTANT]
>
>要在當前工時表中啟用工時單配置檔案更改，必須刪除現有工時單，然後生成新工時單。 如需指示，請參閱 [刪除Adobe Workfront中的工時單](../../timesheets/create-and-manage-timesheets/delete-timesheets.md) 和 [手動生成工時單](../../timesheets/create-and-manage-timesheets/manually-generate-timesheets.md).

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **設定** ![](assets/gear-icon-settings.png).

1. 如果要建立或編輯工時單配置檔案以在整個系統中使用，請按一下 **時間表和小時數**.

   或

   如果建立或編輯組的時間表配置檔案，請按一下 **群組**，然後按一下群組的名稱。

1. 按一下 **時間表配置檔案**.
1. 要建立新的時間表配置檔案，請按一下 **新設定檔**.

   或

   要編輯現有的時間表配置檔案，請選擇要編輯的時間表配置檔案，然後按一下 **編輯**.

   將顯示新的或現有的時間表配置檔案。


1. 在 **設定詳細資訊** 頁簽 **名稱** 和 **說明** 對於時間表配置檔案，並提供以下資訊：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>具有管理存取權的群組</strong> </td> 
      <td> <p> 
      <ul> 
      <li> <p>如果要建立系統級時間表配置檔案，請將此欄位留空。</p> <p>任何可以編輯用戶帳戶的用戶都可以將系統級時間表附加到其他用戶。</p> <p>只有Workfront管理員可以編輯系統級時間表配置檔案。</p> </li> 
      </ul> 
     <ul> 
      <li> <p>如果您正在為您管理的組建立時間表配置檔案，請在此處標識組。</p> <p>這不會將時間表配置檔案分配給組中的用戶；它僅允許組的管理員修改時間表配置檔案。 您會在步驟6中將設定檔指派給使用者。</p> <p><b>附註</b>

   當組外的用戶將時間表配置檔案附加到其他用戶時，他們將無法查看或附加此時間表配置檔案。</p> </li>
   </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>建立時間表</strong> </td> 
      <td> <p> <p>指定時間表配置檔案何時生成時間表。 時間表可設定為每週、每兩週、每半月或每月自動生成。 選擇希望生成工時單的星期幾。</p> <p><b>附註</b>

   如果配置時間表配置檔案以在星期五建立工時單，則用戶無法記錄當周的星期五、星期六和星期日的工時。</p> <p>Workfront一律會建立兩個工時單：第一個時間表始終包括當前日期，第二個時間表在第一個時間表的時間範圍結束時開始。</p> </p> </td>
   </tr> 
     <tr> 
      <td role="rowheader"><p><strong>核准者</strong></p> </td> 
      <td> <p> <p>批准者是批准與時間表關聯的用戶的時間表的用戶。 在時間表中，最多可以將7個用戶標識為批准者。 識別多個使用者對於確保有人外出時，核准者可供使用很有幫助。 當用戶提交工時單進行審批時，將通知所有審批人。 只有一個用戶需要批准時間表，才能批准時間表。</p> <p>只能將具有時間表管理權限的用戶設定為批准者。 有關時間表管理權限的詳細資訊，請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">授予用戶對特定區域的管理訪問權限</a>.</p> <p>使用下拉菜單選擇工時單的批准者（如果需要批准者）。 您可以選取下列選項：</p> 
      <ul> 
      <li><strong>無</strong>:時間表不需要批准。</li> 
      <li><strong>他們的經理</strong>:這是由系統設定的預設核准者。 在這種情況下，指定為其經理的用戶在提交時間表以進行批准時批准該時間表。</li> 
      <li><strong>特定人員：</strong> 您可以按名稱指定特定用戶作為時間表批准者。 時間表上可以有多個批准者。 在這種情況下，在某個批准者批准工時單後，工時單被標籤為 <strong>已關閉</strong> 它會從所有剩餘批准者的時間表批准清單中消失。</li> 
       </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>可編輯時間 </strong> </td> 
      <td> <p> <p>選擇此選項可允許批准者編輯工時單上的工時。

   此選項可與 **將時間表編輯限制給所有者和管理員** 在「設定」>「工時表和小時」>「首選項」區域中進行設定。 如需詳細資訊，請參閱 <a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md">配置工時單和小時首選項</a>.

   存在下列情況：

   <ul>
      <li>當 <b>將時間表編輯限制給所有者和管理員</b> 選項：</li>
      <ul><li>批准者只能批准和拒絕時間表，無論 <b>可編輯時間</b> 是否啟用。 </li>
      <li>工時單所有者的經理只能查看其直接報表的工時單。</li></ul>
      <li>當 <b>將時間表編輯限制給所有者和管理員</b> 選項已停用：</li>
    <ul><li>當 <b>可編輯時間</b> 啟用後，批准者可以提交、重新開啟或關閉時間表，並可以編輯時間。</li>
      <li>當 <b>可編輯時間</b> 禁用時，批准者無法提交、重新開啟或關閉時間表，也無法編輯時間。 批准者只能批准或拒絕工時單。 </li>
      <li>工時單所有者的經理可以提交、重新調用、重新開啟和編輯其直接報告的工時單。</li></ul>
      </ul>

   <p><b>附註</b>

   一旦您提交工時單以進行審批，您就無法再編輯工時。 要將提交的時間表返回到可編輯狀態，請撤回時間表或讓審批人拒絕時間表。 如需詳細資訊，請參閱 <a href="../../timesheets/create-and-manage-timesheets/submit-timesheet-for-approval.md">提交時間表以進行批准</a> 和<a href="../../timesheets/create-and-manage-timesheets/timesheet-approvals.md">批准工時單</a>.</p> </p> </td>
   </tr> 
     <tr> 
      <td role="rowheader"><strong>可用小時類型</strong> </td> 
      <td>預設情況下，用戶將查看時間表上的所有一般小時數。 但是，如果您的組織只想顯示特定一組用戶的特定一般小時數，則可以通過在此欄位的時間表配置檔案中選擇這些小時，來選擇他們在其時間表中需要查看的一般小時數。 如果要禁用所有一般小時數，請取消選擇所有小時數類型以生成不含一般小時數部分的工時單。</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span style="font-weight: bold;">加班</span> </td> 
      <td>您可以選擇在工時單中隱藏「特定時間」(Adverige)框。 預設會停用此選項。</td> 
     </tr> 
    </tbody> 
    </table>

1. 按一下 **指派人員** 頁簽，將工時單配置檔案與特定用戶、組或(如果您是Workfront管理員)團隊關聯。 開始鍵入用戶、組或組的名稱，然後在下拉清單中顯示時按一下它。

   如果您是組管理員，您可以將時間表配置檔案分配給您管理的組，但不能分配給組。 如需詳細資訊，請參閱 [組管理員分配時間表配置檔案的限制](#limitations-for-a-group-administrator-assigning-a-timesheet-profile) 這篇文章。

   >[!NOTE]
   >
   >* 您也可以編輯用戶配置檔案，將用戶與時間表配置檔案關聯。 如需詳細資訊，請參閱 [編輯使用者的設定檔](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).
   >* 新增群組時，「指派人員」索引標籤上只會顯示群組名稱，而不會顯示群組成員清單。 如果要查看此處列出的組成員，請按一下「保存更改」，然後按一下剛建立的時間表配置檔案的名稱。
   >* 完成這些步驟後，工時單配置檔案僅為當前期間沒有現有工時單的已分配用戶或組成員生成工時單。


1. 按一下 **儲存變更**.

   時間表配置檔案第一次生成時間表時，為每個用戶建立2個時間表。 之後，每次它生成新工時單時，都會按用戶建立工時單。

   <!--the content in the table above will need to match the content in the Create timesheets article-->

## 組管理員分配時間表配置檔案的限制 {#limitations-for-a-group-administrator-assigning-a-timesheet-profile}

如果您是組管理員，並且在訪問級別禁用了管理訪問選項時間表和小時，則可以建立時間表配置檔案，但只能將它們分配給：

* 您管理的群組
* 您有權編輯的個別使用者，位於您管理的群組中

對於這些組和用戶，您將無法訪問時間表配置檔案生成的時間表。

此外，如果在訪問級別中禁用了「用戶管理員（組用戶）」選項，則可以將時間表配置檔案分配給您管理的組，但它只影響您有權編輯的組中的用戶。 如果組包含您無權編輯的用戶，則不會將時間表配置檔案連同組的其餘部分一併分配給這些用戶。

有關訪問級別中的時間表和小時選項的資訊，請參閱 [授予用戶對特定區域的管理訪問權限](../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

如需存取層級中「使用者管理員（群組使用者）」選項的相關資訊，請參閱 [授予使用者存取權](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

## 多個循環工時單配置檔案

如果存在以下條件，則組織可以有多個時間表配置檔案：

* 不同用戶集的不重複支付期
* 不同用戶集的唯一批准者
* 不同使用者集的不重複一般小時需求

一個用戶一次不能與多個時間表配置檔案相關聯。 
