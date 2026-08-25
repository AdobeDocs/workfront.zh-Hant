---
user-type: administrator
product-area: system-administration;setup
title: 檢視及管理變更歷史記錄
description: 變更記錄可讓您檢視Workfront物件和欄位的變更記錄。
author: Lisa
feature: System Setup and Administration
role: Admin
source-git-commit: 1e06115eb5688271e2a6f4c8a41647eb644d8292
workflow-type: tm+mt
source-wordcount: '523'
ht-degree: 3%

---

# 檢視及管理變更歷史記錄

{{preview-fast-release-general}}

變更記錄可讓系統管理員設定及追蹤Adobe Workfront中物件和特定欄位的變更。 彈性的設定可讓管理員設定確切要追蹤哪些物件和欄位。

變更記錄可追蹤下列型別的已定義資料：

* 「設定」區域中的活動，例如建立或刪除存取層級或工作角色
* 欄位層級更新，例如編輯專案說明或變更使用者的版面配置範本
* 物件更新，例如更新專案狀態或附加自訂表單到任務
* <span class="preview">統一檢閱和核准工作流程活動，包括參與者和決定</span>

如需定義要追蹤哪些物件和欄位的詳細資訊，請參閱[設定要在變更歷程記錄中追蹤的欄位](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/configure-fields-in-change-history.md)。

在「變更記錄清單」上，您可以檢視Workfront物件的變更記錄，包括屬性，例如：

* 物件名稱
* 物件類型
* 變更型別（作業）
* 變更的日期和時間
* 變更的Source，例如特定使用者、API、Workfront Fusion、AI LLM或Workfront系統

>[!NOTE]
>
>當您存取「變更歷史記錄」時，只會看到您有權檢視之欄位的追蹤變更。
>例如，如果在專案上追蹤財務資料，而您無權存取財務資料，則您不會在「變更歷史記錄清單」中看到財務欄位。

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
   <td><span class="preview">變更歷史記錄的管理存取權</span></td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 檢視變更記錄清單

您可以在「設定」區域中檢視變更歷程記錄。

「變更歷程記錄清單」是一個增強型清單，具有篩選器、欄、列高、日期選擇器和搜尋列。

{{step-1-to-setup}}

1. 在左側面板中，按一下&#x200B;**變更追蹤>變更記錄清單**。

   「變更記錄」清單隨即開啟。

1. 若要調整顯示變更的日期，請按一下日期選擇器並選取新日期。

   變更適用於過去90天。

1. 若要搜尋特定詞語，請按一下搜尋方塊並輸入詞語。 當您鍵入時，結果會在清單中反白顯示。
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
   完成儲存匯出的檔案。 您現在可以在電腦上找到它，並與他人共用。



