---
title: 重複記錄
description: 您可以在表格檢視中複製現有記錄。 現有記錄的相同副本將新增到記錄型別頁面。
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 2fed8c96-0c9c-4662-a9c4-66dae507ff2a
source-git-commit: 9debb7c6d9df0f9f4962f3e66f146e5f605d20f0
workflow-type: tm+mt
source-wordcount: '586'
ht-degree: 2%

---

# 複製記錄

{{planning-important-intro}}

在Adobe Workfront Planning中，記錄是記錄型別的例項。

您可以在表格檢視中複製現有記錄。 現有記錄的相同副本將新增到記錄型別頁面。

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
   <td>   <p>Contribute或更高的工作區許可權</a> </p>  
   <p>系統管理員擁有所有工作區的許可權，包括他們未建立的工作區</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>版面配置範本</p></td> 
   <td> <p>必須為所有使用者(包括Workfront管理員)指派一個版面配置範本，該範本包含主功能表中的Planning區域。 </p> </td> 
  </tr> 
</tbody> 
</table>

*如需Workfront存取需求的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

<!--
OLD:

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the early access stage for Workfront Planning </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license*</p></td>
   <td>
   <p>New: Standard</p>
   <p>Current: Plan</p>  
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level configurations</p></td>
   <td> <p>There are no access controls for Adobe Workfront Planning </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Contribute or higher permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Planning area in your layout template. For information, see <a href="/help/quicksilver/planning/access/access-overview.md">Access overview</a>. </p>  
</td>
  </tr>

 </tbody>
</table>

*For more information, see [Access requirements for Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

-->


## 複製記錄<!--in a record type table (I don't think you can create them elsewhere right now)-->

您可以在記錄型別頁面的表格檢視中複製現有的記錄，藉此建立記錄。 與現有記錄相同的記錄會建立並新增至原始記錄下。


{{step1-to-planning}}

1. 按一下您要新增記錄的工作區。

   工作區隨即開啟，且記錄型別會顯示為卡片。

1. 按一下記錄型別卡。 如需有關建立記錄型別的資訊，請參閱[建立記錄型別](/help/quicksilver/planning/architecture/create-record-types.md)。

   記錄型別頁面會在您上次存取的檢視中開啟。 依預設，會在表格檢視中開啟記錄型別頁面。
所選型別的所有記錄都會顯示在檢視中。

1. （視條件而定）選取表格檢視。

1. 執行下列其中一項：

   * 暫留在記錄名稱上，然後按一下內嵌記錄名稱的&#x200B;**更多**&#x200B;功能表，然後按一下&#x200B;**複製**&#x200B;圖示![](assets/duplicate-icon-gray.png) 。

     ![](assets/more-menu-from-record-in-table-view.png)

   * 選取記錄，然後按一下頁面底部工具列中的&#x200B;**複製**&#x200B;圖示![](assets/duplicate-icon-white-and-blue.png)。

     ![](assets/duplicate-icon-in-toolbar-in-table-view.png)

   在原始記錄下會建立具有相同名稱的相同記錄。 新記錄的所有欄位都會填入與原始記錄相同的資訊。

1. （選擇性）在表格檢視中可用的欄位中開始更新有關新記錄的資訊，或在記錄預覽或頁面中按一下記錄並更新資訊。

   >[!NOTE]
   >
   >  * 記錄沒有必填欄位。 不過，我們建議您為記錄的主要欄位新增資訊，因為將記錄連結至彼此時，識別記錄會很有幫助。 如需主要欄位的詳細資訊，請參閱[管理資料表檢視](/help/quicksilver/planning/views/manage-the-table-view.md)和[主要欄位概述](/help/quicksilver/planning/fields/primary-field-overview.md)。
   >
   >  * 參考其他記錄型別或計算欄位的欄位為唯讀欄位。

   如需編輯記錄的詳細資訊，請參閱[編輯記錄](/help/quicksilver/planning/records/edit-records.md)。

1. （可選）在表格檢視中新增記錄或其資訊時，請使用下列鍵盤快速鍵來復原或重做新增記錄或其資訊：

   * CTRL + Z (Mac為⌘ + Z)可復原變更
   * CTRL + Shift + Z (Mac為⌘ + Shift + Z)以重做變更。
