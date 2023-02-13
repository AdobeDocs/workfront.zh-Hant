---
product-area: reporting
navigation-topic: other-blocks
title: 在報表畫布中新增或編輯網頁內容區塊
description: 網頁內容區塊可讓您直接在報表中顯示外部網站的資訊。
author: Nolan
feature: Reports and Dashboards
exl-id: 29f0c2e1-1644-4989-81b1-c6db6bfec905
source-git-commit: 61fcb4c3646f60fa5f667d874af3320360d5d286
workflow-type: tm+mt
source-wordcount: '323'
ht-degree: 2%

---


# 在報表畫布中新增或編輯網頁內容區塊

網頁內容區塊可讓您直接在報表中顯示外部網站的資訊。

## 必要條件

開始之前，您必須註冊「報表畫布測試版」。 如需詳細資訊，請參閱 [報表畫布測試版：概述](/help/quicksilver/product-announcements/betas/reporting-canvas-beta/reporting-canvas-beta-overview.md).

## 新增或編輯網頁內容區塊

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下&#x200B;**報表**.
1. 按一下 **新報表**.

   或

   前往現有報表，按一下 **更多** 圖示 ![](assets/more-icon-27x15.png) 在報表標題中，按一下 **編輯**.

1. 在螢幕的右側，在 **新增區塊**，其中之一：

   拖曳 **網頁內容** 圖示直接顯示到您想要的位置。

   或

   按兩下 **網頁內容** 圖示將區塊新增至畫布頂端。

   >[!TIP]
   >
   >通過拖動塊的拐角控點，可以在放置塊後更改塊的大小。

1. 按一下 **無標題網頁內容** 在區塊標題中，輸入區塊的標題。
1. 按一下 **編輯** 圖示 ![](assets/edit-icon.png) 在區塊標題中。

   ![](assets/web-content-block-header-350x76.png)

1. 在 **設定** 開啟的面板中，輸入您要在中顯示之頁面的完整URL(包括「https://」) **URL** 欄位。

   >[!NOTE]
   >
   >目前，只能顯示選取網域的網站。 目前可使用的網域包括：
   >   
   >   * workfront.com
   >   * google.com
   >   * sharepoint.com
   >   * attask-ondemand.om
   >   * powerbi.com
   >   * domo.com
   >   * looker.com


   如果您輸入的URL無法內嵌，其下方會顯示警告。 這些警告包括：

   | 警告名稱 | 原因 |
   |---|---|
   | 無效的 URL | 輸入的URL未傳回有效的網站。 |
   | 提供程式站點限制 | 您嘗試內嵌的網站不允許。 |

   {style=&quot;table-layout:auto&quot;}

1. （選用）按一下 **傳遞參數** 切換以開啟可用傳遞參數清單。

   >[!WARNING]
   >
   >傳遞參數當前已禁用。

1. 按一下 **內嵌URL** 以儲存您的選取項目並返回報表。
