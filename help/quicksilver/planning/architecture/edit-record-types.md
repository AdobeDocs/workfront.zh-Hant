---
title: 編輯記錄型別
description: 記錄型別儲存後，您可以編輯記錄型別。 記錄型別是Adobe Workfront Planning的物件型別。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 7d6de742-9657-4286-968c-1fc78ebbb94e
source-git-commit: 939f3d9a4fac609c014acfc3be3d1485f469e947
workflow-type: tm+mt
source-wordcount: '753'
ht-degree: 2%

---


# 編輯記錄型別

<span class="preview">此頁面上的資訊是指尚未普遍提供的功能。 它僅在預覽環境中可供所有客戶使用。 每月發行至生產環境後，生產環境中為啟用快速發行的客戶也提供相同的功能。</span>

<span class="preview">如需快速發行資訊，請參閱[為您的組織啟用或停用快速發行](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>

{{planning-important-intro}}

記錄型別是Adobe Workfront Planning的物件型別。 您可以編輯您或其他人建立的記錄型別外觀。 如需建立Workfront Planning記錄型別的相關資訊，請參閱[建立記錄型別](/help/quicksilver/planning/architecture/create-record-types.md)。

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
<p>貴組織的Workfront例項必須上線至Adobe Unified Experience，才能存取Workfront Planning。</p> 
<p>如需詳細資訊，請參閱<a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">適用於Workfront的Adobe Unified Experience</a>。 </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront授權*</p></td> 
   <td><p> 標準 </p>
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
   <td>   <p>管理工作區<span class="preview">和記錄型別</span>的許可權 </p>  
   <p>系統管理員擁有所有工作區的許可權，包括他們未建立的工作區</p>
   <p>只有系統管理員可以啟用記錄型別以從其他工作區連線</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>版面配置範本</p></td> 
   <td> <p>在生產環境中，所有使用者（包括系統管理員）都必須指派給包含Planning的版面配置範本。</p>
<p><span class="preview">在預覽環境中，標準使用者和系統管理員預設啟用Planning。</span></p> </td> 
  </tr> 
</tbody> 
</table>

*如需Workfront存取需求的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 編輯記錄型別

{{step1-to-planning}}

1. 按一下您要編輯其記錄型別的工作區，

   工作區頁面隨即開啟，且記錄型別隨即顯示。
1. 執行下列其中一項：

   * 暫留在記錄型別的卡片上，然後按一下記錄型別卡片右上角的&#x200B;**更多**&#x200B;功能表![更多功能表](assets/more-menu.png)，然後按一下&#x200B;**編輯**
或
   * 按一下記錄型別卡片以開啟記錄型別頁面，按一下記錄型別名稱右側的&#x200B;**更多**&#x200B;功能表![更多](assets/more-menu.png)，然後按一下&#x200B;**編輯**。

   ![更多記錄型別卡片中的功能表選項](assets/more-menu-options-from-record-type-card.png)

1. 在&#x200B;**編輯記錄型別**&#x200B;方塊中，**外觀**&#x200B;索引標籤預設為開啟。

   ![編輯記錄型別方塊外觀索引標籤](assets/edit-record-type-box-appearance-tab.png)

   更新&#x200B;**外觀**&#x200B;索引標籤中的下列資訊：

   * 視需要編輯記錄型別名稱。<!--did they add a field label for this?-->
   * **描述**：編輯或新增記錄型別的描述，其中包含更多相關資訊。
   * 編輯與記錄型別關聯的圖示的顏色和形狀。 執行下列動作：
      * 選取顏色以識別記錄型別。 這是記錄型別圖示的顏色。
      * 從清單中選取圖示，或開始輸入圖示名稱以說明其代表內容，然後在顯示時選取它。 這是記錄型別的圖示。 依預設，會選取檔案圖示。

1. （條件式）如果您是系統管理員，請按一下&#x200B;**編輯記錄型別**&#x200B;方塊中的&#x200B;**進階設定**&#x200B;索引標籤。<!--the info here is duplicated in the Create record types article-->

   ![編輯記錄型別方塊進階設定索引標籤](assets/edit-record-type-box-advanced-settings-tab.png)

1. （條件式）在&#x200B;**進階設定**&#x200B;標籤中更新下列資訊：

   * 啟用&#x200B;**從其他工作區連線**&#x200B;設定。 啟用時，記錄型別可供存取，並可從其他工作區連線。
   * 選擇可存取記錄型別的工作區。 從下列選項中選擇：

      * **系統範圍**：使用者可以從他們擁有管理許可權的所有工作區連線到此記錄型別。
      * **特定工作區**：新增工作區管理員可連線至此記錄型別的工作區名稱。

1. 按一下「**儲存**」。

   工作區上的記錄型別卡片會在右上角顯示連線圖示![從其他工作區連線圖示](assets/connect-from-other-workspaces-icon.png)，表示現在可以從其他工作區存取記錄。

1. （可選）從工作區區域按一下記錄型別卡以開啟記錄型別的頁面，然後重新命名標題中的記錄型別。

1. （選擇性）若要編輯其他記錄型別，請從記錄型別頁面中，展開記錄型別名稱右側的向下箭頭，搜尋記錄型別，然後在其顯示在清單中時選取該記錄型別。

   ![具有搜尋方塊的記錄型別頁面上的記錄型別下拉式清單](assets/record-type-drop-down-on-record-type-page-with-search-box.png)
