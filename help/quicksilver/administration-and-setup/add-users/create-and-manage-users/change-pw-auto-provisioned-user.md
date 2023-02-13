---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
title: 更改自動布建用戶的密碼
description: 通常，當新用戶嘗試更改其臨時密碼時，他們會輸入其電子郵件地址，並收到錯誤的用戶名。 他們必須輸入系統指派的使用者名稱，即全域唯一識別碼(GUID)。 由於GUID不易記住和使用，建議您將新使用者的使用者名稱變更為其Workfront郵件地址，然後允許他們變更其密碼。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 14124911-e5e1-4a4f-9b25-8b4fab0329e1
source-git-commit: 7bd3d2252b124a07a112aaa2b7798063087e7cab
workflow-type: tm+mt
source-wordcount: '532'
ht-degree: 0%

---

# 更改自動布建用戶的密碼

當您透過自動布建來建立使用者時，Adobe Workfront會為使用者指派GUID（全域唯一識別碼）。 GUID是隨機數字和字母的唯一字串，例如 *5489cb430012526e1ea635e8c29f377f*.

通常，當新用戶嘗試更改其臨時密碼時，他們會輸入其電子郵件地址作為用戶名，並收到錯誤的用戶名。 用戶必須輸入系統分配的用戶名（即GUID）才能更改其密碼。

由於GUID使用者名稱可能難以使用，建議您先將使用者的使用者名稱變更為其Workfront郵件地址，然後允許他們變更其密碼。

>[!TIP]
>
>您可透過下列方式找到使用者的GUID:
>
>* 前往使用者的設定檔，並從瀏覽器的URL複製GUID。
>
>  例如，在URL中 `https://acme.workfront.com/user/61941ab1000af22d7104628efa1c738b/details`，您會複製前兩個正斜線之間的數字和字母字串： `61941ab1000af22d7104628efa1c738b`.
>
>  如需詳細資訊，請參閱 [編輯使用者的設定檔](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).
>
>* 使用「用戶」>「GUID」列建立用戶報告。 如需詳細資訊，請參閱 [建立報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).
>
>* 查詢Workfront API。
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
   <td> <p>您必須是Workfront管理員。</p> <p><b>注意</b>:如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 更改自動布建用戶的密碼

1. 如下列範例所示，透過傳遞API請求來判斷使用者的GUID使用者名稱：

   https://`<domain>`.my.workfront.com/attask/api/v14.0/USER/search?fields=username&amp;ID=`<ID of User>` 其中 *`<domain>`* 是您公司的網域， *`<ID of User>`* 是使用者的Workfront ID。

   您會收到類似下列的回應：

   ![](assets/get-guid.png)

   「使用者名稱」的傳回即為使用者的GUID。

1. 使用其GUID作為用戶名，更改用戶的密碼。

   有關更改密碼的詳細資訊，請參閱 [重設密碼](../../../workfront-basics/manage-your-account-and-profile/managing-your-workfront-account/reset-your-password.md).

   如果貴組織使用SSO系統，則只有Workfront系統管理員可以變更使用者的密碼。 如需詳細資訊，請參閱 [Adobe Workfront中的單一登入概觀](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md)

1. 使用者登入Workfront後，請導覽至：

```
   https://<your domain>.my.workfront.com/login/convertUsername
```

1. 在 **您的登入電子郵件地址** 框中，驗證用戶的電子郵件地址是否正確，然後按一下 **更新帳戶**.

   ![](assets/guidusername-350x272.png)

   使用者的使用者名稱已變更為其Workfront電子郵件地址。

>[!TIP]
>
>若要尋找使用者的ID:
>
>1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **使用者** ![](assets/users-icon-in-main-menu.png).
>
>1. 選取使用者。
>
>   使用者的設定檔頁面隨即開啟，其使用者ID會顯示在URL中。
