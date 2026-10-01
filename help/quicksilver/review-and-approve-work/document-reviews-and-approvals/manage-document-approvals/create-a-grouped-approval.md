---
product-area: documents
navigation-topic: approvals
title: 建立群組核准
description: 您可以將多個資產捆綁到單一核准工作流程中，讓它們一起經過相同的階段。
author: Courtney
feature: Work Management, Digital Content and Documents
source-git-commit: f55042154ac3d93544c152b7b1ad26746a209772
workflow-type: tm+mt
source-wordcount: '1173'
ht-degree: 1%
---

# 建立群組核准

<span class="preview">此頁面上的資訊在預覽Sandbox環境中無法使用，因為Frame.io整合在此無法使用。 此功能將於2026年10月14日和15日在生產環境中可用。</span>

分組的核准會在單一核准工作流程下套件組合多個資產。 您可以使用基本和進階模式、多個階段以及具有分組核准的平行路徑，就像處理單一資產核准一樣。

群組核准僅在新的檔案區域可用，當您的組織使用Adobe雲端儲存空間時就會顯示。 如需詳細資訊，請參閱[Adobe雲端儲存空間概觀](/help/quicksilver/review-and-approve-work/esm-overview.md)。

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
   <p>對於使用Adobe雲端儲存空間的物件，您必須擁有標準授權才能建立核准工作流程。</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader">存取層級設定</td>
   <td> <p>檢視專案、任務、問題、範本、投資組合、計畫、報告、儀表板、行事曆和檔案的或更高存取權</p></td>
  </tr>
  <tr>
   <td role="rowheader">物件許可權</td>
   <td> <p>管理與請求或核准相關聯的物件存取權</p></td>
  </tr>
 </tbody>
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 建立基本的分組核准

若要建立單一階段群組核准，請執行下列動作：

1. 前往包含檔案的專案、任務或問題，然後在左側面板中選取&#x200B;**檔案**。

1. 按一下您要包含的第一個資產，然後按住Shift鍵並按一下其他資產，以選取多個資產。

1. 選取資產後，按一下底部功能表中的&#x200B;**要求核准**。 **要求核准**&#x200B;對話方塊會在基本模式下開啟。

   ![建立群組核准](assets/requeset-grouped-approval.png)

1. 填寫以下詳細資料：

   <table>
   <tr>
   <td><strong>使用核准範本（選擇性）</strong></td>
   <td>預設會收合範本欄位。 按一下欄位以展開，然後從下拉式選單中選取範本。 如果範本具有一個路徑和一個階段，則會套用在「基本」模式中。 如果範本有多個階段或多個路徑，對話方塊會自動切換到「進階」模式，而您在「基本」模式中輸入的任何輸入都會被範本的內容取代。</td>
   </tr>
   <tr>
   <td><strong>在預覽中新增人員或團隊</strong></td>
   <td><p>開始輸入使用者名稱、團隊或電子郵件地址，然後選擇他們是<strong>核准者</strong>或<strong>檢閱者</strong>。 Workfront會個別新增團隊的每個作用中成員。</p>
   <p>注意：如果使用者已經新增，或屬於您新增的多個團隊，則會納入一次。</p></td>
   </tr>
   <tr>
   <td><strong>只需要一個決定（選擇性）</strong></td>
   <td>第一個做出決定的人會完成階段。</td>
   </tr>
   <tr>
   <td><strong>到期日（選擇性）</strong></td>
   <td>設定核准的到期日。 在指定到期日前72小時及24小時，會以電子郵件通知使用者。</td>
   </tr>
   <tr>
   <td><strong>新增自訂訊息（選擇性）</strong></td>
   <td>在<strong>新增自訂訊息</strong>文字方塊中輸入訊息。 該訊息會顯示在核准電子郵件通知和Workfront的「核准」索引標籤中。</td>
   </tr>
   </table>

1. （選擇性）按一下&#x200B;**檔案**&#x200B;索引標籤，以檢閱此核准中包含的資產。

1. 按一下&#x200B;**要求核准**。

   ![基本群組核准](assets/basic-group-approval.png)

## 建立進階群組核准

進階模式支援平行路徑。 每個路徑會獨立執行，並包含一或多個循序階段。 當階段中所有必要的決定都完成時，該路徑中的下一個階段開始，上一個階段被鎖定，新階段的稽核者和核准者會收到電子郵件通知。

「需求工作」決定會停止其所在的路徑，但不會影響其他路徑上的核准工作流程。

<!--
You can configure up to 30 paths and 100 stages total.
-->

若要建立進階群組核准，請執行下列動作：

1. 前往包含檔案的專案、任務或問題，然後在左側面板中選取&#x200B;**檔案**。

1. 按一下您要包含的第一個資產，然後按住Shift鍵並按一下其他資產，以選取多個資產。

1. 選取資產後，按一下底部功能表中的&#x200B;**要求核准**。

   ![建立群組核准](assets/requeset-grouped-approval.png)

1. 在&#x200B;**要求核准**&#x200B;對話方塊的右上方，按一下&#x200B;**移至進階**。 您在[基本]模式中輸入的任何輸入都會保留，並套用至&#x200B;**路徑1**、**階段1**。

   >[!TIP]
   >
   >建立核準時，按一下右上方的&#x200B;**「前往基本**」，即可返回「基本」模式。 一旦您提交核准要求，**前往基本**&#x200B;選項就不再可用。

1. 填寫路徑1中階段1的詳細資訊：

   <table>
   <tr>
   <td><strong>階段名稱</strong></td>
   <td>依預設，階段名為<em>階段1</em>、<em>階段2</em>等。 將階段重新命名為較清楚描述的階段，例如<em>初始稽核</em>或<em>最終核准</em>。</td>
   </tr>
   <tr>
   <td><strong>在預覽中新增人員或團隊</strong></td>
   <td><p>開始輸入使用者名稱、團隊或電子郵件地址，然後選擇他們是<strong>核准者</strong>或<strong>檢閱者</strong>。 Workfront會個別新增團隊的每個作用中成員。</p>
   <p>注意：如果使用者已經新增，或屬於您新增的多個團隊，則會納入一次。</p></td>
   </tr>
   <tr>
   <td><strong>只需要一個決定（選擇性）</strong></td>
   <td>第一個做出決定的人會完成階段。</td>
   </tr>
   <tr>
   <td><strong>到期日（選擇性）</strong></td>
   <td>每個路徑的第一階段支援絕對到期日期。 路徑中的每個後續階段都支援相對到期日（從該階段開啟的天數）。 到期日前72小時及24小時以電子郵件通知使用者。</td>
   </tr>
   <tr>
   <td><strong>新增自訂訊息（選擇性）</strong></td>
   <td>在<strong>新增自訂訊息</strong>文字方塊中輸入訊息。 該訊息會顯示在核准電子郵件通知和Workfront的「核准」索引標籤中。<p>新增第二個階段時，預設會選取<strong>在所有階段顯示此訊息</strong>。 將其保留為選取狀態，以便在每個階段中使用相同的訊息。 若要對每個階段使用不同的訊息，請清除<strong>在所有階段顯示此訊息</strong>，然後在每個階段的<strong>新增自訂訊息</strong>文字方塊中輸入階段專屬訊息。</p></td>
   </tr>
   </table>

1. （可選）將其他階段新增至路徑1：
   1. 按一下&#x200B;**新增階段**，將另一個階段新增至目前路徑。 路徑中的階段會依其列出的順序執行。
   1. 填寫新階段的詳細資訊，然後重複此步驟，視需要新增更多階段。

      >[!NOTE]
      >
      >您可以在路徑內重新排序階段，但無法將階段從一個路徑移動到另一個路徑。 每個路徑可以有不同的階段數量。


1. （可選）新增平行路徑：
   1. 在畫面左側的&#x200B;**平行路徑**&#x200B;下，按一下&#x200B;**新增路徑**&#x200B;以新增其他路徑。
   1. 按照相同的步驟將階段和參與者新增到新路徑中。 每個路徑會獨立執行，因此每個路徑可以有不同數量的階段和不同的參與者。

1. （選用）若要移除路徑，請將游標移至路徑標籤，然後按一下垃圾桶圖示。 **路徑1**&#x200B;無法移除，且路徑無法重新排序。 只有在路徑中沒有鎖定或完成的階段時，才能移除其他路徑。

1. （選擇性）若要清除所有路徑和階段並重新開始，請按一下右上角的&#x200B;**重設**。

1. （選擇性）按一下&#x200B;**檔案**&#x200B;索引標籤，以檢閱此核准中包含的資產。

1. 按一下&#x200B;**要求核准**。

   ![進階群組核准](assets/advanced-group-approval.png)


<!--

## Add additional documents to a grouped approval

You can add additional documents to a grouped approval after the approval has been created as long as the first stage has not been completed. 

To add an additional document to a grouped approval:

1. Click any document in the grouped approval, then click **Manage Approval** in the bottom menu.
1. Click **Documents on this approval**, then click **Add**.

   ![add document grouped approval](assets/add-document-to-grouped-approval.png)
1. Choose the documents you want to add, then click **Add to approval**. 
1. Once you add all of the documents, click **Edit approval**. The new documents are added to the grouped approval and all participants are notified of the change.

-->

## 已知限制

* 目前，群組核准工作流程建立後，您就無法新增或移除工作流程中的檔案。 此功能已規劃於未來版本中。
* 群組的核准暫時限製為每個群組3個路徑和25個資產。