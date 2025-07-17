---
title: 歷史記錄區段總覽
description: 您可以在Adobe Workfront Planning的右側記錄面板中，檢閱系統記錄的變更和記錄。
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 8258589f-a7c3-4d77-9abe-c99e9184bd21
source-git-commit: 298c542afea902d9fc14ef6a4470c0bc1d9bd33c
workflow-type: tm+mt
source-wordcount: '658'
ht-degree: 3%

---

# 歷史記錄區段總覽

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers, or in the Production environment for customers who enabled fast releases.</span>

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>-->

{{planning-important-intro}}

您可以在記錄的右側面板中新增評論或回覆，對Adobe Workfront Planning記錄進行共同作業。 您也可以在此區域中檢視系統記錄的其它變更。

記錄的右側面板會顯示下列區段：

* **註解**：顯示註解及使用者新增至記錄的回覆。 如需有關管理Workfront Planning記錄中的註解的詳細資訊，請參閱[管理記錄註解](/help/quicksilver/planning/records/manage-record-comments.md)。
* **歷程記錄**：顯示使用者對記錄欄位所做的系統記錄變更。

## 存取需求

+++ 展開以檢視存取需求。

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
   <li><p> Adobe Workfront規劃<p></li></ul></td> 
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
   <td role="rowheader"><p>Adobe Workfront規劃套件*</p></td> 
   <td> 
<p>任何 </p> 
<p>如需每個Workfront計畫包含內容的詳細資訊，請聯絡您的Workfront客戶經理。 </p> 
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
   <td role="rowheader"><p>Adobe Workfront授權*</p></td> 
   <td> <p>投稿人或更高授權</p>
   <p>Workfront計畫不適用於舊版Workfront授權</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>存取層級設定</p></td> 
   <td> <p>Adobe Workfront Planning沒有存取層級控制</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>物件許可權</p></td> 
   <td>   <p>檢視或更高的工作區許可權並記錄型別</a> </p>  
   <p>系統管理員擁有所有工作區的許可權，包括他們未建立的工作區</p> </td> 
  </tr> 
<tr>
   <td role="rowheader"><p>版面配置範本</p></td>
   <td> 必須為具有輕度或貢獻者授權的使用者指派包含Planning的版面配置範本。
   <p>標準使用者和系統管理員預設會啟用Planning區域。</p></div></li></ul>

</td>
  </tr>
</tbody> 
</table>

*如需Workfront存取需求的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 找出記錄的「歷史記錄」區段

{{step1-to-planning}}

1. 按一下工作區的卡片。

   工作區隨即開啟，且記錄型別會顯示在卡片上。

1. 按一下記錄型別卡。
記錄型別頁面隨即開啟，並顯示該型別的所有記錄。

1. 從任何檢視中，按一下記錄名稱。

   記錄的頁面隨即開啟。 「註解」區域預設會在右側面板中開啟。
1. 按一下&#x200B;**顯示歷程記錄**&#x200B;圖示![顯示歷程記錄圖示](assets/show-history-icon.png)。 對記錄欄位所做的所有變更都會顯示在右側面板中，從最近的變更開始。
1. （選擇性）按一下&#x200B;**隱藏歷程記錄**&#x200B;圖示![隱藏歷程記錄圖示](assets/hide-history-icon.png)以關閉右側面板。

## 關於「歷史記錄」段落的考量事項

您可以在記錄頁面的右側面板的「歷史記錄」區段中，檢閱對記錄欄位所做的變更。

![註解中的歷程記錄區域](assets/history-area-in-comments.png)

* Workfront Planning會在「歷史記錄」區段中記錄下列資訊：

   * 任何欄位變更

   * 當值變更時，欄位的舊值和新值。 舊值會以刪除線格式顯示。

   * 進行變更的使用者全名

   * 變更發生的日期和時間戳記。

* 下列型別的欄位一律會顯示舊值（以刪除線格式）和新值：

   * 文字
   * 段落
   * 貨幣
   * 日期
   * 數字
   * 百分比
   * 單選

* 只有在刪除了多個值中的至少一個時，以下型別的欄位才會以刪除線格式顯示舊值：

   * 多選
   * 連結的記錄欄位
   * 人員

  如果變更僅新增值至欄位，則不會顯示舊值，而只會顯示新欄位值。

* 核取方塊型別的欄位絕不會以刪除線格式顯示舊值。 如果欄位已編輯，則只顯示進行變更時的目前狀態。

  如需Workfront Planning欄位的詳細資訊，請參閱[建立欄位](/help/quicksilver/planning/fields/create-fields.md)。

* 下列型別的欄位變更不會顯示在「歷史記錄」區段中：

   * 連結（查詢）欄位
   * 公式
   * 建立者
   * 建立日期
   * 上次修改者
   * 上次修改日期

* 如果欄位從系統中移除，對該欄位所做的更新會保留在「歷史記錄」區段中。 沒有跡象顯示欄位在記錄的History區段中已移除。
