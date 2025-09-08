---
title: 開始使用Workfront規劃和GenStudio for Performance Marketing整合
description: 當貴公司同時購買這兩個產品時，即可在Adobe Workfront Planning中使用GenStudio for Performance Marketing工作區。 瞭解使用此整合簡化工作流程的一些基本知識。
hide: true
hidefromtoc: true
exl-id: 3b2fc764-f384-41bb-9d88-b2b88434ffc6
source-git-commit: 9b95b5a52576327a3df8d6955925b96c2e45848f
workflow-type: tm+mt
source-wordcount: '1855'
ht-degree: 0%

---

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


# 開始使用Adobe Workfront規劃和Adobe GenStudio for Performance Marketing整合

<!--update the text in the title everywhere this article is linked from - it changed a few times-->

<!--<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

同時使用Adobe Workfront Planning和Adobe GenStudio for Performance Marketing的組織通常會比GenStudio預設支援的更詳細地定義行銷概念，例如行銷活動、產品和角色。

GenStudio for Performance Marketing與Workfront Planning之間有原生整合。 此整合可讓Workfront Planning中的使用者管理GenStudio中使用的行銷活動、產品、角色、啟用、管道和區域。 它也能讓他們設定GenStudio，以參照Workfront Planning中的現有記錄型別，建立更連線且一致的行銷工作流程。

當貴公司同時購買這兩個產品時，即可在Adobe Workfront Planning中使用GenStudio for Performance Marketing工作區。

## 整合優點

透過Workfront Planning與GenStudio for Performance Marketing的整合，您可以：

<!--check this list and ensure it's accurate and add/ remove some of the benefits-->

* 在Workfront Planning中檢視GenStudio工作區。
* 在GenStudio for Performance Marketing中修改行銷活動，並在Workfront Planning中即時更新相同資訊。
* 在Workfront Planning中修改行銷活動，並在GenStudio for Performance Marketing中即時更新相同資訊。
* 避免重複資料輸入。
* 保持規劃和啟動工作的一致性。

## 整合需求

您的組織必須符合下列要求，Workfront Planning與GenStudio for Performance Marketing之間的整合才能存在：

* Workfront和GenStudio for Performance Marketing必須啟用至相同的組織。

  如需GenStudio的詳細資訊，請參閱[Adobe GenStudio for Performance Marketing使用手冊](https://experienceleague.adobe.com/zh-hant/docs/genstudio-for-performance-marketing/user-guide/home)。

<!--No longer the case: * Your organization must have only one Workfront instance. GenStudio will not be available in Workfront Planning when your company has multiple Workfront instances. -->

* 您的Workfront執行個體是Adobe Unified Experience的一部分，包括使用Identity Management系統(IMS)。

  如需詳細資訊，請參閱[Workfront的Adobe Unified Experience ](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md)。

* 同時使用Workfront Planning和GenStudio for Performance Marketing的使用者必須只屬於IMS組織中的一個Workfront例項。

  僅限Workfront的使用者可檢視GenStudio工作區，即使他們不是GenStudio for Performance Marketing使用者亦然。

<!--not sure: true for Planning? This is true for GenS and WF Proof: * The integration must be enabled in the Workfront Setup area.-->

## 存取需求

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
    <td role="rowheader"><p>Adobe Workfront套件</p></td> 
   <td> 
<p>任何Workfront套件</p>
<p>任何Planning套件</p>

</td> </tr>
   <tr> 
<td> 
   <p> 其他產品</p> </td> 
   <td> 
   <p> Adobe GenStudio for Performance Marketing</p></td> 
  </tr>
  <tr> 
   <td role="rowheader"><p>Adobe Workfront授權</p></td> 
   <td><p> 標準</p>
  </td> 
  </tr>

<tr> 
   <td role="rowheader"><p>Adobe GenStudio for Performance Marketing使用者角色</p></td> 
   <td><p><ul><li>存取行銷活動、產品和角色的任何GenStudio使用者角色</li>
   <li>GenSudio System Manager存取啟用與事件</li></ul>
   如需詳細資訊，請參閱<a href="https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/intro/user-roles">使用者角色和許可權</a>。 
   </p>
  </td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>物件許可權</p></td> 
   <td>  
   <p>在Workfront規劃中： </p>
   <ul>
   <li><p>管理GenStudio工作區的許可權，以新增欄位或記錄型別至GenStudio工作區</p></li>
   <li><p>為GenStudio工作區貢獻許可權，以便在GenStudio工作區中新增、更新或刪除記錄</p> </li>  
   </ul>
   <p>任何使用者都不能從Workfront Planning的GenStudio for Performance Marketing工作區中移除GenStudio記錄型別或欄位</p>
   <p>在Adobe GenStudio for Performance Marketing中： <p>
   <ul>
   <li><p> Adobe GenStudio for Performance Marketing中的任何許可權</p></li>
   <li><p> 在Adobe GenStudio for Performance Marketing中建立許可權以建立專案</p></li></ul>
   </td> 
  </tr> 
</tbody> 
</table>

如需Adobe Workfront Planning存取權的相關資訊，請參閱[Adobe Workfront Planning存取權概觀](/help/quicksilver/planning/access/access-overview.md)。

如需Adobe GenStudio for Performance Marketing的詳細資訊，請參閱[Adobe GenStudio for Performance Marketing使用手冊](https://experienceleague.adobe.com/zh-hant/docs/genstudio-for-performance-marketing/user-guide/home)。


## Workfront Planning與GenStudio for Performance Marketing整合功能總覽

根據組織擁有的Workfront例項數目，您在Planning中自動擁有GenStudio工作區的下列許可權：

<!--this table exists in the article Manage GenStudio workspace in Planning-->

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
    <td role="rowheader"><p>一個Workfront例項</p></td> 
   <td> 
<p>可在您的Workfront Planning例項中看見GenStudio工作區</p>
<p>Workfront管理員擁有在Planning中GenStudio工作區的管理許可權</p>
<p>所有其他使用者皆擁有Planning中GenStudio工作區的「貢獻」存取權</p>
</td> </tr>
   <tr> 
<td> 
   <p> 多個Workfront例項</p> </td> 
   <td> 
   <p>所有Workfront例項皆顯示GenStudio工作區</p>
<p>所有可存取GenStudio for Performance Marketing和Workfront Planning的使用者皆擁有Planning中GenStudio的「貢獻」許可權</p> </td> 
  </tr>
   </tbody> 
</table>

如需Workfront Planning許可權的相關資訊，請參閱[在Adobe Workfront Planning中共用許可權概觀](/help/quicksilver/planning/access/sharing-permissions-overview.md)。

以下各節將說明以下內容：

* 從GenStudio for Performance Marketing更新Workfront Planning資訊的功能
* 從Workfront Planning更新GenStudio for Performance Marketing資訊的功能
* 在Workfront Planning的GenStudio工作區中，您可以及無法管理的專案限制。

<!--maybe make 2 sections here once Iskuhi answers - one for one instance and one for multiple WF instances??-->

<!--add here a link from the GenS articles about what you can/ cannot do from GenStudio that might in the end reflect in Planning - this should come from the GenS team-->

### Workfront Planning中的GenStudio工作區

* GenStudio工作區會在Workfront Planning中顯示視覺指示器，將其識別為代表GenStudio for Performance Marketing工作區。

  Planning中的![GenStudio卡](assets/genstudio-card-with-tag-highlighted.png)

  如需詳細資訊，請參閱[在Adobe Workfront規劃中管理GenStudio工作區](/help/quicksilver/planning/planning-and-genstudio-integration/manage-gen-studio-workspace-in-planning.md)。
* 當您在Planning中擁有GenStudio工作區的管理許可權時，您可以：

   * 更新Planning中的GenStudio工作區（名稱、說明、圖示）
   * 建立區段
   * 新增記錄型別
   * 與其他人共用

     您可以與沒有GenStudio帳戶的其他人共用GenStudio工作區。 您只能與組織之Identity Management系統(IMS)中的可用使用者共用。<!--check to see this is correct-->
     <!--* Delete the workspace - check to see if this is possible; the link is there, but???-->

* 當您在Planning中擁有GenStudio工作區的貢獻許可權時，您無法從Workfront Planning修改工作區。

### GenStudio工作區中的記錄型別

* 在GenStudio for Performance Marketing和Planning中可見的記錄型別在Workfront Planning中具有GenStudio指標。

  Workfront Planning中的![GenStudio記錄型別卡片](assets/genstudio-record-type-with-tag-and-tooltip-highlighted.png)
* 當您在Planning中擁有GenStudio工作區的「管理」許可權時，您可以從Workfront Planning執行下列作業：
   * 編輯GenStudio記錄型別資訊（其外觀、進階設定）。
   * 與其他人共用GenStudio記錄型別。
   * 建立記錄型別。 這些記錄型別僅保留在Workfront Planning中。 它們不會顯示在GenStudio中。
* 當您在Planning中擁有GenStudio工作區的「貢獻」許可權時，您無法從Planning中修改GenStudio記錄型別。

### GenStudio工作區中的記錄

* 當您從GenStudio for Performance Marketing編輯GenStudio記錄時，在GenStudio工作區中，所有Workfront例項中皆可看見變更。
* 您無法從Workfront Planning的GenStudio工作區中建立或刪除啟用記錄。
* 當您在Planning中擁有GenStudio工作區的「管理」或「貢獻」許可權時，您可以從Workfront Planning執行下列動作：
   * 新增或刪除記錄，記錄便會顯示於GenStudio for Performance Marketing中（或從中移除）。

     Workfront Planning或GenStudio for Performance Marketing中的已刪除記錄會放入Workfront Planning最近刪除的資料匣中30天。 GenStudio for Performance Marketing沒有最近刪除的bin。
   * 從最近刪除的資料匣還原記錄。 還原已刪除的記錄會將其放回Workfront Planning和GenStudio for Performance Marketing。
   * 以下列方式新增記錄：

      * 使用「新增記錄」按鈕，從任何檢視手動從頭開始
      * 透過在表格檢視中使用CSV或Excel檔案匯入它們
      * 手動，在Workfront Planning的任何檢視中
      * 透過在Workfront中向記錄型別請求表單提交請求。

  如需詳細資訊，請參閱[建立記錄](/help/quicksilver/planning/records/create-records.md)。
* 您可以在Workfront Planning中編輯GenStudio工作區中所有記錄的記錄資訊。

  如需詳細資訊，請參閱[編輯記錄](/help/quicksilver/planning/records/edit-records.md)。

### GenStudio工作區中的記錄型別欄位

* 依預設，記錄型別欄位會從GenStudio for Performance Marketing匯入至Workfront Planning。
* 您無法從GenStudio for Performance Marketing新增欄位以記錄型別。
<!--Iskuhi said this is not possible but I can add fields: * You cannot create or delete Activation records' fields from the GenStudio workspace in Workfront Planning. -->
* 當您在Planning中擁有GenStudio工作區的「管理」許可權時，您可以從Workfront Planning執行下列作業：

   * 編輯GenStudio欄位設定。
   * 如果您在Gen Studio工作區中擁有「管理」存取權，請建立GenStudio記錄型別的欄位。

     當您在Planning中為GenStudio記錄型別建立欄位時，可從下列區域看到這些欄位：

      * Workfront Planning檢視
      * Workfront Planning記錄詳細資訊頁面
      * GenStudio記錄詳細資料頁面

     >[!TIP]
     >
     >在Workfront Planning中建立的欄位不會顯示在GenStudio清單檢視中。

   * 在Workfront Planning中隱藏GenStudio記錄型別的表格檢視中的欄位。
&lt;！—*從Workfront Planning中刪除在Workfront Planning中為GenStudio記錄型別建立的欄位。  — 根據Iskuhi，這是不可能的；連結在那裡但會產生錯誤 — >

  <!--this is not true: You cannot delete fields imported from GenStudio from Workfront Planning.-->

* 當您在Planning中擁有GenStudio工作區的貢獻許可權時：

   * 您無法在Workfront Planning中編輯欄位設定、刪除或新增來自GenStudio工作區的欄位。
   * 您可以在Workfront Planning的表格檢視中隱藏欄位。

#### 建立者與核准者欄位

* 您可以從Workfront Planning為Workfront Planning中的GenStudio記錄型別新增「建立者」和「核准者」欄位。
* 在「管道」和「地區」記錄型別中顯示的記錄會將「系統」顯示為「建立者」。 在Workfront Planning中建立GenStudio工作區時，會自動建立這些記錄。
* 工作區在Workfront Planning中可供使用後，在GenStudio中建立的記錄將顯示在「建立者」欄位中建立記錄的IMS使用者名稱，即使該使用者在GenStudio中建立記錄且不是Workfront使用者。
* 當在Workfront Planning中提交請求表單以在GenStudio記錄型別中建立記錄時，「核准者」欄位會顯示核准者的名稱。
* 「建立者」和「核准者」欄位會顯示在GenStudio for Performance Marketing的記錄詳細資料中。 它們不會顯示在清單檢視中。

### 在GenStudio工作區中記錄檢視

>[!NOTE]
>
>GenStudio記錄型別會顯示在從GenStudio for Performance Marketing清單檢視匯入的預設表格檢視中。
>
>您無法刪除預設從GenStudio for Performance Marketing匯入的原始表格檢視。

* 您無法在GenStudio for Performance Marketing中建立多個檢視。

* 當您在Planning中擁有GenStudio工作區的「管理」許可權時，您可以從Workfront Planning執行下列作業：

   * 建立GenStudio記錄型別的檢視。

     如需詳細資訊，請參閱[管理記錄檢視](/help/quicksilver/planning/views/manage-record-views.md)。

   * 重新命名、共用、匯出、複製或刪除GenStudio記錄型別中的任何自訂檢視。

* 當您在Planning中擁有GenStudio工作區的「貢獻」許可權時，您可以從Workfront Planning執行下列作業：

   * 建立GenStudio記錄型別的檢視。

     如需詳細資訊，請參閱[管理記錄檢視](/help/quicksilver/planning/views/manage-record-views.md)。

   * 重新命名、匯出、複製或刪除GenStudio記錄型別的自訂檢視。

     您無法在Workfront Planning中從GenStudio工作區共用檢視

### 在GenStudio工作區中記錄連線

您可以在您擁有管理許可權的GenStudio工作區中，建立不同記錄型別之間的連線。

您可以在GenStudio記錄型別與Workfront Planning中的其他記錄或物件型別之間建立下列連線：

* 兩種GenStudio記錄型別
* 來自相同工作區的GenStudio記錄型別和Planning記錄型別
* 來自另一個工作區的GenStudio記錄型別和Planning記錄型別（如果記錄型別設定為從另一個工作區連線）。
* GenStudio記錄型別和Workfront物件型別（專案、投資組合、方案、公司、群組）
* GenStudio記錄型別和AEM Assets物件型別。

### GenStudio記錄型別的請求表單和自動化

* 您可以在Workfront Planning中將請求表單新增至GenStudio記錄型別。

  如需詳細資訊，請參閱[在Adobe Workfront Planning中建立和管理要求表單](/help/quicksilver/planning/requests/create-request-form.md)。
* 您可以在Workfront Planning中設定GenStudio記錄型別的自動化。

  如需詳細資訊，請參閱[設定Adobe Workfront規劃自動化](/help/quicksilver/planning/records/configure-automations-to-create-records.md)。

## 預覽環境

* 可從生產環境存取的GenStudio工作區也會顯示在同一Workfront執行個體的預覽環境中。
* 您可以在預覽環境的Workfront Planning中，於GenStudio工作區上執行本文所述的所有活動，但這些變更不會從GenStudio中顯示。

  只有您對生產環境中的專案所做的變更，才會在Workfront Planning和GenStudio之間同步。

  GenStudio沒有預覽環境。

