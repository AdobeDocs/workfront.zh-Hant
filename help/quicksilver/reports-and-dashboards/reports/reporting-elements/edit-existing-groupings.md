---
title: 編輯現有群組
description: 編輯現有群組
author: Nolan
feature: Reports and Dashboards
exl-id: bd9e6794-3196-4a73-a86a-9ba6048e613b
source-git-commit: 302771f4d64b386149623f87a3436d0c40f421d5
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# 編輯現有群組

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: This is the third part of a former artcle split in 3: two how-tos and one refernece article about creating and customizing groupings)</p>
-->

您可以自訂您最初建立或與您共用的現有群組。 然後，您可將其儲存為新群組。

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront計畫*</strong></td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront授權*</strong></td> 
   <td> <p>計劃 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>訪問級別配置*</strong></td> 
   <td> <p>編輯對篩選器、檢視、群組的存取</p> <p>編輯對報表、控制面板、日曆的存取，以編輯報表中的分組</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>物件權限</strong></td> 
   <td> <p>管理報表的權限，以編輯報表中的分組</p> <p>管理群組的權限 </p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 必要條件

您必須先建立分組，才能加以編輯。

如需建立分組的詳細資訊，請參閱 [在Adobe Workfront中建立群組](../../../reports-and-dashboards/reports/reporting-elements/create-groupings.md).

## 操作步驟

1. 轉到包含要自定義的分組的對象清單。
1. 按一下 **分組** 表徵圖。
1. 選取您要自訂的群組，然後按一下 **編輯** 表徵圖。

   ![選取編輯圖示。](assets/customizegrouping-nwe-standard-350x291.png)

   用於自訂分組的介面產生器隨即開啟。

1. 在 **分組預覽** ，按一下 **添加分組** 定義要如何組織報表中的資訊。 下方顯示分組在報表中的外觀預覽。

1. 開始輸入表示您要在報表中組織資訊的方式的欄位名稱，然後在下拉式清單中顯示時按一下。
1. （選用和條件式）檢視更新清單時，請選取 **預設折疊此分組** 如果希望分組中的結果顯示為已折疊而不是展開。 預設會停用此設定，且群組的結果一律會顯示在展開清單中。

   如需更新和舊版清單的相關資訊，請參閱文章中的「更新和舊版清單之間的差異」一節 [開始使用Adobe Workfront中的清單](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver,QuicksilverOrClassic.Draft mode">(NOTE: the tips repeat in the Create grouping article and Common uses of text mode)</p>
   -->

   >[!TIP]
   >
   >* 當您在檢視清單時手動調整分組時，Workfront會記住您的手動偏好設定，直到您登出為止。 當您重新登入時，清單會根據此設定顯示。
   >* 從圖表元素或舊版清單存取群組後，其結果一律會展開。 在這些情況下，會忽略此設定。


1. 重複步驟4、5和6以定義其他分組。\
   您可以定義最多三個群組，以組織資訊。 您可以建立矩陣報表，以最多四個群組進一步組織資訊。 如需矩陣報表的詳細資訊，請參閱 [建立矩陣報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md).

1. 按一下 **另存為新分組** 以用更改替換當前分組。
