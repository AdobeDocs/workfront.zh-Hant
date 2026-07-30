---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-locations
title: 變更歷史記錄
description: 變更記錄可讓您檢視Workfront物件的變更記錄
author: Lisa
feature: System Setup and Administration
role: Admin
source-git-commit: ba1843cf6be446a809f9526608a3ae3bef69c494
workflow-type: tm+mt
source-wordcount: '472'
ht-degree: 4%

---

# 檢視及管理變更歷史記錄

您可以在「設定」的「變更追蹤」區域中檢視變更歷史記錄，包括稽核記錄。

* **稽核記錄**是由使用者觸發的變更。
如需稽核記錄檔和稽核記錄檔區域的詳細資訊，請參閱[稽核記錄檔概述](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/audit-logs.md)
* **組態**顯示正在追蹤哪一個欄位以取得變更記錄清單。
設定目前僅作為資訊提供，無法變更。在不久的將來，您將會使用變更追蹤哪些欄位的功能。
* **變更記錄清單**&#x200B;可讓您檢視Workfront物件的變更記錄，包括屬性，例如：

  * 物件
  * 物件類型
  * 變更型別（作業）
  * 變更的Source，例如特定使用者、API、Workfront Fusion、AI LLM或Workfront系統

  <span class="preview">在「變更記錄」中追蹤整合稽核及核准工作流程活動，包括參與者和決定。</span>

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
   <td>[！UICONTROL標準]</td> 
  </tr> 
  <tr> 
   <td>存取層級設定</td> 
   <td>系統管理員</td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 檢視及管理稽核記錄

若要檢視及管理稽核記錄，請參閱[檢視及匯出稽核記錄](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/view-and-export-audit-logs.md)。

## 檢視變更追蹤的設定區域

>[!NOTE]
>
>設定目前僅作為資訊提供，無法變更。 在不久的將來，您將會使用變更追蹤哪些欄位的功能。

若要檢視所追蹤的變更型別，請執行下列動作：

{{step-1-to-setup}}

1. 在左側面板中，按一下&#x200B;**變更追蹤** ![變更歷程記錄圖示](assets/change-history-icon.png)。
1. 按一下&#x200B;**組態**。

   欄位會依物件型別分組顯示。

1. 若要顯示特定物件下的欄位，請按一下物件型別旁的下拉箭頭。

## 檢視變更記錄清單

Workfront管理員可在設定區域中檢視變更歷史記錄。

「變更歷程記錄清單」是一個增強型清單，具有篩選器、欄、列高、日期選擇器和搜尋列。

{{step-1-to-setup}}

1. 在左側面板中，按一下&#x200B;**變更追蹤** ![變更歷程記錄圖示](assets/change-history-icon.png)。
1. 按一下&#x200B;**變更歷程記錄清單**。

   「變更記錄」清單隨即開啟。

1. 若要調整顯示變更的日期，請按一下日期選擇器並選取新日期。

   變更適用於過去90天。

1. 若要搜尋特定詞語，請按一下搜尋列並輸入詞語。 當您鍵入時，結果會在清單中反白顯示。
1. （選擇性）若要依欄篩選，請參閱文章[使用增強式清單](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md)中的[篩選增強式清單中的專案](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md#filter-items-in-an-enhanced-list)。
1. （選擇性）若要隱藏、顯示或重新排序欄，請參閱發行項[使用增強式清單](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md)中的[自訂欄](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md#customize-columns)。
1. （選擇性）若要新增或移除欄，請參閱發行項[使用增強式清單](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md)中的[使用欄管理員](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md#add-and-remove-columns-with-the-column-manager)新增及移除欄。
1. （選擇性）若要調整列高，請參閱文章[使用增強式清單](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md)中的[在檢視中變更列高](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md#change-the-row-height-in-a-view)。

## 匯出變更記錄

{{step-1-to-setup}}

1. 在左側面板中，按一下&#x200B;**變更追蹤>變更記錄清單**。
1. 篩選清單以顯示您要匯出的專案。
1. 按一下&#x200B;**匯出**&#x200B;圖示![匯出圖示](assets/export-icon.png)，並選取您要儲存為XLSX或CSV格式。

   儲存檔案方塊開啟，您可以將匯出的檔案儲存在電腦上。
   完成儲存匯出的檔案。您現在可以在電腦上找到它，並與他人共用。



