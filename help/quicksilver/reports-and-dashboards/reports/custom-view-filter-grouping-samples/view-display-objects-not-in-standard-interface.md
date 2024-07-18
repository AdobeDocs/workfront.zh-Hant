---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 「檢視：顯示未包含在標準介面中的物件」
description: 您可以在檢視中顯示未包含在標準模式介面中的物件。 您只能透過文字模式來參照它們。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: c0138730-494b-4443-865a-44f8f00d5342
source-git-commit: bcafa607da733b89747f6b448dd295d9b906d060
workflow-type: tm+mt
source-wordcount: '492'
ht-degree: 0%

---

# 檢視：顯示未包含在標準介面中的物件

您可以在檢視中顯示未包含在標準模式介面中的物件。 您只能透過文字模式來參照它們。\
您可以透過下列其中一種方式來決定哪些欄位可以包含在檢視中：

* 使用[API Explorer](../../../wf-api/general/api-explorer.md)來探索可以透過文字模式參考的其他物件。\
  並非所有在API Explorer中記錄的欄位都是文字模式的有效欄位。 有些欄位只能透過API報告。

* 在欄中尋找物件的ID欄位。 大多數具有欄位ID的物件也有對應的欄或欄位名稱，可能無法透過標準模式介面存取。

  您可以使用文字模式將`fieldnameID`取代為`fieldname:name`，以在檢視中包含欄或欄位名稱而非ID。

  例如，在標準模式介面中，**Portfolio擁有者識別碼**&#x200B;欄位可用於專案檢視，但&#x200B;**Portfolio擁有者名稱**&#x200B;欄位則無法使用。 您可以使用文字模式，在檢視的欄中顯示&#x200B;**Portfolio擁有者名稱**。

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>請求修改檢視 </p>
   <p>計畫修改報表</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>編輯報告、儀表板、行事曆的存取權以修改報告</p> <p>編輯對篩選器、檢視、群組的存取權以修改檢視</p> <p><b>附註</b>

如果您還是沒有存取權，請詢問您的Workfront管理員，他們是否在您的存取層級中設定其他限制。 如需Workfront管理員如何修改存取層級的詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>。</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理報表的許可權</p> <p>如需請求其他存取權的資訊，請參閱<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求物件</a>的存取權。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的Workfront管理員。

## 範例：將「Portfolio擁有者名稱」欄新增至專案檢視

1. 前往專案清單。
1. 從&#x200B;**檢視**&#x200B;下拉式功能表，按一下&#x200B;**新增檢視**。

1. 按一下&#x200B;**新增欄**，然後在&#x200B;**顯示在此欄**&#x200B;欄位中開始輸入「Portfolio擁有者ID」，然後當它顯示在清單中時選取它。

1. 按一下&#x200B;**切換到文字模式**。
1. 暫留在文字模式區域上，然後按一下&#x200B;**按一下以編輯文字**。
1. 將`valuefield`行(`valuefield=portfolio:ownerID`)取代為下列行：

   ```
   valuefield=portfolio:owner:name
   ```

   或

   移除您在&#x200B;**文字模式**&#x200B;方塊中找到的文字，並取代為下列程式碼：

   ```
   valuefield=portfolio:owner:name
   querysort=portfolio:ownerID
   valueformat=HTML
   displayname=Portfolio Owner Name
   linkedname=portfolio
   ```

   在此特定範例中，報告會依Portfolio擁有者ID排序報告，如`querysort`行所示。

   >[!TIP]
   >
   >若要使用文字模式以欄位`name`取代任何欄位`ID`，請一律以`valuefield`行中的`:name`取代`ID`。

1. 按一下&#x200B;**儲存**，然後按一下&#x200B;**儲存檢視**。
