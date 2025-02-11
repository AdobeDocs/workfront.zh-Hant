---
title: 建立記錄
description: 使用Adobe Workfront Planning時，記錄是記錄型別的例項。 您可以在Workfront Planning中為每個記錄型別建立唯一的記錄，方法是手動將它們新增至表格檢視、從清單匯入它們、複製它們，或在將它們連線至其他記錄時建立它們。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: c7de4b1f-674b-424b-af64-a6df62fb738f
source-git-commit: 928ea5da9955b8c1c98782df81698c49987d4c18
workflow-type: tm+mt
source-wordcount: '1562'
ht-degree: 0%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->

# 建立記錄

<!--<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

在Adobe Workfront Planning中，記錄是記錄型別的例項。

您可以執行下列其中一項作業來建立記錄：

* [從表格檢視中的記錄型別頁面新增記錄](#create-records-by-adding-them-to-a-record-type-in-a-record-type-table)
* [從外部清單複製並貼上記錄清單](#create-records-by-copying-and-pasting-them-from-an-external-list)
* [從表格檢視複製記錄](#create-records-by-duplicating-them)
* [從其他記錄連線記錄時建立記錄](#create-records-as-you-connect-them)
* [透過提交請求表單到記錄型別來建立它們](#create-records-by-submitting-a-request-form-to-a-record-type)
* [從CSV或Excel檔案匯入記錄型別時建立記錄](#create-records-when-importing-record-types-from-a-csv-or-excel-file)


如需有關管理表格或時間表檢視中的記錄的資訊，請參閱下列文章：

* [管理表格檢視](/help/quicksilver/planning/views/manage-the-table-view.md)
* [管理時間表檢視](/help/quicksilver/planning/views/manage-the-timeline-view.md)

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
   <td> 標準
   <p>Workfront計畫不適用於舊版Workfront授權</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>存取層級設定</p></td> 
   <td> <p>Adobe Workfront Planning沒有存取層級控制</p> 
   <p>將記錄連線至要建立的物件型別（專案與投資組合）時，可在Workfront中編輯其存取權。 </p>  
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>物件許可權</p></td> 
   <td> <p>管理您要新增記錄的工作區的許可權。 </p>  
   <p>系統管理員擁有所有工作區的許可權，包括他們未建立的工作區</p>
   <p>管理Workfront物件（專案組合）的許可權以新增子物件（專案）。</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>版面配置範本</p></td> 
   <td> <p>必須為所有使用者(包括Workfront管理員)指派一個版面配置範本，該範本包含主功能表中的Planning區域 </p> </td> 
  </tr> 
</tbody> 
</table>

*如需Workfront存取需求的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 將記錄新增至記錄型別表格中的記錄型別以建立記錄

您可以在記錄型別頁面的表格檢視中建立記錄。

如需有關編輯記錄資訊的資訊，請參閱[編輯記錄](/help/quicksilver/planning/records/edit-records.md)。

{{step1-to-planning}}

1. 按一下您要新增記錄的工作區。

   工作區隨即開啟，且記錄型別會顯示為卡片。

1. 按一下記錄型別卡。 如需有關建立記錄型別的資訊，請參閱[建立記錄型別](/help/quicksilver/planning/architecture/create-record-types.md)。

   記錄型別頁面會在您上次存取的檢視中開啟。 依預設，會在表格檢視中開啟記錄型別頁面。
所選型別的所有記錄都會顯示在檢視中。

1. （視條件而定）視您顯示的檢視而定，請執行下列其中一項作業：

   * 從表格檢視中：

      * 在表格的最後一列按一下&#x200B;**新增記錄**

      * 在表格的任何欄或列按一下鍵盤上的&#x200B;**Shift + Enter**。 這會在您開始的記錄底下新增一個空白列。
      * 暫留在記錄的主要欄位上，按一下欄位右邊的&#x200B;**更多**&#x200B;功能表![](assets/more-menu.png)，然後按一下&#x200B;**在上方插入記錄**&#x200B;或&#x200B;**在下方插入記錄**。

     ![](assets/adding-a-new-campaign-in-table-row.png)

   * 從任何檢視：

      * 按一下頁面右上角的&#x200B;**新增記錄**。 記錄預覽方塊開啟。

     Workfront會自動上傳縮圖和封面影像至每張新記錄。 您稍後可以修改這些影像。 如需詳細資訊，請參閱下列文章：

      * [新增封面影像至記錄](/help/quicksilver/planning/records/add-a-cover-image-to-a-record.md)
      * [新增縮圖至記錄](/help/quicksilver/planning/records/add-thumbnails-to-records.md)

1. 開始在您在預覽方塊中看到的欄位中輸入有關新記錄的資訊。

   >[!NOTE]
   >
   >  * 記錄沒有必填欄位。 不過，我們建議您為記錄的主要欄位新增資訊，因為將記錄連結至彼此時，識別記錄會很有幫助。 如需主要欄位的詳細資訊，請參閱[管理資料表檢視](/help/quicksilver/planning/views/manage-the-table-view.md)和[主要欄位概述](/help/quicksilver/planning/fields/primary-field-overview.md)。
   >
   >  * 參考其他記錄型別或計算欄位的欄位為唯讀欄位。

1. （視條件而定）在表格中新增記錄時，請繼續在每一列新增資訊，然後在鍵盤上按一下&#x200B;**Enter**&#x200B;以儲存變更。

   或

   按一下新記錄名稱或記錄名稱左側的&#x200B;**開啟詳細資料**&#x200B;圖示![](assets/open-details-icon-in-table-name-field.png)。 含有記錄詳細資訊的預覽會在表格中開啟。

   >[!TIP]
   >
   >當「名稱」欄位是主要欄位時，您只能從記錄的名稱欄位存取&#x200B;**開啟詳細資料**&#x200B;圖示。

1. 開始編輯記錄預覽中的記錄資訊。 Workfront會自動儲存您的變更。
1. （選擇性）按一下記錄預覽右上角的&#x200B;**在新索引標籤中開啟**&#x200B;圖示![](assets/open-details-in-a-new-tab-icon.png)，以在新索引標籤中開啟記錄的頁面。 繼續編輯記錄頁面上的記錄。 如需詳細資訊，請參閱[編輯記錄](/help/quicksilver/planning/records/edit-records.md)。

1. （可選）在表格檢視中新增記錄或其資訊時，請使用下列鍵盤快速鍵來復原或重做新增記錄或其資訊：

   * CTRL + Z (Mac為⌘ + Z)可復原變更
   * CTRL + Shift + Z (Mac為⌘ + Shift + Z)以重做變更

<!-- this is not possible anymore: 

## Create records by connecting them from another application

You can import records from other applications by linking them to existing records. This creates a linked record for the other application's connected object. 

1. Create a record type, as described in the [Create record types](/help/quicksilver/planning/architecture/create-record-types.md).

1. Create records for the record type you created in the previous step. For information, see the section [Create records by manually adding them to a record type](#create-records-by-manually-adding-them-to-a-record-type) in this article. 

1. Create a connection to an object type from another application for the record type you created. For information, see [Connect record types](/help/quicksilver/planning/architecture/connect-record-types.md).

1. Add objects from another application to the records you created above using the linked record field you created in the previous step. For information, see [Connect records](/help/quicksilver/planning/records/connect-records.md). 

    The following items are created in Workfront Planning:

    * A read-only record type that refers to the other application's record type you linked to in the connected record field. 

      For example, if you connect a Planning record type to Workfront project, a read-only record type named "Workfront project" is created in the same workspace. You can access the read-only Workfront record types from the table view of the Planning records you're linking from. 
   
-->

## 從外部清單複製並貼上記錄，以建立記錄

1. 開始在[資料表]檢視中建立記錄，如本文[將記錄手動新增至記錄型別](#create-records-by-manually-adding-them-to-a-record-type)以建立記錄一節中所述。

   確定表格檢視具有您要填入新記錄資訊的欄（或欄位）。

1. 在表格的最後一列按一下&#x200B;**新增&lt;記錄型別名稱>**，新增您想要的新記錄至表格的所有新列。

   例如，如果要從另一個應用程式貼上10筆新記錄的資訊，請將10列新增到表格檢視中。

1. 在另一個應用程式中，建立您要匯入的記錄清單。

   例如，您可以使用Excel試算表來建立清單。

   清單應包含表格格式的資訊。

   >[!TIP]
   >
   > 清單的欄應包含您在Workfront中擁有的現有欄位資訊。
   >
   > 確定您已在Workfront中建立所需欄位，且工作表中的資訊以符合Workfront中每個欄位資訊的正確格式顯示。

1. 從另一個應用程式中，選取數個列和欄，然後將資訊貼到記錄型別表格檢視中，從第一個新記錄開始。

   下列資訊會匯入Workfront Planning區域：

   * 列包含新記錄
   * 欄會填入記錄欄位的資訊。

## 複製記錄以建立記錄

如需複製記錄的資訊，請參閱[複製記錄](/help/quicksilver/planning/records/copy-or-duplicate-records.md)。

## 連線時建立記錄

當您從其他記錄連線下列物件型別時，可以建立這些物件型別：

* Workfront Planning記錄
* Workfront物件

本節說明當您從其他記錄連線時，如何建立Workfront Planning記錄。

>[!NOTE]
>
>當您將Workfront專案與產品組合連線至Workfront Planning記錄時，建立這些專案與產品組合與當您從其他記錄連線時，建立Planning記錄類似。
>
>如需有關從Workfront Planning建立Workfront物件的資訊，請參閱[從Workfront Planning建立Workfront物件](/help/quicksilver/planning/records/create-workfront-objects-from-workfront-planning.md)。

您必須具備下列條件，才能透過從現有記錄連線來新增記錄：

* 連線的記錄型別。 如需詳細資訊，請參閱[連線記錄型別](/help/quicksilver/planning/architecture/connect-record-types.md)。
* 記錄。
* Workfront Planning和Workfront中的正確存取和許可權，如本文中[存取需求](#access-requirements)一節所述。

若要在連線其他記錄時建立記錄，請執行下列動作：

1. 開始連線Workfront Planning記錄，如文章[連線記錄](/help/quicksilver/planning/records/connect-records.md)中所述。 您可以在Workfront Planning的下列區域中，從連線欄位中連線記錄：

   * 表格檢視
   * 記錄的詳細資訊頁面或預覽方塊

1. （視條件而定）如果您在嘗試從其他記錄的連線記錄欄位新增記錄時找不到記錄，請搜尋記錄，然後按一下[**+新增]**。 **+新增**&#x200B;按鈕後面接著您連線的記錄型別名稱。 例如，將品牌新增至現有行銷活動時，「新增品牌」。 您輸入的名稱也會跟著新增按鈕。

   <!--remove the first part of the step above to say just Click Add when the button will be persistent, for preview and production-->

   ![](assets/add-button-to-create-records-in-context-highlighted.png)

   記錄已建立並新增至連線的記錄欄位。

   <!--
    >[!IMPORTANT]
    >
    >* You can create only projects and portfolios in Workfront when connecting them from a record. 
    >
    >* You cannot create programs, groups, or companies when connecting them from a record in Workfront Planning. 
    >
    >* You cannot create a project from a template when when you create projects by connecting them from a record. You must manually add tasks and project information or a template to the new project after you add it to the record. -->

1. （選擇性）移至您建立其記錄的記錄型別的表格檢視。 新記錄會顯示在檢視的最後一列。
1. （選擇性）開始為表格檢視中的新記錄新增資訊
或
按一下其名稱以開啟詳細資訊頁面並在其中新增資訊。

## 透過向記錄型別提交請求表單來建立記錄

當有人建立記錄型別的請求表單並與您共用連結後，您可以提交建立該記錄型別記錄的請求。

如需詳細資訊，請參閱[在Adobe Workfront Planning中建立和管理要求表單](/help/quicksilver/planning/requests/create-request-form.md)。

如果您的Workfront使用者與組織外部的使用者具有請求表單的連結，則他們皆可提交請求給Planning記錄型別並建立記錄。

如需詳細資訊，請參閱[提交Adobe Workfront Planning要求以建立記錄](/help/quicksilver/planning/requests/submit-requests.md)。

## 從CSV或Excel檔案匯入記錄型別時建立記錄

當您使用CSV或Excel檔案匯入記錄型別時，可以匯入記錄。

如需詳細資訊，請參閱[建立記錄型別](/help/quicksilver/planning/architecture/create-record-types.md)。

