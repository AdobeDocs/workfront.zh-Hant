---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: 在校樣上檢視自動化工作流程階段
description: 您可以方便地跟蹤使用自動工作流配置的校樣的進度。 您可以檢視、修改、新增、啟動和鎖定校樣上已完成的工作。
author: Courtney
feature: Digital Content and Documents
exl-id: 71df1445-c64c-4de2-a9b8-23bd47898b6d
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '527'
ht-degree: 0%

---

# 在校樣上檢視自動化工作流程階段

您可以方便地跟蹤使用自動工作流配置的校樣的進度。 您可以檢視、修改、新增、啟動和鎖定校樣上已完成的工作。

有關使用「自動化工作流」將階段和用戶添加到校樣的資訊，請參閱 [在校樣上將階段和使用者新增至自動化工作流程](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/add-stages-users-to-automated-workflow-proof.md).

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>當前計畫：Pro或更高</p> <p>或</p> <p>舊計畫：Select或Premium</p> <p>如需使用不同計畫校對存取權限的詳細資訊，請參閱 <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">存取Workfront中的校對功能</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>當前計畫：工作或計畫</p> <p>舊計畫：任何（您必須為使用者啟用校對）</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">校訂權限設定檔 </td> 
   <td>管理員或更高</td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯對文檔的訪問</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、角色或校樣權限設定檔，請聯絡您的Workfront或Workfront Proof管理員。

## 檢視自動化工作流程圖表

1. 在包含文檔的文檔清單中，將滑鼠移到包含文檔的行上，然後按一下 **校對工作流程**.

   自動化工作流程的圖表顯示在工作流程標題的正下方。

   圖中的各個階段標籤如下：

   ![dot.png](assets/dot.png) 活動階段

   ![gray_dot.png](assets/grey-dot.png) 非作用中階段\
   ![sbw-key-icon.png](assets/sbw-key-icon.png)  私人舞台

   ![sbw-padlock-icon.png](assets/sbw-padlock-icon.png)  鎖定的舞台

   各級之間的線表示各級之間的依賴關係。 導向非活動階段的線段將呈虛線，直到舞台激活為止。

   您可以將滑鼠移至圖表中的某個階段上，以顯示進度。 如果舞台未活動，並且您在舞台上具有編輯權限，則可以按一下「激活舞台」按鈕 ![](assets/activate-stage-btn.png) 來開始舞台。 如果舞台處於活動狀態，並且您在舞台上具有編輯權限，則可以鎖定它。 ![](assets/lock-stage-btn.png) 如需進度列(S、O、C、D)的詳細資訊，請參閱  [在Workfront校樣中檢視校樣的進度與狀態](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/view-progress-and-status-of-proof.md).

## 檢視階段

1. 在包含文檔的文檔清單中，將滑鼠移到包含文檔的行上，然後按一下 **校對工作流程**.
1. 在圖表上，按一下要查看的舞台。

   ![](assets/view-stage-diagram-350x204.png)

1. 要展開舞台的詳細資訊，請按一下舞台名稱下方的橫箭頭。

   ![](assets/stage-details-caret-350x167.png)

## 查看所有階段

要查看自動化工作流中的所有階段，請執行以下操作：

1. 按一下頁面頂端的「變更檢視」按鈕 ![](assets/change-view-btn.png)，然後按一下 **查看所有階段**.

   「自動化工作流」的所有階段都列在區段中，但是詳細資訊會隱藏。

1. 要展開舞台的詳細資訊，請按一下舞台名稱下方的側箭頭。

## 查看所有階段的詳細資訊

要查看自動化工作流的所有階段，並擴展其詳細資訊：

1. 按一下頁面頂端的「變更檢視」按鈕 ![](assets/change-view-btn.png)，然後按一下 **查看所有階段的詳細資訊**.
1. 要查看舞台的詳細資訊，請按一下其名稱下方的向下箭頭。
