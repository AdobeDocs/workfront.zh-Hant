---
user-type: administrator
product-area: system-administration;timesheets
navigation-topic: configure-timesheets-and-schedules
title: 設定時程表和小時喜好設定
description: 作為 [!DNL Adobe Workfront] 管理員，您可以在 [!DNL Workfront] 中指定時程表和時數的偏好設定，以定義時程表可預先填入的專案以及使用者可記錄時間的專案。
author: Alina and Lisa
feature: System Setup and Administration
role: Admin
exl-id: 8cc49dc2-b23f-4899-85dd-bd53d5242dbe
source-git-commit: 612243e928c6053d9b02715d9fcfef4dae25cb7a
workflow-type: tm+mt
source-wordcount: '1433'
ht-degree: 0%

---

# 設定時程表和時數偏好設定

<!--Audited: 01/2024-->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

作為[!DNL Adobe Workfront]管理員，您可以在[!DNL Workfront]中指定時程表和時數的偏好設定，以定義時程表可預先填入的專案以及使用者可記錄時間的專案。

>[!IMPORTANT]
>
>除了根據本文所述的條件預先填入時程表的專案之外，預設情況下時程表上也會顯示以下專案：
>
>* 您在時程表的時間範圍內記錄時間的專案
>* 釘選到時程表的專案
>* 您搜尋並手動新增至時程表的專案。 預設會釘選手動新增的專案。
>
>如需詳細資訊，請參閱[記錄時間](../../../timesheets/create-and-manage-timesheets/log-time.md)和[時程表總覽](/help/quicksilver/timesheets/timesheets/timesheets-overview.md)。

您對時程表所做的任何變更都會影響未來建立的所有時程表。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

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
   <td><p>目前：[！UICONTROL計畫]</p>
   或
   <p>新增：標準</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td>[！UICONTROL系統管理員]</td>
</tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 設定時程表和小時偏好設定

{{step-1-to-setup}}

1. 按一下&#x200B;**[!UICONTROL 時程表和時數]** > **[!UICONTROL 偏好設定]**。

   時程表和時數偏好設定頁面隨即顯示。

1. （選擇性）在&#x200B;**系統時程表和時數偏好設定**&#x200B;搜尋方塊中，開始輸入群組的名稱，然後在其顯示在清單中時選取它。

   ![搜尋群組方塊](assets/search-for-group-box-in-timesheets-preferences-page.png)

   「時程表和小時偏好設定」頁面會以您所選群組的偏好設定來更新。 系統層級的偏好設定必須解除鎖定，才能修改群組層級的偏好設定。 如需詳細資訊，請參閱本文章的[解除鎖定群組](#unlock-timesheet-and-hour-preferences-for-groups)的時程表和小時偏好設定。

1. 在&#x200B;**[!UICONTROL 一般偏好設定]**&#x200B;區段中，設定下列任一選項：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[！UICONTROL記錄未來日期的時間]</td> 
      <td> <p>可讓使用者在整個系統記錄未來日期的時間，位置如下：</p> 
       <ul> 
        <li>他們有權記錄時間的任何專案、任務和問題</li> 
        <li>他們的時程表作為一般時間</li> 
       </ul> <p>當使用者計畫離開辦公室並想要預先記錄該時間時，此功能會很有用。</p> <p><b>附註</b>：</p> 
       <p>您無法防止使用者記錄已關閉或已取消的任務或問題的時間。 您只能防止使用者記錄完成或廢棄專案的時間。 建議您在任務和問題清單中使用篩選器，以排除已完成或取消的對使用者可見的任務和問題。</p> </td> 
     </tr>

   <tr> 
      <td role="rowheader">[！UICONTROL手動將工作角色指派給時數專案]</td> 
      <td> <p>允許使用者手動選取在其使用者設定檔中指派或指派給物件的任何工作角色。</p> <p><b>重要</b>：  
        <ul> 
         <li>如果您在將工作角色指派給時數專案後停用此設定，使用者必須調整在專案、任務或問題的[！UICONTROL時數]索引標籤上各種角色底下記錄的時數。</li> 
         <li>如果使用者未在其設定檔中指派工作角色，且在[！UICONTROL進階指派]對話方塊中有指派為[！UICONTROL任務擁有者]的任務，則當使用者將時間記錄在任務時，會顯示該工作角色。</li> 
        </ul> </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[！UICONTROL限制所有者和管理員只能編輯時程表]</td> 
      <td> <p>限制僅編輯時程表所有者和[!DNL Workfront]管理員。 停用此選項時，也可以由以下人員編輯時程表：</p> 
       <ul> 
        <li> <p>具有時程表管理存取許可權的使用者及其存取層級的時數</p> </li> 
        <li> <p>時程表核准者（如果時程表上啟用了「可編輯時數」）</p> </li> 
        <li> <p>時程表所有者的經理</p> </li> 
       </ul> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[！UICONTROL限制所有者和管理員只能編輯小時]</td> 
      <td>限制僅編輯輸入時數的使用者和[!DNL Workfront]管理員。 此設定適用於專案或時數報表中的[！UICONTROL時數]索引標籤。</td> 
     </tr> 
    </tbody> 
   </table>

1. 在&#x200B;**[!UICONTROL 使用者可記錄時間]**&#x200B;區段中，設定下列任一選項：

   <table style="table-layout:auto">
    <tr>
        <td>[！UICONTROL直接在專案上]</td>
        <td>允許使用者在專案上記錄時間（同時在[！UICONTROL更新]索引標籤和時程表上）。 如果使用者未在專案層級記錄時間，此選項應保持未勾選狀態。</td>
    </tr>
    <tr>
        <td>[！UICONTROL在完成的專案上]</td>
        <td>允許使用者記錄已標示為完成的專案時間。 如果停用此選項，使用者將無法在[！UICONTROL完成]狀態的專案上記錄已完成工作的時間。</td>
    </tr>
    <tr>
        <td>[！UICONTROL在廢棄的專案上]</td>
        <td>當啟用此選項時，使用者可以在具有[！UICONTROL無法使用]狀態的專案上記錄時數。</td>
    </tr>
   </table>

1. 在&#x200B;**[!UICONTROL 預先填入時程表]**&#x200B;區段中，設定下列任一選項：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[！UICONTROL在時程表工作範圍之內] &lt;周數&gt; [！UICONTROL]的工作</td> 
      <td> <p>定義包含指派給使用者的任務和問題日期的時程表日期範圍之前和之後的周數。</p> 
      <p>預設值為1週，您可以將此範圍延長至4週。</p> 
      <p>也就是說，如果您為範圍選取4週，則時程表已預先填入日期在時程表日期範圍前4週至時程表日期範圍後4週之間的任何時間任務和問題。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL已完成的任務和問題]</td> 
      <td>如果通常將多個資源指派給單一任務，建議您進行此設定。 這表示當一個資源針對任務記錄時間並標籤為完成時，指派給任務的其他資源仍然可以在其時程表中找到任務或問題以記錄其時數。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL計畫日期在時間表日期範圍內的任務和問題]</td> 
      <td> <p>選取時，時程表包含其計劃開始日期或完成日期介於時程表日期範圍內的任務和問題。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> [！UICONTROL計畫日期在時程表日期範圍內的任務]</td> 
      <td> <p>選取時，時程表包含具有專案時間範圍內的預計開始日期或完成日期的任務，即使問題或任務的計畫日期不在時程表日期範圍內。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 在&#x200B;**[!UICONTROL 已刪除的專案、任務和問題]**&#x200B;區段中，指定下列專案：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> 刪除專案時</td> 
      <td> 
       <ul> 
        <li><strong>[！UICONTROL保留記錄時間已新增至時程表作為一般時間]</strong>：如果稍後還原此專案，時間仍會保留在時程表中。</li> 
        <li><strong>[！UICONTROL刪除任何記錄時間]</strong>：如果稍後還原此專案，則已記錄的時間會還原至專案。</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">刪除任務或問題時</td> 
      <td> 
       <ul> 
        <li><strong>[！UICONTROL將任何記錄時間移至任務或問題所在的專案]</strong>：若日後還原此任務或問題，則時間仍會保留在專案上。<br></li> 
        <li> <p><strong>[！UICONTROL刪除任何記錄時間]</strong>：如果稍後還原此任務或問題，則記錄時間會還原至任務或問題。</p> <p>如需這些選項的詳細資訊，請參閱刪除和還原物件時數的<a href="../../../administration-and-setup/manage-workfront/manage-deleted-items/configure-how-hours-affected-when-obj-deleted-restored.md" class="MCXref xref">[！UICONTROL設定影響]</a>。</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下「**[!UICONTROL 儲存]**」。

## 解鎖群組的時程表和小時偏好設定

您組織中的群組可能需要針對其獨特工作流程以不同方式設定的時程表或小時偏好設定。 您可以解鎖整個組織內所有群組的偏好設定，方便群組成員自行設定。

當偏好設定已解除鎖定且群組管理員修改時，如果群組是時間表所有者的主群組，則會影響時間表所有者。

如需有關群組管理員如何為群組設定時程表和小時偏好設定的資訊，請參閱[為群組設定時程表和小時偏好設定](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-timesheet-hour-preferences-group.md)。

>[!NOTE]
>
>在[!DNL Workfront]管理員在系統層級解除鎖定偏好設定後，任何群組管理員都可以對其進行設定，然後將其鎖定，以確保其群組中的所有人和下面的子群組都使用相同的設定。 此功能與[!DNL Workfront]管理員必須設定並鎖定系統中每個人的偏好設定功能平行。 如需詳細資訊，請參閱[鎖定或解除鎖定群組時程表和小時喜好設定](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-timesheet-hour-preference.md)。

若要解鎖專案偏好設定讓群組可以加以設定：

{{step-1-to-setup}}

1. 在左側面板中，按一下&#x200B;**[!UICONTROL 時程表和時數]**，然後按一下&#x200B;**[!UICONTROL 偏好設定]**。

1. 執行下列任一項作業：

   * 如果您希望群組管理員能夠設定其群組的偏好設定，請按一下&#x200B;**解除鎖定**&#x200B;切換![解除鎖定切換](assets/unlock-toggle-button.png)以解除鎖定。
   * 如果您希望所有群組都使用您的偏好設定設定，請確定切換已鎖定![鎖定的偏好設定切換](assets/locked-preference-toggle.png) （此為預設值）。

     >[!IMPORTANT]
     >
     >我們建議您與整個系統群組內的管理員和使用者溝通，以確保以您設定鎖定偏好設定的方式考慮所有需求。
     >
     >當您鎖定時，系統中的所有群組都會繼承您的設定。 如果偏好設定已解除鎖定任何時間段，您的設定會取代群組管理員可能已進行的設定。

1. 按一下「**[!UICONTROL 儲存]**」。
