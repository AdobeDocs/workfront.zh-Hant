---
title: 還原已刪除的記錄
description: 您可以從Adobe Workfront Planning的「最近刪除」區域中復原已刪除的記錄。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
source-git-commit: 6327e5625481ce7ff8d744bc6eb50d417cbb4413
workflow-type: tm+mt
source-wordcount: '534'
ht-degree: 1%

---


# 還原已刪除的記錄

<span class="preview">此頁面上的資訊是指尚未普遍提供的功能。 它僅在預覽環境中可供所有客戶使用。 每月發行至生產環境後，生產環境中為啟用快速發行的客戶也提供相同的功能。</span>

<span class="preview">如需快速發行資訊，請參閱[為您的組織啟用或停用快速發行](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>

{{planning-important-intro}}

您可以從Adobe Workfront Planning的「最近刪除」區域中復原已刪除的記錄。

如需有關刪除記錄的資訊，請參閱[刪除記錄](/help/quicksilver/planning/records/delete-records.md)。

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
   <td>   <p>管理工作區</a>的許可權 </p>  
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

## 復原已刪除記錄的相關考量事項

* 記錄會儲存在「最近刪除」的資料匣中30天。 30天後，記錄會從Workfront Planning中永久刪除。
* 如果刪除的記錄連結到其他記錄，則連結的記錄不會被刪除，但是已刪除的記錄中的資訊也會被刪除。 還原已刪除的記錄將會從連線的記錄中還原資訊。
* 您可以大量還原記錄。
* 刪除記錄時，會將下列資訊儲存在「最近刪除」的資料匣中：
   * **名稱**：這是記錄的[主要]欄位中的資訊。 如需有關記錄主要欄位的詳細資訊，請參閱[主要欄位概述](/help/quicksilver/planning/fields/primary-field-overview.md)。
   * **已刪除日期**：刪除記錄的時間和日期。
   * **最近刪除的時間**：刪除記錄後的時間。 在目前日期前30天以上被刪除的記錄不會顯示在「最近刪除」的資料匣中。
   * **由**&#x200B;刪除：刪除紀錄的使用者名稱。

## 還原已刪除的記錄

1. 移至您刪除記錄的記錄型別頁面。
1. 按一下任何記錄型別頁面檢視右上角的&#x200B;**復原**&#x200B;圖示![](assets/undo-icon.png)，然後按一下&#x200B;**最近刪除**。

   顯示&#x200B;**最近刪除的**&#x200B;方塊。

   ![](assets/recently-deleted-box.png)

1. 選取您要刪除的記錄，然後按一下&#x200B;**還原** > **還原**。 您可以選取多個記錄。

   如果還原成功，您會在畫面底部收到成功通知。
1. 移至表格檢視並檢閱還原的記錄。