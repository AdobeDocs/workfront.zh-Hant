---
title: 使用Workfront計畫記錄自動化建立Adobe Workfront物件
description: 您可以在Workfront Planning中設定自動化，以便在啟動時在Workfront中建立物件。
hide: true
hidefromtoc: true
exl-id: c669217a-40e2-471f-951d-93157a34f1ee
source-git-commit: 00e58ea9a207037b701e1be010c2c4c2995d60e0
workflow-type: tm+mt
source-wordcount: '1252'
ht-degree: 3%

---

# 使用Adobe Workfront Planning記錄自動化建立物件

<!--add screen shots when UI is finalized AND redo all the steps - some things got changed and moved around-->
<!--when you make this public, add this to the metadata above (and take the "hide" tags out):

feature: Workfront Planning
role: User, Admin
author: Alina, Becky
recommendations: noDisplay, noCatalog

-->

<!-- if they give access to use the automation to people with LESS than Manage permissions to a workspace, split this article in two: the Configure section should be for admins and the "Use a Workfront Planning automation to create an object" should be for all other users-->

您可以在Adobe Workfront Planning中設定自動化，以便在啟動時在Workfront或Workfront Planning中建立物件。

您可以在記錄頁面中設定並啟動自動化。 建立的物件會連線至Planning記錄，並放置在自動化中所指定的欄位中。

例如，您可以建立採用Workfront Planning行銷活動的自動化，並在Workfront中建立專案以追蹤該行銷活動的進度。 專案會連結至Workfront規劃行銷活動。

如需有關連線記錄的詳細資訊，請參閱[連線記錄總覽](/help/quicksilver/planning/records/connected-records-overview.md)。

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
   <p>在Workfront中編輯您要建立之物件型別（專案、投資組合、方案）的存取權。 </p>  
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


## 有關使用自動化建立物件和記錄的考量事項

* 新物件或記錄名稱與您建立物件或記錄時的記錄名稱相同。
* 如果您使用的自動化記錄已經連線了您選取用來加入新物件的欄位中的相同型別物件，則新物件會加入至連線欄位，而現有物件也會保持連線。

## 在Workfront Planning中設定自動化

您必須先在Workfront Planning中設定自動化，才能使用它來建立物件。

{{step1-to-planning}}

1. 按一下記錄型別卡，然後按一下記錄名稱。

   記錄型別頁面隨即開啟。
1. 按一下記錄型別名稱右側的&#x200B;**更多**&#x200B;功能表![](assets/more-menu.png)，然後按一下&#x200B;**管理自動化**。

   可用自動化清單隨即開啟。

1. 按一下熒幕右上角的&#x200B;**新自動化**。 **新自動化**&#x200B;方塊開啟。
1. 更新下列欄位：

   * 將&#x200B;**未命名的自動化**&#x200B;取代為您要顯示在自動化按鈕上的文字。 使用自動化建立Workfront物件時，使用者將按一下此按鈕。
   * **描述**：新增描述以識別自動化的目的。

1. 在自動化的詳細資訊頁面上，更新&#x200B;**觸發器**&#x200B;區段中的下列欄位：

   * **觸發器**：選取將觸發自動化的動作。 例如，選取&#x200B;**按一下**。<!--update this step with a list of all possible triggers; right not only Button click is available-->

1. 更新&#x200B;**動作**&#x200B;區段中的下列欄位：
   * **物件型別**：選取您要自動化建立的物件。 這是必填欄位。

     您可以從Workfront Planning記錄中建立下列物件：

      * 專案
      * 專案組合
      * 方案
      * 群組
      * 記錄
1. （視條件而定）視您要建立的物件型別而定，請更新下列欄位：

   * **專案**：
      * **建立物件的已連線欄位**：這是將顯示新專案的已連線欄位。 這是必填欄位
      * **建立專案的範本**：選取Workfront用來建立專案的專案範本。
   * **Portfolio**：
      * **建立物件的已連線欄位**：這是將顯示新投資組合的已連線欄位。 這是必填欄位。
      * **要附加到新投資組合的自訂表單**：選取要附加到新投資組合的自訂表單。 您必須先建立產品組合自訂表單，然後才能進行選取。
   * **程式**：
      * **建立物件的已連線欄位**：這是將顯示新程式的已連線欄位。 這是必填欄位。
      * **方案組合**：選取將新增新方案的組合。 這是必填欄位。
      * 
         * **要附加到新程式的自訂表單**：選取要附加到新程式的自訂表單。 您必須先建立程式自訂表單，然後才能進行選取。
   * **群組**：
      * **建立物件的已連線欄位**：這是將顯示新群組的已連線欄位。 這是必填欄位。
      * **要附加到新群組的自訂表單**：選取要附加到新程式的自訂表單。 您必須先建立程式自訂表單，然後才能進行選取。
   * **記錄**：
      * **連線的記錄型別**：選取您要建立的記錄型別。
      * **建立記錄的已連線欄位**：這是將顯示新記錄的已連線欄位。 這是必填欄位。
      * **對應欄位**：從建立自動化的記錄型別中選取欄位，以將它們對應到連線記錄型別的欄位。
      * **至已連線的記錄欄位**：從已連線的記錄中選取欄位，這些欄位將與您建立自動化之記錄型別中的欄位相對應。
1. （選擇性和條件性）如果您沒有Workfront物件型別的連線欄位，請按一下&#x200B;**建立連線欄位**&#x200B;圖示![](assets/create-a-connection-field-icon.png)以新增欄位。
1. （選擇性和條件性）如果您選取新增記錄，請按一下&#x200B;**對應欄位**&#x200B;區域中的&#x200B;**新增**&#x200B;以新增並對應其他欄位，然後選取要&#x200B;**從**&#x200B;傳輸檔案的欄位和要&#x200B;**傳輸檔案到**&#x200B;檔案的欄位，以指出在連線記錄的欄位中應顯示原始選取記錄的欄位。
1. 按一下「**儲存**」。

   自動化會出現在自動化清單中，並可用於記錄。
1. （可選）若要編輯、停用或刪除自動化，請執行下列動作：

   從自動化清單中，暫留在已儲存的自動化名稱上，然後按一下&#x200B;**更多**&#x200B;功能表![](assets/more-menu.png)，然後選擇下列其中一個選項：

   * **編輯**：更新自動化欄位的相關資訊並設定欄位。
   * **停用**：自動化將不會在記錄表格檢視的工具列中顯示為選項，使用者無法再用它來建立記錄或物件。 若要再次使用，請再按一下&#x200B;**更多**&#x200B;功能表![](assets/more-menu.png)，然後按一下&#x200B;**啟動**。
   * **刪除**：自動化已刪除，無法復原。 已使用自動化建立的記錄會保持與原始選取的記錄連線。

## 使用Workfront Planning自動化來建立物件

1. 在Workfront Planning中，開啟記錄型別頁面，其中包含您要用來建立Workfront物件的記錄。
1. 開啟表格檢視。
1. 選取一或多個記錄。

   表格底部會顯示一個藍色列，內含其他按鈕，包括自動化按鈕。
1. 按一下熒幕右下角附近的自動化按鈕。

   ![自動化按鈕](assets/automation-custom-button.png)

   新物件會顯示在您在設定自動化按鈕時所指示的已連線欄位中。

   >[!NOTE]
   >
   >建議您檢查物件是否已如預期建立及連線。

1. （選擇性）按一下已連線欄位中的新物件。 物件頁面隨即開啟，您可以對新物件進行其他變更。

<!--you might need to add something about notifications and emails?!-->
