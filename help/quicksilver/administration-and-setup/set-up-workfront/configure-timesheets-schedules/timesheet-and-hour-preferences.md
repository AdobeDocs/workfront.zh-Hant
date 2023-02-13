---
user-type: administrator
product-area: system-administration;timesheets
navigation-topic: configure-timesheets-and-schedules
title: 配置工時單和小時首選項
description: 作為 [!DNL Adobe Workfront] 管理員，可以指定工時表和工時的首選項， [!DNL Workfront] 為了定義時間表可以預先填充哪些物料，以及用戶可以登錄哪些物料。
author: Courtney and Alina
feature: System Setup and Administration
role: Admin
exl-id: 8cc49dc2-b23f-4899-85dd-bd53d5242dbe
source-git-commit: 9f7f8a50bb805b1d6845df79ecffaa329d5abc26
workflow-type: tm+mt
source-wordcount: '1309'
ht-degree: 0%

---

# 配置工時單和小時首選項

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

作為 [!DNL Adobe Workfront] 管理員，可以指定工時表和工時的首選項， [!DNL Workfront] 為了定義時間表可以預先填充哪些物料，以及用戶可以登錄哪些物料。

您對工時單所做的任何更改都會影響將來建立的所有工時單。

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計劃</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權</td> 
   <td>[!UICONTROL計畫]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置</td> 
   <td> <p>您必須是 [!DNL Workfront] 管理員。</p> <p><b>附註</b>

如果您仍無法存取，請詢問您的 [!DNL Workfront] 管理員。 若要了解 [!DNL Workfront] 管理員可修改您的存取層級，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td>
</tr> 
 </tbody> 
</table>

## 設定工時單和小時首選項

1. 按一下 **[!UICONTROL 主菜單]** 圖示 ![](assets/main-menu-icon.png) 在 [!DNL Adobe Workfront]，然後按一下 **[!UICONTROL 設定]** ![](assets/gear-icon-settings.png).

1. 按一下 **[!UICONTROL 時間表和小時數]** > **[!UICONTROL 偏好設定]**.

1. 在顯示的頁面上， **[!UICONTROL 一般偏好設定]** ，請配置以下任一選項：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL未來日期的記錄時間]</td> 
      <td> <p>可讓使用者在下列位置記錄系統中未來日期的時間：</p> 
       <ul> 
        <li>他們有權存取記錄時間的任何專案、工作和問題</li> 
        <li>他們的工時單作為一般時間</li> 
       </ul> <p>當用戶計畫離開辦公室並想提前登錄該時間時，此功能非常有用。</p> <p><b>注意</b>:您無法阻止用戶登錄已關閉或已取消的任務或問題。 您只能防止使用者登入已完成或已停用的專案。 建議您在任務和問題清單中使用篩選器，以排除已完成或已取消的任務和問題，使用者無法看到這些任務和問題。</p> </td> 
     </tr>

   <tr> 
      <td role="rowheader">[!UICONTROL手動將作業角色分配給小時條目]</td> 
      <td> <p>允許用戶手動選擇在其用戶配置檔案中分配或分配給對象的任何作業角色。</p> <p><b>重要</b>:  
        <ul> 
         <li>如果在將作業角色分配給小時條目後禁用此設定，則用戶必須調整項目、任務或問題的[!UICONTROL Hours]頁簽上各種角色下記錄的小時數。</li> 
         <li>如果用戶的配置檔案中未分配作業角色，並且在[!UICONTROL高級分配]對話框中有分配為[!UICONTROL任務所有者]的任務，則當用戶記錄該任務的時間時，該作業角色將出現。</li> 
        </ul> </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL將時間表編輯限制給所有者和管理員]</td> 
      <td> <p>限制對時間表所有者和 [!DNL Workfront] 管理員。 禁用此選項時，還可以通過以下方式編輯工時單：</p> 
       <ul> 
        <li> <p>在訪問級別具有對工時單和小時的管理訪問權限的用戶</p> </li> 
        <li> <p>如果工時單上啟用了「可以編輯工時」，則工時單批准者</p> </li> 
        <li> <p>工時單所有者的管理員</p> </li> 
       </ul> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL限制對所有者和管理員進行小時編輯]</td> 
      <td>限制對輸入小時和 [!DNL Workfront] 管理員。 此設定適用於專案或「小時」報表中的「[!UICONTROL小時]」標籤。</td> 
     </tr> 
    </tbody> 
   </table>

1. 在 **[!UICONTROL 記錄時間]** ，請配置以下任一選項：

   <table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL直接記錄項目時間]</td>
        <td>允許用戶登錄項目的時間（在[!UICONTROL更新]頁簽和時間表上）。 如果使用者未在專案層級記錄時間，應保持未勾選此選項。</td>
    </tr>
    <tr>
        <td>登錄已完成的項目</td>
        <td>允許用戶記錄已標籤為完成的項目上的時間。 如果禁用此選項，則用戶無法以[!UICONTROL完成]狀態記錄在項目上完成的工作的時間。</td>
    </tr>
    <tr>
        <td>對已停用的專案登入時間</td>
        <td>啟用此選項時，使用者可以在具有[!UICONTROL無效]狀態的專案上登入數小時。</td>
    </tr>
   </table>

1. 在 **[!UICONTROL 用預填時間表]**&#x200B;部分，配置以下任一選項：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL內工作] &lt;number of="" weeks=""&gt; [！時間表工作範圍的UICONTROL]</td> 
      <td> <p>定義時間表日期範圍前後的周數，該時間表包含分配給用戶的任務和問題日期。 預設設定為1週，您可將此範圍延長至4週。 這表示，如果您為範圍選擇4週，則時間表預先填充任務和問題，這些任務和問題的日期在時間表日期範圍之前四週之間，最多在時間表日期範圍之後四週。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL已完成的任務和問題]</td> 
      <td>如果通常將多個資源指派給單一任務，建議使用此設定。 這意味著，當一個資源根據任務記錄時間並將其標籤為已完成時，分配給任務的其他資源仍可以在其時間表中查找任務或問題，以記錄其小時數。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL任務和在時間表的日期範圍內具有計畫日期的問題]</td> 
      <td> <p>選定後，工時單將包括具有計畫起始日期或完成日期且落在工時單日期範圍內的任務和問題。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> [!UICONTROL任務在時間表的日期範圍內具有預計日期]</td> 
      <td> <p>選定後，時間表包括具有在項目時間範圍內的預計起始日期或完成日期的任務，即使問題或任務的計畫日期超出時間表日期範圍也是如此。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 在 **[!UICONTROL 項目、任務或問題刪除首選項]** 區段，指定下列項目：

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Better title would be Deleting projects, tasks, and issues</p>
   -->

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL刪除項目時]</td> 
      <td> 
       <ul> 
        <li><strong>[!UICONTROL將記錄時間作為一般時間添加到時間表中]</strong>:如果以後還原此項目，則時間將保留在時間表上。</li> 
        <li><strong>[!UICONTROL刪除任何記錄的時間]</strong>:如果此專案稍後還原，則已記錄的時間會還原至專案。</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL刪除任務或問題時]</td> 
      <td> 
       <ul> 
        <li><strong>[!UICONTROL將任何記錄的時間移到任務或問題所在的項目]</strong>:如果稍後還原此任務或問題，則該時間將保留在項目上。<br></li> 
        <li> <p><strong>[!UICONTROL刪除任何記錄的時間]</strong>:如果稍後還原此任務或問題，則記錄的時間將還原到任務或問題。</p> <p>如需這些選項的詳細資訊，請參閱 <a href="../../../administration-and-setup/manage-workfront/manage-deleted-items/configure-how-hours-affected-when-obj-deleted-restored.md" class="MCXref xref">刪除和還原對象時，[!UICONTROL配置將影響]小時</a>.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下&#x200B;**[!UICONTROL 儲存]**。

## 解鎖組的工時單和小時首選項

組織中的組可能需要以不同方式配置時間表或小時首選項，以便其唯一工作流。 您可以解除鎖定組織中所有群組的偏好設定，讓他們能夠自行設定。

當首選項解除鎖定，並且組管理員修改它時，如果組是其主組，則它會影響時間表所有者。

有關組管理員如何配置組的時間表和小時首選項的資訊，請參閱 [配置組的時間表和小時首選項](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-timesheet-hour-preferences-group.md).

>[!NOTE]
>
>之後 [!DNL Workfront] 管理員在系統級別解除對首選項的鎖定，任何組管理員都可以對其進行配置，然後將其鎖定，以確保組中的每個人以及下面的子組都使用相同的配置。 這與 [!DNL Workfront] 管理員必須配置並鎖定系統中每個人的首選項。 如需詳細資訊，請參閱 [鎖定或解除鎖定組時間表和小時首選項](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-timesheet-hour-preference.md).

要解鎖項目首選項，以便組可以進行配置：

1. 按一下 **[!UICONTROL 主菜單]** 圖示 ![](assets/main-menu-icon.png) 在 [!DNL Adobe] Workfront，然後按一下 **[!UICONTROL 設定]** ![](assets/gear-icon-settings.png).

1. 在左側面板中，按一下 **[!UICONTROL 工時單和小時數]**，然後按一下 **[!UICONTROL 偏好設定]**.

1. 執行下列任一操作：

   * 如果希望組管理員能夠為其組配置首選項，請解除鎖定 ![](assets/unlock-toggle-button.png).
   * 如果希望所有組都使用您的配置來獲取首選項，請確保它已鎖定（這是預設值）。

      >[!IMPORTANT]
      >
      >建議您與整個系統中群組的管理員和使用者通訊，以確保以您設定鎖定偏好設定的方式滿足所有需求。 當您鎖定它時，系統中的所有群組都會繼承您的設定。 如果首選項已在任意時間段內解除鎖定，則您的配置將替換組管理員可能所做的配置。

1. 按一下&#x200B;**[!UICONTROL 儲存]**。
