---
title: 新增跨工作區記錄型別
description: 記錄型別是Adobe Workfront Planning的物件型別。 在Workfront Planning中，您可以從另一個工作區匯入現有的記錄型別。
hidefromtoc: true
hide: true
source-git-commit: 459e3883101b644a91d5e2a32288cf5b02a02bd9
workflow-type: tm+mt
source-wordcount: '404'
ht-degree: 2%

---


<!-- add these to the metadata, when making this public: 

feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
-->

# 新增跨工作區記錄類型

<span class="preview">此頁面上的資訊是指尚未普遍提供的功能。 它僅在預覽環境中可供所有客戶使用。 每月發行至生產環境後，生產環境中為啟用快速發行的客戶也提供相同的功能。</span>

<span class="preview">如需快速發行資訊，請參閱[為您的組織啟用或停用快速發行](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>

身為工作區管理員，您可以匯入現有記錄型別或將其新增至另一個工作區。

必須先定義記錄型別的跨工作區功能，工作區管理員才能將其匯入其他工作區。

當您建立或編輯記錄型別時，可以定義記錄型別的跨工作區功能。

如需詳細資訊，請參閱[設定記錄型別的跨工作區功能](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md)。

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
   <p>系統管理員擁有所有工作區的許可權，包括他們未建立的工作區</p>  </td> 
  </tr>  
</tbody> 
</table>

*如需Workfront存取需求的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 從另一個工作區新增現有記錄型別時的注意事項

* 當沒有記錄型別設定為要新增到另一個工作區時，建立記錄型別時不會顯示從另一個工作區匯入它們的選項。<!--add this a tip in the steps below, and/ or add a Conditional step that this is possible only when these record types are first enabled-->
* 從另一個工作區新增記錄型別之後，也會從現有記錄型別新增以下資訊：

   * 欄位
   * 記錄
   * 記錄連線

## 從現有的全域記錄型別建立記錄型別

1. 開始建立記錄型別，如文章[建立記錄型別](/help/quicksilver/planning/architecture/create-record-types.md)中所述，然後按一下&#x200B;**使用全域記錄型別**。<!--check this - the option might have been renamed in the UI-->