---
title: 建立和修改自訂存取層級
user-type: administrator
product-area: system-administration;user-management
navigation-topic: configure-access-to-workfront
description: 身為Adobe Workfront管理員，您可以建立自訂存取層級並套用至使用者。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: d2a73d24-51d3-42e2-9c09-7f4bc30b2caa
source-git-commit: 674c46b699ba445abba06bec3e4da4a710c60d63
workflow-type: tm+mt
source-wordcount: '1521'
ht-degree: 6%

---

# 建立和修改自訂存取層級

<!--Audited: 12/2023-->

<!--Don't delete, draft, or change the title of this article. The UI links to it via context-sensitive help. -->

身為Adobe Workfront管理員，您可以建立自訂存取層級並套用至使用者。 當您使用存取層級時，請務必瞭解它們如何與使用者在共用物件時授與的物件許可權搭配使用。 如需存取層級的詳細資訊，請參閱：

* [新存取層級概觀](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md)
* [存取層級概觀](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md)

>[!IMPORTANT]
>
>我們強烈建議您維持內建的存取層級不變，以便在設定使用者後參考。 若要自訂存取層級，請複製預設存取層級並修改副本。 您可以對每個存取層級（系統管理員和外部使用者除外）執行此操作。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td>新增：標準
   <p>或</p>
   <p>目前：計畫</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>您必須是Workfront管理員。</p></td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 建立或編輯自訂存取層級

{{step-1-to-setup}}

1. 按一下左側面板中的&#x200B;**存取層級**。
1. 
   * 在生產環境中：
選取您要複製及自訂的存取層級，然後按一下[複製]。****

     或

     如果您正在編輯現有的存取層級（您先前複製過的），請按一下其名稱。

   * <span class="preview">在預覽環境中：</span>

     <span class="preview">選取您要複製與自訂的存取層級，然後按一下&#x200B;**複製**&#x200B;圖示![復製圖示](assets/copy-icon.png)。</span>

     <span class="preview">或</span>

     <span class="preview">如果您正在編輯現有的存取層級，請按一下該存取層級左側的方塊來選取存取層級，然後按一下&#x200B;**編輯**&#x200B;圖示![編輯圖示](assets/edit-icon.png)。</span>

1. 在顯示的方塊中，執行下列任一項作業以開始設定自訂存取層級：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">姓名</td> 
      <td> <p>輸入存取層級的名稱。 </p> <p>如果您剛複製存取層級來建立新存取層級，預設名稱為存取層級名稱（複製），其中存取層級名稱是您複製的存取層級。</p> <p><strong>提示</strong>：建議您在副本名稱中加入存取層級的原始名稱。 例如，在ACME公司，「標準」存取層級的復本可能命名為ACME Standard。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">說明 </td> 
      <td>輸入存取層級的說明。 在這裡列出具有此存取層級的使用者將能夠存取哪些內容會很有幫助。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">授權類型</td> 
      <td>請確定此處選取的授權與您建立或編輯的存取層級型別最相關。 選取的授權決定存取層級可用的設定。 如需詳細資訊，請參閱<a href="/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/licenses-overview.md" class="MCXref xref">新授權概述</a>或<a href="/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md">授權概述</a>。</td> 
     </tr> 
    </tbody> 
   </table>

1. （視條件而定）如果在&#x200B;**授權型別**&#x200B;方塊中選取&#x200B;**標準**&#x200B;或&#x200B;**計畫**，請捲動至&#x200B;**允許**&#x200B;的系統管理存取許可權區段，並為擁有此存取層級的使用者選取系統管理存取許可權。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">核准程序</td> 
      <td>建立並管理整個系統和特定群組的核准流程。<p>若無此存取權，使用者只能對其有權管理的專案建立臨時核准流程。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">公司</td> 
      <td>在Workfront中新增及編輯現有公司。<br><p>若無此存取權，使用者只能檢視現有公司。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">自訂表單</td> 
      <td>建立並管理群組中的所有自訂表單。 <br><p>若無此存取權，使用者只能將現有表單附加至他們有權貢獻或管理的物件。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">匯率</td> 
      <td> 在Workfront中新增貨幣。 <p>如果沒有此存取權，使用者只能將現有貨幣新增到他們建立的專案。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">費用</td> 
      <td>檢視Workfront中物件的所有費用。<p>若無此存取權，使用者只能檢視下列專案：</p>
       <ul>
        <li>專案、任務或問題管理的費用</li>
        <li>他們自己的費用</li>
        <li>其下屬的費用</li>
       </ul><p><b>注意</b>：不允許使用者建立新的費用型別。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">職務角色</td> 
      <td> 透過此存取權，使用者可以執行下列動作： 
       <ul> 
        <li>檢視和編輯現有職位角色</li> 
        <li>新增職位角色</li> 
        <li>編輯角色帳單和成本費率</li> 
       </ul> 
       <p>有關對工作角色具有管理存取許可權的「標準」或「規劃」使用者可存取之財務資料的重要資訊，請參閱<a href="#standard-or-planner-users-with-administrative-access-to-job-roles">對工作角色具有管理存取許可權的「標準」或「規劃」使用者</a>。</p>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">我的群組中的里程碑</td> 
      <td>在「設定」的「里程碑路徑」選單下，檢視系統中的所有里程碑路徑。 使用者也可以編輯或刪除屬於任何群組的所有里程碑路徑。 使用者無法管理（編輯或刪除）未指派給其群組的里程碑路徑。<p>若無此存取權，使用者只能檢視現有的里程碑路徑，並將其套用至他們有權管理的專案。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">提醒通知</td> 
      <td>在Workfront中建立和管理提醒通知。<p>若無此存取權，使用者受限於接收及檢視通知。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">時間表和時數</td> 
      <td> 群組管理員可以將時間表設定檔指派給其管理的群組和子群組中的使用者。 <p>如果未啟用此選項，群組管理員無法將時程表設定檔指派給其管理的群組和子群組中的其他使用者，儘管他們可以建立這些設定檔。</p> <p>所有其他使用者擁有Standard或Plan授權，即可在Workfront中檢視所有時數與時間表。</p> <p>若未啟用此選項，使用者只能在下列位置檢視時數：</p> 
       <ul> 
        <li>他們管理的專案、任務或問題</li> 
        <li>他們自己的時間表</li> 
        <li>他人所報之時程表</li> 
        <li>他們核准的時程表</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下&#x200B;**設定其他限制**，然後為存取層級設定下列任何限制。

   >[!IMPORTANT]
   >
   >對於廠商（不在您組織中的任何人）等外部使用者，建議您限制對任務、專案、更新、公告、其他公司、團隊和群組的存取權。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">當專案已指派至任務或問題時，不要將存取權授予整個專案</td> 
      <td> 防止指派給任務或問題的使用者也獲得上層專案的許可權，即使專案許可權允許這樣做。<p>如需有關設定專案許可權的詳細資訊，請參閱文章<a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">編輯專案</a>中的<a href="../../../manage-work/projects/manage-projects/edit-projects.md#access" class="MCXref xref"></a>小節。</p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">不要從專案、任務、問題等繼承文件存取權...</td> 
      <td>防止檔案繼承在其父物件上設定的許可權。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">僅檢視已加入交談的更新</td> 
      <td> 讓使用者只能看見包含其名稱或團隊名稱的註解。 <p> <p><b>注意</b>：這可防止使用者訂閱Workfront中的專案。 如需訂閱專案的詳細資訊，請參閱<a href="../../../workfront-basics/using-notifications/subscribe-to-items-in-workfront.md" class="MCXref xref">在Adobe Workfront中訂閱專案</a>。</p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">永不允許使用者刪除註解 </td> 
      <td> 防止使用者刪除對專案所做的註解。  <p><b>附註</b>：沒有人可以刪除其他使用者的註解。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">僅檢視他們所屬的公司、群組和小組</td> 
      <td>僅允許使用者檢視專案並與他們所屬的公司、群組和團隊共用。<p><strong>注意</strong>：擁有請求者或貢獻者授權的使用者無法檢視他們不屬於的公司，即使選取此選項亦然。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">絕對禁止顯示規劃時數或實際時數</td> 
      <td>防止使用者看見他們有權存取之工作專案的計畫和實際時數。 但是，他們可以檢視自己記錄的實際時數，或向他們報告的人員所記錄的時數。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">永不允許使用者刪除宣告</td> 
      <td>防止使用者刪除公告中心中的公告。 如需詳細資訊，請參閱<a href="../../../administration-and-setup/get-started-wf-administration/view-send-announcements.md" class="MCXref xref">傳送宣告</a>。</td> 
     </tr> 
    </tbody> 
   </table>

1. （條件式與選擇性）如果您的Workfront系統設定給屬於多個公司的使用者，請根據其他使用者在&#x200B;**區段中屬於哪個公司來限制其他使用者的可見度。其他公司的人員應該僅檢視來自**&#x200B;的使用者。

   您可以限制使用者，使其只能看見自己公司或您指定為主要公司之公司的使用者。 主要公司通常代表您大部分使用者工作所在的Workfront帳戶。 如需主要公司的詳細資訊，請參閱[建立和編輯公司](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md)。

   >[!NOTE]
   >
   >如果兩個使用者屬於兩個不同的公司，但他們都可以看到來自主要公司的使用者，則他們可以看到與主要公司相關聯的「更新」區域。

1. （選擇性）若要針對您正在處理的存取層級中的其他物件與區域設定存取設定，請繼續使用[設定對Adobe Workfront的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md)中所列的文章之一，例如[授與對工作的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md)和[授與對財務資料的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)。
1. 按一下「**儲存**」。

   建立存取層級後，您可以將其指派給使用者（除非它是系統管理員存取層級）。

   如需詳細資訊，請參閱[編輯使用者的設定檔](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)。

   如需Adobe管理員如何指派系統管理員存取層級給使用者的詳細資訊，請參閱[授予使用者完整管理存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md)。

## 對職位角色具有管理存取權的標準或規劃工具使用者 {#planner-users}

如果您授予「標準」或「規劃工具」使用者對工作角色的管理存取權，「編輯角色帳單與成本費率」設定會自動為該使用者啟用。

稍後，如果您停用使用者對工作角色的管理存取權，則使用者仍可看見工作角色，因為編輯角色帳單與成本費率設定仍處於啟用狀態。

如果發生此情況，並且您需要移除使用者檢視工作角色的存取權，您需要停用使用者的「編輯角色帳單和成本費率」許可權設定。 如需指示，請參閱[授予財務資料的存取權](grant-access-financial.md)。



