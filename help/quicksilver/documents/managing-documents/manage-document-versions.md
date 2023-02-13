---
product-area: documents
navigation-topic: manage-documents
title: 管理文檔版本
description: 您可以在Workfront中管理檔案的多個版本。
author: Courtney
feature: Digital Content and Documents
exl-id: 477153e4-847b-46ec-8107-72a7399c3767
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '514'
ht-degree: 0%

---

# 管理文檔版本

您可以在Workfront中管理檔案的多個版本。

## 存取需求

您必須具備下列條件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p> 任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>要求或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>查看對文檔的訪問</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>查看對文檔的訪問</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 必要條件

* 本文假設該文檔具有多個版本。

   如果您需要有關上傳新版本檔案至Workfront的資訊，請參閱 [上傳新版本的檔案](../../documents/managing-documents/upload-new-document-version.md).

## 查看文檔的所有版本的清單

1. 在「摘要」中，捲動至檢視 **所有版本** 區段。 您可以在此處查看文檔的所有版本。

## 查看和管理以前文檔版本的詳細資訊

1. 在「文檔詳細資訊」頁面的頂部附近，按一下名稱旁邊的下拉菜單，然後按一下要查看和管理的版本的名稱。

   ![](assets/version-drop-dn-doc-dtls-nwe-350x93.png)

   除了檢視版本的「詳細資料」外，您還可以變更版本，例如名稱、中繼資料和校對設定（如果是檔案校樣）。

## 下載單一檔案版本

1. 在摘要中， **版本**，按一下「更多」功能表 ![](assets/more-icon.png) 在版本的右側，然後按一下 **下載** 中。

   ![](assets/more-versions-350x143.png)

## 下載文檔的所有版本

1. 按一下 **文檔詳細資訊**，然後選取 **所有版本** 中。

1. 按一下 **全部下載** 清單頂端。

## 刪除文檔版本

如果錯誤上傳某個版本的文檔，或者不再需要某個版本，則可以刪除該版本並維護原始文檔。

>[!IMPORTANT]
>
>無法恢復單獨刪除的文檔版本。

考慮刪除文檔版本時，請記住以下事項：

* 一次只能刪除一個版本。 如果刪除版本，此動作會顯示在 **更新** 在檔案上。
* 如果您在刪除版本後上傳新版本，新版本會收到下一個連續號碼。 例如，如果有3個版本的文檔，而您刪除了第3版，則下一個上載的文檔將是第4版。
* 刪除版本後，對版本進行的系統更新和註解會保留在Workfront中。

   <!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Deleting a document version in Workfront does not delete the Proof version.&nbsp;</li>
  -->

要刪除文檔版本：

1. 轉到包含文檔的項目、任務或問題，然後選擇 **檔案**.查找所需的文檔。
1. 在 **版本** 「摘要」中的「 」區域，按一下「版本」，然後按一下 **刪除** 中。 此 **刪除** 只有在至少有兩個版本時，選項才會顯示。

   如果將文檔連結到外部源，該連結將被刪除，並且文檔將不再可以通過Workfront訪問。

   ![](assets/more-versions-350x143.png)
