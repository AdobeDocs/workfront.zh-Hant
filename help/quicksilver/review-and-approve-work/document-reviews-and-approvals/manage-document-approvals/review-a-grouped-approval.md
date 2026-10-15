---
product-area: documents
navigation-topic: approvals
title: 檢閱群組核准
description: 您可以從「首頁」或Frame.io檢視器中的「我的核准」Widget，檢視和決定群組核准中的所有檔案。
author: Courtney
feature: Work Management, Digital Content and Documents
source-git-commit: 9459c6251b2576207e1766d94e6cb634f65f1f68
workflow-type: tm+mt
source-wordcount: '630'
ht-degree: 3%
---

# 檢閱群組核准

{{highlighted-preview-article-level}}

當您被指派給群組核準時，群組中的所有檔案都會顯示在一起，以便您對每個檔案做出決定。 您可以一次核准或請求每個檔案的變更，或單獨對每個檔案做出決定。

如果一個或多個檔案被標籤為&#x200B;**需要工作**&#x200B;在多階段群組核准中，則群組無法前進到下一個階段，直到群組中的所有檔案都有核准的決定。 如需詳細資訊，請參閱[解決多階段群組核准中單一檔案的「需要工作」決定](#resolve-a-needs-work-decision-on-a-single-document-in-a-multi-stage-grouped-approval)。



>[!IMPORTANT]
>
>如果您的組織使用Adobe雲端儲存空間，當您存取Workfront中的檔案時，將會看到新的檔案區域。 群組核准僅在新的檔案區域可用。 如需Adobe雲端儲存空間的詳細資訊，請參閱[Adobe雲端儲存空間概觀](/help/quicksilver/review-and-approve-work/esm-overview.md)。

## 存取權要求

+++ 展開以檢視這篇文章中所述功能的存取權要求。

<table style="table-layout:auto">
 <col>
 <col>
 <tbody>
  <tr>
   <td role="rowheader">Adobe Workfront 封裝</td>
   <td> <p>使用Adobe雲端儲存空間管理核准的任何Workflow套件</p> </td>
  </tr>
  <tr>
   <td role="rowheader">Adobe Workfront授權</td>
   <td>
   <p>投稿人或以上</p>
   <p>評論或以上</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader">存取層級設定</td>
   <td> <p>檢視與核准關聯的物件或更高的存取許可權</p></td>
  </tr>
  <tr>
   <td role="rowheader">物件許可權</td>
   <td> <p>檢視與核准相關聯的物件或更高許可權</p></td>
  </tr>
 </tbody>
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 從首頁中的我的核准Widget檢閱群組核准

首頁中的我的核准Widget會將檔案分組在單一核准下，以便您一起對所有檔案執行動作。

>[!NOTE]
>
>您可能需要將我的核准Widget新增到您的首頁。 如需詳細資訊，請參閱[新增、編輯或移除首頁中的Widget](/help/quicksilver/workfront-basics/using-home/using-the-home-area/add-edit-remove-widgets-in-new-home.md)。

1. 按一下Adobe Workfront左上角的&#x200B;**首頁**&#x200B;圖示，然後尋找&#x200B;**我的核准** Widget。

1. 開啟分組的核准。 群組中的所有檔案都會列在一起，而群組中的專案數量則會列在頂端。

1. 使用下列其中一項，做出決定：

   * **標籤所有已核准專案**：一次記錄群組中每個檔案的已核准決定。
   * **標示所有需求工作**：一次記錄群組中每個檔案的需求工作決定。
   * **做出決定**：對單一檔案做出個別決定。 對要分別決定的每個檔案重複此步驟。


   ![我的核准Widget群組核准](assets/my-approvals-group.png)

## 在Frame.io檢視器中檢閱群組核准

在Frame.io檢視器中，群組中的所有檔案會顯示在一起，因此您可以快速決定每個檔案，或開啟檔案以詳細檢閱。

1. 前往您的檢閱電子郵件通知，然後按一下&#x200B;**前往檢閱**，或從[首頁]中的&#x200B;**我的核准** Widget開啟群組核准。

1. 執行下列其中一項：

   * 直接從群組頁面快速決定每個檔案，無需開啟它。
   * 按一下檔案以開啟、新增註釋或標示，然後使用箭頭移至群組中的下一個檔案。 檔案計數器（例如，**1 / 2**）會顯示您在群組中的位置。

   如需在Frame.io檢視器中加上註解和標示的詳細資訊，請參閱[使用Frame.io檢視器檢閱並核准](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/review-with-frame.md)。

1. 為每個檔案選擇一個決定：

   * **已核准**：檔案不需要變更，已可供使用。
   * **需要工作**：檔案需要變更，而且尚未準備好使用。

   如需決定的詳細資訊，請參閱[檔案決定狀態概觀](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/document-approval-status.md)。

   ![frame.io檢視器群組核准](assets/frame-group-approval.png)

## 其他資源

本文涵蓋有關檢閱一組檔案的資訊。 如需有關對單一檔案做出決策、新增標籤等內容的資訊，請參閱

* [在Workfront中核准檔案](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/review-and-approve-documents/approve-a-document.md)
* [在Workfront中檢閱檔案](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/review-and-approve-documents/review-a-document.md)
* [使用Frame.io檢視器檢閱並核准](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/review-with-frame.md)