---
title: 建立記錄型別
description: 記錄型別是Adobe Workfront Planning的物件型別。 在Workfront Planning中，您可以建立自訂記錄型別，以說明組織生命週期中所需的工作專案。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: ed1c4954-b338-4865-a7a9-5ba0192e7b37
source-git-commit: 4569b5bd004a93396257f3f1f8964831f69399dc
workflow-type: tm+mt
source-wordcount: '1102'
ht-degree: 2%

---


<!--this is linked to the UI in an empty workspace screen-->

# 建立記錄型別

<!--<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

記錄型別是Adobe Workfront Planning的物件型別。 在Workfront Planning中，您可以建立自訂記錄型別，以說明組織生命週期中所需的工作相關專案。

如需有關記錄型別的詳細資訊，請參閱[記錄型別概觀](/help/quicksilver/planning/architecture/overview-of-record-types.md)。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。 

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
<ul><li>選擇</li> 
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
</tbody> 
</table>

*如需Workfront存取需求的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++   

## 建立記錄型別的相關考量事項

* 您可以透過下列方式在工作區中建立記錄型別：

   * 自動：
      * 使用範本建立工作區時。

        如需詳細資訊，請參閱[建立工作區](/help/quicksilver/planning/architecture/create-workspaces.md)。

      * 當您使用CSV或Excel檔案匯入時。

        如需詳細資訊，請參閱[從CSV或Excel檔案匯入資訊，以建立記錄型別](/help/quicksilver/planning/architecture/import-file-to-create-record-types.md)。

     >[!TIP]
     >
     >從CSV或Excel檔案匯入記錄型別時，您也可以匯入記錄和欄位。

   * 手動：

      * 從頭開始。

        本文說明如何從頭開始建立記錄型別。

     <!--
        * <span class="preview">By importing them from another workspace or adding cross-workspace record types</span>
            <span class="preview">For information, see [Add existing record types](/help/quicksilver/planning/architecture/add-cross-workspace-record-types.md). </span>-->


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
1. 按一下&#x200B;**新增記錄型別**，然後按&#x200B;**手動新增**。

   「新增記錄型別」方塊開啟。
   <!--1. (Conditional) When creating record types by importing an Excel or CSV file is enabled, click **From scratch**. Otherwise, the **Add record type** box opens. -->

   ![新增具有外觀選項的記錄型別方塊](assets/add-record-type-box-with-appearance-options.png)

1. 更新&#x200B;**外觀**&#x200B;標籤上的下列資訊：

   * 將「未命名的記錄型別」取代為您未來記錄型別的名稱。<!--did they bring back the field label here and did they rename it to "Name"-->
   * **描述**：新增記錄型別的詳細資訊。
   * 為與記錄型別關聯的圖示選取顏色和形狀。 請執行下列動作：
      * 選取顏色以識別您的新記錄型別。 這是記錄型別圖示的顏色。 預設會選取「灰色」。
      * 從清單中選取圖示，或開始輸入圖示名稱以說明其代表內容，然後在顯示時選取它。 這是記錄型別的圖示。 依預設，會選取檔案圖示。


   <!--old setting:
    1. (Optional and conditional) If you are a system administrator, click **Advanced settings** and update the following information in the **Connectivity scope** section: 
        * Enable the **Connect from other workspace** setting. When enabled, the record type is accessible and can be connected from other workspaces. 
        * Choose from which workspaces the record type can be accessed. Choose from the following options:
            * **System wide**: Users can connect to this record type from all workspaces where they have manage permissions. 
            * **Specific workspaces**: Add the names of the workspaces where workspace managers can connect to this record type. 
    -->

1. （選擇性和條件性）如果您是系統管理員，請按一下&#x200B;**進階設定**，並更新&#x200B;**跨工作區功能**&#x200B;區段中的下列資訊： <!--the info here is duplicated in the Edit record types article-->
   * 啟用&#x200B;**允許連線到其他工作區中的這個記錄型別**&#x200B;設定：這可讓工作區管理員從其他工作區連線到這個記錄型別。\
     您可以指定此記錄型別可以連線哪些工作區。 您可以使其可用於所有工作區，或指定可匯入其的特定工作區。
如需詳細資訊，請參閱[設定記錄型別的跨工作區功能](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md)。


   ![在進階設定索引標籤上建立記錄型別方塊](assets/create-record-type-box-advanced-settings-tab.png)

   <!--replace last point with this when we release dynamic record types; the preview tags might need to be edited, too:
        <div class="preview">
        1. (Optional and conditional) If you are a system administrator, click **Advanced settings** and update the following information in the **Cross-workspace capability** section: **** the info here is duplicated in the Edit record types article ***
            * Enable the **Allow adding this record type to other workspaces** setting: This allows workspace managers to add this record type to other workspaces. 
                You can designate specific users who can add this record type to other workspaces. 
            * Enable the **Allow connecting to this record type in other workspaces** setting: This allows workspace managers to connect to this record type from other workspaces.  
                You can designate which workspaces this record type can be connected from. You can make it available for all workspaces or designate specific ones where you can import it.
            For more information, see [Configure cross-workspace capabilities for record types](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md).  </div>
            ******** replace screen shot below **********
            ![Create record type box on advanced settings tab](assets/create-record-type-box-advanced-settings-tab.png) 
        -->

1. 按一下「**儲存**」。

   記錄型別卡片會新增至區段以及您選取的工作區。
記錄型別的「說明」會顯示在卡片上。

   ![含有說明的記錄型別卡片](assets/record-type-card-with-description.png)

   如果您選擇從其他工作區連線此記錄，記錄卡上會顯示&#x200B;**從其他工作區連線**&#x200B;圖示![從其他工作區連線圖示](assets/connect-from-other-workspaces-icon.png)。

   <!--<span class="preview">If you configured the cross-workspace capabilities for the record, the **connect from other spaces** icon ![Connect record type from other spaces icon](assets/connect-from-other-workspaces-icon.png) and the **add to other workspaces** icon ![Add record type to other workspaces](assets/global-icon.png) also display on the card. </span>-->

1. （選擇性）將滑鼠停留在記錄型別卡片上，按一下右上角的&#x200B;**更多**&#x200B;圖示![更多功能表](assets/more-menu.png)，然後按一下&#x200B;**編輯**&#x200B;以修改有關記錄型別的資訊。
1. （選擇性）按一下記錄型別卡片以開啟記錄型別頁面。

   ![作業記錄型別空白](assets/operational-record-type-blank.png)

   記錄型別頁面預設會顯示在表格檢視中。 表格的欄是與新記錄型別相關聯的欄位。 每一列都是您必須新增的唯一記錄。

   依預設，下列欄位會顯示在作業記錄型別的表格檢視欄中：

   * 姓名
   * 說明
   * 開始日期
   * 結束日期
   * 狀態

1. （選用）更新頁面標頭中的記錄型別名稱

   或

   按一下記錄型別名稱右邊的&#x200B;**更多**&#x200B;圖示![更多功能表](assets/more-menu.png)，然後按一下&#x200B;**編輯**&#x200B;以重新命名或變更相關資訊。 如需詳細資訊，請參閱[編輯記錄型別](/help/quicksilver/planning/architecture/edit-record-types.md)。

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

## 從CSV或Excel檔案匯入資訊，建立記錄型別

從CSV或Excel檔案匯入資訊時，您可以匯入下列內容：

* 記錄類型
* 記錄
* 記錄欄位

如需詳細資訊，請參閱[從CSV或Excel檔案匯入資訊，以建立記錄型別](/help/quicksilver/planning/architecture/import-file-to-create-record-types.md)。

<!--

<div class="preview">

## Create record types by importing them from another workspace 

You can add record types to a workspace by importing them from another workspace. You can only add record types that have been configured as centralized record types. 

For information, see [Add existing record types](/help/quicksilver/planning/architecture/add-cross-workspace-record-types.md).

</div>

-->