---
title: 當您將Workfront物件連線至記錄時，從Workfront Planning建立它們
description: 當您從Workfront Planning中的其他記錄連線物件時，可以建立Workfront物件型別。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 7c3db950-4cd9-424c-a7a7-4fa7dfa995f6
source-git-commit: 8546311acf722c0f4d47d4663b02ff701416894a
workflow-type: tm+mt
source-wordcount: '1377'
ht-degree: 1%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->

# 當您將Workfront物件連線至記錄時，從Workfront Planning建立它們

<!-- update the title (and all the links to this article) at preview, to be this: Create Workfront objects from Workfront Planning as you connect them to records-->
<!-- remove preview and production at release time-->

<span class="preview">本頁標示的資訊是指尚未普遍可用的功能。 它僅在預覽環境中可供所有客戶使用。 每月發行至生產環境後，生產環境中為啟用快速發行的客戶也提供相同的功能。</span>

<span class="preview">如需快速發行資訊，請參閱[為您的組織啟用或停用快速發行](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>

{{planning-important-intro}}

您可以透過下列方式，從Workfront Planning建立Adobe Workfront物件：

* 當您從Planning記錄連線Workfront物件時

  本文說明如何從Workfront Planning建立Workfront物件，以便從Planning記錄連線。
* 當您從記錄的頁面使用自動化時。

  如需有關使用自動化建立Workfront物件的資訊，請參閱[使用Adobe Workfront Planning記錄自動化建立物件](/help/quicksilver/planning/records/create-wf-objects-using-planning-automations.md)。

>[!IMPORTANT]
>
>將下列Workfront物件與Planning記錄連線時，可以從Workfront Planning建立這些物件：
>
>* 專案
>* 專案組合
>* 計劃
>
>您可以將下列Workfront物件與Planning記錄連線，但無法在連線程式中建立它們：
>
>* 群組
>* 公司
>

連線和建立Workfront物件至Workfront Planning記錄時，請考量下列事項：

* 您可以從連線欄位從Workfront計畫的下列區域連線Workfront專案、投資組合、方案、群組和公司：

   * 記錄型別的表格檢視
   * 記錄的詳細資訊頁面或預覽方塊
   * 記錄的「連線」標籤

* 您可以從Workfront Planning的下列區域建立專案：

   * 記錄型別的表格檢視
   * 連線欄位中記錄的詳細資訊區域
   * <span class="preview">記錄的已連線記錄頁面，在詳細資訊區域</span>

* 您可以從Workfront Planning的下列區域建立產品組合和計畫：

   * 記錄型別的表格檢視
   * 連線欄位中記錄的詳細資訊區域

如需有關連線Planning記錄與Workfront物件的資訊，請參閱[連線記錄](/help/quicksilver/planning/records/connect-records.md)。

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
</tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront套件</p></td> 
   <td> 
<ul> 
<li><p>任何Workfront和任何Planning套件</p></li>
或
<li><p>任何工作流程與任何Planning套件</p></li></ul>
<p>如需每個Workfront Planning套件所含內容的詳細資訊，請聯絡您的Workfront客戶代表。 </p> 
   </td> 
<tr> 
<td> 
   <p> 其他產品</p> </td> 
   <td> 
    <p>除了Adobe Workfront，您必須擁有Adobe Experience Manager Assets授權，以及AEM Assets與Workfront之間的整合，才能將AEM資產與Planning記錄連線。</p>
    <p>如需詳細資訊，請參閱<a href="/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/workfront-for-aem-asset-essentials.md">適用於Experience Manager Assets和Assets Essentials的Adobe Workfront：文章索引</a>。 </p>
   </td> 
  </tr>   
<tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront授權</p></td> 
   <td><p>標準</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>存取層級設定</p></td> 
   <td> <p>Adobe Workfront Planning沒有存取層級控制</p> 
   <p>編輯存取權，並存取您要建立之物件型別（專案、投資組合、方案）的「在Workfront中建立物件」。 </p>  
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>物件許可權</p></td> 
   <td> <p>提供或更高許可權給您要新增記錄的工作區和記錄型別。 </p>  
   <p>系統管理員擁有所有工作區的許可權，包括他們未建立的工作區</p>
   <p>管理Workfront物件（專案組合）的許可權以新增子物件（專案）。</p>
   </td> 
  </tr>   
</tbody> 
</table>

如需Workfront存取需求的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++ 

<!--Old:

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Products</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront plan*</p></td> 
   <td> 
<p>Any of the following Workfront plans:</p> 
<ul><li>Select</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning is not available for legacy Workfront plans</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planning package*</p></td> 
   <td> 
<p>Any </p> 
<p>For more information about what is included in each Workfront Planning plan, contact your Workfront account manager. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront platform</p></td> 
   <td> 
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access Workfront Planning.</p> 
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td> Standard
   <p>Workfront Planning is not available for legacy Workfront licenses</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>There are no access level controls for Adobe Workfront Planning</p> 
   <p>Edit access with access to Create objects in Workfront for the object types that you want to create (projects, portfolios, programs). </p>  
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td> <p>Manage permissions to the workspace and record type where you want to add records. </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
   <p>Manage permissions to Workfront objects (portfolios) to add children objects (projects).</p>
   </td> 
  </tr> 
</tbody> 
</table> 

 *For more information about Workfront access requirements, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).  -->


## 從Workfront Planning連線物件與記錄時，建立Workfront物件的先決條件

您必須具備下列條件，才能透過從現有記錄連線來新增專案或投資組合：

* 連結到Workfront專案、投資組合或計畫的記錄型別。 如需詳細資訊，請參閱[連線記錄型別](/help/quicksilver/planning/architecture/connect-record-types.md)。
* 連線至Workfront物件的記錄型別記錄。 如需詳細資訊，請參閱[建立記錄](/help/quicksilver/planning/records/create-records.md)。
* Workfront Planning和Workfront中的正確存取和許可權，如本文中[存取需求](#access-requirements)一節所述。

## 當您從Workfront Planning將專案與記錄連線時，建立專案

您可以在Workfront Planning中建立專案，並透過Workfront Planning的下列區域將其與記錄連結：

* 記錄型別的表格檢視或連線欄位中記錄的詳細資訊區域
* <span class="preview">記錄的[已連線]記錄頁面，在記錄的[詳細資料]區域中</span>

### 從記錄的詳細資訊區域或記錄型別的表格檢視建立專案

若要在從其他記錄連線專案時建立專案：

1. 移至記錄的詳細資訊頁面或記錄型別的表格，並開始將Workfront Planning記錄與Workfront專案連線，如文章[連線記錄](/help/quicksilver/planning/records/connect-records.md)中所述。

1. （視條件而定）按一下&#x200B;**新增專案**
或
開始輸入專案名稱，如果找不到，請按一下[新增專案]。 ****「新增」按鈕後面接著您輸入的專案名稱。

   ![從連線欄位連線時新增專案](assets/add-project-when-connecting-it-from-connection-field.png)

   **建立專案**&#x200B;方塊開啟。

1. （選用）更新&#x200B;**專案名稱**。 根據預設，專案會以您從記錄連線時新增為搜尋專案的名稱命名。
1. （選擇性）選取&#x200B;**專案範本**。 如果您未選取範本，Workfront會建立不含任務的空白專案。
1. 按一下「**建立**」。
1. （視條件而定）如果您選取從範本建立專案，請依照文章[使用範本建立專案](/help/quicksilver/manage-work/projects/create-projects/create-project-from-template.md)中的步驟完成新增專案。

   新專案已建立並新增至所選記錄的已連線欄位。

1. （可選）從Workfront計畫按一下新專案的名稱，以在Workfront中開啟專案頁面，並對專案進行其他更新。

<div class="preview">

### 從記錄的「連線記錄」頁面建立專案

1. 在表格檢視中，將Project物件型別與Workfront Planning記錄型別連線。

   如需詳細資訊，請參閱[連線記錄型別](/help/quicksilver/planning/architecture/connect-record-types.md)。

1. 按一下任何檢視中的記錄名稱。 「細節」預覽方塊開啟。

1. 新增專案的&#x200B;**連線記錄頁面**。

   如需詳細資訊，請參閱文章[管理記錄頁面配置](/help/quicksilver/planning/records/manage-the-record-page.md)中的「新增連線的記錄頁面至記錄」一節。

   「連線的記錄」頁面會顯示在表格檢視中。 連線的專案會顯示在表格中。

   ![連線記錄頁面中的專案資料表檢視](assets/projects-connected-records-page-table.png)

1. 按一下專案表格中的&#x200B;**新增列**&#x200B;以新增專案。

   您只能在此區域中新增空白專案。 您無法使用範本新增專案。
1. （選用）按一下表格檢視中的專案名稱，在Workfront中開啟專案並新增詳細資訊。

</div>

## 在連結投資組合與Workfront Planning的記錄時建立投資組合

您可以從記錄型別的表格檢視或記錄的詳細資訊頁面建立投資組合。

若要在從Planning記錄連線投資組合時建立投資組合：

1. 移至記錄的詳細資訊頁面或記錄型別的表格，然後開始將Workfront Planning記錄與Workfront投資組合連線，如文章[連線記錄](/help/quicksilver/planning/records/connect-records.md)中所述。

1. （視條件而定）按一下&#x200B;**新增投資組合**

   或

   開始輸入投資組合的名稱，如果找不到，請按一下[新增投資組合] ****。 「新增」按鈕後面接著您輸入的投資組合名稱。

   ![從連線欄位連線時新增投資組合](assets/add-portfolio-when-connecting-it-from-connection-field.png)

   投資組合隨即建立並新增至您所選記錄的連線欄位。

1. （選用）從Workfront Planning按一下新投資組合的名稱，即可在Workfront中開啟投資組合頁面，並對投資組合進行其他更新。

## 在程式與Workfront Planning的記錄連線時建立程式

您可以從記錄型別的表格檢視或記錄的詳細資訊頁面建立程式。

若要在從Planning記錄連線程式時建立程式，請執行下列動作：

1. 移至記錄的詳細資訊頁面或記錄型別的表格，然後開始將Workfront Planning記錄與Workfront投資組合連線，如文章[連線記錄](/help/quicksilver/planning/records/connect-records.md)中所述。

1. 按一下&#x200B;**新增程式**

   或

   開始輸入方案的名稱，如果找不到，請按一下[新增方案] ****。 新增按鈕後面接著您輸入的程式名稱。

   ![從連線欄位連線時新增Workfront程式](assets/add-wf-program-when-connecting-it-from-connection-field.png)

   **建立程式**&#x200B;方塊開啟。

1. 更新&#x200B;**程式名稱**。 這是必填欄位。
1. 從下拉式清單中選擇&#x200B;**Portfolio**，或開始輸入投資組合的名稱，然後當它顯示在清單中時選取它。 這是必填欄位。
1. 按一下「**建立**」。

   程式隨即建立並新增至您選取之記錄的連線欄位。

1. （可選）從Workfront Planning按一下新方案的名稱，以在Workfront中開啟方案頁面，並進行其他更新。

