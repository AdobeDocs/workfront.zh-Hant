---
title: 開始使用Workfront規劃和GenStudio for Performance Marketing整合
description: 當貴公司同時購買這兩個產品時，即可在Adobe Workfront Planning中使用GenStudio for Performance Marketing工作區。 瞭解使用此整合簡化工作流程的一些基本知識。
hide: true
hidefromtoc: true
exl-id: 3b2fc764-f384-41bb-9d88-b2b88434ffc6
source-git-commit: a92c85ad5f58700138d7750423cc3d134d980a9e
workflow-type: tm+mt
source-wordcount: '882'
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


Adobe GenStudio for Performance Marketing與Adobe Workfront Planning之間有原生整合。 這項整合的目的是防止使用者在兩個應用程式之間來回切換，以更新相同或類似的資訊。

您現在可以在GenStudio或Workfront Planning中更新或建立行銷活動，然後繼續從任一應用程式處理這些行銷活動。

當貴公司同時購買這兩個產品時，即可在Adobe Workfront Planning中使用GenStudio for Performance Marketing工作區。

透過Workfront Planning與GenStudio for Performance Marketing的整合，您可以：

<!--check this list and ensure it's accurate and add/ remove some of the benefits-->

* 在Workfront Planning中檢視GenStudio工作區。
* 在GenStudio中修改行銷活動，並在Workfront Planning中即時更新相同資訊。
* 在Workfront Planning中修改行銷活動，並在GenStudio中即時更新相同資訊。

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


## 整合需求

* Workfront和GenStudio for Performance Marketing必須啟用至相同的組織。 如果您的公司有多個Workfront執行個體，則只能將一個與GenStudio for Performance Marketing整合。

* Workfront執行個體是Adobe Unified Experience的一部分，包括使用Identity Management系統(IMS)。

  如需詳細資訊，請參閱[Workfront的Adobe Unified Experience ](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md)。

* 同時使用Planning和GenStufio的使用者只能屬於IMS組織內的一個Workfront執行個體。

<!--not sure: true for Planning? This is true for GenS and WF Proof: * The integration must be enabled in the Workfront Setup area.-->


## 在Workfront Planning中管理GenStudio工作區的考量事項

* 貴組織必須先購買Adobe GenStudio for Performance Marketing，才能在Workfront Planning中檢視GenStudio工作區。

  如需GenStudio的詳細資訊，請參閱[Adobe GenStudio for Performance Marketing使用手冊](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/home)。

  如需GenStudio與Workfront Planning整合的詳細資訊，請參閱[開始使用Workfront Planning與GenStudio for Performance Marketing整合](/help/quicksilver/planning/planning-and-genstudio-integration/get-started-with-workfront-planning-and-genstudio-integration.md)

* Workfront使用者必須擁有GenStudio的存取權，才能在Workfront Planning中檢視GenStudio工作區。


* 以下各節說明在Workfront Planning的GenStudio工作區中，您可以及無法管理哪些專案的一些限制。

### Workfront Planning中的GenStudio工作區

* 如果您的組織有多個Workfront執行個體，則只有一個的Workfront執行個體可以顯示您的GenStudio工作區。
* GenStudio工作區會顯示視覺指示器，清楚顯示它是從GenStudio匯入。

### 記錄類型

* 您無法在Workfront Planning中從GenStudio編輯記錄型別。
* 您無法和其他使用者共用來自GenStudio的記錄型別。 Workfront管理員可以在其「規劃」區域中檢視GenStudio工作區。
* 與GenStudio同步的記錄型別會顯示視覺指示器，清楚顯示記錄型別是從GenStudio匯入。

### 記錄

* 您可以在GenStudio中新增或刪除記錄，這些記錄便會顯示在Workfront Planning中（或從中移除）。
您可以在Workfront Planning中新增或刪除記錄，且這些記錄會顯示在GenStudio中（或從中移除）。
* 您可以透過下列方式，從Workfront Planning新增記錄：

   * 手動，從頭開始
   * 使用CSV或Excel檔案匯入這些檔案

  如需詳細資訊，請參閱[建立記錄](/help/quicksilver/planning/records/create-records.md)。
* 您無法從Workfront Planning建立或刪除啟用記錄。

### 欄位

* 所有記錄欄位都是從GenStudio匯入，無法編輯欄位設定。
* 只有當您在Workfront Planning中擁有系統管理員存取權時，才能在GenStudio中建立GenStudio記錄型別的欄位。
* 您可以在Workfront Planning的任何可見欄位中，編輯GenStudio工作區中所有記錄的記錄資訊。

  如需詳細資訊，請參閱[編輯記錄](/help/quicksilver/planning/records/edit-records.md)。
* 您可以在GenStudio記錄型別的表格檢視中隱藏欄位，但無法從Workfront Planning中刪除欄位。

<!-- checking: 
I had this from Iskuhi, so not sure if you CAN create fields in Planning?? - only the newly added fiedsl can be changed or the reference fields. - from this: https://experience.adobe.com/?commentID=6848549f00000091e5f5a16636e381c0#/@adobeinternalworkfront/so:hub-Hub/workfront/project/67649bc00000545810daad1cd1fbb9cc/updates 
-->

<!--document who shows up in the Created by and Updated by fields - not clear, asking-->

### 檢視

* 您可以建立GenStudio記錄型別的檢視。 您無法編輯自動從GenStudio匯入的檢視，但可以變更GenStudio表格檢視的檢視元素。 例如，您可以在表格檢視中修改篩選、排序、群組、列顏色和列高。

  如需詳細資訊，請參閱[管理記錄檢視](/help/quicksilver/planning/views/manage-record-views.md)。

* 您可以透過下列方式共用GenStudio記錄型別的檢視：

   * 複製檢視連結
   * 將檢視匯出至檔案（僅適用於表格檢視）

### 連線

* 您無法從Planning中的GenStudio記錄型別連線其他記錄或物件型別。
* 您可以從Planning中的其他記錄型別連線至GenStudio記錄型別。
