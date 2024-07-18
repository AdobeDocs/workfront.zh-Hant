---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 「檢視：移除欄中物件的連結」
description: 依預設，您在檢視連結中顯示的某些物件會連結到物件的「詳細資訊」頁面。 例如，顯示專案名稱的欄是專案的連結；顯示使用者名稱的欄是使用者設定檔頁面的連結。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 08264437-f12d-43fa-8cb4-264806c6479b
source-git-commit: 5480d6b5e97c4c2e21080bb92ffe255f60ed6f60
workflow-type: tm+mt
source-wordcount: '442'
ht-degree: 0%

---

# 檢視：移除欄中物件的連結

依預設，您在檢視連結中顯示的某些物件會連結到物件的「詳細資訊」頁面。 例如，顯示專案名稱的欄是專案的連結；顯示使用者名稱的欄是使用者設定檔頁面的連結。

您可以使用在所有檢視中顯示的欄中的文字模式來移除此連結。

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

## 範例：從任務檢視的「任務名稱」欄中移除任務的連結：

1. 前往工作清單。
1. 從&#x200B;**檢視**&#x200B;下拉式功能表中，按一下&#x200B;**新增檢視**&#x200B;以建立新檢視。

   或

   按一下&#x200B;**編輯圖示** ![](assets/edit-icon.png)

   若要編輯現有檢視，請選取檢視。

1. 按一下&#x200B;**新增欄**&#x200B;以新增欄。

   或

   按一下具有物件連結的現有欄。

1. 按一下&#x200B;**切換到文字模式**。
1. 暫留在文字模式區域上，然後按一下&#x200B;**按一下以編輯文字**。
1. 移除您在&#x200B;**文字模式**&#x200B;方塊中找到的文字，並取代為下列程式碼：
   <pre>displayname=工作名稱<br>linkedname=direct<br>namekey=name<br>querysort=name<br>textmode=true<br><strong>valueexpression={name}</strong><br>valueformat=Compound</pre>

   >[!TIP]
   >
   >您可以調整下列內容，將類似的程式碼用於其他物件：
   >
   >* 將程式碼的&#x200B;**valuefield**&#x200B;行取代為&#x200B;**valueexpression**，並在等號後面保留包含在大括弧中的相同名稱。
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

1. 按一下&#x200B;**儲存**，然後按一下&#x200B;**儲存檢視**。
