---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 檢視：移除欄中物件的連結
description: 依預設，您在檢視連結中顯示的某些物件會連結到物件的「詳細資訊」頁面。 例如，顯示專案名稱的欄是專案的連結；顯示使用者名稱的欄是使用者設定檔頁面的連結。
author: Nolan
feature: Reports and Dashboards
exl-id: 08264437-f12d-43fa-8cb4-264806c6479b
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '371'
ht-degree: 0%

---

# 檢視：移除欄中物件的連結

<!--Audited: 11/2024-->

依預設，您在檢視連結中顯示的某些物件會連結到物件的「詳細資訊」頁面。 例如，顯示專案名稱的欄是專案的連結；顯示使用者名稱的欄是使用者設定檔頁面的連結。

您可以使用在所有檢視中顯示的欄中的文字模式來移除此連結。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront套件</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td> 
   <p>投稿人或請求修改檢視 </p>
   <p>要修改報告的標準或計畫</p>
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>編輯報告、儀表板、行事曆的存取權以修改報告</p> <p>編輯對篩選器、檢視、群組的存取權以修改檢視</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理報表的許可權</p>  </td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。


+++


## 範例：從任務檢視的「任務名稱」欄中移除任務的連結：

1. 前往工作清單。
1. 從&#x200B;**檢視**&#x200B;下拉式功能表中，按一下&#x200B;**新增檢視**&#x200B;以建立新檢視。

   或

   按一下「**編輯」圖示**「![編輯」圖示](assets/edit-icon.png)以編輯現有的檢視，然後選取檢視。

1. 按一下&#x200B;**新增欄**&#x200B;以新增欄。

   或

   按一下具有物件連結的現有欄。

1. 按一下&#x200B;**切換到文字模式** > **編輯文字模式**。
1. 移除您在&#x200B;**編輯文字模式**&#x200B;方塊中找到的文字，並取代為下列程式碼：

   ```
   displayname=Task Name
   linkedname=direct
   namekey=name
   querysort=name
   textmode=true
   valueexpression={name}
   valueformat=Compound
   ```

   >[!TIP]
   >
   >您可以調整下列內容，將類似的程式碼用於其他物件：
   >
   >* 將程式碼的`valuefield`行取代為`valueexpression`，並在等號後面保留包含在大括弧中的相同名稱。
   >* 從欄的原始文字中排除所有以`link.`開頭的行。 例如，取消下列所有行：
   >
   >  ```
   >  link.linkproperty.0.name=ID
   >  link.linkproperty.0.valuefield=ID
   >  link.linkproperty.0.valueformat=string
   >  link.lookup=link.view
   >  link.value=val(objCode)
   >  ```
   >

1. 按一下&#x200B;**完成**，然後按一下&#x200B;**儲存檢視**。

