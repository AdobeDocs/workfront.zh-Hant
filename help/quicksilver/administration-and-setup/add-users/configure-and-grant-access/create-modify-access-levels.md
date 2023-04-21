---
title: 建立或修改自訂存取層級
user-type: administrator
product-area: system-administration;user-management
navigation-topic: configure-access-to-workfront
description: 身為Adobe Workfront管理員，您可以建立自訂存取層級並將其套用至使用者。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: d2a73d24-51d3-42e2-9c09-7f4bc30b2caa
source-git-commit: 62d1b9563d83bd82b569e143f69e379e2f4ffbc2
workflow-type: tm+mt
source-wordcount: '1402'
ht-degree: 6%

---

# 建立和修改自定義訪問級別

<!--Don't delete, draft, or change the title of this article. The UI links to it via context-sensitive help.-->

身為Adobe Workfront管理員，您可以建立自訂存取層級並將其套用至使用者。 在使用訪問級別時，必須了解它們如何與用戶在彼此共用對象時授予的對象權限一起工作。 有關訪問級別的詳細資訊，請參閱

* [新訪問級別概述](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md)
* [存取層級概觀](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

>[!IMPORTANT]
>
>強烈建議您將內建存取層級維持不變，以便在設定使用者後參照這些層級。 要自定義訪問級別，請複製預設訪問級別並修改副本。 除「系統管理員」和「外部用戶」外，您可以對每個訪問級別執行此操作。

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

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
   <td>當前計畫：標準
   <p>或</p>
   <p>舊計畫：計畫</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置</td> 
   <td> <p>您必須是Workfront管理員。</p></td> 
  </tr> 
 </tbody> 
</table>

## 建立或編輯自訂存取層級

{{step-1-to-setup}}

1. 按一下 **存取層級** 中。
1. 選擇要複製和自定義的訪問級別，然後按一下 **複製**.

   或

   如果您正在編輯現有的訪問級別（您以前複製的），請按一下其名稱。

1. 在顯示的方塊中，執行下列任一操作以開始設定自訂存取層級：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">名稱</td> 
      <td> <p>鍵入訪問級別的名稱。 </p> <p>如果您剛剛複製了訪問級別以建立新訪問級別，則預設名稱為訪問級別名稱（副本），其中訪問級別名稱是您複製的訪問級別。</p> <p><strong>筆尖</strong>:建議您將存取層級的原始名稱包含在復本的名稱中。 例如，在ACME公司，標準存取層級的副本可命名為ACME Standard。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">說明 </td> 
      <td>鍵入訪問級別的說明。 在此處列出具有此存取層級的使用者將可存取哪些內容，將有所幫助。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">授權類型</td> 
      <td>請確保此處選擇的許可證與您正在建立或編輯的訪問級別類型最密切相關。 所選許可證決定了哪些設定可用於訪問級別。 如需詳細資訊，請參閱 <a href="/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/licenses-overview.md" class="MCXref xref">新許可證概述</a> 或 <a href="/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md">授權概觀</a>.</td> 
     </tr> 
    </tbody> 
   </table>

1. （條件性）若 **標準** 或 **計畫** 在 **許可證類型** 框，滾動到「 」部分 **允許的管理存取** 並為具有此訪問級別的用戶選擇管理訪問權限。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">核准程序</td> 
      <td>建立並管理要在整個系統和特定群組使用的核准程式。<p>若沒有此存取權，使用者只能針對有權管理的項目建立臨機核准程式。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">公司</td> 
      <td>在Workfront中新增及編輯現有公司。<br><p>若無此存取權，使用者只能檢視現有公司。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">自訂表單</td> 
      <td>建立並管理其群組中的所有自訂表單。 <br><p>若沒有此存取權，使用者只能將現有表單附加至其可存取的contribute或管理物件。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">匯率</td> 
      <td> <p>在Workfront中新增貨幣。</p> <p>若沒有此存取權，使用者只能將現有貨幣新增至其建立的專案。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">費用</td> 
      <td>查看Workfront中對象的所有費用。<p>若沒有此存取權，使用者只能檢視下列項目：</p>
       <ul>
        <li>他們管理的項目、任務或問題的費用</li>
        <li>自費</li>
        <li>下屬的費用</li>
       </ul><p><b>注意</b>:這不允許用戶建立新的費用類型。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">工作角色</td> 
      <td> <p>透過此存取權，使用者可執行下列作業：</p> 
       <ul> 
        <li>查看和編輯現有作業角色</li> 
        <li>添加新作業角色</li> 
        <li>編輯職責開單和成本費率</li> 
       </ul> 
       <p>有關對具有任務角色管理訪問權限的標準或計畫員用戶可用的財務資料的訪問權限的重要資訊，請參閱 <a href="#planner-users-with-administrative-access-to-job-roles">具有任務角色管理訪問權限的標準或計畫員用戶</a>.</p>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">我的群組中的里程碑</td> 
      <td>在「設定」的「里程碑路徑」菜單下查看系統中的所有里程碑路徑。 使用者也可以編輯或刪除屬於其任何群組的任何里程碑路徑。 使用者無法管理（編輯或刪除）未指派給其群組的里程碑路徑。<p>若沒有此存取權，使用者只能檢視現有的里程碑路徑，並將其套用至其可管理存取權的專案。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">提醒通知</td> 
      <td>在Workfront中建立和管理提醒通知。<p>若無此存取權，使用者只能接收和檢視通知。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">時間表和時數</td> 
      <td> <p>組管理員可以將時間表配置檔案分配給他們管理的組和子組中的用戶。</p> <p>如果未啟用此選項，則組管理員無法將時間表配置檔案分配給他們管理的組和子組中的其他用戶，儘管他們可以建立這些用戶。</p> <p>具有標準或計畫許可證的所有其他用戶都可以查看Workfront中的所有小時和工時單。</p> <p>若未啟用此選項，使用者只能在下列位置檢視小時：</p> 
       <ul> 
        <li>他們管理的專案、工作或問題</li> 
        <li>他們自己的時間表</li> 
        <li>向其報告的人的時間表</li> 
        <li>他們批准的時間表</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下 **設定其他限制**，然後為存取層級設定下列任一限制。

   >[!IMPORTANT]
   >
   >對於廠商（您組織內的任何人）等外部使用者，建議您限制對工作、專案、更新、公告、其他公司、團隊和群組的存取權。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">當專案已指派至任務或問題時，不要將存取權授予整個專案</td> 
      <td> 防止指派給任務或問題的使用者也獲得上層專案的權限，即使專案權限允許亦然。<p>如需有關設定專案權限的詳細資訊，請參閱區段 <a href="../../../manage-work/projects/manage-projects/edit-projects.md#access" class="MCXref xref"></a> 在文章中 <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">編輯專案</a>.</p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">不要從專案、任務、問題等繼承文件存取權...</td> 
      <td>阻止文檔繼承其父對象上設定的權限。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">僅檢視已加入交談的更新</td> 
      <td> <p>允許用戶只查看已包括其名稱或團隊名稱的注釋。</p> <p> <p><b>注意</b>:這會防止使用者訂閱Workfront中的項目。 如需訂閱項目的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/create-and-manage-users/add-users.md" class="MCXref xref">新增使用者</a>.</p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">永不允許使用者刪除註解 </td> 
      <td> <p>防止使用者刪除對項目所做的註解。 </p> <p><b>注意</b>:沒有人可以刪除其他用戶的注釋。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">僅檢視他們所屬的公司、群組和小組</td> 
      <td>只允許使用者檢視項目，並與其所屬的公司、群組和團隊共用。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">絕對禁止顯示規劃時數或實際時數</td> 
      <td>阻止用戶查看他們有權訪問的工作項目的「計畫」和「實際小時」。 但是，他們可以看到自己記錄的實際小時數，或由向他們報告的人記錄的小時數。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">永不允許使用者刪除宣告</td> 
      <td>阻止用戶刪除公告中心中的公告。 如需詳細資訊，請參閱 <a href="../../../administration-and-setup/get-started-wf-administration/view-send-announcements.md" class="MCXref xref">傳送公告</a>.</td> 
     </tr> 
    </tbody> 
   </table>

1. （條件式和選用式）如果您的Workfront系統是為屬於多個公司的使用者所設定，請根據其在區段中所屬的公司，將可見度限制給其他使用者 **其他公司的使用者只應從**.

   您可以限制使用者只能看見來自其公司或您指定為主要公司之公司的使用者。 如需主要公司的詳細資訊，請參閱 [建立和編輯公司](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

   >[!NOTE]
   >
   >如果兩個使用者分屬兩個不同的公司，但兩者都可以看見主要公司的使用者，則可以看見與主要公司相關聯的更新區域。

1. （可選）要配置您正在處理的訪問級別中其他對象和區域的訪問設定，請繼續以下文章之一列出： [設定Adobe Workfront的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md)，例如 [授予任務的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) 和 [授予金融資料的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. 按一下&#x200B;**儲存**。

   建立訪問級別後，您可以將其分配給用戶（除非該級別是系統管理員訪問級別）。

   如需詳細資訊，請參閱 [編輯使用者的設定檔](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

   有關Adobe管理員如何向用戶分配系統管理員訪問級別的資訊，請參見 [授予使用者完整的管理存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md).

## 具有任務角色管理訪問權限的標準或計畫員用戶 {#planner-users}

如果您授予標準或計畫員用戶對任務職責的管理訪問權限，則系統會自動為用戶啟用「編輯職責開單和成本費率」設定。

之後，如果禁用用戶對作業角色的管理訪問，則用戶仍可看到作業角色，因為「編輯角色開單和成本費率」設定仍處於啟用狀態。

如果發生此情況，並且您需要刪除用戶的查看任務角色的訪問權限，則需要禁用用戶的「編輯角色開單和成本費率」權限設定。 如需指示，請參閱 [授予金融資料的存取權](grant-access-financial.md).
