---
title: 匯入使用者
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: 您可以將使用者從網路目錄服務（例如Active Directory或其他LDAP目錄）同步化來匯入使用者至Adobe Workfront網站，也可以使用試算表匯入檔案來匯入使用者。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 3dd99d01-a32f-4af8-90e3-f8c0e9027651
source-git-commit: f8d04790caefd12c9811ea3ed94e1f892311d031
workflow-type: tm+mt
source-wordcount: '480'
ht-degree: 1%

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
   <td><p>標準</p><p>規劃</p></td> 
  </tr> 
  <tr> 
   <td>存取層級設定</td> 
   <td> <p>您必須具備下列其中一項：</p> 
    <ul> 
     <li> <p>系統管理員存取層級。 </li> 
     <li> <p>您的存取層級中的<b>使用者</b>設定已設定為<b>編輯</b>存取權，其中<b>建立</b>以及在<b>微調您的設定</b> <b>下啟用的兩個</b>使用者管理員<img src="assets/gear-icon-in-access-levels.png">選項中的至少一個。 </p> <p>在這兩個選項中，如果已啟用<b>使用者管理員（群組使用者）</b>，您必須是使用者所屬群組的群組管理員。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 使用試算表匯入檔案來匯入使用者

{{step-1-to-users}}

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

<!--
1. (Optional) Select the **Send an invite email to this user** option to send an email invitation to the user, notifying them that a Workfront account has been created and prompting them to set their password.

   Deselect this option if you want to set the password for the user.

-->

1. 按一下&#x200B;**匯入**。

   您會在畫面頂端收到一則確認訊息，告知您已成功匯入使用者。

>[!NOTE]
>
>系統會在已停用及未決核准狀態中建立使用者。
> 
>如果使用者未在數分鐘內從「已停用」和「未決核准」狀態中移出，且畫面重新整理未移除「未決核准」徽章，您可以將使用者批次直接新增到Adobe Admin Console。
>
>如需指示，請參閱[管理多個使用者 | 在Adobe檔案中大量上傳CSV](https://helpx.adobe.com/enterprise/using/bulk-upload-users.html)。
