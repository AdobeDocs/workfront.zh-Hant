---
title: 在Adobe Workfront物件的Planning區段中管理記錄
description: 您可以在左側面板的Workfront物件的Planning區段中，顯示連線至Adobe Workfront物件的Workfront Planning記錄。
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: d86cf3f9-cacc-4457-acb3-a5122ae91be8
source-git-commit: 9debb7c6d9df0f9f4962f3e66f146e5f605d20f0
workflow-type: tm+mt
source-wordcount: '798'
ht-degree: 1%

---


<!--add also Group and Company when they are available-->

# 在Adobe Workfront物件的Planning區段中管理記錄

{{planning-important-intro}}

您可以在左側面板的Workfront物件的Planning區段中，顯示連線至Adobe Workfront物件的Workfront Planning記錄。

「規劃」區段適用於下列Workfront物件：

* 專案
* 專案組合
* 方案
<!--* Group
* Company-->

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
   <td role="rowheader"><p>Adobe Workfront規劃計畫*</p></td>
   <td>
<p>任何</p>
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
   <td>
   <p>標準</p>
   <p>Workfront計畫不適用於舊版Workfront授權</p>
  </td>
  </tr>
  <tr>
   <td role="rowheader"><p>存取層級設定</p></td>
   <td> <p>檢視專案、方案和Portfolio的或更高存取權</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>物件許可權</p></td>
   <td>
   <p>在Workfront中，檢視專案、投資組合或方案的或更高許可權</a> </p> 
   <p>在Workfront Planning中，使用Contribute或更高的工作區許可權</a> </p>  
   <p>系統管理員擁有所有Workfront Planning工作區的許可權，包括他們未建立的工作區</p> 
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>版面配置範本</p></td>
   <td> <p>必須為所有使用者(包括Workfront管理員)指派一個版面配置範本，該範本包含主功能表中的「規劃」區域，以及專案、投資組合和方案的「規劃」區域。 </p> 如需詳細資訊，請參閱<a href="/help/quicksilver/planning/access/access-overview.md">存取總覽</a>。 </p>  </p>  
</td>
  </tr>
 </tbody>
</table>

*如需Workfront存取需求的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 關於Workfront物件Planning區段的考量事項

當您從Workfront物件的Planning區段檢視Workfront Planning記錄時，請考量下列事項：

* Workfront Planning記錄型別必須先連線至Workfront物件型別。

  如需詳細資訊，請參閱下列文章：

   * [連線記錄型別](/help/quicksilver/planning/architecture/connect-record-types.md)
   * [連接記錄](/help/quicksilver/planning/records/connect-records.md)
* 您可以從Workfront物件檢視Planning區段，即使沒有與Workfront物件相關聯的記錄亦然。
* 除了從Workfront的Planning區域連線Workfront物件之外，您還可以從Planning區段將Planning記錄與Workfront的Workfront物件連線。

## 管理Planning區段中的記錄

{{step1-to-planning}}

1. 按一下工作區的卡片。

   工作區隨即開啟，且記錄型別會顯示為卡片。

1. 按一下連線到Workfront專案、投資組合或方案的記錄型別的卡片。
1. 在表格檢視或記錄的詳細資訊頁面中，移至與Workfront物件有連線的已連線記錄欄位。 如需詳細資訊，請參閱[連線記錄](/help/quicksilver/planning/records/connect-records.md)。
1. 在連線的記錄欄位中按一下Workfront物件的名稱。
物件的頁面會在Workfront中開啟。

   >[!NOTE]
   >
   >  如果您知道Workfront物件已連線至Planning記錄，則可以從Workfront物件導覽至Planning區段。

1. 按一下左側面板中的&#x200B;**規劃**。

   >[!NOTE]
   >
   >   您的Workfront或群組管理員必須先將Planning區段新增到您的版面配置範本中，才能為Workfront專案、投資組合或方案顯示該區段。

   Planning區段會顯示下列資訊：

   * 連線的記錄會顯示在包含以下資訊的個別卡片上：
      * 記錄名稱
      * 記錄縮圖
      * 在Workfront Planning中顯示的連線記錄欄位名稱。
   * 記錄會顯示在各自的工作區下。

   ![](assets/planning-section-on-project.png)

1. （選擇性）按一下[顯示所有連線]****&#x200B;以顯示所有連線的記錄型別，包括沒有連線記錄的記錄型別。 依預設，不顯示沒有連線記錄的記錄型別。
1. 按一下記錄卡以顯示有關記錄的更多資訊。 記錄預覽方塊隨即顯示。
1. （選用）開始修改記錄預覽方塊中的欄位。 您的變更會自動儲存。
1. （選擇性）按一下預覽方塊右上角的&#x200B;**在新索引標籤中開啟**&#x200B;圖示![](assets/open-details-in-a-new-tab-icon.png)以開啟記錄的詳細資訊頁面。 記錄的詳細資訊頁面會在Workfront Planning中開啟。
1. （選擇性）將游標停留在記錄卡上，然後按一下中斷連線記錄圖示&#x200B;**-**，然後按一下&#x200B;**中斷連線**。
會發生下列情況：
   * 記錄不再連線至Workfront物件。
   * Workfront物件也會從Workfront Planning的記錄連線欄位中移除。
   * 連線至Planning記錄的Workfront查閱欄位值也會一併刪除。
1. 按一下&#x200B;**連線**，為連線的記錄型別連線更多記錄。 如需詳細資訊，請參閱[連線記錄](/help/quicksilver/planning/records/connect-records.md)。

   會發生下列情況：

   * 記錄會立即連線至Workfront物件，並顯示在Planning區段中。
   * Workfront物件會新增至Workfront Planning記錄的已連線欄位。
   * 與Planning記錄連線之Workfront查詢欄位的值會填入Workfront Planning中。


