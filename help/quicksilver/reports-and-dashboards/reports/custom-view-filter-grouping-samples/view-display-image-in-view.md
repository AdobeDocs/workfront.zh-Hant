---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 檢視：在欄中顯示影像而非字串
description: 您可以使用文字模式將檢視中的物件名稱取代為影像。 您也可以將連結新增至影像，以開啟其取代的物件。
author: Nolan
feature: Reports and Dashboards
exl-id: e1e4a993-f05c-4b6e-b00a-e96c9ab4c94f
source-git-commit: ecce7484423419823effa2cb41da892ba3fb207c
workflow-type: tm+mt
source-wordcount: '488'
ht-degree: 0%

---

# 檢視：在欄中顯示影像而非字串

<!--Audited: 11/2024-->

您可以使用文字模式將檢視中的物件名稱取代為影像。 您也可以將連結新增至影像，以開啟其取代的物件。

>[!NOTE]
>
>影像會以實際解析度顯示，因此請嘗試使用小型影像。

![](assets/replace-project-name-with-image-and-link-350x125.png)

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> 
    <p>新增：</p>
   <ul><li><p>修改篩選器的貢獻者 </p></li>
   <li><p>用於修改報告的標準</p></li> </ul>

<p>目前：</p>
   <ul><li><p>請求修改篩選器 </p></li>
   <li><p>計畫修改報表</p></li> </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>編輯報告、儀表板、行事曆的存取權以修改報告</p> <p>編輯篩選器、檢視和群組的存取權以修改篩選器</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理報表的許可權</p>  </td> 
  </tr> 
 </tbody> 
</table>

*如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 範例：將專案檢視中的專案名稱取代為影像：

1. 將影像上傳至Adobe Workfront外部的網站或伺服器。 您必須能夠使用網頁瀏覽器存取影像。

   >[!TIP]
   >
   >* 每種瀏覽器型別不同，但都能顯示URL。
   >* 避免使用上傳至Workfront的影像。 由於儲存在Workfront中的影像無法公開使用，且存取金鑰經過一段時間後過期，因此這些影像會隨著時間停止顯示在檢視中。
   >* 儲存在您電腦上的影像沒有固有的URL。 尋找提供影像託管的網站，並將您的影像託管在那裡。 您的組織可能已經擁有這類網站。

1. 使用您的網頁瀏覽器，前往您儲存的影像。
1. 請執行以下動作來取得影像的URL：

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: I used this blog post to document what kind of image we need for this: https://www.canto.com/blog/image-url/ (consulting uses this)) </p>
   -->

   1. 按一下滑鼠右鍵並選取&#x200B;**複製影像位置**，或&#x200B;**取得連結**（視您的瀏覽器而定）。 您現在擁有該特定影像的URL，並可從剪貼簿中貼上。
   1. 確保具有該連結的每個人只要前往該連結，就能擁有檢視影像的許可權，而且他們不需要登入即可存取該連結。

1. 前往專案，按一下專案名稱旁的&#x200B;**更多**&#x200B;功能表![](assets/more-icon-45x33.png)，然後按一下&#x200B;**編輯**。

1. 在&#x200B;**URL**&#x200B;欄位中，新增影像的連結。
1. 前往專案清單中的專案檢視。
1. 按一下&#x200B;**檢視**&#x200B;下拉式功能表，然後按一下&#x200B;**新增檢視**。
1. 按一下&#x200B;**專案名稱**&#x200B;的資料行標題，然後按一下&#x200B;**切換至文字模式**。

1. 將下列程式碼新增至欄中的現有程式碼：

   ```
   displayname=Link Project
   image.name=Link Project
   image.valuefield=URL
   link.linkproperty.0.name=projectID
   link.linkproperty.0.value=ID
   link.lookup=link.edit
   link.page=/view
   link.valuefield=objCode
   link.valueformat=val
   textmode=true
   type=image
   valueformat=
   ```

1. 按一下&#x200B;**完成** > **儲存檢視**。
您選取的影像會取代專案檢視中的「專案名稱」，而且該影像是專案的連結。