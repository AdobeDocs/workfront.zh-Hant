---
title: 刪除工作區
description: 當工作區不再相關時，您可以將其刪除。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: adec4b8e-2964-479b-8cf0-79d3afa27b2a
source-git-commit: e25f6ac3fb4ffc114d59bf5cceecfe718ae914ec
workflow-type: tm+mt
source-wordcount: '522'
ht-degree: 1%

---


# 刪除工作區

<span class="preview">此頁面上的資訊是指尚未普遍提供的功能。 它僅在預覽環境中可供所有客戶使用。 每月發行至生產環境後，生產環境中為啟用快速發行的客戶也提供相同的功能。</span>

<span class="preview">如需快速發行資訊，請參閱[為您的組織啟用或停用快速發行](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>

{{planning-important-intro}}

在Adobe Workfront Planning中，工作區是團隊規劃工作的集中位置。 如需詳細資訊，請參閱[建立工作區](/help/quicksilver/planning/architecture/create-workspaces.md)。

您可以刪除不再相關的工作區。

建議您先在其他工作區中重新建立與您要刪除的工作區相關聯的部分或全部記錄型別、記錄、欄位和檢視，然後再刪除工作區。

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
   <td>   <p>管理工作區</a>的許可權 </p>  
   <p>系統管理員擁有所有工作區的許可權，包括他們未建立的工作區</p> </td> 
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

## 有關刪除工作區的考量事項

* 當您刪除工作區時，也會刪除所有記錄型別、記錄、其欄位和檢視。
* 已刪除的工作區及其包含的資訊無法復原。

## 刪除工作區

{{step1-to-planning}}

1. （視條件而定）如果您是Workfront管理員，請按一下「**我所在的工作區**」以存取您建立的工作區，或按一下「**其他工作區**」以存取其他人與您共用的工作區。

1. （選擇性）按一下「**全部顯示**」以顯示其他工作區。 **顯示全部**&#x200B;連結只有在您有兩列以上的工作區卡片時才會顯示。
1. （選用） ClicK **顯示較少**&#x200B;以限制熒幕上顯示的工作區數目。
1. 若要刪除工作區，請執行下列任一項作業：

   * 將滑鼠停留在工作區卡片上，然後按一下卡片右上角的&#x200B;**更多**&#x200B;功能表![更多功能表](assets/more-menu.png)
或
   * 按一下工作區卡以開啟工作區，然後按一下工作區名稱右側的&#x200B;**更多**&#x200B;功能表![更多](assets/more-menu.png)。
1. 按一下&#x200B;**刪除**。

   ![永久刪除工作區確認](assets/permanently-delete-workspace-confirmation.png)

1. 在提供的空白處輸入&#39;&#39;**&#39;delete**&#39;&#39;，然後按一下&#x200B;**&#39;永久刪除**。 不區分大小寫。

   工作區已刪除且無法復原。 任何與其關聯的記錄型別、記錄、欄位和檢視也會被刪除。<!--ensure this is right at or before GA-->
