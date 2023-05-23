---
title: 編輯現有分組
description: 編輯現有分組
author: Nolan
feature: Reports and Dashboards
exl-id: bd9e6794-3196-4a73-a86a-9ba6048e613b
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '485'
ht-degree: 0%

---

# 編輯現有分組

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: This is the third part of a former artcle split in 3: two how-tos and one refernece article about creating and customizing groupings)</p>
-->

您可以自定義最初建立或與您共用的現有分組。 然後，可將其另存為新分組。

## 訪問要求

您必須具有以下訪問權限才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront計畫</strong></td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront許可證*</strong></td> 
   <td> <p>請求或更高 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>訪問級別配置*</strong></td> 
   <td> <p>編輯對篩選器、視圖、分組的訪問</p> <p>編輯對報表、儀表板、日曆的訪問以編輯報表中的分組</p> <p>注：如果您仍然沒有訪問權限，請詢問您的Workfront管理員是否在您的訪問級別設定了其他限制。 有關Workfront管理員如何修改您的訪問級別的資訊，請參見 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自定義訪問級別</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>對象權限</strong></td> 
   <td> <p>管理對報表的權限以編輯報表中的分組</p> <p>管理對分組的權限 </p> <p>有關請求附加訪問的資訊，請參見 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求訪問對象 </a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要瞭解您擁有的計畫、許可證類型或訪問權限，請與您的Workfront管理員聯繫。

## 先決條件

必須先建立分組，然後才能編輯它。

有關建立分組的資訊，請參閱 [在Adobe Workfront建立分組](../../../reports-and-dashboards/reports/reporting-elements/create-groupings.md)。

## 操作步驟

1. 轉到包含要自定義的分組的對象清單。
1. 按一下 **分組** 表徵圖
1. 選擇要自定義的分組，然後按一下 **編輯** 表徵圖

   ![選擇編輯表徵圖。](assets/customizegrouping-nwe-standard-350x291.png)

   將開啟用於自定義分組的介面生成器。

1. 在 **分組預覽** ，按一下 **添加分組** 定義要組織報表中資訊的方式。 下面顯示了分組在報告中的預覽。

1. 開始鍵入表示要在報告中組織資訊的方式的欄位名稱，然後在該欄位出現在下拉清單中時按一下它。
1. （可選和條件）查看更新清單時，選擇 **預設情況下折疊此分組** 的子菜單。 預設情況下，此設定處於禁用狀態，分組結果始終顯示在展開清單中。

   有關更新清單和舊清單的資訊，請參閱文章中的「更新清單和舊清單之間的差異」一節 [開始使用Adobe Workfront](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md)。

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver,QuicksilverOrClassic.Draft mode">(NOTE: the tips repeat in the Create grouping article and Common uses of text mode)</p>
   -->

   >[!TIP]
   >
   >* 當您在查看清單時手動調整分組時，Workfront會記住您的手動首選項，直到您註銷。 當您重新登錄時，會根據此設定顯示清單。
   >* 在從圖表元素或舊式清單中訪問分組後，總會顯示展開的分組結果。 在這些情況下，將忽略此設定。


1. 重複步驟4、5和6以定義附加分組。\
   您最多可以定義三個分組來組織資訊。 通過建立矩陣報告，您可以通過最多四個分組來進一步組織資訊。 有關矩陣報表的詳細資訊，請參見 [建立矩陣報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md)。

1. 按一下 **另存為新分組** 替換當前分組。
