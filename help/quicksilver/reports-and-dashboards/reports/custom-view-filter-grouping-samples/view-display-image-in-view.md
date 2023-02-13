---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '''檢視：顯示影像，而非欄中的字串'
description: 可以使用文本模式將視圖中對象的名稱替換為影像。 您也可以新增連結至影像，以開啟其取代的物件。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: e1e4a993-f05c-4b6e-b00a-e96c9ab4c94f
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '499'
ht-degree: 0%

---

# 查看：在欄中顯示影像，而非字串

可以使用文本模式將視圖中對象的名稱替換為影像。 您也可以新增連結至影像，以開啟其取代的物件。

>[!NOTE]
>
>影像會以實際解析度顯示，因此請嘗試使用小型影像。

![](assets/replace-project-name-with-image-and-link-350x125.png)

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

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
   <td> <p>計劃 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯對報表、控制面板、日曆的存取</p> <p>編輯對篩選器、檢視、群組的存取</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>管理報表權限</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 範例：將專案檢視中的專案名稱取代為影像：

1. 上傳影像至Adobe Workfront外部的網站或伺服器。 您必須能夠使用網頁瀏覽器存取影像。

   >[!TIP]
   >
   >* 每種瀏覽器類型都不同，但都能顯示URL。
   >* 避免使用上傳至Workfront的影像。 由於儲存在Workfront中的影像無法公開使用，且具有一段時間後到期的存取金鑰，因此這些影像會隨著時間停止顯示在檢視中。
   >* 儲存在電腦上的影像沒有固有的URL。 尋找提供影像托管的網站，並將您的影像托管於該處。 您的組織可能已擁有此類網站。


1. 使用網頁瀏覽器，前往您儲存的影像。
1. 執行下列操作，取得影像的URL:

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: I used this blog post to document what kind of image we need for this: https://www.canto.com/blog/image-url/ (consulting uses this)) </p>
   -->

   1. 按一下滑鼠右鍵並選取 **複製影像位置**，或 **取得連結**，視您的瀏覽器而定。 您現在擁有該特定影像的URL，並可從剪貼簿貼上。
   1. 請確定每個具有該連結的人都有權僅前往連結檢視影像，而且不需要登入即可存取。

1. 前往專案，按一下 **更多** 功能表 ![](assets/more-icon-45x33.png) 在專案名稱旁，按一下 **編輯**.

1. 在 **URL** 欄位，將連結新增至影像。
1. 導覽至清單或報表中的專案檢視，然後自訂檢視。
1. 按一下 **專案名稱**，然後按一下 **切換到文本模式**.

1. 將下列程式碼新增至欄至現有程式碼：

   ```
   displayname=Link Project
   ```

   ```
   image.name=Link Project
   ```

   ```
   image.valuefield=URL
   ```

   ```
   link.linkproperty.0.name=projectID
   ```

   ```
   link.linkproperty.0.value=ID
   ```

   ```
   link.lookup=link.edit
   ```

   ```
   link.page=/view
   ```

   ```
   link.valuefield=objCode
   ```

   ```
   link.valueformat=val
   ```

   ```
   textmode=true
   ```

   ```
   type=image
   ```

   ```
   valueformat=
   ```

   您選取的影像會取代專案檢視中的「專案名稱」，且該影像為專案的連結。

1. 按一下 **保存視圖**.
