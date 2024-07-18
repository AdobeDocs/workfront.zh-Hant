---
title: 匯入使用者
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: 您可以將使用者從網路目錄服務（例如Active Directory或其他LDAP目錄）同步化來匯入使用者至Adobe Workfront網站，也可以使用試算表匯入檔案來匯入使用者。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 3dd99d01-a32f-4af8-90e3-f8c0e9027651
source-git-commit: 1949a0bb213553f1f1f252c4382a90514fcd0b5b
workflow-type: tm+mt
source-wordcount: '494'
ht-degree: 0%

---

# 匯入使用者

<!--

>[!IMPORTANT]
>
>The procedure described on this page applies only to organizations that have not yet been onboarded to the Admin Console. If your organization has been onboarded to the Adobe Admin Console, you must perform this action through the Adobe Admin Console.
>
>For instructions on editing a user's profile in the Adobe Admin Console, see the section "Add users" in the article [Bulk Upload Users](https://helpx.adobe.com/enterprise/using/bulk-upload-users.html) or contact your Adobe Admin Console Administrator.
>
>For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Admin Console, see [Platform-based administration differences (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

-->

您可以使用試算表匯入檔案來匯入使用者。

在建立新使用者之前，請先確定您已建立所有要與該使用者關聯的物件。 例如，如果您尚未建立排程，則無法將排程指派給新使用者，而且您用來關聯排程與新使用者的欄位不會出現在「新使用者」畫面中。

## 存取需求

您必須具備下列專案才能執行本文所述的步驟：

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
   <td role="rowheader">存取層級設定</td> 
   <td> <p>您必須具備下列其中一項：</p> 
    <ul> 
     <li> <p>系統管理員存取層級。 如需詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予使用者完整管理存取權</a>。 </p> </li> 
     <li> <p>您的存取層級中的<b>使用者</b>設定已設定為<b>編輯</b>存取權，其中<b>建立</b>以及在<b>微調您的設定</b> <img src="assets/gear-icon-in-access-levels.png">下啟用的兩個<b>使用者管理員</b>選項中的至少一個。 </p> <p>在這兩個選項中，如果已啟用使用者<b>管理員（群組使用者）</b>，您必須是該使用者所屬群組的群組管理員。</p> <p>如需存取層級中<b>使用者</b>設定的詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">授予使用者存取權</a>。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## 使用試算表匯入檔案來匯入使用者

1. 按一下Adobe Workfront右上角的&#x200B;**主要功能表**&#x200B;圖示![](assets/main-menu-icon.png)，然後按一下&#x200B;**使用者** ![](assets/users-icon-in-main-menu.png)。

1. 按一下&#x200B;**新增使用者**&#x200B;下拉式箭號，然後按一下&#x200B;**匯入使用者**。

1. 在顯示的&#x200B;**匯入使用者**&#x200B;方塊中，下載範例檔案，然後更新範例檔案以包含您自己的使用者個人資訊。

   每一列包含下列欄位：

   * **名字**
   * **姓氏**
   * **電子郵件地址**

     電子郵件地址必須是唯一的。

   * **存取層級**

     存取層級區分大小寫。

   * **SSO登入ID**

     只有在系統中啟用SSO時，才會包含此欄位。 您必須在此欄位中為每個使用者新增同盟ID。 當您從「人員」標籤建立使用者時，如果要允許使用者不使用SSO登入，您可以設定使用者的密碼。 不過，匯入功能不允許您將SSO登入ID保留空白。

   * 確定使用者的電子郵件地址之前或之後沒有額外的空格。

   當您完成某列時，看起來應該像這樣：

   ![importing-new-users.png](assets/importing-new-users.png)

1. 將檔案儲存至工作站上的某個位置。
1. 在&#x200B;**匯入使用者**&#x200B;方塊中按一下&#x200B;**選擇檔案**。

1. 瀏覽並選取您儲存的檔案。
1. （選擇性）選取&#x200B;**傳送邀請電子郵件給此使用者**&#x200B;選項，傳送電子郵件邀請給使用者，通知他們已建立Workfront帳戶，並提示他們設定密碼。

   如果要設定使用者的密碼，請取消選取此選項。

1. 按一下&#x200B;**匯入**。

   您會在畫面頂端收到一則確認訊息，告知您使用者已成功匯入。
