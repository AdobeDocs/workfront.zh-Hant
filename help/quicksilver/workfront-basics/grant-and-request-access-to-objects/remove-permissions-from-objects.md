---
product-area: user-management;portfolios
navigation-topic: grant-and-request-access-to-objects
title: 從對象中刪除權限
description: 您可以刪除其他用戶對您有權訪問共用的對象的權限。 對於所有可共用的對象，從對象中刪除權限是相同的。
author: Alina
feature: Get Started with Workfront
exl-id: 8e191b5e-31df-4291-8b9d-9ca69be27561
source-git-commit: bbd64e9deed1b89d720272508b3562c354578704
workflow-type: tm+mt
source-wordcount: '1076'
ht-degree: 0%

---

# 從對象中刪除權限

您可以刪除其他用戶對您有權訪問共用的對象的權限。 對於所有可共用的對象，從對象中刪除權限是相同的。 

與共用對象類似的注意事項適用於從對象中刪除權限。 如需詳細資訊，請參閱 [共用物件的考量事項](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md#consider) 在文章中 [對象共用權限概述](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)

## 存取需求

<!--drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Workfront license*</td> 
   <td> <p>Current license: Contributor or higher</p>
   Or  
   <p>Legacy license: Request or higher</p>
   <p><b>NOTE</b></p>

   <p>Some objects require a higher access than Request. </p>
   
   <p>For example, for the current license, a Contributor can share issues, but only Standard-license users can share a project.</p>
   
   <p>For the legacy license, a Requestor can share issues, but only Workers or Planners can share a project.</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View access or higher to the objects you want to share</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View permissions or higher to the objects you want to share</p> <p>Manage permissions to remove inherited permissions on objects</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

您必須具備以下條件才能共用物件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>任何 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Workfront授權*</td> 
   <td> <p>要求或更高版本</p>
   <p><b>附註</b></p>

某些物件的存取權限比要求高。 例如，請求者可以共用問題，但只有工人或規劃者才能共用項目。

</td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>查看要共用的對象的訪問權限或更高</p> <p><b>附註</b>

如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>查看要共用的對象的權限或更高</p> <p>管理權限以移除物件的繼承權限</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 從對象的共用清單中刪除實體 {#remove-entities-from-the-sharing-list-of-an-object}

您可以從物件的共用清單中移除實體（使用者、工作角色、團隊、群組、公司）。 這會移除其物件的權限。

1. 前往您要共用的物件。

   有關可共用對象的資訊，請參見 [對象共用權限概述](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

1. 按一下 **更多** 圖示 ![](assets/more-icon.png)在物件名稱旁，按一下 **共用** 或&#x200B;**共用。**

   ![](assets/share-a-document-350x160.png)

1. 按一下 **x** 在用戶、團隊、組、公司、作業角色的名稱旁邊，以在對象訪問框中刪除它們。

   ![](assets/remove-permissions-on-project-nwe-350x479.png)

1. 在 `<User Name>`的Workfront訪問權限將從此下拉菜單中刪除，選擇是否僅從所選對象或與其關聯的所有子對象中刪除其訪問權限。\
   存在下列情況：

   * 如果僅從對象中刪除實體，則該實體將丟失其對對象的權限，並丟失其對子對象的繼承權限。 如果它們先前被單獨授予子項的權限，則當您選擇此選項時，它們將保留與其關聯的所有子項對象的相同權限。 
   * 如果從對象和所有子對象中刪除實體，則該實體將丟失對對象和所有子對象的權限，即使它們以前被授予每個子對象的單獨權限。 

1. 按一下&#x200B;**儲存**。

## 大量從多個物件移除權限

在清單中大量選取實體時，您一次可以從多個物件中移除實體（使用者、工作角色、團隊、群組、公司）。 

>[!NOTE]
>
>當批量選擇所有對象時，無法查看所選對象具有哪些訪問實體。 在刪除所選對象的權限之前，您必須知道要從共用對象中刪除的實體。

1. 轉到要共用的對象清單。

   有關可共用對象的資訊，請參見 [對象共用權限概述](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

1. 在清單中選取數個物件，然後按一下 **共用** 圖示 ![](assets/share-icon.png)清單頂端。
1. 輸入您要移除其存取權的使用者、角色、團隊、群組或公司名稱， **編輯 `<Object Name>` 存取** 欄位。
1. 從存取下拉式功能表中，選取 **無權存取**.

   ![](assets/no-access-option-removing-permissions-bulk-tasks-nwe-350x166.png)

1. 在 `<User Name>`的Workfront訪問權限將從此下拉菜單中刪除，選擇是否僅從已選擇的對象或與其關聯的所有其他子對象中刪除其訪問權限。\
   存在下列情況：

   * 如果僅從對象中刪除實體，則該實體將丟失其對對象的權限，並丟失其對子對象的繼承權限。 如果它們先前被單獨授予子項的權限，則當您選擇此選項時，它們將保留與其關聯的所有子項對象的相同權限。 
   * 如果從對象和所有子對象中刪除實體，則該實體將丟失對對象和所有子對象的權限，即使它們以前被授予每個子對象的單獨權限。

   **範例：** 選擇是否僅刪除您在清單中選擇的任務，還是刪除附加到任務的問題和文檔的權限。

   ![](assets/remove-permissions-bulk-drop-down-for-attached-objects-nwe-350x96.png)

1. （可選）要批量更改多個對象的權限，請為所選實體選擇其他共用級別。

   例如，如果他們有「管理」權限，請改為選取「貢獻」或「檢視」。

1. 按一下&#x200B;**儲存**。

## 移除繼承的權限

可以從對象中刪除繼承的權限，使所有者能夠明確標識誰將訪問子對象，而不管用戶對父對象的訪問權限如何。

>[!IMPORTANT]
>
>只有具有「管理」權限的使用者才能移除繼承的權限。

若要移除繼承的權限：

1. 前往您擁有「管理」權限的物件。 例如，前往任務。
1. 移至物件存取方塊，如 [從對象的共用清單中刪除實體](#remove-entities-from-the-sharing-list-of-an-object) 一節。
1. 選取 **x** 下一頁 **繼承的權限** ，移除該處列出的任何人。

   ![](assets/remove-inherited-permissions-on-project-nwe-350x475.png)

   這可確保預設情況下，沒有授予父對象（如項目）權限的人擁有此任務的權限。 您必須在任務的共用清單中列出各個實體，以授予任務的權限。

   >[!TIP]
   >
   >您無法從「繼承的權限」清單中移除個別實體。 您只能停用所列實體的繼承權限。

1. 按一下 **儲存**. 

## 將物件設為私人

如果已在系統範圍內共用對象，或者已將其設定為公用，從而與外部用戶共用對象，則可以通過刪除系統範圍或公共權限將其重新設定為專用。 

有關使對象在系統範圍內或公開可用的詳細資訊，請參閱 [共用物件](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).

若要將物件設為私人：

1. 移至您要設為私人的物件。\
   例如，導覽至報表。
1. 按一下 **報表動作**，然後 **共用**.

   ![](assets/report-permissions-make-private-nwe-350x477.png)

1. 按一下 **刪除公共訪問** 移除外部使用者檢視報表的存取權。
1. 按一下 **刪除系統範圍的訪問** 停止與所有Workfront使用者共用。 
1. 按一下&#x200B;**儲存**。
