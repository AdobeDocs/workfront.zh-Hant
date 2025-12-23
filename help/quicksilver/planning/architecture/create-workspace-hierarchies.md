---
title: 建立Workspace階層
description: 身為工作區管理員，您可以在Adobe Workfront Planning的記錄型別之間建立多個工作區階層。 在工作區中連線記錄型別並建立階層後，記錄型別會彼此連線，其中一個記錄型別被指定為父項，而最多3個其他記錄型別被設定為子項。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 2f83c427-4439-499d-a0b2-fc8630552cae
source-git-commit: 34921b12ad902ba7390e4ea34825331280e7a8d6
workflow-type: tm+mt
source-wordcount: '953'
ht-degree: 1%

---


# 建立工作區階層

<span class="preview">此頁面上的資訊是指尚未普遍提供的功能。 它僅在預覽環境中可供所有客戶使用。 每月發行至生產環境後，生產環境中為啟用快速發行的客戶也提供相同的功能。</span>

<span class="preview">如需快速發行資訊，請參閱[為您的組織啟用或停用快速發行](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>

身為工作區管理員，您可以在Adobe Workfront Planning的記錄型別之間建立多個工作區階層。

在工作區中連線記錄型別後，您可以建立組織這些連線的階層。 階層將記錄和物件型別組織成父子關係，最多可包含四個層級的物件型別。

如果兩個記錄型別之間的連線尚未存在，則可在您設定階層時建立該連線。 定義之後，階層會跨工作區內的相關記錄型別建立結構化路徑。

階層會為其各自的記錄產生階層連結，並顯示在它們的標題中。 如此一來，使用者就能在工作流程的任何階段知道自己在階層中的位置。

如需階層與階層連結的一般資訊，請參閱[階層與階層連結概觀](/help/quicksilver/planning/architecture/hierarchy-and-breadcrumb-overview.md)。

## 存取權要求

+++ 展開以檢視存取需求，以執行本文中的步驟：  

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
   <td role="rowheader"><p>Adobe Workfront 封裝</p></td> 
   <td> 
<ul> 
<li><p>任何Workfront和任何Planning套件</p></li>
或
<li><p>任何工作流程與任何Planning套件</p></li></ul>
<p>如需每個Workfront Planning套件所含內容的詳細資訊，請聯絡您的Workfront客戶代表。 </p> 
   </td> 
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

## 建立工作區階層

您最多可以在一個工作區中建立5個階層。

{#step1-to-planning}

1. 按一下工作區卡片。
1. 按一下工作區名稱右側的&#x200B;**更多**&#x200B;功能表![更多功能表](assets/more-menu.png)，然後按一下&#x200B;**設定**。
**階層**&#x200B;區段預設會開啟。
1. 按一下&#x200B;**階層**&#x200B;頁面右上角的&#x200B;**新階層**。
1. 按一下&#x200B;**新增物件**，然後從下拉式功能表中選取物件型別。 這將是階層中的第一個物件型別。<!--logged bug to correct to "Add object type"-->

   第一個物件型別只能是Planning記錄型別。

   Workfront專案不能選取為階層中其他物件型別的父項。

1. 按一下&#x200B;**新增物件**&#x200B;以新增第二個物件型別，這是階層中的第一個子系，然後在下拉式選單中選取另一個物件型別。
每個額外的物件型別都會成為先前物件型別的子系。

   ![未選取欄位的新階層方塊](assets/new-hierarchy-modal-without-connecte-fielf-selected.png)

1. 按一下&#x200B;**選取連線的欄位**，以指出連線兩個物件的欄位。
1. （視條件而定）如果有多個連線欄位，請從清單中選取一個，

   或

   按一下[新增連線]&#x200B;**&#x200B;**&#x200B;以新增連線欄位。

   這會根據您當作父項的記錄型別建立一個連線欄位，並根據您當作子項的記錄型別建立一個對應的連線欄位。

   如果您要建立與Workfront專案的連線，專案上不會建立任何欄位。

1. （視條件而定）如果沒有可用的連線欄位，請按一下[建立連線] **並新增連線，然後按一下[儲存]**&#x200B;**。**

1. （視條件而定）如果您要新增連線，請執行下列動作：

   1. 在&#x200B;**名稱**&#x200B;方塊中新增連線欄位的名稱。
   1. 從下列連線型別中選取：

      * **多對多**
      * **一對多**
      * **多對一**
      * **一對一**

   1. 選取下列記錄外觀型別之一：

      * **名稱和影像**
      * **名稱**
      * **影像**

      如需詳細資訊，請參閱[連線記錄型別](/help/quicksilver/planning/architecture/connect-record-types.md)。

   1. 按一下「**儲存**」。

1. （視條件而定）如果在建立連線的欄位時，未選取連結的記錄型別&#x200B;**上的**&#x200B;建立對應欄位，您會收到錯誤訊息，必須先執行下列動作： <!--check back on these steps; this is supposed to be seamless, but now you have to abandon creating a hierarchy to do this-->

   1. 在&#x200B;**新階層**&#x200B;方塊中按一下&#x200B;**取消**。
   1. 按一下工作區名稱左側的返回箭頭，然後按一下您要選擇作為父項的記錄型別的卡片。
   1. 開啟您在上一步驟中所選記錄型別的表格檢視，然後移至連線欄位，其中含有您要做為子項的物件型別，將游標停留在欄標題上，然後按一下&#x200B;**編輯**&#x200B;欄位。
   1. 開啟&#x200B;**在連結的記錄型別**&#x200B;上建立對應的欄位，然後按一下&#x200B;**儲存**。
   1. 返回工作區的&#x200B;**設定**&#x200B;區域，再按一下&#x200B;**新增階層**，然後依照步驟建立階層。

1. （選用）依照上述步驟，繼續新增最多4種物件型別至您的階層。 您可以先新增所有物件型別，然後再新增它們之間的連線欄位。
1. （選擇性）按一下&#x200B;**移除**&#x200B;圖示![移除圖示](assets/minus-icon.png)以移除連線。
1. 按一下&#x200B;**儲存**&#x200B;以儲存您的階層。

   >[!TIP]
   >
   >如果您未設定所有連線的欄位，**儲存**&#x200B;按鈕會變暗。

   會發生下列情況：

   * 階層已新增至工作區的&#x200B;**階層**&#x200B;區段。
   * 當您前往記錄的頁面時，填入連線欄位的記錄會顯示其階層連結中的所有連線。

   >[!NOTE]
   >
   >您可以將子記錄型別的一個記錄連線到父記錄型別的最多10個記錄。
   >
   >如需詳細資訊，請參閱[階層與階層連結概觀](/help/quicksilver/planning/architecture/hierarchy-and-breadcrumb-overview.md)。

1. （選用）暫留在階層上，然後按一下&#x200B;**更多**&#x200B;功能表。

   ![階層更多功能表已展開](assets/hierarchy-more-menu-expanded.png)

1. 按一下下列其中一項：

   * **編輯**：這會開啟&#x200B;**編輯階層**&#x200B;方塊，您可以在此進行變更。
   * **刪除**：這會永久刪除階層。 已刪除的階層無法復原。 不會刪除連線欄位。





