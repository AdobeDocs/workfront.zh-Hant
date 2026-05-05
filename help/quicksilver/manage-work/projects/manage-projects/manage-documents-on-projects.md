---
product-area: projects
navigation-topic: manage-projects
title: 專案和相關物件的檔案管理概觀
description: 視您的Workfront管理員是否為儲存偏好設定預設值選擇而定，您可以將檔案儲存在舊版Workfront儲存空間或Adobe企業儲存空間中。 本文說明如何管理專案、投資組合、方案、範本、任務和問題的檔案。
author: Alina
feature: Work Management
exl-id: 5623157e-946e-4475-9df3-b1888a2a0934
source-git-commit: ada25d0b7c359cfb258dfc4e68a628033e66562d
workflow-type: tm+mt
source-wordcount: '1470'
ht-degree: 0%

---

# 專案和相關物件的檔案管理概觀

您的Adobe Workfront管理員可為貴組織的儲存偏好設定定義預設值，以指出檔案應儲存在Workfront中的何處。

Workfront管理員可選擇下列其中一個選項：

* Workfront儲存空間
* Adobe企業儲存空間

此偏好設定可讓您在其中一個可用的儲存位置上，自動儲存附加至Workfront物件的檔案。

>[!IMPORTANT]
>
>您的Workfront執行個體可能同時無法存取Workfront和Adobe儲存空間。 有些Workfront執行個體僅能存取Workfront，其他則預設僅能存取Adobe企業儲存空間。 僅能存取一種儲存型別的客戶，不需要任何設定。

Workfront管理員可以執行下列任一項作業：

* 選擇兩個儲存選項之一，作為貴組織的預設值
* 可讓您選擇建立下列其中一個物件時偏好使用的儲存空間：

   * 專案
   * 專案組合
   * 範本

如需設定Workfront的儲存偏好設定的相關資訊，請參閱[為您的組織啟用Adobe企業儲存空間](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-esm.md)。

本文說明如何管理專案、投資組合、方案、任務、問題、範本和範本任務的檔案。

<!--

Not sure we need these since this became an overview article: 

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>Light or higher</p>
   <p>Review or higher</p>
   
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>View or higher access to the objects you want to add documents to:</p>
   <ul><li>Projects</li>
   <li>Portfolios</li>
<li>Programs</li>
<li>Templates</li> 
<li>Tasks</li> 
<li>Issues</li> </ul>  
   
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p> View or higher permissions to the objects you want to add documents to:</p>

<ul><li>A project</li>
   <li>A portfolio</li>
<li>A program</li>
<li>A template</li> 
<li>A task</li> 
<li>An issue</li> </ul>    
   
</td> 
  </tr> 
 </tbody> 
</table>

*For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

-->

## 檔案儲存概述

客戶可以存取下列其中一項檔案儲存功能：

* 僅限Workfront儲存空間。 「系統偏好設定」中的「儲存偏好設定」區域不存在。
* 僅限Adobe企業儲存空間。 「系統偏好設定」中的「儲存偏好設定」區域不存在。
* Workfront儲存空間和Adobe企業儲存空間。 Workfront管理員可選擇下列選項：

   * 選取未來處理檔案的預設儲存環境。
   * 允許使用者選擇建立下列物件時所選擇的儲存空間：

      * 專案
      * 專案組合
      * 範本

  >[!NOTE]
  >
  >* 任務和問題會繼承專案的儲存型別。
  >* 範本任務會繼承範本的儲存型別
  >* 程式會繼承產品組合的儲存型別。


儲存在Workfront儲存空間中物件上的檔案，其管理方式與Adobe企業儲存空間中儲存的檔案不同。

如需詳細資訊，請參閱[Adobe企業儲存概述](/help/quicksilver/review-and-approve-work/esm-overview.md)。

以下幾節將記錄當Workfront和Workfront企業儲存選項都就緒時，檔案儲存如何用於Adobe物件。

### 專案的檔案管理

使用專案時，請考量下列事項：

* 建立Adobe企業儲存專案時，Workfront會在專案的「檔案」區段中建立一個資料夾，以便儲存檔案。 資料夾名稱與專案名稱相同。 您無法刪除或手動重新命名資料夾。 如果您變更專案名稱以符合專案的新名稱，資料夾會重新命名。
* 當您建立或將Adobe企業儲存專案移動到舊版Workfront儲存產品組合或方案時，產品組合或方案會自動轉換為Adobe企業儲存物件。
* 您無法為Workfront企業儲存產品組合或方案建立Adobe儲存專案。

### 投資組合的檔案管理

使用投資組合時，請考慮下列事項：

* 當您建立Adobe企業儲存產品組合時，Workfront會在產品組合的檔案區段中建立一個資料夾，以儲存檔案。 資料夾名稱與投資組合名稱相同。 您無法刪除或手動重新命名資料夾。 如果您變更投資組合名稱以符合投資組合的新名稱，資料夾會重新命名。
* 當您建立或移動Adobe企業儲存專案至舊版Workfront儲存產品組合時，產品組合會自動轉換成Adobe企業儲存物件。
* 如果轉換後的產品組合先前已有附加檔案，則會繼續保留在Workfront儲存空間中。 新檔案也會儲存在Workfront儲存空間中。
* 如果轉換後的產品組合未在Workfront儲存空間中附加任何檔案，則新檔案會儲存在Adobe企業儲存空間中。

### 方案的檔案管理

使用方案時，請考慮下列事項：

* 當您建立Adobe企業儲存方案時，Workfront會在方案的檔案區段中建立一個資料夾，用來儲存檔案。 資料夾名稱與方案相同。 您無法刪除或手動重新命名資料夾。 如果您變更方案名稱，資料夾會重新命名，以符合方案的新名稱。
* 當您建立或移動Adobe企業儲存專案至舊版Workfront儲存產品組合時，產品組合會自動轉換成Adobe企業儲存物件。
* 如果轉換後的程式先前已有附加檔案，這些檔案仍會儲存在Workfront儲存空間。 新檔案也會儲存在Workfront儲存空間中。
* 如果轉換後的程式在Workfront儲存空間中沒有任何附加檔案，則新檔案會儲存在Adobe企業儲存空間中。

### 任務的檔案管理

處理任務時請考慮下列事項：

* 任務會從專案繼承儲存型別。
* 當您將檔案上傳到Adobe儲存專案上的任務時，Workfront會自動在任務的檔案區段中建立資料夾。 資料夾名稱與工作相同。
* 您可以在Adobe企業儲存工作中重新命名和刪除檔案資料夾，這也會刪除資料夾中的檔案。 將新檔案新增至任務後，資料夾會自動重新建立。 刪除的檔案不會放回資料夾。
* 對於Adobe企業儲存專案，任務上的檔案資料夾顯示為專案自動建立的檔案資料夾的子資料夾。
* 您無法將任務從Workfront儲存專案複製或移動到Adobe儲存專案。 也不可能反轉。

### 問題的檔案管理

處理問題時請考慮下列事項：

* 從專案繼承儲存型別時發生問題。
* 當您將檔案上傳至Adobe儲存專案的問題時，Workfront會自動在問題的檔案區段中建立資料夾。 資料夾名稱與問題相同。
* 您可以重新命名檔案資料夾，並從Adobe企業儲存問題中刪除該檔案資料夾，這也會刪除資料夾中的檔案。 將新檔案新增到問題中後，會自動重新建立資料夾。 刪除的檔案不會放回資料夾。
* 對於Adobe企業儲存專案，問題上的檔案資料夾顯示為專案自動建立的檔案資料夾的子資料夾。
* 您無法將問題從Workfront儲存專案複製或移動到Adobe儲存專案。 也不可能反轉。

### 專案範本的檔案管理

使用範本時，請考量下列事項：

* 當您建立Adobe企業儲存範本時，Workfront會在範本的「檔案」區段中建立一個資料夾，用來儲存檔案。 資料夾名稱與方案相同。 您無法刪除或手動重新命名資料夾。 如果您變更範本的名稱，資料夾會重新命名，以符合範本的新名稱。
* 您可以使用Workfront儲存範本來建立Workfront儲存專案；您可以使用Adobe儲存範本來建立Adobe儲存專案。
* 您可以將Workfront儲存體範本附加至Adobe儲存體專案，但這不會變更專案的儲存位置。
* 您可以將Adobe儲存體範本附加至Workfront儲存體專案，但這不會變更專案的儲存位置。 範本的Adobe-storage資料夾中的檔案會直接新增到專案中，而不會新增資料夾，而範本任務資料夾中的檔案會新增到任務的「檔案」區段中附加到專案任務的資料夾。

### 範本任務的檔案管理

使用範本任務時，請考量下列事項：

* 範本任務會繼承範本的儲存型別。
* 當您將檔案上傳到Adobe儲存範本上的範本任務時，Workfront會自動在範本任務的檔案區段中建立資料夾。 資料夾名稱與範本任務相同。
* 您可以重新命名並刪除Adobe企業儲存範本任務中的檔案資料夾，這樣也會刪除資料夾中的檔案。 將新檔案加入範本任務後，資料夾會自動重新建立。 刪除的檔案不會放回資料夾。
* 對於Adobe企業儲存範本，範本任務上的檔案資料夾顯示為自動為範本建立的檔案資料夾的子資料夾。
* 您無法將範本任務從Workfront儲存範本複製或移動到Adobe儲存範本。 也不可能反轉。
* 當您將檔案附加至您提交至與Adobe儲存相關聯之請求佇列的問題時，會針對每個提交的問題建立一個資料夾，其中儲存檔案。 資料夾也會新增為請求佇列上自動建立的專案資料夾的子資料夾。
