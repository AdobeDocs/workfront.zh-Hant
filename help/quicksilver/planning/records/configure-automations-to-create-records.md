---
title: 設定Adobe Workfront Planning自動化
description: 您可以在Adobe Workfront Planning中設定自動化，以啟動後在Workfront中建立物件或Workfront Planning中的記錄。 建立的物件與記錄會自動連線至現有的Planning記錄。 本文說明如何管理自動化，包括如何編輯、停用或刪除自動化。
feature: Workfront Planning
role: User, Admin
author: Alina, Becky
recommendations: noDisplay, noCatalog
exl-id: cde20e5a-15a2-413a-8de4-ccf6eeb4395f
source-git-commit: 298c542afea902d9fc14ef6a4470c0bc1d9bd33c
workflow-type: tm+mt
source-wordcount: '1687'
ht-degree: 3%

---

# 設定Adobe Workfront Planning自動化

<!--add screen shots when UI is finalized AND redo all the steps - some things got changed and moved around-->

<!--you might need to add something about notifications and emails?!-->
<!--add a new section to this article to mention a new way to create objects: help/quicksilver/planning/records/create-records.md-->
<!-- add a new section to this article to mention a new way to create WF objects from Planning: help/quicksilver/planning/records/create-workfront-objects-from-workfront-planning.md-->

<!-- if they give access to use the automation to people with LESS than Manage permissions to a workspace, split this article in two: the Configure section should be for admins and the "Use a Workfront Planning automation to create an object" should be for all other users-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

您可以在Adobe Workfront Planning中設定自動化，以便在從Planning記錄觸發時，在Workfront中建立物件或Workfront Planning中的記錄。 建立的物件或記錄會自動連線至您觸發自動處理的記錄。

您可以在Workfront Planning的記錄型別頁面中設定並啟動自動化。

例如，您可以建立採用Workfront Planning行銷活動的自動化，並在Workfront中建立專案以追蹤該行銷活動的進度。

本文說明如何管理自動化，包括如何編輯、停用、刪除和觸發自動化，以建立物件和記錄。

如需有關如何使用現有的自動化建立記錄或物件的資訊，請參閱[使用Adobe Workfront Planning記錄自動化建立物件](/help/quicksilver/planning/records/create-wf-objects-using-planning-automations.md)。

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
   <td> 標準
   <p>Workfront計畫不適用於舊版Workfront授權</p> 
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
   <td> <p>管理您要建立自動的工作區和記錄型別的許可權。 </p>
   <p>系統管理員擁有所有工作區的管理許可權，包括他們未建立的工作區</p>
   </td> 
  </tr> 
</tbody> 
</table>

*如需Workfront存取需求的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 在Workfront Planning中設定自動化

您必須先在Workfront Planning中設定記錄型別的自動化，才能使用它來建立物件。

{{step1-to-planning}}

1. 按一下記錄型別卡，然後按一下記錄名稱。

   記錄型別頁面隨即開啟。
1. 按一下記錄型別名稱右側的&#x200B;**更多**&#x200B;功能表![更多功能表](assets/more-menu.png)，然後按一下&#x200B;**管理自動化**。

   所選記錄型別的可用自動化清單隨即開啟。

1. 按一下熒幕右上角的&#x200B;**新自動化**。 **新自動化**&#x200B;方塊開啟。
1. 更新下列欄位：

   * 將&#x200B;**未命名的自動化**&#x200B;取代為您要顯示在自動化按鈕上的文字。 使用自動化建立Workfront物件或Planning記錄時，使用者將按一下此按鈕。
   * **描述**：新增描述以識別自動化的目的。
1. 按一下&#x200B;**儲存**。
自動化詳細資訊頁面隨即開啟。

1. 在自動化的詳細資訊頁面上，更新&#x200B;**觸發器**&#x200B;區段中的下列欄位：

   * **觸發器**：選取將觸發自動化的動作。 例如，選取&#x200B;**按一下**。<!--update this step with a list of all possible triggers; right now only Button click is available-->

1. 更新&#x200B;**動作**&#x200B;區段中的下列欄位： <!--submitted bugs for these fields - see if they need changing here-->
   * **動作**：選取您希望Workfront在觸發自動化時執行的動作。 這是必填欄位。
選取下列其中一個動作：

      * 建立多個專案
      * 建立單一專案
      * 建立專案
      * 建立記錄
      * 建立方案
      * 建立專案組合
      * 建立群組

     >[!TIP]
     >
     >儲存自動化後，您將無法再變更在此欄位中選取的動作。

1. （視條件而定）根據您選取的動作，更新下列欄位：

   * **建立單一專案**： <!--replace to the left: Create a single project-->
      * **建立專案的已連線欄位**：這是將顯示新專案的已連線欄位。 這是必填欄位。
      * **專案範本**：選取Workfront用來建立專案的專案範本。

   * 建立多個專案：
      * **建立專案的已連線欄位**：這是將顯示新專案的已連線欄位。 這是必填欄位。
      * **其選擇將建立記錄的欄位**：從選取的記錄型別中選擇多重或單一選取欄位。 Workfront會為您觸發自動化的記錄上目前選取的每個欄位選擇建立一個專案。

     >[!TIP]
     >
     >專案只會針對您執行自動化之記錄的多重或單重選取欄位中目前選取的選項而建立，不會針對該欄位的所有可能選項而建立。
     >

      * **使用相同的範本**：選取此選項可針對每個新專案使用相同的範本。 如果取消選取選項，請為每個欄位選擇選取&#x200B;**專案範本**。
      * **專案範本**：如果您已選取&#x200B;**使用相同範本**&#x200B;選項，請選取Workfront將用來建立專案的專案範本。

   * **建立投資組合**：
      * **建立投資組合的已連線欄位**：這是將顯示新投資組合的已連線欄位。 這是必填欄位。
      * **要附加到新投資組合的自訂表單**：選取要附加到新投資組合的自訂表單。 您必須先建立產品組合自訂表單，然後才能進行選取。
   * **建立程式**：
      * **建立程式的已連線欄位**：這是將顯示新程式的已連線欄位。 這是必填欄位。
      * **方案組合**：選取將新增新方案的組合。 這是必填欄位。
      * **要附加到新程式的自訂表單**：選取要附加到新程式的自訂表單。 您必須先建立程式自訂表單，然後才能進行選取。
   * **建立群組**：
      * **建立群組的已連線欄位**：這是將顯示新群組的已連線欄位。 這是必填欄位。
      * **要附加到新群組的自訂表單**：選取要附加到新程式的自訂表單。 您必須先建立程式自訂表單，然後才能進行選取。
   * **建立記錄**：
      * **記錄型別**：選取您要建立的記錄型別。

        **設定**&#x200B;子區段隨即顯示。 更新&#x200B;**設定**&#x200B;子區段中的下列欄位：

         * **目前記錄將顯示的連線記錄型別欄位**：這是針對目前記錄將顯示的動作選取的記錄型別上的連線欄位。

        例如，如果您正在建立行銷活動的自動化，以便從連線產品記錄，這是產品記錄型別上顯示的行銷活動之已連線欄位（使用自動化建立產品後）。

        這是必填欄位。

        <!--submitted a change in functionality and UI text for this - revise??-->
在**對應欄位**&#x200B;區域中，更新下列資訊：

         * **傳輸自**：從建立自動化的記錄型別中選取欄位，以將它們對應到連線記錄型別的欄位。
         * **傳輸至**：從新建立的記錄中選取欄位，這些欄位會填入您執行自動化之記錄中的資訊。

        >[!TIP]
        >
        >* 來自原始記錄型別的欄位型別必須與來自新建記錄型別的欄位型別匹配。
        >* 如果您選擇無欄位，則新記錄的名稱將為&#x200B;**未命名的記錄**。

1. （選擇性和條件性）如果您選取建立記錄，請按一下&#x200B;**新增欄位**，將其他查詢欄位從一筆記錄對應到另一筆記錄。
1. （條件式）如果原始記錄型別與在&#x200B;**記錄型別**&#x200B;欄位中選取的記錄型別之間沒有連線欄位，請按一下&#x200B;**新增連線欄位**。

   ![建立記錄的自動化設定](assets/automation-setup-create-record.png)

   將建立下列兩個欄位：

   * 已針對您在&#x200B;**記錄型別**&#x200B;欄位中指定的記錄型別，建立名為&#x200B;**連線記錄**&#x200B;的新連線欄位。
   * 已為您設定自動化的記錄型別建立與&#x200B;**記錄型別**&#x200B;欄位中指定的名稱相同的新連線欄位。

     例如，如果您正在設定Campaigns的自動化，以自動建立另一個名為Brands的記錄型別，然後按一下&#x200B;**新增連線的欄位**，則會建立下列欄位：

      * 已為&#x200B;**品牌**&#x200B;記錄型別建立&#x200B;**連線記錄**&#x200B;連線欄位。
      * 已針對&#x200B;**行銷活動**&#x200B;記錄型別建立&#x200B;**品牌**&#x200B;連線欄位。

1. （選擇性）如果原始記錄型別與在[動作]區域中選取的Workfront物件之間沒有連線欄位，請按一下[新增]連線欄位&#x200B;**。**

   ![建立多個專案的自動化設定](assets/automation-setup-create-multiple-projects.png)

   將建立下列專案：

   * 名稱為&#x200B;**Connected &lt; Workfront物件名稱>**&#x200B;的新連線欄位是為您建置自動化之記錄型別所建立。 例如，當您選擇自動建立專案時，會針對您正在建立自動化的記錄型別建立&#x200B;**已連線的專案**&#x200B;欄位。
   * 新記錄型別卡片會新增至Workfront中Workfront專案的「計畫」區段，其名稱為您設定自動化的記錄型別。

1. 按一下自動化詳細資料頁面右上角的&#x200B;**儲存**。

   自動化會顯示在自動化清單上，且可用於記錄。

## 管理現有的自動化

{{step1-to-planning}}

1. 按一下記錄型別卡，然後按一下記錄名稱。

   記錄型別頁面隨即開啟。
1. 按一下記錄型別名稱右側的&#x200B;**更多**&#x200B;功能表![更多功能表](assets/more-menu.png)，然後按一下&#x200B;**管理自動化**。

   所選記錄型別的可用自動化清單隨即開啟。

1. （可選）若要編輯、停用或刪除自動化，請執行下列任一項作業：

   1. 從自動化清單中，暫留在已儲存的自動化名稱上，然後按一下&#x200B;**更多**&#x200B;功能表![更多](assets/more-menu.png)。

   1. 按一下&#x200B;**編輯**&#x200B;以更新下列資訊：

      * 按一下自動化名稱右邊的&#x200B;**更多**&#x200B;功能表![更多功能表](assets/more-menu.png)，然後按一下&#x200B;**編輯**&#x200B;以變更自動化名稱。
      * 自動化中除了&#x200B;**動作**&#x200B;欄位以外的所有欄位。

        >[!TIP]
        >
        >您無法變更您最初為自動化選取的動作。


   1. 按一下&#x200B;**停用**&#x200B;以從記錄的資料表檢視中移除自動化，並防止使用者使用它來建立記錄或物件。

      使用已停用的自動化所建立的記錄仍會連線至最初選取的記錄。

      若要再次使用，請按一下&#x200B;**更多**&#x200B;功能表![更多](assets/more-menu.png)，然後按一下&#x200B;**啟動**。
   1. 按一下&#x200B;**刪除**&#x200B;以刪除自動化。 已刪除的自動化無法復原。

      使用已刪除的自動化所建立的記錄會保持與原始選取的記錄連線。
