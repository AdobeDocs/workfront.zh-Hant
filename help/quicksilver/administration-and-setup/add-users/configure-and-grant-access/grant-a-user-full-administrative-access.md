---
title: 授予使用者完整管理存取權
description: 您可以授予使用者Workfront的完整管理存取權。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 46bcb65a-1cb7-443b-88ba-6d0e516e3050
source-git-commit: eb68357ed4fd8f323707aa4a54a0f946253bf4e0
workflow-type: tm+mt
source-wordcount: '1550'
ht-degree: 4%

---

# 授予使用者完整管理存取權

<!--Audited: 12/2024-->

>[!IMPORTANT]
>
>此頁面中說明的程式僅適用於尚未加入Admin Console的組織。 如果您的組織已加入Adobe Admin Console，您必須透過Adobe Admin Console執行此動作。
>
>如需在Adobe Admin Console中授與完整管理員存取權的指示，請參閱[在Adobe Admin Console中管理使用者](../../../administration-and-setup/add-users/create-and-manage-users/admin-console.md)。
>
>如需根據貴組織是否已加入Adobe Admin Console而有所差異的程式清單，請參閱[以平台為基礎的管理差異(Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md)。

作為Adobe Workfront管理員，您可以指派系統管理員存取層級來建立另一個Workfront管理員。 具有此存取層級的使用者對Workfront中的所有專案具有完整管理存取權，包括他們自己未建立的專案。

>[!NOTE]
>
>這不同於使用存取層級來授與使用者對系統特定區域的管理存取權。 如需詳細資訊，請參閱下列內容：
>
>* [授與使用者對特定區域的管理存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md)
>* [Workfront管理員的存取權與具有系統管理許可權之Plan使用者的存取權](#access-of-a-workfront-administrator-vs-access-of-a-plan-user-with-administrative-rights)的比較（在本文中）
>

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
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>新增：標準</p>
   <p>目前：計畫</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>您必須是Workfront管理員。 </td> 
  </tr> 
 </tbody> 
</table>

*如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。
+++

## 授予單一使用者完整的系統管理員存取權

{{step-1-to-users}}

1. 按一下您要授予管理員許可權的使用者名稱。
1. 按一下使用者名稱右側的&#x200B;**更多**&#x200B;功能表![](assets/more-icon.png)，然後按一下&#x200B;**編輯**。

   **編輯人員**&#x200B;方塊隨即顯示。
1. 按一下左側面板中的&#x200B;**存取**。
1. 在&#x200B;**存取層級**&#x200B;下拉式清單中，選取&#x200B;**系統管理員**&#x200B;存取層級。

   根據系統中進行的變更，此存取層級的名稱可能已變更。

1. 按一下&#x200B;**儲存變更。**

   使用者現在在系統中具有完整的系統管理員許可權。

## Workfront管理員的存取權與具有管理許可權的計畫使用者的存取權  {#access-of-a-workfront-administrator-vs-access-of-a-plan-user-with-administrative-rights}

以下兩個表格顯示具有Workfront系統管理員存取層級的使用者存取許可權，與具有某些管理許可權之「計畫」授權的使用者存取許可權之間的差異。

Workfront管理員可以檢視系統中的所有物件（不論物件的建立者為何）、建立新物件，以及修改或刪除現有物件。 使用者擁有系統中所有物件的完整存取權。

擁有Plan授權且可以在一個區域中編輯功能的使用者，可以完整存取該區域中的功能。

>[!NOTE]
>
>擁有計畫授權且被指定為群組管理員的使用者可以執行一些允許Workfront管理員執行的動作。 他們只能為其管理的群組、其子群組以及這些群組和子群組中的使用者執行這些動作。 如需詳細資訊，請參閱[群組管理員](../../../administration-and-setup/manage-groups/group-roles/group-administrators.md)。

* [存取設定區域](#access-to-the-setup-area)
* [存取物件](#access-to-objects)

### 存取設定區域 {#access-to-the-setup-area}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>區域/物件</th> 
   <th>Workfront管理員 </th> 
   <th>擁有Plan授權和某些管理許可權的使用者</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>專案偏好設定：專案</td> 
   <td>完整存取權</td> 
   <td>無存取權</td> 
  </tr> 
  <tr> 
   <td>專案偏好設定：任務和問題</td> 
   <td>完整存取權</td> 
   <td>無存取權</td> 
  </tr> 
  <tr> 
   <td>專案偏好設定：狀態</td> 
   <td>完整存取權</td> 
   <td> <p>無存取權</p> </td> 
  </tr> 
  <tr> 
   <td>專案偏好設定：優先順序</td> 
   <td>完整存取權</td> 
   <td>無存取權</td> 
  </tr> 
  <tr> 
   <td>專案偏好設定：嚴重程度</td> 
   <td>完整存取權</td> 
   <td>無存取權</td> 
  </tr> 
  <tr> 
   <td>專案偏好設定：匯率</td> 
   <td>完整存取權</td> 
   <td>完整存取權</td> 
  </tr> 
  <tr> 
   <td>處理：核准</td> 
   <td> <p>完整存取權</p> </td> 
   <td>完整存取權</td> 
  </tr> 
  <tr> 
   <td>程式：里程碑路徑</td> 
   <td>完整存取權</td> 
   <td>完整存取權</td> 
  </tr> 
  <tr> 
   <td>自訂表單</td> 
   <td>完整存取權</td> 
   <td> <p>管理他們建立的自訂表單或與他們共用的自訂表單。</p> <p>將他們建立的自訂表單或與他們共用的自訂表單附加至他們擁有管理或貢獻許可權的物件。</p> </td> 
  </tr> 
  <tr> 
   <td>資源回收筒：最近刪除</td> 
   <td>完整存取權</td> 
   <td> <p>身為群組管理員的使用者可還原指派給其管理之群組的專案，以及與這些專案相關的任務、問題或檔案。</p> </td> 
  </tr> 
  <tr> 
   <td>資源回收筒：最近已還原</td> 
   <td>完整存取權</td> 
   <td>身為群組管理員的使用者可檢視最近還原的專案。</td> 
  </tr> 
  <tr> 
   <td>職務角色</td> 
   <td>完整存取權</td> 
   <td> <p>修改但不刪除現有的工作角色。</p> <p>新增職位角色。</p> </td> 
  </tr> 
  <tr> 
   <td>團隊</td> 
   <td>完整存取權</td> 
   <td> <p>沒有建立團隊的許可權。</p> <p>建立或編輯使用者時，將現有團隊新增至使用者。</p> </td> 
  </tr> 
  <tr> 
   <td>群組</td> 
   <td>完整存取權</td> 
   <td> <p>沒有建立群組的許可權。</p> <p>只有群組管理員可以管理其管理的群組的群組成員資格、子群組和群組層級狀態。 </p> </td> 
  </tr> 
  <tr> 
   <td>公司</td> 
   <td>完整存取權</td> 
   <td>完整存取權</td> 
  </tr> 
  <tr> 
   <td>登入身份</td> 
   <td>完整存取權 </td> 
   <td> <p>如果他們的群組管理存取權在其存取層級上已啟用，並且他們被指定為群組管理員，則他們可以以其所管理群組及其子群組中的使用者身分登入。 他們無法以系統管理員身分登入。<br>如需啟用使用者群組管理存取權的詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">授予使用者存取權</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>排程</td> 
   <td>完整存取權</td> 
   <td> <p>無權編輯排程。</p> <p>存取權可在使用者層級將現有排程新增給其他使用者。 </p> </td> 
  </tr> 
  <tr> 
   <td>時程表和時數：時程表設定檔</td> 
   <td>完整存取權</td> 
   <td> <p>存取權以在使用者層級將現有的週期性時程表指派給使用者。</p> <p>身為群組管理員的使用者可以為其管理的群組及其子群組建立時間表設定檔。 </p> </td> 
  </tr> 
  <tr> 
   <td>時程表和小時：小時型別</td> 
   <td>完整存取權</td> 
   <td> <p>在使用者層級存取以指派時數型別給使用者。</p> </td> 
  </tr> 
  <tr> 
   <td>時程表和時數：偏好設定</td> 
   <td>完整存取權</td> 
   <td>無存取權</td> 
  </tr> 
  <tr> 
   <td>電子郵件：通知：事件通知</td> 
   <td>全部啟用/停用</td> 
   <td>無存取權</td> 
  </tr> 
  <tr> 
   <td>電子郵件：通知：提醒通知</td> 
   <td>完整存取權</td> 
   <td>完整存取權</td> 
  </tr> 
  <tr> 
   <td>電子郵件：通知：電子郵件範本</td> 
   <td>完整存取權</td> 
   <td> <p>無權編輯電子郵件範本。</p> <p>存取以將現有的電子郵件範本新增到提醒通知。</p> </td> 
  </tr> 
  <tr> 
   <td>電子郵件：自動提醒</td> 
   <td>完整存取權</td> 
   <td>無存取權</td> 
  </tr> 
  <tr> 
   <td>電子郵件：邀請</td> 
   <td>完整存取權</td> 
   <td> <p>無權編輯電子郵件邀請。</p> <p>僅從「人員」標籤存取重新傳送電子郵件邀請給未註冊的使用者。</p> </td> 
  </tr> 
  <tr> 
   <td>電子郵件：設定</td> 
   <td>完整存取權</td> 
   <td> <p>無存取權</p> </td> 
  </tr> 
  <tr> 
   <td>計分卡</td> 
   <td>完整存取權</td> 
   <td> <p>完整存取權</p> </td> 
  </tr> 
  <tr> 
   <td>費用類型</td> 
   <td>完整存取權</td> 
   <td> <p>無存取權</p> </td> 
  </tr> 
  <tr> 
   <td>風險類型</td> 
   <td>完整存取權</td> 
   <td>無存取權</td> 
  </tr> 
  <tr> 
   <td>存取層級</td> 
   <td> <p>修改所有存取層級的完整存取權。</p> <p>預設無法修改系統管理員和外部使用者存取層級。</p> </td> 
   <td> <p>無權編輯存取層級。</p> <p>將存取層級指派給在使用者層級低於或等於其存取層級的其他使用者。</p> </td> 
  </tr> 
  <tr> 
   <td>介面：版面配置範本</td> 
   <td>完整存取權</td> 
   <td> <p>在使用者層級存取將現有版面配置範本指派給其他使用者。 </p> <p>指定為群組管理員的使用者可為其管理的群組和子群組建立版面配置範本。</p> </td> 
  </tr> 
  <tr> 
   <td>介面：更新摘要</td> 
   <td>完整存取權</td> 
   <td> <p>無權修改更新摘要。</p> <p>存取權，可在編輯自訂Forms時新增要在更新摘要中追蹤的欄位。</p> </td> 
  </tr> 
  <tr> 
   <td>介面：篩選器</td> 
   <td>完整存取權</td> 
   <td> <p>無權在設定區域中建立篩選器。</p> <p>存取在物件清單中建立新篩選器。</p> </td> 
  </tr> 
  <tr> 
   <td>介面：檢視</td> 
   <td>完整存取權</td> 
   <td> <p>沒有在「設定」區域中建立檢視的存取權。</p> <p>存取在物件清單中建立新檢視。</p> </td> 
  </tr> 
  <tr> 
   <td>介面：群組</td> 
   <td>完整存取權</td> 
   <td> <p>無權在「設定」區域中建立「群組」。</p> <p>存取在物件清單中建立新群組。</p> </td> 
  </tr> 
  <tr> 
   <td>介面：清單控制項</td> 
   <td>完整存取權</td> 
   <td> <p>無存取權</p> </td> 
  </tr> 
  <tr> 
   <td>檔案：雲端提供者</td> 
   <td>完整存取權</td> 
   <td> <p>無權設定雲端提供者。</p> <p>雲端提供者與Workfront整合後，存取檔案標籤，將檔案連結至雲端提供者，以及從雲端提供者連結。</p> </td> 
  </tr> 
  <tr> 
   <td>檔案：中繼資料對應</td> 
   <td>完整存取權</td> 
   <td>無存取權</td> 
  </tr> 
  <tr> 
   <td>檔案： SharePoint整合</td> 
   <td>完整存取權</td> 
   <td> <p>無權設定SharePoint整合。</p> <p>設定SharePoint與SharePoint的整合後，存取檔案標籤，將檔案連結至Workfront或是從連結。</p> </td> 
  </tr> 
  <tr> 
   <td>檔案：自訂整合</td> 
   <td>完整存取權</td> 
   <td> <p>無權設定自訂整合。</p> <p>協力廠商提供者與Workfront整合後，您就可以從Documents標籤存取與協力廠商提供者之間的連結檔案。</p> </td> 
  </tr> 
  <tr> 
   <td>系統：品牌</td> 
   <td>完整存取權</td> 
   <td>無存取權</td> 
  </tr> 
  <tr> 
   <td>系統：客戶資訊</td> 
   <td>完整存取權</td> 
   <td>無存取權</td> 
  </tr> 
  <tr> 
   <td>系統：單一登入(SSO)</td> 
   <td>完整存取權</td> 
   <td>無存取權</td> 
  </tr> 
  <tr> 
   <td>系統：更新SSO的使用者</td> 
   <td>完整存取權</td> 
   <td>無存取權</td> 
  </tr> 
  <tr> 
   <td>系統： Kick-Start</td> 
   <td>完整存取權</td> 
   <td>無存取權</td> 
  </tr> 
  <tr> 
   <td>系統：診斷</td> 
   <td>完整存取權</td> 
   <td>無存取權</td> 
  </tr> 
  <tr> 
   <td>系統：偏好設定</td> 
   <td>完整存取權</td> 
   <td>無存取權</td> 
  </tr> 
 </tbody> 
</table>

### 存取物件 {#access-to-objects}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>區域/物件</th> 
   <th>Workfront管理員 </th> 
   <th>擁有Plan授權和某些管理許可權的使用者</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>行事曆</td> 
   <td>完整存取權</td> 
   <td>管理他們建立的行事曆和他們共用的行事曆。</td> 
  </tr> 
  <tr> 
   <td>儀表板</td> 
   <td>完整存取權</td> 
   <td>管理他們建立的儀表板以及與他們共用的儀表板。</td> 
  </tr> 
  <tr> 
   <td>文件</td> 
   <td>完整存取權</td> 
   <td>管理他們上傳的檔案或與他們共用的檔案。</td> 
  </tr> 
  <tr> 
   <td>問題</td> 
   <td>完整存取權</td> 
   <td>管理他們建立的問題或與他們共用的問題。</td> 
  </tr> 
  <tr> 
   <td>專案組合</td> 
   <td>完整存取權</td> 
   <td>管理他們建立的投資組合或他們共用的投資組合。 </td> 
  </tr> 
  <tr> 
   <td>計劃</td> 
   <td>完整存取權</td> 
   <td>管理他們建立的計畫或與他們共用的計畫。</td> 
  </tr> 
  <tr> 
   <td>專案</td> 
   <td>完整存取權</td> 
   <td>管理他們建立的專案或與他們共用的專案。</td> 
  </tr> 
  <tr> 
   <td>報告</td> 
   <td>完整存取權</td> 
   <td>管理他們建立或與他們共用的報告。 檢視、複製和編輯系統報告。</td> 
  </tr> 
  <tr> 
   <td>任務</td> 
   <td>完整存取權</td> 
   <td>管理他們建立的工作或與共用的工作</td> 
  </tr> 
  <tr> 
   <td>範本</td> 
   <td>完整存取權</td> 
   <td>管理他們建立的範本或與他們共用的範本</td> 
  </tr> 
  <tr> 
   <td>時程表</td> 
   <td>完整存取權</td> 
   <td>完整存取權</td> 
  </tr> 
  <tr> 
   <td>使用者</td> 
   <td>完整存取權</td> 
   <td> <p>有限存取</p> <p>他們無法將群組指派給不是群組管理員的使用者或非公開群組。</p> <p>他們無法將存取層級指派給高於他們自己的存取層級的使用者。</p> <p>如果他們的群組管理存取權在其存取層級上已啟用，並且他們被指定為群組的群組管理員，則他們可以重設密碼，並以其管理的群組及其子群組中的使用者身分登入。 他們無法重設密碼或以系統管理員身分登入。<br>如需啟用使用者群組管理存取權的詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">授予使用者存取權</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>
