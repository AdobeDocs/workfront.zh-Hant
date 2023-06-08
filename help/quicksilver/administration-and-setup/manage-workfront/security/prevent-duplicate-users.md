---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: security
title: 防止重複的使用者
description: 在Adobe Workfront中建立新使用者時，您無法再使用已由其他使用者使用的電子郵件地址，即使電子郵件地址依大小寫而異(例如JohnDoe@example.com和johndoe@example.com)。 此外，為了準備好迎接未來的驗證增強功能，請確定所有使用者在Workfront執行個體中都擁有唯一的電子郵件地址。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 84d9a752-e894-42cf-9b40-375e35f02c97
source-git-commit: 8bcc2859b3b6ce7a264c8f234536a93b7761ab6b
workflow-type: tm+mt
source-wordcount: '608'
ht-degree: 0%

---

# 防止重複的使用者

在Adobe Workfront中建立新使用者時，您無法再使用已由其他使用者使用的電子郵件地址，即使電子郵件地址依大小寫而異(例如JohnDoe@example.com和johndoe@example.com)。 此外，為了準備好迎接未來的驗證增強功能，請確定所有使用者在Workfront執行個體中都擁有唯一的電子郵件地址。

## 存取需求

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
   <td>計劃</td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>您必須是Workfront管理員。</p> <p><b>注意</b>：如果您還是沒有存取權，請洽詢Workfront管理員，瞭解他們是否對您的存取層級設定其他限制。 如需有關Workfront管理員如何修改您的存取層級的資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 建立具有唯一電子郵件地址的使用者

自2019.4版開始，在Workfront中建立新使用者時，即使電子郵件地址依大小寫而異，也不再能使用已由其他使用者使用的電子郵件地址。 例如，如果另一個使用者的電子郵件地址是JohnDoe@example.com ，則您無法以johndoe@example.com的電子郵件地址建立另一個使用者。

## 更新Workfront執行個體中現有使用者的電子郵件地址

身為Workfront管理員，您必須更新擁有相符電子郵件地址（僅限大小寫不同）的現有使用者。
若要修正Workfront執行個體中的重複電子郵件地址：

1. 檢查任何重複的使用者，並決定不再需要哪個使用者。

   1. 按一下 **主要功能表** 圖示 ![](assets/main-menu-icon.png) Workfront右上角，然後按一下 **使用者**. ![](assets/users-icon-in-main-menu.png)

   1. 在 **篩選** 功能表，選取 **全部**.

   1. 在 **檢視** 功能表，選取 **使用者登入**.

   1. 在 **分組** 功能表，選取 **無**.

   1. 自訂「使用者登入」檢視。

      1. 按一下 **檢視** > **自訂檢視**.

      1. 取代 **ID** 欄與 **電子郵件地址** 欄。

      1. 重新命名檢視並儲存。
   1. 建立新的群組。

      1. 按一下 **分組** > **新群組**.

      1. 按一下 **切換至文字模式** 在頁面的右上角。
      1. 貼上下列文字模式代碼：

         `group.0.linkedname=direct`
         `group.0.namekey=emailAddr`
         `group.0.valueexpression=LOWER({emailAddr})`
         `group.0.valueformat=string`
         `textmode=true`
   1. 重新命名群組並儲存。



1. 執行下列任一項作業：

   * （偏好方法）為使用者每個額外帳戶的電子郵件地址新增+位址。

      如果您組織中的單一使用者需要存取一個以上的使用者帳戶，請選擇此選項。 如果您的電子郵件提供者不支援加號定址，您必須為每個Workfront帳戶提供個別的電子郵件帳戶。

      例如，John Doe的日常使用帳戶可以有一個使用者帳戶，而測試用途可以有一個使用者帳戶：

      * johndoe@workfront.com
      * johndoe+reviewer@workfront.com
   * 將下列文字附加至電子郵件地址，將網域變更為使用偽網域：

      `.inactive`

      例如，John Doe可以有下列網域： （這些網域必須是唯一的。）

      * johndoe@workfront.inactive
      * johndoe@workfront.inactive2

      您無法再登入這些帳戶，因為密碼重設需要有效的電子郵件地址。 只有使用「登入身份」功能才能存取這些帳戶。

   * 刪除不需要的使用者

      >[!IMPORTANT]
      >
      >只有錯誤建立的帳戶或測試帳戶才選擇此選項。 此選項通常僅針對登入錯誤為零或1的帳戶執行。 不應刪除已定期使用的帳戶。



如果您的Workfront執行個體中有使用者，其相符的電子郵件地址依大小寫不同，Workfront會在需要更新這些使用者時，透過其他資訊和時間表與您連絡。
