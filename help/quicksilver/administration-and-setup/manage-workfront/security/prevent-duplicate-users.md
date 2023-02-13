---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: security
title: 防止重複的使用者
description: 在Adobe Workfront中建立新使用者時，您無法再使用其他使用者已使用的電子郵件地址，即使電子郵件地址會因個案而異(例如JohnDoe@example.com和johndoe@example.com)。 此外，為了準備未來的驗證增強功能，請確定所有使用者在Workfront例項中都有唯一的電子郵件地址。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 84d9a752-e894-42cf-9b40-375e35f02c97
source-git-commit: 6f5b9e7638a85eca16d722cec6185cd5ed755eca
workflow-type: tm+mt
source-wordcount: '620'
ht-degree: 0%

---

# 防止重複的使用者

在Adobe Workfront中建立新使用者時，您無法再使用其他使用者已使用的電子郵件地址，即使電子郵件地址會因個案而異(例如JohnDoe@example.com和johndoe@example.com)。 此外，為了準備未來的驗證增強功能，請確定所有使用者在Workfront例項中都有唯一的電子郵件地址。

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

## 逐步說明

<!--WRITER
<iframe class="vimeo-player_0" src="assets/371505632?" frameborder="0" allowfullscreen="1" width="560px" height="315px"></iframe>
-->

[觀看此功能的影片示範。](https://vimeo.com/371505632/2e6938ce06)

## 使用不重複的電子郵件地址建立使用者

自2019.4版開始，在Workfront中建立新使用者時，您無法再使用其他使用者已使用的電子郵件地址，即使電子郵件地址會因個案而異。 例如，如果另一個使用者的電子郵件地址為johndoe@example.com，則無法以JohnDoe@example.com建立一個使用者。

## 更新Workfront例項中現有使用者的電子郵件地址

身為Workfront管理員，您必須更新具有相符電子郵件地址的現有使用者，這些地址只會因案例而異。
若要修正Workfront例項中重複的電子郵件地址：

1. 檢查任何重複的使用者，並決定不再需要哪個使用者。

   1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Workfront的右上角，然後按一下 **使用者**. ![](assets/users-icon-in-main-menu.png)

   1. 在 **篩選** 菜單，選擇 **全部**.

   1. 在 **檢視** 菜單，選擇 **使用者登入**.

   1. 在 **分組** 菜單，選擇 **無**.

   1. 自訂使用者登入檢視。

      1. 按一下 **檢視** > **自訂檢視**.

      1. 取代 **ID** 欄 **電子郵件地址** 欄。

      1. 重新命名檢視並儲存。
   1. 建立新的分組。

      1. 按一下 **分組** > **新分組**.

      1. 按一下 **切換到文本模式** 在頁面的右上角。
      1. 貼上下列文字模式程式碼：

         `group.0.linkedname=direct`
         `group.0.namekey=emailAddr`
         `group.0.valueexpression=LOWER({emailAddr})`
         `group.0.valueformat=string`
         `textmode=true`
   1. 重新命名「分組」並儲存。



1. 執行下列任一操作：

   * （偏好使用的方法）為每個額外帳戶新增一個+地址至使用者的電子郵件地址。

      如果貴組織中的單一使用者需要存取超過1個使用者帳戶，請選擇此選項。 如果您的電子郵件提供者不支援加號，您必須為每個Workfront帳戶提供個別的電子郵件帳戶。

      例如，John Doe可以有一個用於其每日使用帳戶的使用者帳戶，以及一個用於測試的帳戶：

      * johndoe@workfront.com
      * johndoe+reviewer@workfront.com
   * 將下列文字附加至電子郵件地址，將網域變更為使用假網域：

      `.inactive`

      例如，John Doe可以有下列網域：（這些必須是唯一的。）

      * johndoe@workfront.inactive
      * johndoe@workfront.inactive2

      您無法再登入這些帳戶，因為密碼重設需要有效的電子郵件地址。 這些帳戶只能使用「登入方式」功能來存取。

   * 刪除不需要的用戶

      >[!IMPORTANT]
      >
      >僅針對錯誤建立的帳戶或測試帳戶選擇此選項。 此選項通常僅針對登入為零或1錯誤的帳戶執行。 不應刪除經常使用的帳戶。



如果您的Workfront例項中有使用者，其相符的電子郵件地址只會因案例而異，Workfront會聯絡您，提供其他資訊和需要更新的時間表。
