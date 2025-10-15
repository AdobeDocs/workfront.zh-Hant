---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: 列印儀表板
description: 您可以列印儀表板或將儀表板匯出到。PDF檔案。 若要列印儀表板，您必須擁有檢視許可權。
author: Nolan
feature: Reports and Dashboards
exl-id: 30f3481b-23b6-4dc9-be0d-9cffd5d4dfed
source-git-commit: c8b7ad473b0c2120ef5ea52374b3501ad6f553f1
workflow-type: tm+mt
source-wordcount: '460'
ht-degree: 0%

---

# 列印儀表板

<!-- Audited: 1/2025 -->

您可以列印儀表板或將儀表板匯出到。PDF檔案。 若要列印儀表板，您必須擁有檢視許可權。

>[!NOTE]
>
>此功能僅供標準「儀表板」檢視使用。 它不適用於內嵌於專案區域或設定為自訂標籤的控制面板。

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
      <p>標準</p>
      <p>工作或更高</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>編輯報告、儀表板和行事曆的存取權</p></td> 
  </tr>  
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>檢視儀表板的許可權</p> </td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先決條件

必須先建立儀表板，然後才能列印。

如需有關建立儀表板的資訊，請參閱[建立儀表板](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md)。

## 瞭解列印儀表板時列印了哪些資訊

列印儀表板或將其儲存為。PDF檔案時，儀表板的某些資訊(如顯示在Adobe Workfront Web應用程式中的資訊)可能不會顯示在列印或匯出的檔案中。

* [顯示什麼？](#what-is-displayed)
* [不會顯示哪些內容？](#what-is-not-displayed)

### 會顯示哪些內容？ {#what-is-displayed}

下列資訊會包含在列印或匯出的儀表板檔案中：

* 儀表板標題
* 報告標題
* 上次產生報表的時間戳記
* 控制面板上的所有物件，包括清單檢視、外部網頁、報告和行事曆
* 貴公司的標誌(如果您的Workfront管理員已在您的全域導覽列中自訂該標誌)。 如需品牌化Workfront網站的詳細資訊，請參閱[品牌化Adobe Workfront執行個體](../../../administration-and-setup/customize-workfront/brand-workfront/brand-your-workfront-instance.md)。

### 不會顯示哪些內容？ {#what-is-not-displayed}

下列資訊不包含在列印或匯出的儀表板檔案中：

* Workfront導覽列
* Workfront特定的任何其他格式
* 根據報表的大小以及個別欄的數量和寬度，匯出和列印儀表板可能會導致某些欄被截斷。

## 列印儀表板

1. 移至您要列印的儀表板。
1. 執行下列任一項作業：

   * 按一下&#x200B;**儀表板動作** > **列印預覽**

   * 按&#x200B;**Ctrl+P** （在Windows上）或&#x200B;**Command+P** (在Mac上)

     >[!IMPORTANT]
     >
     >* 當控制面板內嵌在自訂標籤中時，這些選項都無法使用。 如需建立自訂標籤的相關資訊，請參閱[建立自訂標籤或區段](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/create-custom-tabs.md)。
     >* 使用Internet Explorer瀏覽器時，無法使用鍵盤快速鍵選項。

1. 在&#x200B;**目的地**&#x200B;欄位中，從各種可用的列印選項中選取。\
   列印選項會依您使用的瀏覽器和瀏覽器版本而有所不同。

1. （選擇性）將儀表板儲存為。PDF檔案，然後按一下[儲存] **&#x200B;**&#x200B;以儲存。PDF。\
   若要瞭解如何將儀表板儲存為。PDF檔案，請參閱[匯出儀表板](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/export-dashboard.md)。

1. 按一下&#x200B;**列印**。
