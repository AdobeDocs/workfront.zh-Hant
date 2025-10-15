---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: security
title: 防止重複使用者
description: 在Adobe Workfront中建立新使用者時，您無法再使用已由其他使用者使用的電子郵件地址，即使電子郵件地址依大小寫而異(例如JohnDoe@example.com和johndoe@example.com)。 此外，為了準備迎接未來的驗證增強功能，請確保所有使用者在Workfront執行個體中具有唯一的電子郵件地址。
author: Becky, Lisa
feature: System Setup and Administration
role: Admin
exl-id: 84d9a752-e894-42cf-9b40-375e35f02c97
source-git-commit: 6b2d93d2573d72e4390761038d8078f47d96d55e
workflow-type: tm+mt
source-wordcount: '564'
ht-degree: 0%

---

# 防止重複使用者

在Adobe Workfront中建立新使用者時，您無法再使用已由其他使用者使用的電子郵件地址，即使電子郵件地址依大小寫而異(例如JohnDoe@example.com和johndoe@example.com)。 此外，為了準備迎接未來的驗證增強功能，請確保所有使用者在Workfront執行個體中具有唯一的電子郵件地址。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront套件</td> 
   <td><p>任何</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td><p>標準</p><p>規劃</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>您必須是Workfront管理員。</p> </p> </td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 建立具有唯一電子郵件地址的使用者

從2019.4版開始，在Workfront中建立新使用者時，您無法再使用已由其他使用者使用的電子郵件地址，即使電子郵件地址會依大小寫而異。 例如，如果另一個使用者的電子郵件地址為JohnDoe@example.com，則您無法以johndoe@example.com的電子郵件地址建立另一個使用者。

## 更新Workfront執行個體中現有使用者的電子郵件地址

身為Workfront管理員，您必須更新其匹配電子郵件地址僅隨大小寫不同的現有使用者。
若要修正Workfront執行個體中重複的電子郵件地址：

1. 檢查任何重複的使用者，並決定不再需要哪個使用者。

   {{step-1-to-users}}

   1. 在&#x200B;**篩選器**&#x200B;功能表中，選取&#x200B;**全部**。

   1. 在&#x200B;**檢視**&#x200B;功能表中，選取&#x200B;**使用者登入**。

   1. 在&#x200B;**群組**&#x200B;功能表中，選取&#x200B;**無**。

   1. 自訂「使用者登入」檢視。

      1. 按一下&#x200B;**檢視** > **自訂檢視**。

      1. 將&#x200B;**ID**&#x200B;資料行取代為&#x200B;**電子郵件地址**&#x200B;資料行。

      1. 重新命名檢視並儲存。

   1. 建立新的群組。

      1. 按一下&#x200B;**群組** > **新群組**。

      1. 按一下頁面右上角的&#x200B;**切換至文字模式**。
      1. 貼上下列文字模式程式碼：

         `group.0.linkedname=direct`
         `group.0.namekey=emailAddr`
         `group.0.valueexpression=LOWER({emailAddr})`
         `group.0.valueformat=string`
         `textmode=true`

   1. 重新命名群組並儲存。

1. 執行下列任一項作業：

   * （偏好方法）為使用者每個額外帳戶的電子郵件地址新增+位址。

     如果貴組織中的單一使用者需要存取一個以上的使用者帳戶，請選擇此選項。 如果您的電子郵件提供者不支援加號定址，您必須為每個Workfront帳戶提供個別的電子郵件帳戶。

     例如，John Doe可以有一個使用者帳戶用於其日常使用帳戶，以及一個用於測試目的的使用帳戶：

      * johndoe@workfront.com
      * johndoe+reviewer@workfront.com

   * 將下列文字附加至電子郵件地址，將網域變更為使用偽網域：

     `.inactive`

     例如，John Doe可能有下列網域： （這些網域必須是唯一的。）

      * johndoe@workfront.inactive
      * johndoe@workfront.inactive2

     您無法再登入這些帳戶，因為密碼重設需要有效的電子郵件地址。 這些帳戶只能使用「登入身份」功能來存取。

   * 刪除不需要的使用者

     >[!IMPORTANT]
     >
     >只有錯誤建立的帳戶或測試帳戶才選擇此選項。 此選項通常僅針對登入錯誤為零或1的帳戶執行。 不應刪除已定期使用的帳戶。

如果您的Workfront執行個體中有使用者，其相符的電子郵件地址因大小寫而異，Workfront會在需要更新這些使用者時，提供其他資訊和時間表，與您連絡。
