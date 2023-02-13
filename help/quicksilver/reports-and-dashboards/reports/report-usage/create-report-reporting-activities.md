---
product-area: reporting
keywords: 變更，擁有者，共用，報表，共用，執行，使用者，存取，權限，輸入，上次，檢視，日期，報表，活動
navigation-topic: report-usage
title: 建立報告活動的報告
description: 當您建立報表相關報表時，可以識別特定報表資訊，這些資訊可以包括如果報表已指派給停用的使用者、如果報表設定為以停用的使用者的存取權限執行、使用者正在存取您打算刪除的報表等。
author: Nolan
feature: Reports and Dashboards
exl-id: 3861ac81-d2e4-4dec-b9cd-96eee0b66a38
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '673'
ht-degree: 2%

---

# 建立報告活動的報告

當您建立報表相關報表時，可以識別特定報表資訊，這些資訊可以包括如果報表已指派給停用的使用者、如果報表設定為以停用的使用者的存取權限執行、使用者正在存取您打算刪除的報表等。

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

## 建立關於現有報表的報表 {#create-the-report-about-existing-reports}

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角。
1. 按一下 **報表**，然後 **新增報表**.
1. 在 **新增報表** 下拉菜單，選擇 **報表** 來建立現有報表。

1. 在 **欄（檢視）** 頁簽，在報表中新增您想要的欄。\
   下列部分欄位可能很實用：

   | 欄位 | 說明 |
   |---|---|
   | **以用戶身份運行：名稱** | 這是 **以下列權限運行此報告：** 欄位。 如果此使用者已停用，則不會針對共用該報表的任何使用者顯示報表。 |
   | **共用** | 這些是報告共用的所有實體。 |
   | **輸入者** | 這是報表的擁有者。 |
   | **上一次檢視日期** | 這是使用者上次檢視報表的日期和時間。 |

   {style=&quot;table-layout:auto&quot;}

1. （可選）若要將報表清單限制為特定停用的使用者：

   1. 選取 **篩選器** ，然後按一下 **新增篩選規則**.

   1. 新增篩選 **以用戶ID的身份運行** > **等於**.

   1. 輸入您要新增至篩選器的停用使用者名稱，然後在名稱顯示於清單時按一下。
   1. 重複步驟C，直到您選取了要納入報表的所有停用使用者為止。

1. （選用）若要將報表清單限制為排程報表：

   1. 選取 **篩選器** ，然後按一下 **新增篩選規則**.

   1. 新增篩選 **排程報表ID** > **非空白**.

1. 按一下 **儲存+關閉**，然後輸入報表的名稱，然後按一下 **儲存報表**.

   您的報表資訊隨即顯示。

1. （選用）將此報表匯出至Excel並儲存在您的電腦上。\
   如需匯出報表的詳細資訊，請參閱 [匯出資料](../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).

## 更新報表的相關資訊

建立報表後，您就可以視需要更新報表。

1. 前往您要更新的報表。
1. 視您要採取的動作而定，執行下列其中一項操作：

   * 更新 **以下列權限運行此報告：** 欄位至作用中使用者：如需詳細資訊，請參閱 [使用其他使用者的存取權限執行並傳送報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md).

   * 建立報表復本：如需詳細資訊，請參閱 [建立報表副本](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).
   * 刪除報表：如需詳細資訊，請參閱 [建立報表的精確副本](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md#update2) 文章一節 [建立報表副本](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).

   * 共用報表：如需詳細資訊，請參閱 [在Adobe Workfront中共用報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md).

1. （條件性）如果您複製原始報表，請使用您在中建立之報表的資訊 [建立關於現有報表的報表](#create-the-report-about-existing-reports) 將新副本與原始報表的實體共用。
