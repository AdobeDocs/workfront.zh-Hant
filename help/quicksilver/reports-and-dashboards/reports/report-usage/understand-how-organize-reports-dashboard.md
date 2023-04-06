---
content-type: overview
product-area: reporting;dashboards
navigation-topic: report-usage
title: 了解如何在控制面板上組織報表
description: 您可以查看報表是否已新增至Adobe Workfront中的控制面板。 這在決定可以保留哪些報表以及可以從系統中刪除哪些報表時可能很有用。 如果報表位於控制面板上，則使用者仍可能依賴這些報表。 建議您不要刪除列在使用者使用之控制面板上的報表。 如需新增報表至控制面板的詳細資訊，請參閱新增報表至控制面板一文。
author: Nolan
feature: Reports and Dashboards
exl-id: ce00c307-9e64-49f5-997b-f7fc461c960c
source-git-commit: d738ef3f6642d5b1a646f58896575a2971bbc06a
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# 了解如何在控制面板上組織報表

## 存取報表清單中的控制面板資訊

您可以查看報表是否已新增至Adobe Workfront中的控制面板。 這在決定可以保留哪些報表以及可以從系統中刪除哪些報表時可能很有用。 如果報表位於控制面板上，則使用者仍可能依賴這些報表。 建議您不要刪除列在使用者使用之控制面板上的報表。\
如需將報表新增至控制面板的詳細資訊，請參閱文章 [新增報表至控制面板](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/add-report-dashboard.md).

您可以執行下列其中一項操作，查看報表是否已新增至控制面板：

* 建立報表清單的檢視，並在欄中加入控制面板資訊
* 依您知道目前正在使用的一或多個特定控制面板，篩選報表清單
* 建立報表物件的報表，並使用包含控制面板資訊的檢視或篩選器

任何人都可以建立檢視或篩選，但您必須在存取層級中擁有「編輯」報表存取權，才能建立報表。\
如需存取報表的詳細資訊，請參閱文章 [授予對報表、控制面板和日曆的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).\
如需建立報表的詳細資訊，請參閱文章 [建立自訂報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

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

## 在報表清單的檢視中顯示控制面板資訊

>[!WARNING]
>
>在報表清單中加入控制面板欄可大幅增載入入時間，尤其是長報表清單。

要為報表清單建立包含儀表板資訊的視圖，請執行以下操作：

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Workfront的右上角，然後按一下 **報表**.
1. 在報表清單上，按一下 **檢視** 下拉式功能表。
1. 按一下 **新建視圖**.
1. 按一下 **添加列**.
1. 開始在 **開始鍵入欄位名稱** 欄位。
1. 在 **報表** 對象，選擇 **控制面板**.

1. 按一下 **保存視圖**.\
   報表顯示的控制面板會顯示在報表清單的「控制面板」欄中。\
   ![](assets/qs-dashboards-in-report-view.png)

## 依控制面板資訊篩選報表清單

若要依控制面板資訊篩選報表清單：

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Workfront的右上角，然後按一下 **報表**.

1. 在報表清單上，按一下 **篩選** 下拉式功能表。
1. 按一下 **新增篩選**，然後按一下 **新增篩選規則**.

1. 開始在 **開始鍵入欄位名稱** 欄位。

1. 在 **控制面板** 對象，選擇 **名稱**.

1. 選擇 **等於** 在修飾詞下拉式功能表中，然後開始輸入您要篩選依據的控制面板名稱。 您可以為篩選器選取多個控制面板。\
   ![](assets/qs-dashboards-in-report-filters-350x143.png)

1. 按一下 **儲存+關閉**.\
   這會顯示僅在指定控制面板上列出的報表清單。\
   您也可以建立報表物件的報表，並在報表中使用此篩選器。
