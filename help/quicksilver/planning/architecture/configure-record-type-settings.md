---
title: 設定記錄型別的設定區域
description: 除了在「編輯記錄型別」方塊中編輯記錄型別外，您還可以在「設定」頁面中編輯記錄型別。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
source-git-commit: 2fb95d37c32984e248767993c4858038d27e0590
workflow-type: tm+mt
source-wordcount: '483'
ht-degree: 2%

---


# 設定記錄型別的設定區域

<span class="preview">此頁面上的資訊是指尚未普遍提供的功能。 它僅在預覽環境中可供所有客戶使用。 每月發行至生產環境後，生產環境中為啟用快速發行的客戶也提供相同的功能。</span>

<span class="preview">如需快速發行資訊，請參閱[為您的組織啟用或停用快速發行](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>

{{planning-important-intro}}

在Adobe Workfront Planning中儲存記錄型別後，您就可以設定記錄型別的其他設定。

根據您要為記錄型別定義哪些功能，您可以執行下列操作之一來設定其他設定：

<!--the above will need to be reworded when we add automations and manage request forms to this area-->

* 編輯它們

  如需詳細資訊，請參閱[編輯記錄型別](/help/quicksilver/planning/architecture/edit-record-types.md)。

* 正在設定記錄型別的「設定」頁面。

  本文說明如何透過設定記錄的「設定」頁面來編輯記錄型別。

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

<p>若要設定全域記錄型別，請執行下列動作：</p>

<ul> 
<li><p>任何Workfront套件和Planning Plus套件</p></li>
<p>或</p>
<li><p>任何工作流程和Planning Prime或Ultimate套件</p></li></ul>
<p>如需每個Workfront Planning套件所含內容的詳細資訊，請聯絡您的Workfront客戶代表。 </p>
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
</table> 

-->

## 在設定頁面中設定記錄型別資訊

您可以在記錄型別的「設定」頁面中設定資訊，以定義記錄型別的跨工作區功能。

<!--the intro above will change when we can configure more in this area -->

{{step1-to-planning}}

1. 按一下您要編輯其記錄型別的工作區，

   工作區頁面隨即開啟，且記錄型別隨即顯示。
1. 執行下列其中一項：

   * 將滑鼠停留在記錄型別的卡片上，然後按一下記錄型別卡片右上角的&#x200B;**更多**&#x200B;功能表![更多功能表](assets/more-menu.png)，然後按一下&#x200B;**設定**

     ![更多記錄型別卡片中的功能表選項](assets/more-menu-options-from-record-type-card-with-settings-link.png)

     或

   * 按一下記錄型別卡片以開啟記錄型別頁面，按一下記錄型別名稱右側的&#x200B;**更多**&#x200B;功能表![更多](assets/more-menu.png)，然後按一下&#x200B;**設定**。

   <!--update screen shot at prod??-->

   ![設定頁面上的跨工作區設定](assets/settings-page-cross-workspace-settings.png)

1. 預設會選取&#x200B;**跨工作區設定**&#x200B;區段。
1. 開啟或關閉下列其中一個設定：

   * **允許將此記錄型別新增至其他工作區**，以表示這是全域記錄型別
   * **允許連線到其他工作區中的這個記錄型別**，以表示這是可連線的記錄型別。

   設定預設為關閉。

   如需詳細資訊，請參閱[設定記錄型別的跨工作區功能](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md)