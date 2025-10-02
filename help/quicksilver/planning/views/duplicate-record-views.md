---
title: 複製記錄檢視
description: 如果要保留一個檢視的多個版本，並在這些版本之間做些細微的變更，您可以在Adobe Workfront Planning中複製檢視。 本文說明如何複製檢視。
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 441a53d1-ad39-41b7-93fe-2ae1836476c9
source-git-commit: fbf902196c9f5b55ddd1e20516e4237309dff2ed
workflow-type: tm+mt
source-wordcount: '454'
ht-degree: 1%

---

# 複製記錄檢視

<!--remove preview and production references-->

<span class="preview">本頁醒目提示的資訊指出尚未普遍可用的功能。 它僅在預覽環境中可供所有客戶使用。 每月發行至生產環境後，生產環境中為啟用快速發行的客戶也提供相同的功能。</span>

<span class="preview">如需快速發行資訊，請參閱[為您的組織啟用或停用快速發行](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>


{{planning-important-intro}}

如果要保留一個檢視的多個版本，並在這些版本之間做些細微的變更，您可以在Adobe Workfront Planning中複製檢視。

複製檢視會建立現有檢視的相同副本。

原始檢視的共用許可權不會轉移到複製的檢視。

在Workfront Planning中，所有檢視型別的複製檢視都相同。

## 存取需求

+++ 展開以檢視存取需求。 

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
<ul><li>選擇</li> 
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
   <td>   <p>管理檢視的許可權</p>  
   <p>檢視檢視許可權以暫時變更檢視設定或複製檢視。</p> </td> 
  </tr> 
</tbody> 
</table>

*如需Workfront存取需求的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++   

## 複製記錄檢視

{{step1-to-planning}}

1. 按一下工作區的卡片。

   工作區隨即開啟，且記錄型別會顯示為卡片。

1. 按一下記錄型別卡。

   記錄型別頁面隨即開啟。
依預設，所選型別的所有記錄都會顯示在表格檢視中。

1. 根據您使用的環境，執行下列動作：

   * 在生產環境中，將滑鼠停留在檢視標籤中其中一個檢視名稱上，然後按一下檢視名稱左側的&#x200B;**更多** ![更多功能表](assets/more-menu.png)，然後按一下&#x200B;**複製**。
   * <span class="preview">在預覽環境中，按一下目前檢視名稱旁邊的下拉式清單圖示![下拉式清單圖示](assets/drop-down-icon.png)，將滑鼠移至檢視名稱上，按一下&#x200B;**更多**，然後按一下&#x200B;**複製**。</span>

     ![檢視的其他功能表（含選項）](assets/more-menu-for-views-expanded-with-delete-option.png)

     檢視重複，新檢視的名稱遵循下列模式： `Original view's name (Copy)`。 新的檢視標籤會顯示在所有檢視標籤的末尾。
