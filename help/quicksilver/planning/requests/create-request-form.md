---
title: 在Adobe Workfront Planning中建立和管理請求表單
description: 在Adobe Workfront Planning區域中選取記錄型別後，您可以建立請求表單，並將其與該記錄型別建立關聯。 然後，您可以與其他內部或外部使用者共用與其的連結。 具有表單連結的使用者可以填寫其上的欄位值，透過提交它，他們可以為與其關聯的記錄型別新增記錄。
feature: Workfront Planning
role: User, Admin
author: Alina, Becky
recommendations: noDisplay, noCatalog
exl-id: 49f25b03-90bb-4317-9e48-289fd61df791
source-git-commit: 1b7964b533093c4eee20d69a74512a145e207e29
workflow-type: tm+mt
source-wordcount: '3046'
ht-degree: 1%

---

# 在Adobe Workfront Planning中建立和管理請求表單

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!--take Preview and Production references at Production time-->

<span class="preview">本頁醒目提示的資訊指出尚未普遍可用的功能。 它僅在預覽環境中可供所有客戶使用。 每月發行至生產環境後，生產環境中為啟用快速發行的客戶也提供相同的功能。</span>

<span class="preview">如需快速發行資訊，請參閱[為您的組織啟用或停用快速發行](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>


{{planning-important-intro}}

您可以建立請求表單，並將其與Adobe Workfront Planning中的記錄型別建立關聯。 然後，您可以與其他人共用表單，他們也可以提交請求以建立該型別的記錄。

本文說明工作區管理員如何建立與記錄型別相關聯的請求表單。

如需有關將請求提交至記錄型別以建立記錄的資訊，請參閱[提交Adobe Workfront Planning請求以建立記錄](/help/quicksilver/planning/requests/submit-requests.md)。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront套件</p></td> 
   <td> 
<ul><li><p>任何Workfront套件</p></li>
與
<li><p>任何Planning套件</p></li></ul>
或
<ul><li><p>任何Workflow封裝</p></li>
與
<li><p>任何Planning套件</p></li></ul>
   </td> </tr>

</tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront授權</p></td> 
   <td><p>標準</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>物件許可權</p></td> 
   <td>   <p>管理工作區或記錄型別</a>的許可權 </p>  
   <p>系統管理員擁有所有工作區的許可權，包括他們未建立的工作區</p>  </td> 
  </tr>  
</tbody> 
</table>

如需Workfront存取需求的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 請求表單中的欄位和值顯示限制

在您提交請求後，某些欄位在請求表單上的顯示方式，以及它們的值稍後如何在記錄或請求詳細資訊頁面上顯示，皆有限制。

如需有關提交Workfront Planning要求的資訊，請參閱[提交Adobe Workfront Planning要求以建立記錄](/help/quicksilver/planning/requests/submit-requests.md)。

* 以下為要求表單、要求表單建立的記錄或要求詳細資訊頁面中特定欄位顯示方式的限制：

   * 您無法將下列型別的欄位新增至請求表單：

      * 建立者，上次修改者，<span class="preview">核准者</span>
      * 建立日期，上次修改日期，<span class="preview">核准日期</span>
      * Workfront物件的查閱欄位
      * Workfront Planning連線記錄的查詢欄位

* 以下為欄位格式在請求表單產生器中顯示方式，與欄位值在記錄或請求詳細資訊頁面中的格式設定方式之間的差異：

   * 「貨幣」、「數字」和「百分比」欄位會在表單產生器中顯示為「單行」文字欄位型別。

     但是，欄位格式會保留，並在提交請求後、在記錄型別和請求詳細資訊頁面中，欄位值將顯示為貨幣、數字和百分比。

* 以下說明某些欄位值如何在請求表單和請求詳細資訊頁面上顯示：

   * 不保留貨幣、數字和百分比欄位的特殊格式。 例如，這些區域中的這些欄位值不會保留小數精確度。
   * 人員欄位值會顯示為ID。
   * 未參考其他欄位或計算的公式欄位不顯示任何值。 例如，具有`STRING`公式的欄位會顯示「N/A」值。
   * 參考「幣別」欄位的公式欄位會顯示不含匯率會計的值。
   * 段落欄位的值在請求表單上顯示「N/A」值，並在請求詳細資訊頁面中顯示html標籤而不是格式化文字。

## 建立請求表單

若要建立請求表單，您必須開始建立表單、設定表單詳細資料，然後發佈並共用表單以完成作業。

### 開始建立請求表單

您可以從與表單<span class="preview">關聯的記錄型別或Workfront的「請求」區域建立請求表單。</span>

#### 從記錄型別建立請求表單

{{step1-to-planning}}

1. 按一下您要新增記錄的工作區。

   工作區隨即開啟，且記錄型別會顯示為卡片。

1. 按一下記錄型別卡。 如需有關建立記錄型別的資訊，請參閱[建立記錄型別](/help/quicksilver/planning/architecture/create-record-types.md)。

   記錄型別頁面會在您上次存取的檢視中開啟。 依預設，會在表格檢視中開啟記錄型別頁面。

1. 按一下頁面標頭中記錄型別名稱右側的&#x200B;**更多**&#x200B;功能表![更多功能表](assets/more-menu.png)，然後按一下&#x200B;**建立請求表單**&#x200B;或&#x200B;**管理請求表單** （如果您已經有表單，而且想要建立其他表單）。
1. （視條件而定）若要新增其他表單，請按一下&#x200B;**新增請求表單**。

   「建立請求表單」方塊隨即開啟。

1. 在「建立請求表單」方塊中，更新請求表單的名稱。 依預設，表單的名稱為&#x200B;**未命名表單**。<!--check this; you logged a bug to rename it to 'Untitled request form' but was it fixed?-->
1. （選用）為要求表單新增&#x200B;**描述**。

   <!--Not possible yet: The Description is visible when you access the request form from the Requests area of Workfront.-->

1. 按一下「**建立**」。

   所選記錄型別的請求表單會在「表單」標籤中開啟。
1. 繼續[設定表單](#configure-the-form)。

<div class="preview">

#### 從Workfront的「請求」區域建立請求表單

1. 按一下Adobe Workfront右上角的&#x200B;**[!UICONTROL 主功能表]**&#x200B;圖示![主功能表](/help/_includes/assets/main-menu-icon.png)，或（如果有的話）按一下左上角的&#x200B;**[!UICONTROL 主功能表]**&#x200B;圖示![主功能表](/help/_includes/assets/main-menu-icon-left-nav.png)，然後按一下&#x200B;**要求**。
1. 在熒幕的右上角，按一下&#x200B;**要求表單**。
1. （視條件而定）如果您正在編輯現有的請求表單，請從清單中選取它，然後繼續[設定表單](#confgure-the-form)。
1. 如果您正在建立新的要求表單，請在畫面的右上角，按一下&#x200B;**新增要求表單**。

   建立請求表單方塊隨即開啟

1. 在「建立請求表單」方塊中，更新請求表單的名稱。 依預設，表單的名稱是&#x200B;**未命名的表單**。
1. 在「物件型別」欄位中，選取與請求表單相關聯的記錄型別。 記錄型別會分組到其所在的工作區。
1. （選用）為要求表單新增&#x200B;**描述**。

   <!--Not possible yet: The Description is visible when you access the request form from the Requests area of Workfront.-->

1. 按一下「**建立**」。

   所選記錄型別的請求表單會在「表單」標籤中開啟。
1. 繼續[設定要求表單](#set-up-details-for-the-request-form)的詳細資料。

</div>

### 設定請求表單的詳細資料

表單詳細資料會分為幾個索引標籤。

* **表單**&#x200B;索引標籤可讓您新增欄位和內容元素至表單
* **組態**&#x200B;索引標籤可讓您設定表單<span class="preview">的核准程式，以及設定要求完成選項</span>。
* <span class="preview">**自動化**&#x200B;索引標籤可讓您根據使用表單發出的請求功能自動執行即將發生的事件。</span>

#### 設定表單詳細資料

1. 開始建立或編輯要求表單，如[開始建立要求表單](#begin-creating-a-request-form)一節中所述。

   所選記錄型別的請求表單會在「表單」標籤中開啟。

   ![行銷活動要求表單編輯模式](assets/campaigns-request-form-edit-mode.png)

   依預設，請求表單包含下列資訊：

   * 所選記錄型別的表格檢視中可用的記錄欄位。<!--they are working on removing the limitation below-->

   * **預設的分節**：這是Workfront套用至要求表單的預設分割槽符號。 所有記錄欄位都顯示在&#x200B;**預設區段**&#x200B;區域。
   * **主旨**&#x200B;欄位：將在Workfront中識別要求的欄位。 主旨欄位的設定和值無法編輯。

     >[!NOTE]
     >
     >* **Subject**&#x200B;欄位在要求表單上可見時需要值。 不過，您可以視需要移除&#x200B;**主旨**&#x200B;欄位，要求者提交要求時不會在表單上看到該欄位。
     >* 當請求表單上缺少「主旨」欄位，但未來記錄的名稱有「名稱」欄位時，會自動將請求名稱指派給與所建立記錄相同的名稱。
     >* 當要求表單上同時遺漏[主旨]和[名稱]欄位時，要求會以下列模式命名： `< Record name > request form < Entry date of the request >`；記錄命名為&#x200B;**未命名**。

   * 與記錄型別關聯的所有欄位。

     向此記錄型別提交請求的所有人均可看到請求表單中包含的欄位。

1. （選擇性）將滑鼠停留在您要移除的表單上任何欄位上，然後按一下&#x200B;**x**&#x200B;圖示以移除它們。 已將它們新增至表單左側的&#x200B;**欄位**&#x200B;索引標籤。

   例如，移除&#x200B;**主旨**&#x200B;欄位，因為在Workfront Planning中看不到此欄位。<!--remove this example if this becomes visible in Planning?-->

1. （選擇性）若要從表單中移除&#x200B;**預設區段**，請執行下列動作：

   1. 從預設區段中移除所有欄位。
   1. 按一下&#x200B;**內容元素**&#x200B;並新增區段，然後新增區段的名稱。
   1. 新增欄位至新區段。
   1. 按一下&#x200B;**x**&#x200B;圖示以移除&#x200B;**預設區段**。
1. 按一下任何欄位，然後使用表單右側面板中的控制項來定義其大小或下列任何資訊：

   * **標籤**：這是欄位在要求表單上顯示的名稱。 這不會變更記錄欄位的名稱。
   * **指示**：新增欄位的詳細資訊。
   * **建立必要欄位**：選取時，該欄位必須具有值。 否則，無法提交表單。
   * **新增邏輯**：定義必須符合哪些條件才能顯示或隱藏欄位。

   >[!TIP]
   >
   >   在表單上選取欄位後，每個欄位的欄位型別都會顯示在右側面板的頂端。
   >     

1. （選擇性）按一下表單左側的&#x200B;**Content elements**&#x200B;標籤，然後新增下列任一元素：

   * **描述文字**
   * **分割槽符號**

   如需建立自訂表單的詳細資訊，請參閱[建立自訂表單](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)。

1. （選擇性）按一下&#x200B;**預覽**&#x200B;以檢視其他使用者使用表單提交新記錄時表單的顯示方式。
1. 如果您想要設定表單的詳細資訊，請繼續[設定詳細資訊](#set-up-configuration-details)，或前往[完成建立請求表單](#complete-request-form-creation)。

#### 設定組態詳細資料

在[組態]索引標籤上，您可以設定核准程式<span class="preview">並設定從此表單建立的要求何時將標示為[已完成]</span>。

1. 開始建立或編輯要求表單，如[開始建立要求表單](#begin-creating-a-request-form)一節中所述。

   所選記錄型別的請求表單會在「表單」標籤中開啟。
1. （選擇性）設定任何表單詳細資料，如[設定表單詳細資料](#set-up-form-details)中所述。

1. （選擇性）按一下&#x200B;**組態**&#x200B;標籤，然後新增至少一位使用者<span class="preview">或團隊</span>至&#x200B;**核准者**&#x200B;欄位，以核准此記錄表單的新要求。

   ![設定索引標籤](assets/configuration-tab.png)

   <!--below bullet list is duplicated in the Add approval to a request form article-->

   * 將請求表單與核准者建立關聯時，任何新請求都必須先由所有核准者核准，才能產生新記錄。
   * 您可以將一個或多個核准者新增至請求表單。
   * 如果至少有一位核准者拒絕請求，則請求會遭到拒絕，且不會建立記錄。
   * 在核准或拒絕請求之前，所有核准者都必須做出決定。
   * <span class="preview">如果團隊設定為核准者，則僅需要團隊中的一個決定。</span>

     如需新增核准至請求表單的詳細資訊，請參閱[新增核准至請求表單](/help/quicksilver/planning/requests/add-approval-to-request-form.md)。

1. <span class="preview">（條件式）如果您要在任何核准者核准記錄後建立記錄，請勾選&#x200B;**僅需要一個決定**&#x200B;核取方塊。</span>

1. <span class="preview">選取您是否要在建立要求的物件時，或是當要求的物件完成時，將從這個表單建立的要求標示為完成。</span>
1. <span class="preview">（條件式）如果您已選取在要求的物件完成時將要求標籤為完成，請選取表示物件完成的欄位和值。 例如，當建立的物件狀態設定為Complete時，您可以選取Status欄位和Complete值以完成要求。</span>
1. 如果您想要設定表單的更多詳細資料，請繼續[設定自動詳細資料](#set-up-configuration-details)，或前往[完成建立請求表單](#complete-request-form-creation)。

<div class="preview">

#### 設定自動化

您可以在Adobe Workfront Planning中設定自動化，以便在從Planning記錄觸發時，在Workfront中建立物件或Workfront Planning中的記錄。

如需有關在Workfront Planning的其他區域建立自動化的資訊，請參閱[設定Adobe Workfront Planning自動化](/help/quicksilver/planning/records/configure-automations-to-create-records.md)。

1. 在自動化的詳細資訊頁面上，更新&#x200B;**觸發器**&#x200B;區段中的下列欄位：

   * **觸發器**：選取將觸發自動化的動作。 目前唯一可用的要求表單自動化觸發程式是`When request object status equals pending creation`。

1. 更新&#x200B;**動作**&#x200B;區段中的下列欄位： <!--submitted bugs for these fields - see if they need changing here-->
   * **動作**：選取您希望Workfront在觸發自動化時執行的動作。 這是必填欄位。
目前，要求表單自動化的唯一可用動作是`Create record`。

     >[!TIP]
     >
     >儲存自動化後，您將無法再變更在此欄位中選取的動作。
1. 繼續[完成請求表單建立](#complete-request-form-creation)。


</div>

### 完成請求表單建立

1. 依照[開始建立要求表單](#begin-creating-a-request-form)和[設定要求表單的詳細資料](#set-up-details-for-the-request-form)中的說明建立及設定表單。
1. （選擇性）按一下標題中表單名稱右側的&#x200B;**更多**&#x200B;功能表![更多功能表](assets/more-menu.png)，然後按一下&#x200B;**編輯**&#x200B;以更新表單名稱。

1. 按一下&#x200B;**發佈**&#x200B;以發佈表單並取得其唯一連結。

   會發生下列情況：

   * **發佈**&#x200B;按鈕已移除。
   * **取消發佈**&#x200B;按鈕已新增至表單。 按一下此按鈕，表單將無法存取。
   * **共用**&#x200B;按鈕已新增至表單。
   * 此表單將在Workfront主要功能表的請求區域中變得可用。

1. 按一下&#x200B;**共用**&#x200B;以與其他人共用表單。

   如需共用申請表格的詳細資訊，請參閱本文的[共用申請表單](#share-a-request-form)一節
1. 按一下頁首中表單名稱左側的向左箭頭以關閉表單。

   **請求表單**&#x200B;表格檢視會開啟，並將表單新增至其中。

## 管理現有的請求表單


1. 按一下您要管理請求表單的工作區。

   工作區隨即開啟，且記錄型別會顯示為卡片。

1. 按一下記錄型別卡。 如需有關建立記錄型別的資訊，請參閱[建立記錄型別](/help/quicksilver/planning/architecture/create-record-types.md)。

   記錄型別頁面會在您上次存取的檢視中開啟。 依預設，會在表格檢視中開啟記錄型別頁面。

1. 按一下頁面標頭中記錄型別名稱右側的&#x200B;**更多**&#x200B;功能表![更多功能表](assets/more-menu.png)，然後按一下&#x200B;**管理請求表單**。

   與記錄型別相關的所有請求表單都會顯示在表格檢視中。

1. （選擇性）暫留在表格檢視中的要求表單名稱上，然後按一下表單名稱右側的&#x200B;**更多**&#x200B;功能表![更多](assets/more-menu.png)，然後按一下下列其中一項：

   * **編輯表單**：按一下以進一步編輯表單上的資訊。
   * **取消發佈**：按一下以取消發佈表單，該表單會從Workfront的要求區域移除它。
   * **共用**：按一下此以修改誰可以存取表單。
   * **複製連結**：按一下此以快速複製要求表單的連結，而不開啟表單。
   * **刪除**：按一下以刪除表單。 使用表單新增的所有請求和記錄都不會刪除。 無法復原表單。

   從請求表單清單中請求表單上的![更多功能表](assets/more-menu-on-request-form-from-request-forms-list.png)

1. 按一下標題中&#x200B;**要求表單**&#x200B;左側的向左箭頭，關閉要求表單表格。

   記錄型別頁面隨即開啟。
1. （選擇性和條件式）按一下標題中記錄型別名稱右側的&#x200B;**更多**&#x200B;功能表![更多功能表](assets/more-menu.png)，然後執行下列其中一項作業：

   1. 按一下&#x200B;**更新要求表單**&#x200B;以變更要求表單，然後按一下要求表單以開啟並編輯。
   1. 按一下&#x200B;**複製表單連結**&#x200B;以與其他人共用表單連結。

1. （選用）前往Workfront中的&#x200B;**要求**&#x200B;區域，並尋找共用表單以提交要求。 如需詳細資訊，請參閱[提交Adobe Workfront Planning要求以建立記錄](/help/quicksilver/planning/requests/submit-requests.md)。

## 共用請求表單

1. 依照本文中[建立記錄型別](#create-a-request-form-for-a-record-type)區段中的說明建立要求表單。
1. 按一下記錄型別頁面中要求表單名稱右側的&#x200B;**更多**&#x200B;功能表![更多功能表](assets/more-menu.png)。
1. 按一下&#x200B;**共用**&#x200B;以與其他人共用表單。

1. 若要在內部共用表單，請選取&#x200B;**內部共用**&#x200B;索引標籤，在&#x200B;**授予許可權以提交此表單**&#x200B;欄位，搜尋使用者、團隊、工作角色、群組或公司的名稱，然後當它出現在清單中時選取它。 預設會為每個實體選取&#x200B;**提交**&#x200B;許可權。

   ![分享要求表單](assets/share-box-for-request-form.png)的方塊

1. （選擇性）按一下實體名稱后的下拉式功能表，然後按一下&#x200B;**移除**，將其從清單中移除並停止與它們共用表單。

   >[!NOTE]
   >
   >除了團隊、群組、公司和職務角色之外，您只能與已新增至Adobe Admin Console的使用者共用。 您無法新增僅限Workfront的使用者。 如需詳細資訊，請參閱[在Adobe Admin Console中管理使用者](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md)。

1. 在&#x200B;**可以透過此表單**&#x200B;提交請求的使用者區段中，從下列選項中選取，以指出哪些型別的使用者可以存取此表單：

   * 只有受邀人員才能存取
   * 在工作區擁有檢視或更高存取權限的任何人
   * 對工作區具有貢獻或更高權限的任何人
1. （選擇性）按一下&#x200B;**複製連結**，與有存取許可權的人共用表單連結。 連結已複製到您的剪貼簿。
1. 若要公開共用表單，請選取&#x200B;**公開共用**&#x200B;標籤，然後啟用&#x200B;**建立公開連結**&#x200B;設定。

   ![公開共用要求表單](assets/share-request-form-publicly-tab.png)

   >[!WARNING]
   >
   >* 當您啟用&#x200B;**建立公開連結**&#x200B;設定時，任何人都可以存取表單並提交新記錄，甚至組織外沒有Workfront帳戶的人也可以。
   >
   >* 包含下列欄位型別的表單無法公開共用：
   >
   >     * Workfront或AEM Assets連線
   >     * 人員
   >

1. 選擇&#x200B;**連結到期日**。

   您可以從目前日期起180天內選取未來日期。

   >[!TIP]
   >
   >共用日期過期後，Workfront的「要求」區域中不再提供要求表單，且無法再存取與其他使用者共用的連結。

   連結過期後，人員會收到錯誤，您必須更新連結日期，並產生新連結以共用，人員才能再次存取表單。


1. （選擇性和條件性）按一下&#x200B;**儲存**&#x200B;以儲存表單的共用詳細資料。
1. （視條件而定）如果表單先前已儲存，請按一下&#x200B;**複製連結**。

   表單共用選項會儲存且連結會複製到您的剪貼簿。 您現在可以與其他人共用。

   如需使用要求表單的連結來建立記錄的相關資訊，請參閱[提交Adobe Workfront Planning要求](/help/quicksilver/planning/requests/submit-requests.md)。

1. 按一下&#x200B;**表單**&#x200B;標籤右下角的&#x200B;**儲存**&#x200B;以儲存表單。
