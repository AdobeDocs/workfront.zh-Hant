---
title: 匯入使用者
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: 您可以從網路目錄服務（如Active Directory或其他LDAP目錄）同步使用者，將使用者匯入Adobe Workfront網站，或使用試算表匯入檔案匯入使用者。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 3dd99d01-a32f-4af8-90e3-f8c0e9027651
source-git-commit: 2cbdd0cb065dee01ad128d782334a55233c13156
workflow-type: tm+mt
source-wordcount: '599'
ht-degree: 2%

---

# 匯入使用者

>[!IMPORTANT]
>
>本頁面上描述的程式僅適用於尚未上線至Admin Console的組織。 如果貴組織已上線至Adobe Admin Console，您必須透過Adobe Admin Console執行此動作。
>
>如需在Adobe Admin Console中編輯使用者設定檔的指示，請參閱文章中的「新增使用者」一節 [大量上傳使用者](https://helpx.adobe.com/enterprise/using/bulk-upload-users.html) 或聯絡您的Adobe Admin Console管理員。
>
>如需依貴組織是否已上線至Adobe Admin Console而有所不同的程式清單，請參閱 [平台管理差異(Adobe Workfront/Adobe業務平台)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

您可以使用試算表匯入檔案匯入使用者。

建立新用戶之前，請先確保已建立要與該用戶關聯的所有對象。 例如，如果尚未建立計畫，則無法將計劃分配給新用戶，而用於將計畫與新用戶關聯的欄位不會顯示在「新用戶」螢幕中。

## 存取需求

您必須具備下列條件才能執行本文所述步驟：

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
   <td> <p>您必須具備下列其中一項：</p> 
    <ul> 
     <li> <p>系統管理員訪問級別。 如需詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予使用者完整的管理存取權</a>. </p> </li> 
     <li> <p><b>使用者</b> 在您的存取層級中設定 <b>編輯</b> 存取，使用 <b>建立</b> 和兩者中的至少一個 <b>使用者管理</b> 選項 <b>微調您的設定</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>在這兩個選項中，如果用戶 <b>管理員（群組使用者）</b> 啟用時，您必須是使用者所屬群組的群組管理員。</p> <p>如需 <b>使用者</b> 在存取層級中設定，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">授予使用者存取權</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## 使用電子錶格導入檔案導入用戶

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **使用者** ![](assets/users-icon-in-main-menu.png).

1. 按一下 **新用戶** 下拉箭頭，然後按一下 **匯入使用者**.

1. 在 **匯入使用者** 方塊中顯示、下載範例檔案，然後更新範例檔案以包含您自己使用者的個人資訊。

   每一列皆包含下列欄位：

   * **名字**
   * **姓氏**
   * **電子郵件位址**

      電子郵件地址必須是唯一的。

   * **存取層級**

      訪問級別區分大小寫。

   * **SSO 登入 ID**

      只有在系統中啟用SSO時，才會包含此欄位。 您必須在此欄位中為每個使用者新增同盟ID。 當您從「人物」索引標籤建立使用者時，如果您想要讓使用者不透過SSO登入，可以為使用者設定密碼。 不過，匯入功能不允許將SSO登入ID保留為空白。

   * 請確定使用者電子郵件地址之前或之後不存在額外空格。

   完成列後，應該會如下所示：

   ![importing-new-users.png](assets/importing-new-users.png)

1. 將檔案儲存至工作站上的位置。
1. 按一下 **選擇檔案** 在 **匯入使用者** 框。

1. 導覽至並選取您儲存的檔案。
1. （選用）選取 **傳送邀請電子郵件給此使用者** 選項，向使用者傳送電子郵件邀請，通知他們已建立Workfront帳戶，並提示他們設定密碼。

   如果要為用戶設定密碼，請取消選擇此選項。

1. 按一下 **匯入**.

   畫面頂端會顯示確認訊息，指出使用者已成功匯入。
