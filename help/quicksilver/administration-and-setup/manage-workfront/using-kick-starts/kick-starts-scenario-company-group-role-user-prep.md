---
user-type: administrator
product-area: system-administration;user-management
keywords: kickstart,kickstart,kickstarts,kickstarts
navigation-topic: use-kick-starts
title: 『啟動情況：公司、組、角色和用戶啟動準備
description: 開始實作Adobe Workfront時，您可以匯入客戶清單、內部部門、工作角色和使用者資訊，而不是手動輸入資料。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: b83e2e35-dd9d-4d98-b8d4-2f8718b3c6c1
source-git-commit: 5d36c2c959dbfd00920eaf0a16409102b99de042
workflow-type: tm+mt
source-wordcount: '1103'
ht-degree: 10%

---

# 啟動方案：公司、組、角色和用戶啟動準備

開始實作Adobe Workfront時，您可以匯入客戶清單、內部部門、工作角色和使用者資訊，而不是手動輸入資料。

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

## 可匯入的項目

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
   <td valign="top"> <p>Acme, Co</p> <p>Workfront公司</p> <p><em>貴公司</em> </p> <p>XYZ, Inc.</p> </td> 
   <td valign="top"> <p valign="top" rowspan="7">財務</p> <p valign="top" rowspan="7">IT </p> <p valign="top" rowspan="7">行銷 </p> <p valign="top" rowspan="7">銷售</p> </td> 
   <td valign="top"> <p valign="top">業務分析人員</p> <p valign="top">控制器創意</p> <p valign="top">設計者</p> <p valign="top">資源管理員</p> <p valign="top">Scrum主版</p> <p valign="top">技術撰稿人</p> <p valign="top">網頁開發人員</p> </td> 
  </tr> 
 </tbody> 
</table>

角色名稱必須是唯一的，不能導入現有作業角色。

下表顯示要匯入的使用者，以及每個使用者的數個使用者屬性：

### 使用者1

| **名字** | 克里斯 |
|---|---|
| **姓氏** | 曼寧 |
| **使用者名稱/電子郵件** | mailto:cmanning@foo.com |
| **密碼** | updateMe |
| **存取** | 小組成員 |
| **公司** | &lt;*你的公司>* |
| **主群組** | 行銷 |
| **職務角色** | 業務分析人員 |

{style=&quot;table-layout:auto&quot;}

### 使用者2

| **名字** | 珍妮弗 |
|---|---|
| **姓氏** | 坎貝爾 |
| **使用者名稱/電子郵件** | jcampbell@foo.com |
| **密碼** | updateMe |
| **存取** | 專案經理 |
| **公司** | &lt;*你的公司>* |
| **主群組** | 行銷 |
| **職務角色** | 專案經理 |

{style=&quot;table-layout:auto&quot;}

### 使用者3

| **名字** | 吉爾 |
|---|---|
| **姓氏** | 沙利文 |
| **使用者名稱/電子郵件** | jsullivan@foo.com |
| **密碼** | updateMe |
| **存取** | 服務台 |
| **公司** | &lt;*你的公司>* |
| **主群組** | 銷售 |
| **職務角色** | 銷售代表 |

{style=&quot;table-layout:auto&quot;}

### User 4

| **名字** | 馬克 |
|---|---|
| **姓氏** | 路易斯 |
| **使用者名稱/電子郵件** | mlewis@foo.com |
| **密碼** | updateMe |
| **存取** | 投資組合經理 |
| **公司** | &lt;*你的公司>* |
| **主群組** | 財務 |
| **職務角色** | 控制器 |

{style=&quot;table-layout:auto&quot;}

### 使用者5

| **名字** | 帕姆 |
|---|---|
| **姓氏** | 雷諾 |
| **使用者名稱/電子郵件** | preynolds@foo.com |
| **密碼** | updateMe |
| **存取** | 專案經理 |
| **公司** | *你的公司>* |
| **主群組** | 行銷 |
| **職務角色** | IT |

{style=&quot;table-layout:auto&quot;}

### 使用者6

| **名字** | 雷 |
|---|---|
| **姓氏** | 安德魯斯 |
| **使用者名稱/電子郵件** | randrews@foo.com |
| **密碼** | updateMe |
| **存取** | 管理員 |
| **公司** | *你的公司>* |
| **主群組** | 資源管理員 |
| **職務角色** | 無 |

{style=&quot;table-layout:auto&quot;}

## 下載啟動範本

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **設定** ![](assets/gear-icon-settings.png).

1. 按一下 **系統** > **開始** > **匯入資料。**

1. 按一下 **更多選項** 以查看匯入選項的完整清單。
1. 選擇要導入的訪問級別、公司、組、作業角色和用戶對象。

## 輸入公司資訊

1. 開啟 **Workfront.xlsx** 檔案。

   >[!TIP]
   >
   >使用非常寬的資料表時，您可能會想使用試算表編輯器的「凍結窗格」（或同等工具）工具，讓試算表更容易使用。

1. 轉至「CMPY公司」表。

   除非公司已在系統中，否則應為空。 ![](assets/cmpysheet-350x16.png)

   ![](assets/companyid--1--350x78.png)

1. 在 **isNew** 欄。
1. 對每個要新增的公司重複此動作。 （在此範例中，針對第3到6列完成此動作，因為有四家公司正在新增。）

   ![](assets/cmpyisnew-350x86.png)

1. 指定唯一ID。

   必須對ID欄的每一列執行此動作。 從1開始的整數在建立新記錄時很有效。

   ![](assets/cmpyisnew-350x86.png)

1. 設定名稱。

   指定 **setName** 欄。

   ![](assets/companyid-350x78.png)

1. 轉到「組組」表。

   除非您已在Workfront中建立群組，否則此工作表應僅顯示已布建每個Workfront帳戶的預設群組。

   ![](assets/groupsheet-350x15.png) ![](assets/emptygroupsheet-350x85.png)

1. 設定 **isNew** column.根據情況，將導入4個組，因此請為「isNew」列將TRUE指定到第4到第7行。
1. 指定唯一ID。

   必須對ID欄的每一列執行此動作。 從1開始的整數在建立新記錄時很有效。

   ![](assets/groupids-350x85.png)

1. 設定名稱。

   指定 **setName** 欄。

   ![](assets/groupnames-350x85.png)

   指定角色資訊。 轉到「角色」(ROLE)「角色」(Role)工作表。

1. 除非您已在帳戶中建立或刪除角色，否則此工作表應顯示8個已隨Workfront每個帳戶布建的角色。

   ![](assets/groupnames-350x85.png)

1. 設定True語句。

   正在匯入7個工作角色，請針對「isNew」欄將TRUE輸入第12到第18行。

   ![](assets/roleisnew-350x104.png)

1. 指定唯一ID。

   必須對ID欄的每一列執行此動作。 從1開始的整數在建立新記錄時很有效。

   ![](assets/usersheet-350x16.png)

   ![](assets/roleisnew--1--350x104.png)

1. 在setName欄中輸入每個角色的名稱。

   ![](assets/roleisnew-350x104.png)

1. 視需要提供其他詳細資訊。

   包括您正在建立的職責的開單費率、成本費率和說明（視需要）。

1. 轉到「用戶」(USER)用戶表以輸入用戶資訊。

   除非您已在帳戶中建立使用者，否則此工作表應僅顯示已布建每個Workfront帳戶的管理員使用者。

   ![](assets/rolenames-350x104.png) ![](assets/emptyusersheet-350x52.png)

1. 將「isNew」列的第4到第9行指定TRUE，以設定True值，因為正在導入6個用戶。

   ![](assets/userisnew-350x52.png)

1. 在ID欄的每一列中指定唯一ID，以設定唯一ID。 通常，從1開始的整數對於新記錄非常有效。

   ![](assets/userisnew-350x52.png)

1. 將每個用戶的名稱輸入到「setFirstName」和「setLastName」列中。

   ![](assets/usernames-350x52.png)

1. 通過在「setEmail」、「setPassword」和「setUsername」列中指定值來設定詳細值。

   ![](assets/usercredentials-350x52.png)

1. 指定訪問級別值。

   例如，Chris Manning是團隊成員，在「ACSLVL訪問級別」工作表上查找「團隊成員訪問級別」的ID。 將ID複製到剪貼簿中，然後在「使用者」工作表上貼到 **setAccessLevelID** 克里斯的專欄。

   對每個使用者和存取層級重複此步驟。

   ![](assets/copyalid-350x171.png) ![](assets/pastealid-350x59.png)

1. 指定首頁組詳細資訊。

   根據情景，克里斯·曼寧屬於市場部。 在「群組」工作表中，找出行銷群組的ID，將其複製到剪貼簿中，然後在「使用者」工作表上將其貼到 **setHomeGroupID**&#x200B;克里斯的專欄。&#x200B;對每個用戶和組分配重複此步驟。

   ![](assets/copygroupid-1-350x133.png) ![](assets/pastegroupid-350x59.png)

1. 指定公司詳細資訊。

   此情境中的所有使用者都屬於同一家公司。 在「CMPY公司」工作表中，找出*您自己的公司*公司的ID，將該ID複製到剪貼簿中，然後在「USER User」（用戶）頁簽中，將此值貼到「setCompanyID」列的每&#x200B;行中。

   對每個用戶和組分配重複此步驟。

   ![](assets/companyid--1--350x78.png)

   ![](assets/pastecompanyid-350x84.png)

1. 指定作業角色詳細資訊。

   根據情景，克里斯·曼寧將擔任商業分析師。 在「角色」表中，找到業務分析員角色的ID，將其複製到剪貼簿中，然後在「用戶」表中，將其貼到Chris行的「setRoleID」列中。&#x200B;對每個用戶和組分配重複此步驟。

   ![](assets/copyroleid-350x149.png)

   ![](assets/pasteroleid-350x95.png)

1. 視需要填入其他使用者詳細資訊，然後儲存檔案。
1. 匯入Excel檔案。

   遵循 **導入Kick Start檔案** 本文的一節。
