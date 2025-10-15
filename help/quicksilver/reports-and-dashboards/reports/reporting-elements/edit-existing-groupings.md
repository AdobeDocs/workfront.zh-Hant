---
title: 編輯現有群組
description: 編輯現有群組
author: Nolan
feature: Reports and Dashboards
exl-id: bd9e6794-3196-4a73-a86a-9ba6048e613b
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '439'
ht-degree: 0%

---

# 編輯現有群組

<!-- Audited: 11/2024 -->

<!--NOTE: This is the third part of a former article split in 3: two how-tos and one reference article about creating and customizing groupings)-->

您可以自訂您最初建立或與您共用的現有群組。 然後，您就可以將其儲存為新群組。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront套件</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</strong></td> 
   <td> 
    <p>投稿人或以上</p>
    <p>要求或更高版本</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>編輯對篩選器、檢視、群組的存取權</p> <p>編輯報告、儀表板、行事曆的存取權，以編輯報告中的分組</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
    <td> <p>管理報告的許可權以編輯報告中的分組</p> <p>管理群組的許可權</p></td> 
   </td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。
+++

## 先決條件

您必須先建立群組，才能進行編輯。

如需建立群組的詳細資訊，請參閱[在Adobe Workfront中建立群組](../../../reports-and-dashboards/reports/reporting-elements/create-groupings.md)。

## 操作步驟

1. 移至包含您要自訂之群組的物件清單。
1. 按一下&#x200B;**群組**&#x200B;圖示。
1. 選取您要自訂的分組，然後按一下&#x200B;**編輯**&#x200B;圖示![編輯圖示](assets/edit-icon.png)。

   ![選取編輯圖示。](assets/customizegrouping-nwe-standard-350x291.png)

   用於自訂分組的介面產生器隨即開啟。

1. 在&#x200B;**群組預覽**&#x200B;區段中，按一下&#x200B;**新增群組**&#x200B;以定義您想要如何整理報告中的資訊。 報表中的群組預覽如下所示。

1. 開始輸入欄位名稱，代表您要在報告中組織資訊的方式，然後在下拉式清單中出現時按一下它。
1. （選擇性和條件性）檢視更新的清單時，如果您希望群組中的結果顯示摺疊而非展開，請選取&#x200B;**依預設摺疊此群組**。 此設定預設為停用，群組結果一律顯示在展開清單中。

   如需有關更新清單和舊版清單的資訊，請參閱[開始使用Adobe Workfront中的清單](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md)一文中的「更新清單和舊版清單的差異」一節。

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver,QuicksilverOrClassic.Draft mode">(NOTE: the tips repeat in the Create grouping article and Common uses of text mode)</p>
   -->

   >[!TIP]
   >
   >* 當您在檢視清單時手動調整群組，Workfront會記住您的手動偏好設定，直到您登出為止。 當您重新登入時，清單會根據此設定顯示。
   >* 從圖表元素或舊版清單存取群組結果後，群組結果一律展開顯示。 在這些情況下，會忽略此設定。

1. 重複步驟4、5和6以定義其他群組。\
   您最多可以定義三個群組來組織資訊。 您可以建立矩陣報表，將資訊進一步組織為最多四個群組。 如需矩陣報表的詳細資訊，請參閱[建立矩陣報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md)。

1. 按一下「儲存群組」**&#x200B;**，以變更取代目前的群組。
