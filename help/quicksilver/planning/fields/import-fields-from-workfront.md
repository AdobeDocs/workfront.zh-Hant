---
title: 從Adobe Workfront匯入欄位
description: 在Adobe Workfront Planning中，您可以為每種記錄型別建立自訂欄位。 然後，您可以將此欄位與Workfront Planning記錄建立關聯。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
source-git-commit: 0da877936ba8f52341a5b151f76710c979ce9294
workflow-type: tm+mt
source-wordcount: '718'
ht-degree: 7%

---


<!--add to TOC-->

# 從Adobe Workfront匯入欄位

<span class="preview">此頁面上的資訊是指尚未普遍提供的功能。 它僅在預覽環境中可供所有客戶使用。 每月發行至生產環境後，生產環境中為啟用快速發行的客戶也提供相同的功能。</span>

<span class="preview">如需快速發行資訊，請參閱[為您的組織啟用或停用快速發行](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>


{{planning-important-intro}}

您可以匯入現有Workfront欄位的復本。 從Workfront匯入欄位會為Workfront Planning記錄型別建立每個欄位的副本。


## 存取需求

+++ 展開以檢視Workfront Planning的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

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
<p>貴組織的Workfront例項必須加入Adobe統一體驗，才能存取Workfront規劃的所有功能。</p> 
<p>如需詳細資訊，請參閱<a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Workfront的Adobe統一體驗</a>。 </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront授權*</p></td> 
   <td><p> 標準 </p>
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
   <td>   <p>管理工作區</a>的許可權 </p>  
   <p>系統管理員擁有所有工作區的許可權，包括他們未建立的工作區。</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>版面配置範本</p></td> 
   <td> <p>必須為所有使用者(包括Workfront管理員)指派一個版面配置範本，該範本包含主功能表中的Planning區域。 </p> </td> 
  </tr> 
</tbody> 
</table>

*如需Workfront存取需求的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 有關從Workfront匯入欄位的考量事項

* 您可以在Workfront Planning中將原生或自訂Workfront欄位匯入記錄型別。
* 匯入Workfront欄位會建立相同欄位的復本，並在Workfront Planning中保留欄位名稱。 複製到Workfront Planning後，這些欄位獨立於原始Workfront欄位，不會共用資訊。
<!--check this: * You do not need permissions or access to Workfront objects to be able to add their fields to Workfront Planning. -->
* 您可以從下列Workfront物件新增原生或自訂欄位：
   * 專案組合
   * 方案
   * 專案
   * 任務
   * 問題
   * 文件
   * 公司
   * 群組
   * 使用者
   * 職務角色
   * 指派
   * 小時
   * 計費記錄
     <!--Available only to Preview, but might not come to Prod:* Rate card-->
   * 費用
   * 反覆項目
     <!--* Non-labor resource-->
     <!--* Non-labour resource category-->
* Workfront欄位匯入Workfront Planning後，可能不會保留其欄位型別。

  下表顯示Workfront欄位型別及其對應的Workfront Planning欄位型別。

  | Workfront欄位型別 | Workfront Planning欄位型別 |
  |------------------------------------------|-------------------------------|
  | 文字格式的單行文字 | 單行文字 |
  | 數字格式的單行文字 | 數字 |
  | 貨幣格式的單行文字 | 貨幣 |
  | 段落 | 段落 |
  | 含格式的文字 | 段落 |
  | 單選下拉式清單 | 單選 |
  | 多選下拉式清單 | 多選 |
  | 不支援使用者預先輸入篩選器 | 人員 |
  | 已計算* | 公式 |
  | 日期 | 日期 |
  | 核取方塊群組 | 多選 |
  | 選項按鈕 | 多選 |

  *計算欄位將在稍後提供。
Workfront Planning不支援所有其他Workfront欄位型別。


## 從 Workfront 匯入欄位

<!--the first 3 steps are the same as in Create fields-->

{{step1-to-planning}}

1. 按一下您要為其建立欄位之記錄型別的工作區。

   工作區隨即開啟，且記錄型別隨即顯示。

1. 按一下記錄型別的卡片。

   與記錄型別關聯的所有現有記錄都會顯示在表格檢視的列中。

   >[!TIP]
   >
   >    某些欄位可能已隱藏。 按一下&#x200B;**欄位**&#x200B;並啟用您要在表格檢視中做為欄檢視的欄位切換。

1. 按一下表格檢視右上角的&#x200B;**+**&#x200B;圖示

   或

   將游標暫留在任何欄的標頭上，按一下欄位名稱后面的向下箭頭，然後按一下&#x200B;**插入左側**&#x200B;或&#x200B;**插入右側**&#x200B;以新增欄位。
1. 按一下&#x200B;**新增欄位**&#x200B;索引標籤右下角的&#x200B;**新增現有**。<!--check UI - did they change this??-->

   ![](assets/add-existing-fields-from-workfront-modal.png)

1. 開始在搜尋區域中輸入現有Workfront欄位的名稱，然後按一下清單中顯示&#x200B;**+**。
1. （選擇性）輸入其他欄位，然後在清單中顯示&#x200B;**+**&#x200B;時按一下。
1. （選擇性）按一下&#x200B;**篩選器**&#x200B;圖示![](assets/filters-in-import-fields-icon.png)，然後更新下列一個或兩個欄位：

   * 物件型別：選取您要匯入其欄位的Workfront物件型別。
   * 自訂表單：從Workfront中選取一個或多個自訂表單。 您可以不先選取物件型別而選取自訂表單。
1. 按一下&#x200B;**+**，然後按&#x200B;**新增欄位**。
欄位會新增至表格檢視和記錄的詳細資訊頁面。
