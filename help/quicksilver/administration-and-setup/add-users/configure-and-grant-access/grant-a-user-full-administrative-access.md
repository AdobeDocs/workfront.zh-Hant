---
title: 授予使用者完整的管理存取權
description: 您可以授與使用者對Workfront的完整管理存取權。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 46bcb65a-1cb7-443b-88ba-6d0e516e3050
source-git-commit: 253a116e04e0b3a729331f5d0a29405e82808390
workflow-type: tm+mt
source-wordcount: '1614'
ht-degree: 1%

---

# 授予使用者完整的管理存取權

>[!IMPORTANT]
>
>本頁面上描述的程式僅適用於尚未上線至Admin Console的組織。 如果貴組織已上線至Adobe Admin Console，您必須透過Adobe Admin Console執行此動作。
>
>如需在Adobe Admin Console中授予完整管理員存取權的指示：
>
>* 請參閱 [使用Adobe Admin Console在Workfront中建立系統管理員](../../../administration-and-setup/add-users/create-and-manage-users/admin-console.md#create2)
>* 請參閱文章中的「編輯使用者詳細資料」一節 [個別管理使用者](https://helpx.adobe.com/enterprise/using/manage-users-individually.html) 在Adobe Admin Console檔案中。
>* 請連絡您的Adobe Admin Console管理員。
>
>如需依貴組織是否已上線至Adobe Admin Console而有所不同的程式清單，請參閱 [平台管理差異(Adobe Workfront/Adobe業務平台)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

身為Adobe Workfront管理員，您可以指派系統管理員存取層級來建立另一個Workfront管理員。 具有此存取層級的使用者可完整管理存取Workfront中的所有項目，包括他們未自行建立的項目。

>[!NOTE]
>
>這與使用訪問級別來授予用戶對系統某些區域的管理訪問權限不同。 如需詳細資訊，請參閱下列內容：
>
>* [授予用戶對特定區域的管理訪問權限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md)
>* [Workfront管理員的存取權與具有管理權限的計畫使用者的存取權](#access-of-a-workfront-administrator-vs-access-of-a-plan-user-with-administrative-rights) 本文
>


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
   <td>計劃</td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置</td> 
   <td> <p>您必須是Workfront管理員。 如需詳細資訊，請參閱 <a href="#" class="MCXref xref selected">授予使用者完整的管理存取權</a>.</p> <p><b>注意</b>:如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 授予單個用戶的完整系統管理員訪問權限

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **使用者** ![](assets/users-icon-in-main-menu.png).

1. 按一下您要授予管理員權限的使用者名稱。
1. 按一下「更多」功能表 ![](assets/more-icon.png)，然後按一下 **編輯**.

1. 在 **編輯人員** 框，按一下 **存取**.

1. 在 **存取層級** 下拉式清單，選取 **系統管理員** 存取層級。

   根據您在系統中所做的更改，此訪問級別的名稱可能已更改。

1. 按一下 **儲存變更。**

   用戶現在在系統中擁有完整的系統管理員權限。

## Workfront管理員的存取權與具有管理權限的計畫使用者的存取權  {#access-of-a-workfront-administrator-vs-access-of-a-plan-user-with-administrative-rights}

下表顯示具有Workfront管理員存取層級的使用者的存取權限，與具有某些管理權限之計畫授權的使用者的存取權限之間的差異。

Workfront管理員可以檢視系統中的所有物件（無論建立對象是誰）、建立新物件，以及修改或刪除現有物件。 他們可完全訪問系統中的所有對象。

具有計畫許可證且可以編輯某一區域中功能的用戶可以完全訪問該區域中的功能。

>[!NOTE]
>
>擁有計畫授權且指定為群組管理員的使用者，可以執行Workfront管理員允許的部分動作。 他們只能對所管理的組、其子組以及這些組和子組中的用戶執行這些操作。 如需詳細資訊，請參閱 [群組管理員](../../../administration-and-setup/manage-groups/group-roles/group-administrators.md).

* [訪問「設定」區域](#access-to-the-setup-area)
* [對對象的訪問](#access-to-objects)

### 訪問「設定」區域 {#access-to-the-setup-area}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>區域/對象</th> 
   <th>Workfront管理員 </th> 
   <th>具有計畫許可證和某些管理權限的用戶</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>專案偏好設定：專案</td> 
   <td>完全存取</td> 
   <td>無權存取</td> 
  </tr> 
  <tr> 
   <td>專案偏好設定：工作與問題</td> 
   <td>完全存取</td> 
   <td>無權存取</td> 
  </tr> 
  <tr> 
   <td>專案偏好設定：狀態</td> 
   <td>完全存取</td> 
   <td> <p>無權存取</p> </td> 
  </tr> 
  <tr> 
   <td>專案偏好設定：優先順序</td> 
   <td>完全存取</td> 
   <td>無權存取</td> 
  </tr> 
  <tr> 
   <td>專案偏好設定：嚴重性</td> 
   <td>完全存取</td> 
   <td>無權存取</td> 
  </tr> 
  <tr> 
   <td>專案偏好設定：匯率</td> 
   <td>完全存取</td> 
   <td>完全存取</td> 
  </tr> 
  <tr> 
   <td>流程：核准</td> 
   <td> <p>完全存取</p> </td> 
   <td>完全存取</td> 
  </tr> 
  <tr> 
   <td>流程：里程碑路徑</td> 
   <td>完全存取</td> 
   <td>完全存取</td> 
  </tr> 
  <tr> 
   <td>自訂表單</td> 
   <td>完全存取</td> 
   <td> <p>管理他們建立的自訂表單或與他們共用的自訂表單。</p> <p>將他們建立的自訂表單或與他們共用的自訂表單附加至他們擁有管理或貢獻權限的物件。</p> </td> 
  </tr> 
  <tr> 
   <td>資源回收筒：最近刪除</td> 
   <td>完全存取</td> 
   <td> <p>屬於群組管理員的使用者可以還原指派給他們管理之群組的專案，以及與這些專案相關聯的任務、問題或檔案。</p> </td> 
  </tr> 
  <tr> 
   <td>資源回收筒：最近恢復</td> 
   <td>完全存取</td> 
   <td>屬於群組管理員的使用者可以查看他們最近還原的項目。</td> 
  </tr> 
  <tr> 
   <td>職務角色</td> 
   <td>完全存取</td> 
   <td> <p>修改但不刪除現有作業角色。</p> <p>添加新作業角色。</p> </td> 
  </tr> 
  <tr> 
   <td>團隊</td> 
   <td>完全存取</td> 
   <td> <p>無法建立團隊。</p> <p>建立或編輯使用者時，將現有團隊新增至使用者。</p> </td> 
  </tr> 
  <tr> 
   <td>群組</td> 
   <td>完全存取</td> 
   <td> <p>無權建立群組。</p> <p>只有群組管理員才能管理其所管理群組的群組成員資格、子群組和群組層級狀態。 </p> </td> 
  </tr> 
  <tr> 
   <td>公司</td> 
   <td>完全存取</td> 
   <td>完全存取</td> 
  </tr> 
  <tr> 
   <td>登入方式</td> 
   <td>完全存取 </td> 
   <td> <p>如果在其訪問級別上啟用了其組管理訪問，並將其指定為組管理員，則它們可以以其所管理的組中的用戶及其子組中的用戶身份登錄。 他們無法以系統管理員身份登錄。<br>如需為使用者啟用群組管理存取權限的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">授予使用者存取權</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>排程</td> 
   <td>完全存取</td> 
   <td> <p>無法編輯排程。</p> <p>在使用者層級存取將現有排程新增至其他使用者。 </p> </td> 
  </tr> 
  <tr> 
   <td>時間表和小時數：時間表配置檔案</td> 
   <td>完全存取</td> 
   <td> <p>在用戶級別訪問將現有時間表配置檔案分配給用戶。</p> <p>作為組管理員的用戶可以為其管理的組及其子組建立時間表配置檔案。 </p> </td> 
  </tr> 
  <tr> 
   <td>時間表和小時數：小時類型</td> 
   <td>完全存取</td> 
   <td> <p>在使用者層級存取指派小時類型給使用者。</p> </td> 
  </tr> 
  <tr> 
   <td>時間表和小時數：偏好設定</td> 
   <td>完全存取</td> 
   <td>無權存取</td> 
  </tr> 
  <tr> 
   <td>電子郵件：通知：事件通知</td> 
   <td>全部啟用/停用</td> 
   <td>無權存取</td> 
  </tr> 
  <tr> 
   <td>電子郵件：通知：提醒通知</td> 
   <td>完全存取</td> 
   <td>完全存取</td> 
  </tr> 
  <tr> 
   <td>電子郵件：通知：電子郵件範本</td> 
   <td>完全存取</td> 
   <td> <p>無法編輯電子郵件範本。</p> <p>存取新增現有電子郵件範本以提醒通知。</p> </td> 
  </tr> 
  <tr> 
   <td>電子郵件：自動提醒</td> 
   <td>完全存取</td> 
   <td>無權存取</td> 
  </tr> 
  <tr> 
   <td>電子郵件：邀請</td> 
   <td>完全存取</td> 
   <td> <p>無權編輯電子郵件邀請。</p> <p>只能從「人物」索引標籤存取將電子郵件邀請重新傳送給未註冊的使用者。</p> </td> 
  </tr> 
  <tr> 
   <td>電子郵件：設定</td> 
   <td>完全存取</td> 
   <td> <p>無權存取</p> </td> 
  </tr> 
  <tr> 
   <td>計分卡</td> 
   <td>完全存取</td> 
   <td> <p>完全存取</p> </td> 
  </tr> 
  <tr> 
   <td>費用類型</td> 
   <td>完全存取</td> 
   <td> <p>無權存取</p> </td> 
  </tr> 
  <tr> 
   <td>風險類型</td> 
   <td>完全存取</td> 
   <td>無權存取</td> 
  </tr> 
  <tr> 
   <td>存取層級</td> 
   <td> <p>完全訪問以修改所有訪問級別。</p> <p>預設情況下，無法修改系統管理員和外部用戶訪問級別。</p> </td> 
   <td> <p>無權編輯訪問級別。</p> <p>將訪問級別分配給在用戶級別上與其較低或相等的其他用戶。</p> </td> 
  </tr> 
  <tr> 
   <td>介面：版面範本</td> 
   <td>完全存取</td> 
   <td> <p>在使用者層級存取將現有的版面範本指派給其他使用者。 </p> <p>指定為群組管理員的使用者可為他們管理的群組和子群組建立版面範本。</p> </td> 
  </tr> 
  <tr> 
   <td>介面：更新摘要</td> 
   <td>完全存取</td> 
   <td> <p>無權修改更新摘要。</p> <p>在編輯自訂Forms時，存取新增要在更新摘要中追蹤的欄位。</p> </td> 
  </tr> 
  <tr> 
   <td>介面：篩選器</td> 
   <td>完全存取</td> 
   <td> <p>無權在「設定」區域中建立篩選器。</p> <p>在對象清單中建立新篩選器的訪問權限。</p> </td> 
  </tr> 
  <tr> 
   <td>介面：檢視</td> 
   <td>完全存取</td> 
   <td> <p>無權在「設定」區域中建立視圖。</p> <p>在對象清單中建立新視圖的訪問權限。</p> </td> 
  </tr> 
  <tr> 
   <td>介面：分組</td> 
   <td>完全存取</td> 
   <td> <p>無權在「設定」區域中建立分組。</p> <p>在對象清單中建立新分組的訪問權限。</p> </td> 
  </tr> 
  <tr> 
   <td>介面：清單控制項</td> 
   <td>完全存取</td> 
   <td> <p>無權存取</p> </td> 
  </tr> 
  <tr> 
   <td>文檔：雲端提供者</td> 
   <td>完全存取</td> 
   <td> <p>無法設定雲端提供者。</p> <p>在雲端提供者已與Workfront整合後，您即可從「檔案」標籤存取連結檔案至雲端提供者與雲端提供者的功能。</p> </td> 
  </tr> 
  <tr> 
   <td>文檔：中繼資料對應</td> 
   <td>完全存取</td> 
   <td>無權存取</td> 
  </tr> 
  <tr> 
   <td>文檔：SharePoint整合</td> 
   <td>完全存取</td> 
   <td> <p>無法設定SharePoint整合。</p> <p>設定SharePoint與Workfront的整合後，您就可從「檔案」標籤存取連結檔案至SharePoint和從。</p> </td> 
  </tr> 
  <tr> 
   <td>文檔：自訂整合</td> 
   <td>完全存取</td> 
   <td> <p>無法設定自訂整合。</p> <p>在第三方提供者已與Workfront整合後，您即可從「檔案」標籤存取連結檔案至協力廠商和從協力廠商。</p> </td> 
  </tr> 
  <tr> 
   <td>系統：品牌推廣</td> 
   <td>完全存取</td> 
   <td>無權存取</td> 
  </tr> 
  <tr> 
   <td>系統：客戶資訊</td> 
   <td>完全存取</td> 
   <td>無權存取</td> 
  </tr> 
  <tr> 
   <td>系統：單一登入(SSO)</td> 
   <td>完全存取</td> 
   <td>無權存取</td> 
  </tr> 
  <tr> 
   <td>系統：更新SSO的用戶</td> 
   <td>完全存取</td> 
   <td>無權存取</td> 
  </tr> 
  <tr> 
   <td>系統：開始</td> 
   <td>完全存取</td> 
   <td>無權存取</td> 
  </tr> 
  <tr> 
   <td>系統：診斷</td> 
   <td>完全存取</td> 
   <td>無權存取</td> 
  </tr> 
  <tr> 
   <td>系統：偏好設定</td> 
   <td>完全存取</td> 
   <td>無權存取</td> 
  </tr> 
 </tbody> 
</table>

### 對對象的訪問 {#access-to-objects}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>區域/對象</th> 
   <th>Workfront管理員 </th> 
   <th>具有計畫許可證和某些管理權限的用戶</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>行事曆</td> 
   <td>完全存取</td> 
   <td>管理建立的日曆和與其共用的日曆。</td> 
  </tr> 
  <tr> 
   <td>儀表板</td> 
   <td>完全存取</td> 
   <td>管理其建立的控制面板以及與其共用的控制面板。</td> 
  </tr> 
  <tr> 
   <td>文件</td> 
   <td>完全存取</td> 
   <td>管理其上傳的檔案或與其共用的檔案。</td> 
  </tr> 
  <tr> 
   <td>問題</td> 
   <td>完全存取</td> 
   <td>管理其建立的問題或與其共用的問題。</td> 
  </tr> 
  <tr> 
   <td>專案組合</td> 
   <td>完全存取</td> 
   <td>管理其建立的產品組合或與其共用的產品組合。 </td> 
  </tr> 
  <tr> 
   <td>計劃</td> 
   <td>完全存取</td> 
   <td>管理他們建立的方案或與他們共用的方案。</td> 
  </tr> 
  <tr> 
   <td>專案</td> 
   <td>完全存取</td> 
   <td>管理其建立的專案或與其共用的專案。</td> 
  </tr> 
  <tr> 
   <td>報告</td> 
   <td>完全存取</td> 
   <td>管理其建立的報表或與其共用的報表。 查看、複製和編輯系統報告。</td> 
  </tr> 
  <tr> 
   <td>任務</td> 
   <td>完全存取</td> 
   <td>管理其建立的任務或與共用的任務</td> 
  </tr> 
  <tr> 
   <td>範本</td> 
   <td>完全存取</td> 
   <td>管理其建立的範本或與其共用的範本</td> 
  </tr> 
  <tr> 
   <td>時程表</td> 
   <td>完全存取</td> 
   <td>完全存取</td> 
  </tr> 
  <tr> 
   <td>使用者</td> 
   <td>完全存取</td> 
   <td> <p>有限存取</p> <p>他們無法將群組指派給非群組管理員或非公用群組的使用者。</p> <p>他們無法將訪問級別分配給高於其自身訪問級別的用戶。</p> <p>如果其組管理訪問權限在其訪問級別上啟用，並且被指定為組的組管理員，則他們可以重置的密碼，並以其所管理的組及其子組中的用戶的身份登錄。 他們無法重設的密碼或以系統管理員身份登錄。<br>如需為使用者啟用群組管理存取權限的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">授予使用者存取權</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
