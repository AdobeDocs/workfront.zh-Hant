---
product-area: documents
navigation-topic: manage-documents
title: 管理檔案版本
description: You can manage multiple versions of a document in Workfront.
author: Courtney
feature: Digital Content and Documents
exl-id: 477153e4-847b-46ec-8107-72a7399c3767
source-git-commit: 90eb99fa46e706a53427f995d484e2fb42e9c293
workflow-type: tm+mt
source-wordcount: '634'
ht-degree: 3%

---

# 管理檔案版本

<!-- Audited: 5/2025 -->

You can manage multiple versions of a document in Workfront.

## 存取權要求

+++ 展開以檢視這篇文章中所述功能的存取權要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 封裝</td> 
   <td> <p>使用舊版Workfront儲存來管理檔案的任何Workfront套件</p>
<p>使用Adobe企業儲存體管理檔案的任何Workflow套件</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 授權</td> 
   <td> 
   <p>投稿人或以上</p>
   <p>要求或更高版本 </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>檢視檔案的存取權</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>View access to the Document</p></td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先決條件

* This article assumes that the document has multiple versions.

  如果您需要有關將檔案新版本上傳到Workfront的資訊，請參閱[上傳檔案新版本](../../documents/managing-documents/upload-new-document-version.md)。

## View a list of all versions of a document

{{step1-to-documents}}

1. On the **Documents** page, select a document in the list.

1. In the upper-right corner of the page, click the **Open Summary** icon ![Open Summary icon](assets/qs-summary-in-new-toolbar-small.png). The **Document Summary** side panel opens.

1. Scroll down to the **Versions** section to view all the document versions.

## View and manage details for a previous document version

{{step1-to-documents}}

1. Hover over the document, then click **Document Details**.

1. Near the top of the **Document Details** page, click the drop-down menu next to the name, then click the name of the version you want to view and manage.

   ![Version drop-down on the Document Details page](assets/version-drop-dn-doc-dtls-nwe-350x93.png)

   Along with viewing the version&#39;s details, you can make changes to the version, such as its name, metadata, and proofing settings (if it&#39;s a document proof).

## 下載單一檔案版本

{{step1-to-documents}}

1. 在&#x200B;**檔案**&#x200B;頁面上，選取清單中的檔案。

1. 在頁面的右上角，按一下&#x200B;**開啟摘要**&#x200B;圖示![開啟摘要圖示](assets/qs-summary-in-new-toolbar-small.png)。 **檔案摘要**&#x200B;側面板隨即開啟。

1. 在&#x200B;**版本**&#x200B;區段中，按一下版本右側的&#x200B;**更多**&#x200B;功能表![更多](assets/more-icon.png)，然後按一下出現的下拉式清單中的&#x200B;**下載**。

   ![下載單一檔案](assets/more-versions-350x143.png)

## 下載檔案的所有版本

{{step1-to-documents}}

1. 在&#x200B;**檔案**&#x200B;頁面上，選取清單中的檔案。

1. 在頁面的右上角，按一下&#x200B;**開啟摘要**&#x200B;圖示![開啟摘要圖示](assets/qs-summary-in-new-toolbar-small.png)。 **檔案摘要**&#x200B;側面板隨即開啟。

1. 向下捲動至&#x200B;**版本**&#x200B;區段，然後按一下&#x200B;**全部下載**。

## 刪除檔案版本

如果您誤上傳檔案版本，或不再需要某個版本，可以刪除該版本並維護原始檔案。

>[!IMPORTANT]
>
>您無法復原個別刪除的檔案版本。

當您考慮刪除檔案版本時，請牢記下列事項：

* 一次只能刪除一個版本。 如果刪除了版本，則此動作會出現在檔案上的「更新」區段中。
* 如果您在刪除版本後上傳新版本，則新版本會收到下一個連續數字。 例如，如果檔案有3個版本，而您刪除了版本3，則下一個上傳的檔案將是版本4。
* 刪除版本後，針對版本所做的系統更新和註解會保留在Workfront中。

  <!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Deleting a document version in Workfront does not delete the Proof version.&nbsp;</li>
  -->

若要刪除檔案版本：

{{step1-to-documents}}

1. 在&#x200B;**檔案**&#x200B;頁面上，從清單中選取檔案。

1. 在頁面的右上角，按一下&#x200B;**開啟摘要**&#x200B;圖示![開啟摘要圖示](assets/qs-summary-in-new-toolbar-small.png)。 **檔案摘要**&#x200B;側面板隨即開啟。

1. 向下捲動至&#x200B;**版本**&#x200B;區段以檢視所有檔案版本。
1. In the **Versions** section, click the click the **More** menu ![More menu](assets/more-icon.png) to the right of the version, then click **Delete** in the drop-down list that appears.

   >[!NOTE]
   >
   >* The **Delete** option is visible only if there are at least 2 versions.
   >* If the document is linked to an outside source, that link is deleted and the document is no longer accessible through Workfront.

   ![Delete the document version](assets/more-versions-350x143.png)
