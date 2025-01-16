---
title: 建立記錄型別
description: 記錄型別是Adobe Workfront Planning的物件型別。 在Workfront Planning中，您可以建立自訂記錄型別，以說明組織生命週期中所需的工作專案。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: ed1c4954-b338-4865-a7a9-5ba0192e7b37
source-git-commit: ba17bd824717f61e72fb9a73c8b90fbe755e20d8
workflow-type: tm+mt
source-wordcount: '1394'
ht-degree: 1%

---


<!--this is linked to the UI in an empty workspace screen-->

# 建立記錄型別

<!--<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

記錄型別是Adobe Workfront Planning的物件型別。 在Workfront Planning中，您可以建立自訂記錄型別，以說明組織生命週期中所需的工作相關專案。

如需有關記錄型別的詳細資訊，請參閱[記錄型別概觀](/help/quicksilver/planning/architecture/overview-of-record-types.md)。

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
   <td><p> 標準</p>
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
   <p>系統管理員擁有所有工作區的許可權，包括他們未建立的工作區</p>  </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>版面配置範本</p></td> 
   <td> <p>必須為所有使用者(包括Workfront管理員)指派一個版面配置範本，該範本包含主功能表中的Planning區域。 </p> </td> 
  </tr> 
</tbody> 
</table>

*如需Workfront存取需求的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++


## 建立記錄型別的相關考量事項

* 您可以透過下列方式在工作區中建立記錄型別：

   * 自動：
      * 使用範本建立工作區時。

        如需詳細資訊，請參閱[建立工作區](/help/quicksilver/planning/architecture/create-workspaces.md)。

      * 當您使用Excel或CSV檔案匯入時。

     >[!TIP]
     >
     >從Excel或CSV檔案匯入記錄型別時，您也可以匯入記錄和欄位。

   * 手動：

      * 從頭開始。

        本文說明如何從頭開始建立記錄型別。

* 您可以在區段內以及工作區一個區段之間移動記錄型別。 您無法將記錄型別從一個工作區移動到另一個工作區。

## 使用工作區範本建立記錄型別

使用Workfront Planning範本建立工作區時，您可以自動建立記錄型別。 每個範本都包含範例記錄型別。

從範本建立工作區時，記錄型別會分組到下列區段中：

* 作業記錄型別
* 分類法

您可以在「作業記錄型別」與「分類」段落中手動新增記錄型別。

如需有關建立工作區的資訊，請參閱[建立工作區](/help/quicksilver/planning/architecture/create-workspaces.md)。

如需每個範本包含哪些記錄型別的詳細資訊，請參閱[工作區範本清單](/help/quicksilver/planning/architecture/workspace-templates.md)。

## 從頭開始建立記錄型別

{{step1-to-planning}}

1. 按一下您要建立記錄型別的工作區，

   或

   從工作區中，展開現有工作區名稱右側的向下箭頭，搜尋工作區，然後在工作區顯示在清單中時選取該工作區。
1. （選擇性）按一下&#x200B;**新增區段**&#x200B;以新增區段至工作區。
1. 按一下&#x200B;**新增記錄型別**，然後按&#x200B;**新增**。

   「新增記錄型別」方塊開啟。
   <!--1. (Conditional) When creating record types by importing an Excel or CSV file is enabled, click **From scratch**. Otherwise, the **Add record type** box opens. -->

   ![](assets/add-record-type-box-with-appearance-options.png)

1. 更新下列資訊：

   * 將「未命名的記錄型別」取代為您未來記錄型別的名稱。<!--did they bring back the field label here and did they rename it to "Name"-->
   * **描述**：新增記錄型別的詳細資訊。
   * 為與記錄型別關聯的圖示選取顏色和形狀。 執行下列動作：
      * 選取顏色以識別您的新記錄型別。 這是記錄型別圖示的顏色。 預設會選取「灰色」。
      * 從清單中選取圖示，或開始輸入圖示名稱以說明其代表內容，然後在顯示時選取它。 這是記錄型別的圖示。 依預設，會選取檔案圖示。

1. 按一下「**建立**」。

   記錄型別卡片會新增至區段以及您選取的工作區。
記錄型別的「說明」會顯示在卡片上。

   ![](assets/record-type-card-with-description.png)

1. （選擇性）將滑鼠停留在記錄型別卡片上，按一下右上角的&#x200B;**更多**&#x200B;圖示![](assets/more-menu.png)，然後按一下&#x200B;**編輯**&#x200B;以修改有關記錄型別的資訊。
1. （選擇性）按一下記錄型別卡片以開啟記錄型別頁面。

   ![](assets/operational-record-type-blank.png)

   記錄型別頁面預設會顯示在表格檢視中。 表格的欄是與新記錄型別相關聯的欄位。 每一列都是您必須新增的唯一記錄。

   依預設，下列欄位會顯示在作業記錄型別的表格檢視欄中：

   * 姓名
   * 說明
   * 開始日期
   * 結束日期
   * 狀態

1. （選用）更新頁面標頭中的記錄型別名稱

   或

   按一下記錄型別名稱右側的&#x200B;**更多**&#x200B;圖示![](assets/more-menu.png)，然後按一下&#x200B;**編輯**&#x200B;以重新命名或變更相關資訊。 如需詳細資訊，請參閱[編輯記錄型別](/help/quicksilver/planning/architecture/edit-record-types.md)。

1. （選擇性）按一下&#x200B;**+新記錄**&#x200B;以新增所選記錄型別的記錄。 如需詳細資訊，請參閱[建立記錄](/help/quicksilver/planning/records/create-records.md)。
1. （選擇性）按一下表格右上角的&#x200B;**+**&#x200B;圖示，將更多欄位新增至記錄型別。

   如需有關建立欄位的詳細資訊，請參閱[建立欄位](/help/quicksilver/planning/fields/create-fields.md)。

1. （可選）在標題中，按一下記錄型別名稱左側的向左箭頭，返回選取的工作區。

1. （選擇性）在工作區中，按一下並按住記錄型別卡片，以將記錄型別拖放到所需位置，或將其移動到其他區段。

   變更會自動儲存。

   如需有關在記錄型別頁面中新增記錄、刪除或編輯記錄型別或更新檢視的其他資訊，請參閱下列文章：

   * [建立記錄](/help/quicksilver/planning/records/create-records.md)
   * [刪除記錄型別](/help/quicksilver/planning/architecture/delete-record-types.md)
   * [編輯記錄型別](/help/quicksilver/planning/architecture/edit-record-types.md)
   * [管理記錄檢視](/help/quicksilver/planning/views/manage-record-views.md)

## 匯入Excel或CSV檔案來建立記錄型別

使用Excel或CSV檔案匯入記錄型別時，請考量下列事項：

* Excel檔案的每一頁都會變成記錄型別。 工作表的名稱會變成記錄型別的名稱。
* 如果只有一張工作表，或者如果匯入CSV檔案，則檔案的名稱會變成記錄型別的名稱。
* 每個工作表的欄標題會成為與每個記錄型別相關聯的欄位。
* 欄位對於其各自的記錄型別來說都是唯一的。
* 每個工作表中的每一列都會成為與其個別記錄型別相關聯的唯一記錄。
* 每個Excel檔案工作表不應超過下列專案：
   * 10,000列
   * 500欄
* Excel檔案不應大於5MB。
* 不支援空白工作表。

若要使用Excel或CSV檔案匯入記錄型別：

{{step1-to-planning}}

1. 按一下您要建立記錄型別的工作區，

   或

   從工作區中，展開現有工作區名稱右側的向下箭頭，搜尋工作區，然後在工作區顯示在清單中時選取該工作區。
1. 按一下&#x200B;**新增記錄型別**。
1. 按一下&#x200B;**從檔案**。
1. 拖放先前儲存在電腦上的Excel或CSV檔案，或按一下&#x200B;**選取CSV或Excel檔案**&#x200B;以瀏覽檔案。
1. 按一下&#x200B;**預覽和編輯**。

   **預覽和編輯**&#x200B;方塊會顯示下列資訊：

   * 工作表或未來記錄型別的名稱會顯示在左側面板中。 根據預設，Workfront Planning會選取每個新記錄型別的圖示和顏色。
   * 選擇第一個工作表或記錄型別，並且與其關聯的欄位名稱顯示為欄標題。 依預設，會選取每個欄位的型別。
   * 每一列代表新記錄。 只有前10筆記錄會顯示在「預覽與編輯」方塊中。

   ![](assets/preview-and-edit-box.png)

1. （選擇性）按一下左側面板中每個工作表的名稱，以檢閱其中包含的資訊。

   >[!NOTE]
   >
   >不支援空白的頁面，這些頁面會變暗。

1. （選擇性）從左側面板取消選取您不想要匯入的頁面。

   ![](assets/select-sheets-to-import-drop-down-with-unselected.png)

   取消選取的頁面會以灰色背景顯示。

1. （選擇性）按一下欄標題右側的向下箭頭，執行下列任一項作業：

   * 重新命名其中一個欄位
   * 變更&#x200B;**欄位型別**
   * 更新欄位&#x200B;**描述**

1. （視條件而定）更新欄位相關資訊後，按一下&#x200B;**儲存**。

1. 當您準備好匯入您的檔案時，請按一下[匯入]。****

   下列資訊會匯入Workfront Planning中：

   * 新記錄型別
   * 與每個記錄型別關聯的新欄位
   * 與每個記錄型別關聯的新記錄

   您可以開始管理記錄型別頁面上的欄位和記錄。

   所有有權存取Workfront Planning的人員現在都能檢視及編輯匯入的記錄型別及其資訊。
