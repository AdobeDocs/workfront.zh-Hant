---
title: 使用Workfront計畫記錄自動化建立Adobe Workfront物件
description: 您可以在Adobe Workfront Planning中設定自動化，以啟動後在Workfront中建立物件或Workfront Planning中的記錄。 建立的物件與記錄會自動連線至現有的Planning記錄。 本文說明如何管理自動化，包括如何編輯、停用、刪除和觸發自動化，以建立物件和記錄。
hide: true
hidefromtoc: true
feature: Workfront Planning
role: User, Admin
author: Alina, Becky
recommendations: noDisplay, noCatalog
exl-id: c669217a-40e2-471f-951d-93157a34f1ee
source-git-commit: fd8e5d3baf6af0dbdd1275494fad54b204abd1a5
workflow-type: tm+mt
source-wordcount: '1800'
ht-degree: 2%

---

# 使用Adobe Workfront Planning記錄自動化建立物件

<!--add screen shots when UI is finalized AND redo all the steps - some things got changed and moved around-->

<!--you might need to add something about notifications and emails?!-->
<!--add a new section to this article to mention a new way to create objects: help/quicksilver/planning/records/create-records.md-->
<!-- add a new section to this article to mention a new way to create WF objects from Planning: help/quicksilver/planning/records/create-workfront-objects-from-workfront-planning.md-->

<!-- if they give access to use the automation to people with LESS than Manage permissions to a workspace, split this article in two: the Configure section should be for admins and the "Use a Workfront Planning automation to create an object" should be for all other users-->

<span class="preview">本頁醒目提示的資訊指出尚未普遍可用的功能。 它僅在預覽環境中可供所有客戶使用。 每月發行至生產環境後，生產環境中為啟用快速發行的客戶也提供相同的功能。</span>

<span class="preview">如需快速發行資訊，請參閱[為您的組織啟用或停用快速發行](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>

您可以在Adobe Workfront Planning中設定自動化，以便在從Planning記錄觸發時，在Workfront中建立物件或Workfront Planning中的記錄。 建立的物件或記錄會自動連線至您觸發自動處理的記錄。

您可以在Workfront Planning的記錄型別頁面中設定並啟動自動化。 建立的已連線物件會放置在您執行自動化時所使用的記錄型別已連線欄位中。

例如，您可以建立採用Workfront Planning行銷活動的自動化，並在Workfront中建立專案以追蹤該行銷活動的進度。 此專案會連結至行銷活動上「已連線的專案」欄位中的Workfront規劃行銷活動。

如需有關連線記錄的詳細資訊，請參閱[連線記錄總覽](/help/quicksilver/planning/records/connected-records-overview.md)。

## 存取需求

+++ 展開以檢視存取需求。

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
<p>貴組織的Workfront例項必須上線至Adobe Unified Experience，才能存取Workfront Planning的所有功能。</p> 
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
   <p>在Workfront中編輯您要建立之物件型別（專案、投資組合、方案）的存取權。 </p>  
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>物件許可權</p></td> 
   <td> <p>為您要建立物件的工作區<!--<span class="preview">and record type</span>-->貢獻或更高的許可權。 </p>  
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


## 有關使用自動化建立物件和記錄的考量事項

* 自動化建立的物件或記錄的名稱與從中建立它的記錄名稱相同。
* 新物件或記錄不會覆寫相同欄位中的現有物件或記錄。 為同一記錄多次觸發相同的自動化，除了之前建立的物件或記錄外，還會新增原始記錄的相同連線欄位中的新物件或記錄。

<!--hide this for now; they are trying to remove this militation: * The automation adds additional objects only in the Many to many or One to many connection type fields. In the all other cases, the automation creates the object, but it does not connect it to the original record from which the automation is triggered.-->

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

      * 建立群組
      * 建立方案
      * 建立專案組合
      * 建立專案
      * 建立記錄

     >[!TIP]
     >
     >儲存自動化後，您將無法再變更在此欄位中選取的動作。

1. （視條件而定）根據您選取的動作，更新下列欄位：

   * **建立專案**：
      * **建立物件的已連線欄位**：這是將顯示新專案的已連線欄位。 這是必填欄位。
      * **專案範本**：選取Workfront用來建立專案的專案範本。
   * **建立投資組合**：
      * **建立物件的已連線欄位**：這是將顯示新投資組合的已連線欄位。 這是必填欄位。
      * **要附加到新投資組合的自訂表單**：選取要附加到新投資組合的自訂表單。 您必須先建立產品組合自訂表單，然後才能進行選取。
   * **建立程式**：
      * **建立物件的已連線欄位**：這是將顯示新程式的已連線欄位。 這是必填欄位。
      * **方案組合**：選取將新增新方案的組合。 這是必填欄位。
      * **要附加到新程式的自訂表單**：選取要附加到新程式的自訂表單。 您必須先建立程式自訂表單，然後才能進行選取。
   * **建立群組**：
      * **建立物件的已連線欄位**：這是將顯示新群組的已連線欄位。 這是必填欄位。
      * **要附加到新群組的自訂表單**：選取要附加到新程式的自訂表單。 您必須先建立程式自訂表單，然後才能進行選取。
   * **建立記錄**：
      * **記錄型別**：選取您要建立的記錄型別。

     **設定**&#x200B;子區段隨即顯示。 更新&#x200B;**設定**&#x200B;子區段中的下列欄位：

      * **目前記錄將顯示的連線記錄型別欄位**：這是針對目前記錄將顯示的動作選取的記錄型別上的連線欄位。

     例如，如果您正在建立行銷活動的自動化，以便從連線產品記錄，這是產品記錄型別上顯示的行銷活動之已連線欄位（使用自動化建立產品後）。

     這是必填欄位。

     <!--submitted a change in functionality and UI text for this - revise??-->
      * **對應欄位**
         * **傳輸自**：從建立自動化的記錄型別中選取欄位，以將它們對應到連線記錄型別的欄位。
         * **傳輸至**：從新建立的記錄中選取欄位，這些欄位會填入您執行自動化之記錄中的資訊。

     >[!TIP]
     >
     >來自原始記錄型別的欄位型別必須與來自新建記錄型別的欄位型別匹配。

1. （選擇性和條件性）如果您選取建立記錄，請按一下&#x200B;**新增欄位**，將其他查詢欄位從一筆記錄對應到另一筆記錄。
1. （視條件而定）如果您選取建立記錄，且原始記錄型別與在&#x200B;**動作**&#x200B;區域中所選記錄型別之間沒有連線欄位，請按一下連線記錄型別&#x200B;**欄位（目前記錄將顯示在此欄位）右邊的問號圖示**，然後按一下&#x200B;**新增**&#x200B;圖示![建立連線欄點陣圖示](assets/create-a-connection-field-icon.png)以新增連線欄位。

   系統會自動為您在&#x200B;**動作**&#x200B;區域中選取的記錄型別建立新欄位，並命名為&#x200B;**連線的記錄**。

   您設定自動化的原始記錄型別也會建立所選記錄型別的已連線欄位。
1. （選擇性和條件性）如果您選取建立Workfront物件，但沒有所選Workfront物件型別的連線欄位，請按一下&#x200B;**建立&lt; Workfront物件型別名稱>的「連線」欄位**&#x200B;欄位右側的問號圖示，然後按一下&#x200B;**新增**&#x200B;圖示![建立連線欄點陣圖示](assets/create-a-connection-field-icon.png)以新增連線欄位。

   ![](assets/question-mark-icon-to-add-connected-fields-in-automations-with-workfront.png)

   新欄位會自動建立並命名為&#x200B;**連線&lt; Workfront物件名稱>**。 例如，為記錄建立投資組合已連線欄位時，將其命名為「已連線投資組合」。

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

   1. 按一下&#x200B;**編輯**&#x200B;以更新有關自動化欄位的資訊並設定欄位。

      >[!TIP]
      >
      >   您無法變更您最初為自動化選取的動作。


   1. 按一下&#x200B;**停用**&#x200B;以從記錄的資料表檢視中移除自動化，並防止使用者使用它來建立記錄或物件。

   使用已停用的自動化所建立的記錄仍會連線至最初選取的記錄。

   若要再次使用，請按一下&#x200B;**更多**&#x200B;功能表![更多](assets/more-menu.png)，然後按一下&#x200B;**啟動**。
   1. 按一下&#x200B;**刪除**&#x200B;以刪除自動化。 已刪除的自動化無法復原。

   使用已刪除的自動化所建立的記錄會保持與原始選取的記錄連線。

## 使用Workfront Planning自動化建立物件或記錄

1. 在Workfront Planning中，開啟記錄型別頁面，其中包含您要用來自動建立及連線記錄或物件的自動化。
1. 開啟表格檢視。
1. 選取一或多個記錄。

   表格底部會顯示一個藍色列，內含其他按鈕，包括自動化按鈕。
1. 按一下熒幕右下角附近的自動化按鈕。

   ![自動化按鈕](assets/automation-custom-button.png)

   會發生下列情況：

   * 如果自動化成功建立了物件或記錄，畫面底部會顯示確認訊息。

   * 新物件會顯示在您在設定自動化按鈕時所指示的已連線欄位中。 您可能需要重新整理頁面才能檢視新物件。

   * 您從中觸發自動化的記錄已新增至新記錄的已連線欄位。

   >[!NOTE]
   >
   >建議您檢查物件或記錄是否已如預期建立及連線。

1. （選擇性）按一下已連線欄位中的新物件。 物件頁面隨即開啟，您可以對新物件進行其他變更。

<!--ORIGINAL AUTOMATION FUNCTIONALITY - BEFORE FEB. 20, 2025

You can configure automations in Adobe Workfront Planning that, when activated, create objects in Workfront or records in Workfront Planning when triggered from a Planning record. The created objects or records are automatically connected to the records you are triggering the automation from. 

You can configure and activate the automation in the record type's page in Workfront Planning. The connected object that is created is placed in the connected field of the record type you run the automation from. 

For example, you could create an automation that takes a Workfront Planning campaign and creates a project in Workfront to track that campaign's progress. The project would be connected to the Workfront Planning campaign in the Connected Project field on the campaign.

For more information on connected records, see [Connected records overview](/help/quicksilver/planning/records/connected-records-overview.md).

## Access requirements

+++ Expand to view access requirements.. 

You must have the following access to perform the steps in this article:  

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
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access all the capabilities of Workfront Planning.</p> 
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
   <p>Edit access in Workfront for the object types that you want to create (projects, portfolios, programs). </p>  
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td> <p>Manage permissions to the workspace you want to add records to. </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
   <p>Manage permissions to Workfront objects (portfolios) to add children objects (projects).</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Layout template</p></td> 
   <td> <p>All users, including Workfront administrators,  must be assigned a layout template that includes the Planning area in the Main Menu </p> </td> 
  </tr> 
</tbody> 
</table> 

 *For more information about Workfront access requirements, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).   

+++


## Considerations about creating objects and records using an automation

* The new object or record name is the same as the record name from which you create it. 
* New objects or records don't override existing ones in the same field. Triggering the same automation multiple times for the same records adds the new objects or records in the same connected field of the original record, in addition to the ones created before. 
* The automation adds additional objects only in the Many to many or One to many connection type fields. In the all other cases, the automation creates the object, but it does not connect it to the original record from which the automation is triggered. 

## Configure an automation in Workfront Planning

You must configure an automation for a record type in Workfront Planning, before you can use it to create objects.

{{step1-to-planning}}

1. Click a record type card, then click the name of a record. 

   The record type page opens. 
1. Click the **More** menu ![More menu](assets/more-menu.png) to the right of the record type name, then click **Manage automations**. 

   The list of available automations for the selected record type opens.

1. Click **New automation** in the upper-right corner of the screen. The **New automation** box opens.
1. Update the following fields:

   * Replace **Untitled automation** with the text that you want to appear on the automation button. Users will click this button when using the automation to create a Workfront object or a Planning record.
   * **Description**: Add a description to identify the purpose of the automation.
1. Click **Save**.
   The automation details page opens. 

1. On the automation's details page, update the following fields in the **Triggers** section: 

   * **Trigger**: Select the action that will trigger the automation. For example, select **Button click**. (********update this step with a list of all possible triggers; right not only Button click is available***********)

1. Update the following fields in the **Actions** section: <********submitted bugs for these fields - see if they need changing here*********)
   * **Object type**: Select the object that you want the automation to create. This is a required field.
      
      You can create the following objects from Workfront Planning records: 

      * Project
      * Portfolio
      * Program
      * Group
      * Record

      >[!TIP]
      >
      >After you saved the automation, you can no longer change the object type in this field.

1. (Conditional) Depending on what type of object you want to create, update the following fields:


   * **Project**: 
      * **Connected field where the object is created**: This is the connected field where the new project will display. This is a required field. 
      * **Template from which to create the project**: Select a project template that Workfront will use to create the project.  
   * **Portfolio**:
      * **Connected field where the object is created**: This is the connected field where the new portfolio will display. This is a required field.
      * **Custom form to attach to the new portfolio**: Select a custom form to attach to the new portfolio. You must create a portfolio custom form before you can select it. 
   * **Program**: 
      * **Connected field where the object is created**: This is the connected field where the new program will display. This is a required field.
      * **Program portfolio**: Select a portfolio where the new program will be added. This is a required field.
      * **Custom form to attach to the new program**: Select a custom form to attach to the new program. You must create a program custom form before you can select it. 
   * **Group**:
      * **Connected field where the object is created**: This is the connected field where the new group will display. This is a required field.
      * **Custom form to attach to the new group**: Select a custom form to attach to the new program. You must create a program custom form before you can select it. 
   * **Record**: 
      * **Connected record type**: Select the record type you want to create. 
      * **Connected field where the record is created**: This is the connected field where the new record will display. This is a required field. (******this might need revision as right now it shows the field on the connected record table where the current record will display; submitted a bug to correct this label*********)
      * **Map fields**
         * **Transfer from**: Select fields from the record type the automation is created for to map them to the fields of the connected record type. 
      * **Transfer to**: Select fields from the newly created record that will populate with information from the record you are running the automation from. 
1. (Optional and conditional) If you selected to create a record, click **Add fields** to map additional lookup fields from one record to another.
1. (Optional and conditional) If you don't have a connection field for a Workfront object type, click the **Create a connection field** icon ![Create a connection field icon](assets/create-a-connection-field-icon.png) to add a field.

   The new field is automatically created and named **Connected < Workfront object name >**. For example, when a portfolio connected field is created for the record, it is named "Connected portfolio." 

1. Click **Save** in the upper-right corner of the automation details page. 

   The automation displays on the list of automations, and is available to use in records.
1. (Optional) To edit, disable, or delete an automation, do the following:

   1. From the list of automations, hover over the name of a saved automation, then click the **More** menu ![More menu](assets/more-menu.png).

   1. Click **Edit** to update information about and configure fields on the automation.
   1. Click **Disable** to remove the automation from the table view and prevent users from using it to create records or objects. To make it available again, click the **More** menu ![More menu](assets/more-menu.png) again, then click **Activate**.
   1. Click **Delete** to delete the automation. A deleted automation cannot be recovered. Records that have been created using the automation remain connected to the record originally selected.  

## Use a Workfront Planning automation to create an object or a record

1. In Workfront Planning, open the record type page that contains the records you want to use to create Workfront objects or Planning records. 
1. Open the table view. 
1. Select one or more records.
   
   A blue bar displays at the bottom of the table with additional buttons, including automation buttons. 
1. Click the automation button near the lower-right corner of the screen. 

   ![Automation button](assets/automation-custom-button.png)

   A confirmation message displays at the bottom of the screen, if the automation successfully created an object or a record. 

   The new object displays in the connected field you indicated in the setup of the automation button. You might need to refresh your page before viewing the new object. 

   >[!NOTE]
   >
   >We recommend checking that the object was created and connected as expected.

1. (Optional) Click the new object in the connected field. The object page opens and you can make additional changes to the new object. 

-->

