---
title: 編輯記錄型別
description: 記錄型別儲存後，您可以編輯記錄型別。 記錄型別是Adobe Workfront Planning的物件型別。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 7d6de742-9657-4286-968c-1fc78ebbb94e
source-git-commit: 2fb95d37c32984e248767993c4858038d27e0590
workflow-type: tm+mt
source-wordcount: '634'
ht-degree: 2%

---


# 編輯記錄型別

<span class="preview">本頁醒目提示的資訊指出尚未普遍可用的功能。 它僅在預覽環境中可供所有客戶使用。 每月發行至生產環境後，生產環境中為啟用快速發行的客戶也提供相同的功能。</span>

<span class="preview">如需快速發行資訊，請參閱[為您的組織啟用或停用快速發行](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>

{{planning-important-intro}}

記錄型別是Adobe Workfront Planning的物件型別。 您可以編輯您或其他人建立的記錄型別外觀。 如需建立Workfront Planning記錄型別的相關資訊，請參閱[建立記錄型別](/help/quicksilver/planning/architecture/create-record-types.md)。

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
<p>任何Workfront和Planning套件</p>
<p>任何Workfront和Planning套件</p>
<p><b>附註</b></p>
<p>若要設定可連線的記錄型別： </p>
<ul> 
<li><p>任何Workfront套件和任何Planning套件</p></li>
<p>或</p>
<li><p>任何工作流程和Planning Prime或Ultimate套件</p></li></ul>

<div class="preview">
<p>若要設定全域記錄型別，請執行下列動作：</p>

<ul> 
<li><p>任何Workfront套件和Planning Plus套件</p></li>
<p>或</p>
<li><p>任何工作流程和Planning Prime或Ultimate套件</p></li></ul>
<p>如需每個Workfront Planning套件所含內容的詳細資訊，請聯絡您的Workfront客戶代表。 </p>

</div>
   </td> </tr>
  <tr> 
   <td role="rowheader"><p>Adobe Workfront授權</p></td> 
   <td><p>標準</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>物件許可權</p></td> 
   <td>   <p>管理工作區的許可權</p>  
   <p>系統管理員擁有所有工作區的許可權，包括他們未建立的工作區</p>  </td> 
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
   <td><p> Standard </p>
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
   <td>   <p>Manage permissions to a workspace and record type </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
   <p>Only system administrators can enable record types to connect from other workspaces</p> </td> 
  </tr> 

</tbody> 
</table> -->

## 編輯記錄型別

{{step1-to-planning}}

1. 按一下您要編輯其記錄型別的工作區。

   工作區頁面隨即開啟，且記錄型別隨即顯示。
1. 執行下列其中一項：

   * 暫留在記錄型別的卡片上，然後按一下記錄型別卡片右上角的&#x200B;**更多**&#x200B;功能表![更多功能表](assets/more-menu.png)，然後按一下&#x200B;**編輯**
     <span class="preview">或&#x200B;**設定**</span>
或
   * 按一下記錄型別卡片以開啟記錄型別頁面，按一下記錄型別名稱右邊的&#x200B;**更多**&#x200B;功能表![更多](assets/more-menu.png)，然後按一下&#x200B;**編輯** <span class="preview">或&#x200B;**設定**</span>。

   <span class="preview">![更多含設定的記錄型別卡片功能表選項](assets/more-menu-options-from-record-type-card-with-settings-link.png)</span>

1. 在&#x200B;**編輯記錄型別**&#x200B;方塊中，**外觀**&#x200B;索引標籤預設為開啟。<!--update screen shot below at production-->

   ![編輯記錄型別方塊外觀索引標籤](assets/edit-record-type-box-appearance-tab.png)

   更新&#x200B;**外觀**&#x200B;索引標籤中的下列資訊：

   * 視需要編輯記錄型別名稱。<!--did they add a field label for this?-->
   * **描述**：編輯或新增記錄型別的描述，其中包含更多相關資訊。
   * 編輯與記錄型別關聯的圖示的顏色和形狀。 請執行下列動作：
      * 選取顏色以識別記錄型別。 這是記錄型別圖示的顏色。
      * 從清單中選取圖示，或開始輸入圖示名稱以說明其代表內容，然後在顯示時選取它。 這是記錄型別的圖示。 依預設，會選取檔案圖示。

1. （選擇性和條件性）如果您是系統管理員，請按一下&#x200B;**進階設定** <span class="preview">或&#x200B;**跨工作區設定**</span>&#x200B;索引標籤，並更新記錄型別的跨工作區功能相關資訊。

   如需詳細資訊，請參閱[設定記錄型別的跨工作區功能](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md)。<!--update screen shot at production - Jan 2026-->

   ![使用進階設定索引標籤編輯記錄型別方塊](assets/edit-record-type-box-advanced-settings-tab.png)

1. 按一下「**儲存**」。

   如果您選擇從其他工作區連線此記錄，記錄卡上會顯示&#x200B;**可連線的記錄**&#x200B;圖示![從其他工作區連線圖示](assets/connect-from-other-workspaces-icon.png)。

   <span class="preview">如果您選取允許將此記錄新增至其他工作區，記錄卡上會顯示&#x200B;**全域記錄**&#x200B;圖示![全域記錄型別圖示](assets/global-icon.png)。</span>

1. （可選）從工作區區域按一下記錄型別卡以開啟記錄型別的頁面，然後重新命名標題中的記錄型別。

1. （選擇性）若要編輯其他記錄型別，請從記錄型別頁面中，展開記錄型別名稱右側的向下箭頭，搜尋記錄型別，然後在其顯示在清單中時選取該記錄型別。

   ![具有搜尋方塊的記錄型別頁面上的記錄型別下拉式清單](assets/record-type-drop-down-on-record-type-page-with-search-box.png)
