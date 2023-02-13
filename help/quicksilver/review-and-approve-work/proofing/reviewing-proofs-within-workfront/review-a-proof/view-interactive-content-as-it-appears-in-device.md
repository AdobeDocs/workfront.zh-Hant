---
product-area: documents
navigation-topic: review-proofs-within-workfront
title: 變更校對檢視器中的互動式校樣解析度
description: 您可以預覽互動式校樣在不同裝置上的外觀，讓您了解內容如何根據不同的解析度顯示和回應。
author: Courtney
feature: Digital Content and Documents
exl-id: 99165790-0c34-4540-92d9-956ae178a874
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '579'
ht-degree: 1%

---

# 變更校對檢視器中的互動式校樣解析度

您可以預覽互動式校樣在不同裝置上的外觀，讓您了解內容如何根據不同的解析度顯示和回應。

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
   <td> <p>編輯對文檔的訪問</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、角色或校樣權限設定檔，請聯絡您的Workfront或Workfront Proof管理員。

## 案頭校對檢視器與網頁校對檢視器中的裝置和解析度檢視

您的Adobe Workfront管理員已設定您的系統，讓您可以在案頭測試檢視器中，或在網頁測試檢視器中，以ZIP檔案中的套件內容形式檢閱互動式內容：

* 在案頭打樣檢視器中，您可以檢視內容的顯示方式，以及在各種解析度和裝置上回應。 審核者指定特定裝置時，內容會如同在該裝置上顯示一樣，並附上該裝置的使用者介面規格。 例如，一個品牌智慧手機上的紅色按鈕可能是不同品牌上的藍色按鈕。

* 在Web校對檢視器中，您可以檢視各種裝置的解析度中顯示的互動式內容。 但網頁校對檢視器不會在這些裝置上使用介面規格（例如按鈕顏色）來模擬內容。

   >[!NOTE]
   >
   >您的Workfront管理員可以為組織中的使用者設定自訂裝置，如文章的為互動式校樣設定自訂裝置中所述。

## 使用預設設備或解析度設定查看校樣

1. 轉到包含要開啟的校樣的文檔清單。
1. 將滑鼠指標暫留在檔案上，然後按一下 **開啟校樣**.
1. 按一下 **回應式** 在校樣檢視器的中下方。

   ![Resolution_option_in_DPV.png](assets/resolution-option-in-dpv-350x64.png)

1. 在「案頭校對檢視器」中，在顯示的裝置和解析度清單中，按一下您想要的裝置。

   或

   在「Web校對查看器」中，在顯示的解析度清單中，按一下所需的解析度。

   如果您需要有關這兩個檢視器之間差異的資訊，請參閱 [Web校對查看器與Desktop Pooting Viewer之間的差異概述](../../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md).

   互動式校樣會呈現您選取的解析度。

## 使用自訂解析度設定檢視校樣

1. 轉到包含要開啟的校樣的文檔清單。
1. 將滑鼠指標暫留在檔案上，然後按一下 **開啟校樣**.
1. 按一下 **回應式** 在「校對查看器」的中下方。
1. 輸入自訂 **回應式** 解析度。

   ![Type_a_custom_resolution_DPV.png](assets/type-a-custom-resolution-dpv.png)

   或

   將滑鼠移至互動式內容上，然後將右下角、右下邊或下邊的藍色邊框拖曳至您想要的解析度。

   ![Drag_blue_edges_for_resolution.png](assets/drag-blue-edges-for-resolution-350x251.png)

   自訂解析度會顯示在下列位置：

   * 在 **解析度** 面板。\
      ![螢幕截圖2018-05-15_10-27-54.png](assets/screenshot-2018-05-15-10-27-54.png)

   * 在任何注釋中，審核者都會將校樣加入。 每個注釋都包含審核者建立注釋時選擇的螢幕解析度。
