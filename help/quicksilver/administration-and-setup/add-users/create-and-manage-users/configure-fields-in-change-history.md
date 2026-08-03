---
user-type: administrator
product-area: system-administration;setup
title: 設定要在變更記錄中追蹤的欄位
description: 身為Workfront管理員，您可以設定Workfront追蹤的物件欄位和動作。
author: Lisa
feature: System Setup and Administration
role: Admin
source-git-commit: 71bd341da0b506429ab25726ae3be82829034f9f
workflow-type: tm+mt
source-wordcount: '435'
ht-degree: 6%

---

# 設定要在變更記錄中追蹤的欄位

{{highlighted-preview-article-level}}

Adobe Workfront會產生自動系統更新，以記錄下列事件：

* 使用者在物件欄位中所做的變更
* 使用者對物件執行的動作

這些系統更新包含下列型別的資訊：

* 已進行的變更
* 進行變更的使用者名稱
* 變更的時間和日期

身為Workfront管理員，您可以設定Workfront追蹤的物件欄位和動作。

例如，您可以讓Workfront追蹤使用者對整個系統中的問題名稱所做的所有變更。 然後，任何問題名稱變更都會作為專案出現在變更記錄日誌中。 如需詳細資訊，請參閱[檢視及管理變更記錄](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/view-and-manage-change-history.md)。

## 存取權要求

+++ 展開以檢視這篇文章中所述功能的存取權要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] 封裝</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] 授權</td> 
   <td>[!UICONTROL 標準]</td> 
  </tr> 
  <tr> 
   <td>存取層級設定</td> 
   <td>系統管理員</td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 欄位追蹤的限制

您可追蹤的欄位數限制是由Workfront套件定義。

| Workfront套件 | 追蹤欄位的最大數量 |
|---------|----------|
| 選擇 | 700 |
| Prime | 3000 |
| Ultimate | 5000 |
| Workflow Select | 1000 |
| Workflow Prime | 5000 |
| Workflow Ultimate | 無限制 |

## 新增您要追蹤的欄位

{{step-1-to-setup}}

1. 在左側面板中，按一下&#x200B;**變更追蹤>組態**。
1. 在[設定]畫面上，按一下[新增]欄位&#x200B;**。**
1. 在&#x200B;**新增欄位**&#x200B;方塊中，選取物件。 您可以開始輸入物件名稱，然後在物件出現在清單中時選取它。
1. 接著，選取您要追蹤該物件的欄位名稱。 您可以開始輸入欄位名稱，然後在欄位出現在清單中時選取它。

   自訂欄位和原生欄位都可供物件使用。
   已追蹤的欄位會顯示在清單中選取的欄位。

   ![新增變更追蹤的欄位](assets/change-history-config-add-fields.png)

1. 選取您要追蹤的所有欄位後，按一下[新增]。**&#x200B;**

   這些欄位會新增至「追蹤的欄位」清單中。

## 移除您不再想要追蹤的欄位

您可以移除不希望系統透過Workfront介面追蹤特定物件型別的欄位。

{{step-1-to-setup}}

1. 在左側面板中，按一下&#x200B;**變更追蹤>組態**。
1. 在設定畫面上，選取要停止追蹤的一個或多個欄位。

   您可能會多次看到相同的欄位名稱。 欄位會依物件分組，以便您找到正確的欄位。 您也可以使用畫面頂端的搜尋方塊。

1. 在熒幕底部的動作列中選取&#x200B;**刪除**。
1. 按一下確認訊息上的&#x200B;**移除**。

   這些欄位會從「追蹤的欄位」清單中移除。


