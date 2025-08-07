---
title: 開始使用Workfront規劃和GenStudio for Performance Marketing整合
description: 當貴公司同時購買這兩個產品時，即可在Adobe Workfront Planning中使用GenStudio for Performance Marketing工作區。 瞭解使用此整合簡化工作流程的一些基本知識。
hide: true
hidefromtoc: true
exl-id: 3b2fc764-f384-41bb-9d88-b2b88434ffc6
source-git-commit: 36cd1c23dfb6e01dc1016a6a12ae47e4f9172d20
workflow-type: tm+mt
source-wordcount: '1029'
ht-degree: 1%

---

# 開始使用Workfront規劃和GenStudio for Performance Marketing整合

<!--Better metadata, at publishing:
---
title: Get Started with the Workfront Planning and GenStudio for Performance Marketing Integration
description: The GenStudio for Performance Marketing workspace is available in Adobe Workfront Planning when your company has purchased both products. Learn some of the basics about how you can streamline your workflows using this integration.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog

---
-->

<!--use this article to make this one similar to it: https://experienceleague.adobe.com/en/docs/workfront/using/adobe-workfront-integrations/review-approval-integrations/wf-proof-and-genstudio-->

同時使用Adobe Workfront Planning和Adobe GenStudio for Performance Marketing的組織通常會比GenStudio預設支援的更詳細地定義行銷概念，例如行銷活動、產品和角色。

GenStudio for Performance Marketing與Workfront Planning之間有原生整合。 此整合可讓Workfront Planning中的使用者管理GenStudio中使用的行銷活動、產品、角色、啟用、管道和區域。 它也能讓他們設定GenStudio，以參照Workfront Planning中的現有記錄型別，建立更連線且一致的行銷工作流程。

此整合可協助您避免重複資料輸入、保持規劃和啟用工作的一致性，並支援您的行銷記錄系統。

當貴公司同時購買這兩個產品時，即可在Adobe Workfront Planning中使用GenStudio for Performance Marketing工作區。

透過Workfront Planning與GenStudio for Performance Marketing的整合，您可以：

<!--check this list and ensure it's accurate and add/ remove some of the benefits-->

* 在Workfront Planning中檢視GenStudio工作區。
* 在GenStudio中修改行銷活動，並在Workfront Planning中即時更新相同資訊。
* 在Workfront Planning中修改行銷活動，並在GenStudio中即時更新相同資訊。

## 整合需求

* Workfront和GenStudio for Performance Marketing必須啟用至相同的組織。

  如需GenStudio的詳細資訊，請參閱[Adobe GenStudio for Performance Marketing使用手冊](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/home)。

* 當您的公司有多個GenStudio執行個體時，Workfront Planning中將無法使用Workfront。<!--this will change-->

* Workfront執行個體是Adobe Unified Experience的一部分，包括使用Identity Management系統(IMS)。

  如需詳細資訊，請參閱[Workfront的Adobe Unified Experience ](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md)。

* 同時使用Planning和GenStudio的使用者只能屬於IMS組織內的一個Workfront例項。

<!--not sure: true for Planning? This is true for GenS and WF Proof: * The integration must be enabled in the Workfront Setup area.-->

## 存取需求

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> 產品</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront規劃<p></li>
   <p><li> Adobe GenStudio for Performance Marketing<p></li>
   </ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront計畫*</p></td> 
   <td> 
<p>下列任一Workfront計畫：</p> 
<ul><li>選取</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>舊版Workfront計畫不提供Workfront計畫</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront規劃套件</p></td> 
   <td> 
<p>任何 </p> 
<p>如需每個Workfront Planning套件所含專案的詳細資訊，請連絡您的Workfront客戶經理。 </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront平台</p></td> 
   <td> 
<p>貴組織的Workfront例項必須上線至Adobe Unified Experience，才能存取Workfront Planning。</p> 
<p>如需詳細資訊，請參閱<a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">適用於Workfront的Adobe Unified Experience</a>。 </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront授權</p></td> 
   <td><p> 系統管理員</p>
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>存取層級設定</p></td> 
   <td> <p>Adobe Workfront Planning沒有存取層級控制</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>物件許可權</p></td> 
   <td>   <p>貢獻或更高的許可權到工作區和記錄型別  </p>  
   <p>系統管理員擁有所有工作區的許可權，包括他們未建立的工作區</p> </td> 
  </tr> 
</tbody> 
</table>

*如需Workfront存取需求的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。


## Workfront Planning與GenStudio整合概述

以下各節將說明以下內容：

* 從GenStudio更新Workfront Planning資訊的功能
* 從Workfront Planning更新GenStudio資訊的功能
* 在Workfront Planning的GenStudio工作區中，您可以及無法管理的專案限制。

<!--add here a link from the GenS articles about what you can/ cannot do from GenStudio that might in the end reflect in Planning - this should come from the GenS team-->

### Workfront Planning中的GenStudio工作區

* 如果您的組織有多個Workfront執行個體，則在您的任何Workfront執行個體中都看不到GenStudio工作區。<!-- this might change-->
* GenStudio工作區會顯示視覺指示器，清楚顯示它是從GenStudio匯入。 如需詳細資訊，請參閱[在Adobe Workfront規劃中管理GenStudio工作區](/help/quicksilver/planning/planning-and-genstudio-integration/manage-gen-studio-workspace-in-planning.md)。
* 所有同時有權存取GenStudio和Workfront Planning的使用者也可以在Workfront Planning中看到GenStudio工作區。
* Workfront Planning使用者必須透過Adobe Identity Management System (IMS)管理，才能從Workfront檢視及使用GenStudio工作區。

  僅限Workfront的使用者無法看見GenStudio工作區，即使它可在Workfront中使用。

  如需詳細資訊，請參閱[Workfront的Adobe Unified Experience ](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md)。


### 記錄類型

* 您可以在Workfront Planning中從GenStudio編輯記錄型別資訊（例如其外觀）。
* 您可以在Planning中與其他人共用GenStudio記錄型別。 <!--checking with Ani H.-->
* 您可以在GenStudio工作區上從Planning建立記錄型別。<!-- checking with Ani where these show up in GenS-->
* 與GenStudio同步的記錄型別會顯示視覺指示器，清楚顯示記錄型別是從GenStudio匯入。

### 記錄

* 您可以在GenStudio中新增或刪除記錄，這些記錄便會顯示在Workfront Planning中（或從中移除）。
您可以在Workfront Planning中新增或刪除記錄，且這些記錄會顯示在GenStudio中（或從中移除）。
* 您可以透過下列方式，從Workfront Planning新增記錄：

   * 使用「新增記錄」按鈕，從任何檢視手動從頭開始
   * 使用CSV或Excel檔案匯入這些檔案
   * 手動、內嵌、在表格檢視中
   * 手動、直接在時間軸檢視中

  如需詳細資訊，請參閱[建立記錄](/help/quicksilver/planning/records/create-records.md)。
* 您無法從Workfront Planning建立或刪除啟用記錄。
* 您可以在Planning的GenStudio工作區中，從Workfront Planning的任何可見欄位編輯所有記錄的記錄資訊。

  如需詳細資訊，請參閱[編輯記錄](/help/quicksilver/planning/records/edit-records.md)。

  <!--asking Ani if I delete a record in GS - will it move to Recovery box in Planning?-->

### 欄位

* 記錄欄位會從GenStudio匯入。 您可以在Workfront規劃中編輯欄位設定。
* 如果您在Gen Studio中擁有「管理」存取權，即可在Workfront Planning中為GenStudio記錄型別建立更多欄位。
* 當您在Planning中為GenStudio記錄型別建立欄位時，可從下列區域看到這些欄位：
   * Planning檢視
   * Planning記錄詳細資訊頁面
   * GenStudio記錄詳細資料頁面

  >[!TIP]
  >
  >在Workfront Planning中建立的欄位不會顯示在GenStudio清單檢視中。

* 您可以在Planning中隱藏GenStudio記錄型別的表格檢視中的欄位，但無法從Workfront Planning中刪除欄位。


<!-- checking: 
I had this from Iskuhi, so not sure if you CAN create fields in Planning?? - only the newly added fiedsl can be changed or the reference fields. - from this: https://experience.adobe.com/?commentID=6848549f00000091e5f5a16636e381c0#/@adobeinternalworkfront/so:hub-Hub/workfront/project/67649bc00000545810daad1cd1fbb9cc/updates 
-->

<!--document who shows up in the Created by and Updated by fields - not clear, asking-->

### 檢視

* 您可以建立GenStudio記錄型別的檢視。

  如需詳細資訊，請參閱[管理記錄檢視](/help/quicksilver/planning/views/manage-record-views.md)。

* 當您要共用Planning記錄型別的檢視時，可以共用GenStudio記錄型別的檢視。

### 連線

* 您可以在GenStudio記錄型別與Workfront Planning中的其他記錄或物件型別之間建立下列連線：

   * 兩種GenStudio記錄型別和
   * 來自相同工作區的GenStudio記錄型別和Planning記錄型別
   * 來自另一個工作區的GenStudio記錄型別和Planning記錄型別（如果記錄型別設定為從另一個工作區連線）。
   * GenStudio記錄型別和Workfront物件型別（專案、投資組合、方案、公司、群組）