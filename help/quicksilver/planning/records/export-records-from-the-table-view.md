---
title: 從表格檢視匯出記錄
description: 您可以從表格檢視將記錄及其資訊匯出至CSV或Excel檔案。
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: d8ac4d94-28b5-41d6-acb8-259696897c8a
source-git-commit: 8546311acf722c0f4d47d4663b02ff701416894a
workflow-type: tm+mt
source-wordcount: '464'
ht-degree: 1%

---

# 從表格檢視匯出記錄

<!--<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

您可以在Adobe Workfront Planning中，從表格檢視將記錄及其資訊匯出至Excel或CSV檔案。

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
   <td role="rowheader"><p>Adobe Workfront授權</p></td> 
   <td><p>淺色或更高</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>物件許可權</p></td> 
   <td> <p>檢視或更高的工作區許可權和記錄型別</p>   
   <p>檢視或更高的檢視許可權</p>

</td> 
  </tr> 
  <tr>
   <td role="rowheader"><p>版面配置範本</p></td>
   <td> 必須為具有輕度或貢獻者授權的使用者指派包含Planning的版面配置範本。
   <p>標準使用者和系統管理員預設會啟用Planning區域。</p></div></li></ul>
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
   <td><p> Light or higher </p>
   <p>Workfront Planning is not available for legacy Workfront licenses</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>View or higher permissions to a view</p>  
   </td> 
  </tr> 
</tbody> 
</table> -->


## 從表格檢視匯出記錄

匯出表格檢視時，請考量下列事項：

* 匯出至Excel檔案的資訊會保留套用至Workfront Planning表格檢視的篩選器、群組和排序。 群組在CSV檔案中不可見。

* 匯出的檔案不支援縮圖和自訂列顏色。

* 只會匯出Workfront介面中顯示的欄位。 隱藏欄位不會匯出。

若要從表格檢視或記錄型別匯出資訊，請執行下列動作：

1. 移至記錄型別頁面，然後按一下表格檢視標籤。
1. 執行下列其中一項：

   * 暫留在表格檢視標簽名稱上，然後按一下檢視名稱右邊的&#x200B;**更多**&#x200B;功能表![更多](assets/more-menu.png)，然後按一下&#x200B;**匯出**。

   檢視表上的![更多功能表](assets/view-more-menu-with-duplicate-option.png)

   * 按一下「共用&#x200B;**>**&#x200B;匯出目前的檢視&#x200B;**」。**&#x200B;只有在顯示表格檢視時，才能使用此選項。

   ![含有記錄型別和檢視共用選項的[共用]按鈕](assets/share-button-with-record-type-and-view-sharing-options.png)

1. 選取下列其中一種格式：

   * **Excel**
   * **CSV**

   >[!IMPORTANT]
   >
   >當您在熒幕上顯示不同的檢視時，無法從表格檢視中匯出資訊。 您必須顯示要匯出的表格檢視，才能存取「更多」選單中的「匯出」選項。

   檔案已下載到您的電腦。

1. （選擇性）前往電腦上的下載資料夾，並尋找已下載的檔案。

   匯出的檔案名稱會遵循下列格式：

   `Name of the view - name of the record type`

   例如，促銷活動記錄型別的表格檢視會產生名為`Table view - Campaigns`的檔案。

   檔案會顯示下列資訊：

   * 在Excel檔案中，欄標題會以黑色反白
   * Workfront介面中可見的所有欄位，皆依相同條件排序和篩選
   * 群組會保留在Excel檔案中

   您現在可以與其他人共用匯出的檔案，或將它們附加到任何通訊中。

</div>
