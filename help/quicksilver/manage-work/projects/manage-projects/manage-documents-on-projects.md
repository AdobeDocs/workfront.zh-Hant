---
product-area: projects
navigation-topic: manage-projects
title: 專案和相關物件的檔案管理概觀
description: 根據您的Workfront管理員是否選擇儲存偏好設定預設值，您可以將檔案儲存在舊版Workfront儲存空間或Adobe雲端儲存空間。 本文說明如何管理專案、投資組合、方案、範本、任務和問題的檔案。
author: Alina
feature: Work Management
exl-id: 5623157e-946e-4475-9df3-b1888a2a0934
source-git-commit: 9a35246858141a3b69ec85be3372c7a8d9497d6e
workflow-type: tm+mt
source-wordcount: '1920'
ht-degree: 0%

---

# 專案和相關物件的檔案管理概觀

您的Adobe Workfront管理員可為貴組織的儲存偏好設定定義預設值，以指出檔案應儲存在Workfront中的何處。

Workfront管理員可選擇下列其中一個選項：

* Workfront儲存空間
* Adobe雲端儲存空間

此偏好設定可讓您在其中一個可用的儲存位置上，自動儲存附加至Workfront物件的檔案。

>[!IMPORTANT]
>
>您的Workfront執行個體可能無法同時存取Workfront和Adobe儲存空間。 有些Workfront執行個體僅能存取Workfront，有些則預設僅能存取Adobe雲端儲存空間。 僅能存取一種儲存型別的客戶，不需要任何設定。

Workfront管理員可以執行下列任一項作業：

* 選擇兩個儲存選項之一，作為貴組織的預設值
* 可讓您選擇建立下列其中一個物件時偏好使用的儲存空間：

   * 專案
   * 專案組合
   * 範本

如需有關設定Workfront的儲存偏好設定的資訊，請參閱[為您的組織啟用Adobe雲端儲存空間](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-esm.md)。

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
* 僅限Adobe雲端儲存空間。 「系統偏好設定」中的「儲存偏好設定」區域不存在。
* Workfront儲存空間和Adobe雲端儲存空間。 Workfront管理員可選擇下列選項：

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


儲存在Workfront儲存空間中物件上的檔案，其管理方式與Adobe雲端儲存空間中儲存的檔案不同。

如需詳細資訊，請參閱[Adobe雲端儲存空間概觀](/help/quicksilver/review-and-approve-work/esm-overview.md)。

以下小節記錄當Workfront和Workfront雲端儲存選項存在於相同環境中時，檔案儲存如何用於Adobe物件。

### 專案的檔案管理

使用專案時，請考量下列事項：

* 當您建立Adobe雲端儲存空間專案時，Workfront會在專案的「檔案」區段中建立一個資料夾，以便儲存檔案。 資料夾名稱與專案名稱相同。 您無法刪除或手動重新命名資料夾。 如果您變更專案名稱以符合專案的新名稱，資料夾會重新命名。
* 當您建立或將Adobe雲端儲存空間專案移動到舊版Workfront儲存空間專案組合或方案時，如果該組合或方案在新增專案之前沒有附加檔案，則該組合或方案會自動轉換為Adobe雲端儲存空間物件。
* 您無法為Workfront雲端儲存產品組合或方案建立舊版Adobe儲存專案。
* 當您從MS Project匯入專案時，Workfront會建立舊版Workfront儲存空間專案，即使Workfront管理員將Adobe雲端儲存空間設為您系統的預設值亦然。
* 當您使用Workfront Planning自動化建立專案時，Workfront會使用您系統的預設專案儲存偏好設定。 您必須購買Planning套件，才能存取Workfront Planning。

### 投資組合的檔案管理

使用投資組合時，請考慮下列事項：

* 當您建立Adobe雲端儲存空間產品組合時，Workfront會在產品組合的「檔案」區段中建立一個資料夾，以儲存檔案。 資料夾名稱與投資組合名稱相同。 您無法刪除或手動重新命名資料夾。 如果您變更投資組合名稱以符合投資組合的新名稱，資料夾會重新命名。

* 當您將Adobe雲端儲存空間專案新增至舊版Workfront儲存空間產品組合，且該產品組合沒有附加任何檔案時，該產品組合會轉換為Adobe雲端儲存空間產品組合。
* 當您將Adobe雲端儲存空間專案新增至舊版Workfront儲存產品組合，且該產品組合已附加檔案，則產品組合檔案儲存空間仍會保留在Workfront儲存空間中。 不過，產品組合![舊版產品組合儲存圖示](assets/legacy-storage-project-icon.png)的舊版Workfront儲存圖示已從產品組合中移除。
* 您無法將舊版Workfront儲存空間專案新增到Adobe雲端儲存空間產品組合。

* 當您使用Workfront Planning自動化建立產品組合時，Workfront會使用您系統的預設產品組合儲存偏好設定。 您必須購買Planning套件，才能存取Workfront Planning。

### 方案的檔案管理

使用方案時，請考慮下列事項：

* 當您建立Adobe雲端儲存空間計畫時，Workfront會在計畫的檔案區段中建立一個資料夾，以便儲存檔案。 資料夾名稱與方案的名稱相同。 您無法刪除或手動重新命名資料夾。 如果您變更方案名稱，資料夾會重新命名，以符合方案的新名稱。

* 當您將Adobe雲端儲存空間專案新增至舊版Workfront儲存空間方案，且方案沒有附加任何檔案時，方案會轉換為Adobe雲端儲存空間方案。 計畫的投資組合也會轉換。
* 當您將Adobe雲端儲存空間專案新增至舊版Workfront儲存空間方案，且方案具有附加檔案時，方案檔案儲存空間仍會保留在Workfront儲存空間中。 如果產品組合也有檔案，則其檔案儲存空間也會保留在Workfront儲存空間中；否則，產品組合會轉換為Adobe雲端儲存空間。

  程式![舊版產品組合儲存圖示](assets/legacy-storage-project-icon.png)的舊版Workfront儲存圖示已從程式中移除。
* 您無法將舊版Workfront儲存空間專案新增到Adobe雲端儲存空間方案。

* 當您使用Workfront Planning自動化建立程式時，Workfront會使用您系統的預設程式儲存偏好設定。 您必須購買Planning套件，才能存取Workfront Planning。

### 任務的檔案管理

處理任務時請考慮下列事項：

* 任務會從專案繼承儲存型別。
* 當您將檔案上傳到Adobe雲端儲存空間專案上的任務時，Workfront會自動在任務的檔案區段中建立資料夾。 資料夾名稱與工作相同。
* 您可以重新命名並從Adobe雲端儲存任務中刪除檔案資料夾，這也會刪除資料夾中的檔案。 將新檔案新增至任務後，資料夾會自動重新建立。 刪除的檔案不會放回資料夾。
* 對於Adobe雲端儲存空間專案，任務上的檔案資料夾顯示為專案自動建立的檔案資料夾的子資料夾。
* 您無法將任務從舊版Workfront儲存空間專案複製或移動到Adobe雲端儲存空間專案。 也不可能反轉。
* 將任務轉換為專案時有下列情況： <!--this info also duplicated in Convert tasks to projects-->
   * 舊版Workfront儲存空間任務會建立舊版Workfront儲存空間專案。
   * Adobe雲端儲存空間任務會建立Adobe雲端儲存空間專案。
   * 使用舊版Workfront儲存範本來轉換Adobe雲端儲存空間任務，會建立Adobe雲端儲存空間專案。
   * 使用Adobe雲端儲存空間範本來轉換舊版Workfront儲存空間任務，會建立舊版Workfront儲存空間專案。
* 您無法在摘要面板中新增檔案至Adobe雲端儲存空間任務。

### 問題的檔案管理

處理問題時請考慮下列事項：

* 從專案繼承儲存型別時發生問題。
* 當您將檔案上傳到Adobe雲端儲存空間專案的問題時，Workfront會自動在問題的檔案區段中建立資料夾。 資料夾名稱與問題相同。
* 您可以重新命名檔案資料夾，並從Adobe雲端儲存空間問題中刪除該檔案資料夾，這也會刪除資料夾中的檔案。 將新檔案新增到問題中後，會自動重新建立資料夾。 刪除的檔案不會放回資料夾。
* 對於Adobe雲端儲存空間專案，問題上的檔案資料夾顯示為專案自動建立的檔案資料夾的子資料夾。
* 您無法將問題從舊版Workfront儲存空間專案複製或移動到Adobe雲端儲存空間專案。 也不可能反轉。
* 當您提交請求，並附上附加到舊版Workfront儲存專案的檔案時，請求的檔案區域會使用專案的儲存型別顯示檔案，即使系統儲存預設偏好設定是Adobe雲端儲存亦然。
* 將問題轉換為專案時，有下列情況： <!--this info also duplicated in Convert an issue to a project-->
   * 舊版Workfront儲存空間問題會建立舊版Workfront儲存空間專案。
   * Adobe雲端儲存空間問題會建立Adobe雲端儲存空間專案。
   * 使用舊版Workfront儲存空間範本來轉換Adobe雲端儲存空間問題，會建立Adobe雲端儲存空間專案。
   * 使用Adobe雲端儲存空間範本轉換舊版Workfront儲存空間問題時，會建立舊版Workfront儲存空間專案。
* 您無法在摘要面板中新增檔案至Adobe雲端儲存空間問題。

### 專案範本的檔案管理

使用範本時，請考量下列事項：

* 當您建立Adobe雲端儲存空間範本時，Workfront會在範本的「檔案」區段中建立一個資料夾，用來儲存檔案。 資料夾名稱與方案相同。 您無法刪除或手動重新命名資料夾。 如果您變更範本的名稱，資料夾會重新命名，以符合範本的新名稱。
* 您可以使用舊版Workfront儲存空間範本來建立舊版Workfront儲存空間專案；您可以使用Adobe雲端儲存空間範本來建立Adobe雲端儲存空間專案。
* 您可以將舊版Workfront儲存體範本附加至Adobe雲端儲存體專案，但這不會變更專案上檔案的儲存位置。
* 您可以將Adobe雲端儲存空間範本附加至舊版Workfront儲存空間專案，但這不會變更專案上檔案的儲存位置。 範本的Adobe雲端儲存資料夾中的檔案會直接新增至專案，而不會新增資料夾，而範本任務資料夾中的檔案會新增至任務的「檔案」區段中附加到專案任務的資料夾。

### 範本任務的檔案管理

使用範本任務時，請考量下列事項：

* 範本任務會繼承範本的儲存型別。
* 當您在Adobe雲端儲存空間範本上傳檔案至範本任務時，Workfront會自動在範本任務的「檔案」區段中建立資料夾。 資料夾名稱與範本任務相同。
* 您可以重新命名並從Adobe雲端儲存空間範本任務中刪除檔案資料夾，這也會刪除資料夾中的檔案。 將新檔案加入範本任務後，資料夾會自動重新建立。 刪除的檔案不會放回資料夾。
* 對於Adobe雲端儲存範本，範本任務上的檔案資料夾顯示為自動為範本建立的檔案資料夾的子資料夾。
* 您無法將範本任務從舊版Workfront儲存體範本複製或移動到Adobe雲端儲存體範本。 也不可能反轉。
* 當您將檔案附加至您提交至與Adobe儲存相關聯之請求佇列的問題時，會針對每個提交的問題建立一個資料夾，其中儲存檔案。 資料夾也會新增為請求佇列上自動建立的專案資料夾的子資料夾。
