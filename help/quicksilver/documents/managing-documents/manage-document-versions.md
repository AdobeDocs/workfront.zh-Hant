---
product-area: documents
navigation-topic: manage-documents
title: 管理檔案版本
description: 您可以在Workfront中管理檔案的多個版本。
author: Courtney
feature: Digital Content and Documents
exl-id: 477153e4-847b-46ec-8107-72a7399c3767
source-git-commit: 9aa6822c9c1ecade776d4c71b113c1afd997f40c
workflow-type: tm+mt
source-wordcount: '528'
ht-degree: 0%

---

# 管理檔案版本

您可以在Workfront中管理檔案的多個版本。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

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
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>檢視檔案的存取權</p> <p>注意：如果您還是沒有存取權，請詢問您的Workfront管理員，他們是否在您的存取層級中設定其他限制。 如需Workfront管理員如何修改存取層級的詳細資訊，請參閱<a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>檢視檔案的存取權</p> <p>如需請求其他存取權的資訊，請參閱<a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求物件</a>的存取權。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的Workfront管理員。

+++

## 先決條件

* 本文假設檔案有多個版本。

  如果您需要有關將檔案新版本上傳到Workfront的資訊，請參閱[上傳檔案新版本](../../documents/managing-documents/upload-new-document-version.md)。

## 檢視檔案所有版本的清單

1. 在[摘要]中，捲動至檢視&#x200B;**所有版本**&#x200B;區段。 您可以在此檢視檔案的所有版本。

## 檢視和管理先前檔案版本的詳細資訊

1. 在「檔案詳細資訊」頁面頂端附近，按一下名稱旁邊的下拉式功能表，然後按一下您要檢視及管理的版本名稱。

   ![](assets/version-drop-dn-doc-dtls-nwe-350x93.png)

   除了檢視版本的詳細資訊之外，您還可以變更版本，例如其名稱、中繼資料和校訂設定（如果是檔案校訂）。

## 下載單一檔案版本

1. 在[摘要]中的&#x200B;**版本**&#x200B;下，按一下版本右側的[更多]功能表![](assets/more-icon.png)，然後按一下出現的下拉式清單中的&#x200B;**下載**。

   ![](assets/more-versions-350x143.png)

## 下載檔案的所有版本

1. 按一下&#x200B;**檔案詳細資料**，然後在左側面板中選取&#x200B;**所有版本**。

1. 按一下清單頂端的&#x200B;**全部下載**。

## 刪除檔案版本

如果您誤上傳檔案版本，或不再需要某個版本，可以刪除該版本並維護原始檔案。

>[!IMPORTANT]
>
>您無法復原個別刪除的檔案版本。

當您考慮刪除檔案版本時，請牢記下列事項：

* 一次只能刪除一個版本。 如果刪除了版本，此動作會出現在檔案上的&#x200B;**更新**&#x200B;中。
* 如果您在刪除版本後上傳新版本，則新版本會收到下一個連續數字。 例如，如果檔案有3個版本，而您刪除了版本3，則下一個上傳的檔案將是版本4。
* 刪除版本後，針對版本所做的系統更新和註解會保留在Workfront中。

  <!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Deleting a document version in Workfront does not delete the Proof version.&nbsp;</li>
  -->

若要刪除檔案版本：

1. 前往包含檔案的專案、任務或問題，然後選取「**檔案**」。尋找您需要的檔案。
1. 在[摘要]的&#x200B;**版本**&#x200B;區域中，按一下版本，然後按一下出現的下拉式清單中的&#x200B;**刪除**。 **刪除**&#x200B;選項只有在至少有兩個版本時才可見。

   如果檔案連結到外部來源，則該連結會遭到刪除，並且該檔案無法再透過Workfront存取。

   ![](assets/more-versions-350x143.png)
