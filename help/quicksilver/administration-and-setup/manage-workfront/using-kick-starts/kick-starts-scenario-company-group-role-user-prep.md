---
user-type: administrator
product-area: system-administration;user-management
keywords: kickstart，kick-start，kickstart，kick-start
navigation-topic: use-kick-starts
title: Kick-Start情境：公司、群組、角色和使用者Kick-Start準備
description: 開始實作Adobe Workfront時，您可以匯入客戶清單、內部部門、職位角色和使用者資訊，而不是手動輸入資料。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: b83e2e35-dd9d-4d98-b8d4-2f8718b3c6c1
source-git-commit: 612243e928c6053d9b02715d9fcfef4dae25cb7a
workflow-type: tm+mt
source-wordcount: '1150'
ht-degree: 2%

---

# Kick-Starts情境：公司、群組、角色和使用者Kick-Starts準備

開始實作Adobe Workfront時，您可以匯入客戶清單、內部部門、職位角色和使用者資訊，而不是手動輸入資料。

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
   <td role="rowheader">Adobe Workfront授權</td> 
   <td>
   <p> 新增：標準</p>
   或
   <p>目前：計畫</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td>[！UICONTROL系統管理員]</td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 您可以匯入的內容

下表顯示要匯入的公司、群組和角色：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>公司</strong> </th> 
   <th><strong>群組</strong> </th> 
   <th><strong>角色</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td valign="top"> <p>Acme， Co</p> <p>Workfront公司</p> <p><em>您的公司</em> </p> <p>XYZ， Inc.</p> </td> 
   <td valign="top"> <p valign="top" rowspan="7">財務</p> <p valign="top" rowspan="7">IT </p> <p valign="top" rowspan="7">行銷 </p> <p valign="top" rowspan="7">銷售額</p> </td> 
   <td valign="top"> <p valign="top">業務分析師</p> <p valign="top">Controller Creative</p> <p valign="top">設計師</p> <p valign="top">資源管理員</p> <p valign="top">Scrum Master</p> <p valign="top">技術撰稿人</p> <p valign="top">Web開發人員</p> </td> 
  </tr> 
 </tbody> 
</table>

角色名稱必須是唯一的。 無法匯入現有職位角色。

下表顯示要匯入的使用者以及每個使用者的數個使用者屬性：

### 使用者1

| **名字** | Chris |
|---|---|
| **姓氏** | 人員管理 |
| **使用者名稱/電子郵件** | mailto:cmanning@foo.com |
| **密碼** | 更新我 |
| **存取** | 小組成員 |
| **公司** | &lt;*您的公司>* |
| **主群組** | 行銷 |
| **工作角色** | 業務分析師 |

{style="table-layout:auto"}

### 使用者2

| **名字** | Jennifer |
|---|---|
| **姓氏** | 坎貝爾 |
| **使用者名稱/電子郵件** | jcampbell@foo.com |
| **密碼** | 更新我 |
| **存取** | 專案經理 |
| **公司** | &lt;*您的公司>* |
| **主群組** | 行銷 |
| **工作角色** | 專案經理 |

{style="table-layout:auto"}

### 使用者3

| **名字** | 吉爾 |
|---|---|
| **姓氏** | 沙利文 |
| **使用者名稱/電子郵件** | jsullivan@foo.com |
| **密碼** | 更新我 |
| **存取** | 服務台 |
| **公司** | &lt;*您的公司>* |
| **主群組** | 銷售額 |
| **工作角色** | 銷售代表 |

{style="table-layout:auto"}

### 使用者4

| **名字** | 馬克 |
|---|---|
| **姓氏** | Lewis |
| **使用者名稱/電子郵件** | mlewis@foo.com |
| **密碼** | 更新我 |
| **存取** | 投資組合經理 |
| **公司** | &lt;*您的公司>* |
| **主群組** | 財務 |
| **工作角色** | 控制器 |

{style="table-layout:auto"}

### 使用者5

| **名字** | Pam |
|---|---|
| **姓氏** | Reynolds |
| **使用者名稱/電子郵件** | preynolds@foo.com |
| **密碼** | 更新我 |
| **存取** | 專案經理 |
| **公司** | *您的公司>* |
| **主群組** | 行銷 |
| **工作角色** | IT |

{style="table-layout:auto"}

### 使用者6

| **名字** | Ray |
|---|---|
| **姓氏** | Andrews |
| **使用者名稱/電子郵件** | randrews@foo.com |
| **密碼** | 更新我 |
| **存取** | 管理員 |
| **公司** | *您的公司>* |
| **主群組** | 資源管理員 |
| **工作角色** | 無 |

{style="table-layout:auto"}

## 下載Kick-Start范

{{step-1-to-setup}}

1. 按一下&#x200B;**系統** > **Kick-Starts** > **匯入資料。**

1. 按一下&#x200B;**其他選項**&#x200B;檢視匯入選項的完整清單。
1. 選取您要匯入的存取層級、公司、群組、工作角色和使用者物件。

## 輸入公司資訊

1. 開啟您剛下載的&#x200B;**Workfront.xlsx**&#x200B;檔案。

   >[!TIP]
   >
   >使用非常寬的資料表時，您可能想要使用試算表編輯器的「凍結窗格」（或同等功能）工具，讓試算表更易於使用。

1. 前往「公司」表。

   除非系統中已有公司，否則應留空。 ![公司工作表](assets/cmpysheet-350x16.png)

   ![公司ID](assets/companyid--1--350x78.png)

1. 在&#x200B;**isNew**&#x200B;資料行中指定TRUE。
1. 對每個要新增的公司重複此動作。 （在此範例中，請針對列3-6完成此動作，因為將新增4家公司）。

   ![公司是新的](assets/cmpyisnew-350x86.png)

1. 指定唯一識別碼。

   您必須針對ID欄的每一列執行此作業。 建立新記錄時，從1開始的整數可正常運作。

   ![公司是新的](assets/cmpyisnew-350x86.png)

1. 設定名稱。

   在&#x200B;**setName**&#x200B;欄中指定每個客戶的名稱。

   ![公司ID](assets/companyid-350x78.png)

1. 移至「群組」工作表。

   除非您已在Workfront中建立群組，否則此工作表應該僅顯示與Workfront的每個帳戶布建的「預設群組」。

   ![群組工作表](assets/groupsheet-350x15.png) ![空白群組工作表](assets/emptygroupsheet-350x85.png)

1. 設定&#x200B;**isNew**&#x200B;欄。根據情境，將匯入4個群組，因此請為&#39;isNew&#39;欄的第4到7列指定TRUE。
1. 指定唯一識別碼。

   您必須針對ID欄的每一列執行此作業。 建立新記錄時，從1開始的整數可正常運作。

   ![群組ID](assets/groupids-350x85.png)

1. 設定名稱。

   指定&#x200B;**setName**&#x200B;欄中每個部門的名稱。

   ![群組名稱](assets/groupnames-350x85.png)

   指定角色資訊。 前往「角色」角色表。

1. 除非您已建立或刪除帳戶中的角色，否則此工作表應顯示8個已布建每個Workfront帳戶的角色。

   ![群組名稱](assets/groupnames-350x85.png)

1. 設定True陳述式。

   正在匯入7個工作角色，在「isNew」欄的列12到18中輸入TRUE。

   ![角色是新的](assets/roleisnew-350x104.png)

1. 指定唯一識別碼。

   您必須針對ID欄的每一列執行此作業。 建立新記錄時，從1開始的整數可正常運作。

   ![使用者工作表](assets/usersheet-350x16.png)

   ![角色是新的](assets/roleisnew--1--350x104.png)

1. 在setName欄中鍵入每個角色的名稱。

   ![角色是新的](assets/roleisnew-350x104.png)

1. 視需要提供其他詳細資訊。

   視需要包含您正在建立之角色的收費率、成本費率和說明。

1. 移至「使用者」工作表以輸入使用者資訊。

   除非您已在您的帳戶中建立使用者，否則本工作表應該僅顯示已布建每個Workfront帳戶的「管理員使用者」。

   ![角色名稱](assets/rolenames-350x104.png) ![空白的使用者工作表](assets/emptyusersheet-350x52.png)

1. 在&#39;isNew&#39;欄的列4到列9中指定TRUE，設定True值，因為有6個使用者正在匯入。

   ![使用者是新使用者](assets/userisnew-350x52.png)

1. 在ID欄的每一列中指定唯一ID，以設定唯一ID。 通常從1開始的整數對於新記錄來說很有效。

   ![使用者是新使用者](assets/userisnew-350x52.png)

1. 在&#39;setFirstName&#39;和&#39;setLastName&#39;欄中輸入每個使用者的名稱。

   ![使用者名稱](assets/usernames-350x52.png)

1. 在「setEmail」、「setPassword」和「setUsername」欄中指定值，以設定詳細值。

   ![使用者認證](assets/usercredentials-350x52.png)

1. 指定存取層級值。

   例如，團隊成員Chris Manning會在「ACSLVL存取層級」表上查詢「團隊成員」存取層級的ID。 將ID複製到剪貼簿，然後在[使用者使用者]工作表中貼到Chris&#39;列上的&#x200B;**setAccessLevelID**&#x200B;欄。

   對每個使用者和存取層級重複此步驟。

   ![複製存取層級ID](assets/copyalid-350x171.png) ![貼上存取層級ID](assets/pastealid-350x59.png)

1. 指定主群組詳細資料。

   根據情境，Chris Manning屬於行銷群組。 在「群組群組」工作表上，找到「行銷」群組的ID，將其複製到剪貼簿，然後在「使用者」工作表上將其貼到Chris列上的&#x200B;**setHomeGroupID**&#x200B;欄。&#x200B;URL對每個使用者和群組指派重複此步驟。

   ![複製群組識別碼](assets/copygroupid-1-350x133.png) ![貼上群組識別碼](assets/pastegroupid-350x59.png)

1. 指定公司詳細資料。

   此情境中的所有使用者都屬於相同公司。 在CMPY公司工作表上，找到*Your Own Company *company的ID，將ID複製到剪貼簿，然後在「使用者」索引標籤上，將此值貼到「setCompanyID」欄的每一列&#x200B;。

   對每個使用者和群組指派重複此步驟。

   ![公司ID](assets/companyid--1--350x78.png)

   ![貼上公司ID](assets/pastecompanyid-350x84.png)

1. 指定工作角色詳細資訊。

   根據情況，Chris Manning將擔任Business Analyst角色。 在「角色角色」工作表上，找到「業務分析員」角色的ID，將其複製到剪貼簿，然後在「使用者」工作表上，將其貼到Chris列上的「setRoleID」欄。&#x200B;URL對每個使用者和群組指派重複此步驟。

   ![複製角色ID](assets/copyroleid-350x149.png)

   ![貼上角色ID](assets/pasteroleid-350x95.png)

1. 視需要填寫其他使用者詳細資訊，然後儲存檔案。
1. 匯入Excel檔案。

   遵循[使用Kick-Start範本將資料匯入Adobe Workfront](/help/quicksilver/administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md)中提供的指示。
