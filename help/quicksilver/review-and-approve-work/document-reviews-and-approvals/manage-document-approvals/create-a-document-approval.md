---
product-area: documents
navigation-topic: approvals
title: 建立檔案核准工作流程
description: 您可以在Adobe Workfront中請求其他使用者的檔案核准。
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: a02699e1-3557-47f0-89b7-dbecb507a174
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/OoGv4oNg6GkKeo-zoVi5lSxtPK3UE64-EYW21Mz7GRA
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 2fb0effe42a24898bb3389f72405a92f38ed5cc9
workflow-type: tm+mt
source-wordcount: 2758
ht-degree: 1%

---

# 建立檔案核准工作流程

{{highlighted-preview}}

您可以在Adobe Workfront中請求其他使用者或團隊核准檔案，或請求他們稽核檔案而無需核准。

>[!IMPORTANT]
>
>本文內容指的更新檔案核准功能僅適用於特定帳戶。 如需有關標準核准程式的資訊，請參閱[工作核准](/help/quicksilver/review-and-approve-work/manage-approvals/manage-approvals.md)中列出的文章。

## 存取權要求

+++ 展開以檢視這篇文章中所述功能的存取權要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 封裝</td> 
   <td> <p>使用舊版Workfront儲存空間管理核准的任何Workfront套件</p>
<p>使用Adobe雲端儲存空間管理核准的任何Workflow套件</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td>  
   <td>
   <p>投稿人或以上</p>
   <p>評論或以上</p>
   <p>如果您使用Frame.io整合，您必須有Standard授權才能建立核准工作流程。</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>檢視專案、任務、問題、範本、投資組合、計畫、報告、儀表板和行事曆、檔案的或更高存取權</p> </td> 
  </tr>
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理與請求存取或核准相關聯的物件存取權 </p> </td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 在生產環境的舊版檔案區域中建立核准工作流程

如果您的組織使用Workfront儲存空間，當您存取Workfront中的檔案時，將會看到舊版檔案區域。 如需Workfront儲存體的詳細資訊，請參閱[Adobe雲端儲存體與舊版Workfront儲存體之間的差異](/help/quicksilver/review-and-approve-work/esm-overview.md#differences-between-adobe-cloud-storage-and-legacy-workfront-storage)。

若要建立核准工作流程：

1. 前往包含檔案的專案、任務或問題，然後在左側面板中選取&#x200B;**檔案**。

1. 按一下您需要的檔案，該檔案的「檔案摘要」面板隨即開啟。

1. 在版本下拉式清單中選取您要建立核准的檔案版本。 預設會選取最新版本。

1. 向下捲動至&#x200B;**核准**&#x200B;區段，然後按一下&#x200B;**建立工作流程**。


1. 填寫以下詳細資料：

   <table>
   <tr>
   <td><strong>階段名稱</strong></td>
   <td>新增階段名稱。 您可以將名稱變更為描述性更強的名稱，例如<em>初始稽核</em>或<em>最終核准</em>。</td>
   </tr>
   <tr>
   <td><strong>新增姓名或電子郵件</strong></td>
   <td>開始輸入使用者或團隊名稱，以新增為核准者或稽核者。 如果您只有稽核者，他們將會收到通知並可以選擇完成稽核，但不需要或做出任何決定。</td>
   </tr>
   <tr>
   <td><strong>需要一項決定（選擇性）</strong></td>
   <td>第一個做出決定的人會完成階段。</td>
   </tr>
   <tr>
   <td><strong>到期日（選擇性）</strong></td>
   <td>設定核准的到期日。 使用者與團隊會收到電子郵件通知，通知時間為指定到期日前72小時或24小時。</td>
   </tr>
   </table>

1. （選擇性）重複上一步驟，視需要新增其他階段。

   >[!NOTE]
   >
   >如果您新增多個階段，核准工作流程會依階段列出的順序進行。 完成所有必要的決定後，下一個階段會開始，而上一個階段會鎖定。

   ![檔案詳細資料](assets/new-stage.png)


<div class="preview">

## 在預覽的舊版檔案區域中建立核准工作流程

如果您的組織使用Workfront儲存空間，當您存取Workfront中的檔案時，將會看到舊版檔案區域。 如需Workfront儲存體的詳細資訊，請參閱[Adobe雲端儲存體與舊版Workfront儲存體之間的差異](/help/quicksilver/review-and-approve-work/esm-overview.md#differences-between-adobe-cloud-storage-and-legacy-workfront-storage)。

### 建立基本核准工作流程

若要建立單一階段核准工作流程：

1. 前往包含檔案的專案、任務或問題，然後在左側面板中選取&#x200B;**檔案**。

1. 按一下您需要的檔案，該檔案的「檔案摘要」面板隨即開啟。

1. 在版本下拉式功能表中，選取您要建立核准的檔案版本。 預設會選取最新版本。

1. 向下捲動至&#x200B;**核准**&#x200B;區段，然後按一下&#x200B;**建立工作流程**。 **要求核准**&#x200B;對話方塊會在基本模式下開啟。

1. 填寫以下詳細資料：

   <table>
   <tr>
   <td><strong>使用核准範本（選擇性）</strong></td>
   <td>從下拉式選單中選取範本。 如果範本具有一個路徑和一個階段，則會套用在「基本」模式中。 如果範本有多個階段或多個路徑，對話方塊會自動切換到「進階」模式，而您在「基本」模式中輸入的任何輸入都會被範本的內容取代。</td>
   </tr>
   <tr>
   <td><strong>新增姓名或電子郵件</strong></td>
   <td>開始輸入使用者或團隊名稱，以新增為核准者或稽核者。 如果您只有稽核者，他們將會收到通知並可以選擇完成稽核，但不需要或做出任何決定。</td>
   </tr>
   <tr>
   <td><strong>只需要一個決定（選擇性）</strong></td>
   <td>第一個做出決定的人會完成階段。</td>
   </tr>
   <tr>
   <td><strong>到期日（選擇性）</strong></td>
   <td>設定核准的到期日。 使用者與團隊會收到電子郵件通知，通知時間為指定到期日前72小時或24小時。</td>
   </tr>
   <tr>
   <td><strong>新增自訂訊息（選擇性）</strong></td>
   <td>在<strong>新增自訂訊息</strong>文字方塊中輸入訊息。 該訊息會顯示在核准電子郵件通知和Workfront的「核准」索引標籤中。<p>附註：如果您在建立核准工作流程後編輯自訂訊息，則會傳送更新的電子郵件通知給所有現有參與者。 如果您稍後新增參與者，則自訂訊息會包含在其電子郵件通知中。</p>
   </td>
   </tr>
   </table>

1. 按一下&#x200B;**要求核准**。

   ![在基本模式下要求核准](assets/request-approval-basic.jpeg)

### 建立進階核准工作流程

進階模式支援多個階段以及平行路徑。 每個路徑會獨立執行，並包含一或多個循序階段。 當階段中所有必要的決定都完成時，該路徑中的下一個階段開始，上一個階段被鎖定，新階段的稽核者和核准者會收到電子郵件通知。

「需求工作」決定會停止其上的路徑，但不會影響其他路徑上的核准工作流程。 您最多可以設定30個路徑和100個階段總計。

若要建立進階核准工作流程：

1. 前往包含檔案的專案、任務或問題，然後在左側面板中選取&#x200B;**檔案**。

1. 按一下您需要的檔案，該檔案的「檔案摘要」面板隨即開啟。

1. 在版本下拉式功能表中，選取您要建立核准的檔案版本。 預設會選取最新版本。

1. 向下捲動至&#x200B;**核准**&#x200B;區段，然後按一下&#x200B;**建立工作流程**。

1. 在&#x200B;**要求核准**&#x200B;對話方塊的右上方，按一下&#x200B;**移至進階**。 您在[基本]模式中輸入的任何輸入都會保留，並套用至&#x200B;**路徑1**、**階段1**。

   >[!TIP]
   >
   >建立核準時，按一下右上方的&#x200B;**「前往基本**」，即可返回「基本」模式。 在您按一下&#x200B;**要求核准**&#x200B;後，**前往基本**&#x200B;選項就不再可用。

1. 填寫路徑1中階段1的詳細資訊：

   <table>
   <tr>
   <td><strong>階段名稱</strong></td>
   <td>依預設，階段名為<em>階段1</em>、<em>階段2</em>等。 將階段重新命名為較清楚描述的階段，例如<em>初始稽核</em>或<em>最終核准</em>。</td>
   </tr>
   <tr>
   <td><strong>新增姓名或電子郵件</strong></td>
   <td>開始輸入使用者或團隊名稱，以新增為核准者或稽核者。 如果您只有稽核者，他們將會收到通知並可以選擇完成稽核，但不需要或做出任何決定。<p>附註：一次只能將檢閱者或核准者指派給相同資產上的一個開啟階段。 如果同時開啟多個平行階段，則無法將同一個使用者新增至多個階段。</p></td>
   </tr>
   <tr>
   <td><strong>只需要一個決定（選擇性）</strong></td>
   <td>第一個做出決定的人會完成階段。</td>
   </tr>
   <tr>
   <td><strong>到期日（選擇性）</strong></td>
   <td>每個路徑的第一階段支援絕對到期日期。 路徑中的每個後續階段都支援相對到期日 — 從該階段開啟的天數。 使用者及團隊會透過電子郵件在到期日前72小時及24小時收到通知。</td>
   </tr>
   <tr>
   <td><strong>新增自訂訊息（選擇性）</strong></td>
   <td>在<strong>新增自訂訊息</strong>文字方塊中輸入訊息。 該訊息會顯示在核准電子郵件通知和Workfront的「核准」索引標籤中。<p>新增第二個階段時，預設會選取<strong>在所有階段顯示此訊息</strong>。 將其保留為選取狀態，以便在每個階段中使用相同的訊息。 若要對每個階段使用不同的訊息，請清除<strong>在所有階段顯示此訊息</strong>，然後在每個階段的<strong>新增自訂訊息</strong>文字方塊中輸入階段專屬訊息。</p></td>
   </tr>
   </table>

1. （選擇性）按一下&#x200B;**新增階段**&#x200B;以新增另一個階段至路徑。 路徑中的階段會依其列出的順序執行。 您可以在路徑內重新排序階段，但無法將階段從一個路徑移動到另一個路徑。 每個路徑可以有不同的階段數量。

1. （選擇性）在&#x200B;**平行路徑**&#x200B;下，按一下&#x200B;**新增路徑**&#x200B;以新增其他路徑。 新路徑會從一個空白階段開始，成為選取的路徑。 若要重新命名路徑，請將游標停留在路徑標籤上，按一下鉛筆圖示，然後輸入新名稱。

1. （選用）若要移除路徑，請將游標移至路徑標籤，然後按一下垃圾桶圖示。 **路徑1**&#x200B;無法移除，且路徑無法重新排序。 只有在路徑中沒有鎖定或完成的階段時，才能移除其他路徑。

   ![具有平行路徑的進階模式](assets/request-approval-parallel-paths.jpeg)

1. （選擇性）若要清除所有路徑和階段並重新開始，請按一下右上方的&#x200B;**重設**。

1. 按一下&#x200B;**要求核准**。

</div>


## 在生產環境的新檔案區域中建立核准工作流程

如果您的組織使用Adobe雲端儲存空間，當您存取Workfront中的檔案時，將會看到新的檔案區域。 如需Adobe雲端儲存空間的詳細資訊，請參閱[Adobe雲端儲存空間概觀](/help/quicksilver/review-and-approve-work/esm-overview.md)。

若要建立核准工作流程：

1. 前往包含檔案的專案、任務或問題，然後在左側面板中選取&#x200B;**檔案**。

1. 按一下檔案，然後按一下頁面右側的&#x200B;**核准**&#x200B;圖示。

   ![在檔案摘要中新增核准者](assets/approvals-icon-new.png)

1. 按一下「**建立工作流程**」，然後填寫下列詳細資料：

   <table>
   <tr>
   <td><strong>階段名稱</strong></td>
   <td>新增階段名稱。 您可以將名稱變更為描述性更強的名稱，例如<em>初始稽核</em>或<em>最終核准</em>。</td>
   </tr>
   <tr>
   <td><strong>新增姓名或電子郵件</strong></td>
   <td>開始輸入使用者或團隊名稱，以新增為核准者或稽核者。 如果您只有稽核者，他們將會收到通知並可以選擇完成稽核，但不需要或做出任何決定。</td>
   </tr>
   <tr>
   <td><strong>需要一項決定（選擇性）</strong></td>
   <td>第一個做出決定的人會完成階段。</td>
   </tr>
   <tr>
   <td><strong>到期日（選擇性）</strong></td>
   <td>設定核准的到期日。 使用者與團隊會收到電子郵件通知，通知時間為指定到期日前72小時或24小時。</td>
   </tr>
   </table>

1. （選擇性）重複上一步驟，視需要新增其他階段。

   >[!NOTE]
   >
   >如果您新增多個階段，核准工作流程會依階段列出的順序進行。 完成所有必要的決定後，下一個階段會開始，而上一個階段會鎖定。

   ![檔案詳細資料](assets/new-stage.png)


<div class="preview">

## 在預覽中的新檔案區域中建立核准工作流程

如果您的組織使用Adobe雲端儲存空間，當您存取Workfront中的檔案時，將會看到新的檔案區域。 如需Adobe雲端儲存空間的詳細資訊，請參閱[Adobe雲端儲存空間概觀](/help/quicksilver/review-and-approve-work/esm-overview.md)。

根據預設，**要求核准**&#x200B;對話方塊會以&#x200B;**基本**&#x200B;模式開啟。 基本模式是一個單一階段，其中包含一組核准者或稽核者。 切換至&#x200B;**進階**&#x200B;模式以設定多階段核准或平行路徑。

### 建立基本核准工作流程

若要建立單一階段核准工作流程：

1. 前往包含檔案的專案、任務或問題，然後在左側面板中選取&#x200B;**檔案**。

1. 按一下檔案，然後按一下頁面右側的&#x200B;**核准**&#x200B;圖示。

   ![在檔案摘要中新增核准者](assets/approvals-icon-new.png)

1. 按一下&#x200B;**建立工作流程**。 **要求核准**&#x200B;對話方塊會在基本模式下開啟。

1. 填寫以下詳細資料：

   <table>
   <tr>
   <td><strong>使用核准範本（選擇性）</strong></td>
   <td>預設會收合範本欄位。 按一下欄位以展開，然後從下拉式選單中選取範本。 如果範本具有一個路徑和一個階段，則會套用在「基本」模式中。 如果範本有多個階段或多個路徑，對話方塊會自動切換到「進階」模式，而您在「基本」模式中輸入的任何輸入都會被範本的內容取代。</td>
   </tr>
   <tr>
   <td><strong>新增姓名或電子郵件</strong></td>
   <td>開始輸入使用者或團隊名稱，以新增為核准者或稽核者。 如果您只有稽核者，他們將會收到通知並可以選擇完成稽核，但不需要或做出任何決定。</td>
   </tr>
   <tr>
   <td><strong>只需要一個決定（選擇性）</strong></td>
   <td>第一個做出決定的人會完成階段。</td>
   </tr>
   <tr>
   <td><strong>到期日（選擇性）</strong></td>
   <td>設定核准的到期日。 使用者與團隊會收到電子郵件通知，通知時間為指定到期日前72小時或24小時。</td>
   </tr>
   <tr>
   <td><strong>新增自訂訊息（選擇性）</strong></td>
   <td>在<strong>新增自訂訊息</strong>文字方塊中輸入訊息。 該訊息會顯示在核准電子郵件通知和Workfront的「核准」索引標籤中。</td>
   </tr>
   </table>

1. 按一下&#x200B;**要求核准**。

   ![在基本模式下要求核准](assets/request-approval-basic.jpeg)

>[!NOTE]
>
>* **要求核准**&#x200B;對話方塊每次都會以基本模式開啟，無論您先前的工作階段為何。
>* 如果您在建立核准工作流程後編輯自訂訊息，則會傳送更新的電子郵件通知給所有現有參與者。 如果您稍後新增參與者，則自訂訊息會包含在其電子郵件通知中。
>* 核准儲存後，您無法將它切換回「基本」模式。 只要核准未鎖定或完成，您就可以將進行中的核准從基本切換到進階。

### 建立進階核准工作流程

進階模式支援平行路徑。 每個路徑會獨立執行，並包含一或多個循序階段。 當階段中所有必要的決定都完成時，該路徑中的下一個階段開始，上一個階段被鎖定，新階段的稽核者和核准者會收到電子郵件通知。

「需求工作」決定會停止其上的路徑，但不會影響其他路徑上的核准工作流程。 您最多可以設定30個路徑和100個階段總計。

若要建立進階核准工作流程：

1. 前往包含檔案的專案、任務或問題，然後在左側面板中選取&#x200B;**檔案**。

1. 按一下檔案，然後按一下頁面右側的&#x200B;**核准**&#x200B;圖示。

   ![在檔案摘要中新增核准者](assets/approvals-icon-new.png)

1. 按一下&#x200B;**建立工作流程**。

1. 在&#x200B;**要求核准**&#x200B;對話方塊的右上方，按一下&#x200B;**移至進階**。 您在[基本]模式中輸入的任何輸入都會保留，並套用至&#x200B;**路徑1**、**階段1**。

   >[!TIP]
   >
   >建立核準時，按一下右上方的&#x200B;**「前往基本**」，即可返回「基本」模式。 在您按一下&#x200B;**要求核准**&#x200B;後，**前往基本**&#x200B;選項就不再可用。

1. 填寫路徑1中階段1的詳細資訊：

   <table>
   <tr>
   <td><strong>階段名稱</strong></td>
   <td>依預設，階段名為<em>階段1</em>、<em>階段2</em>等。 將階段重新命名為較清楚描述的階段，例如<em>初始稽核</em>或<em>最終核准</em>。</td>
   </tr>
   <tr>
   <td><strong>新增姓名或電子郵件</strong></td>
   <td>開始輸入使用者或團隊名稱，以新增為核准者或稽核者。 如果您只有稽核者，他們將會收到通知並可以選擇完成稽核，但不需要或做出任何決定。<p>附註：一次只能將檢閱者或核准者指派給相同資產上的一個開啟階段。 如果同時開啟多個平行階段，則無法將同一個使用者新增至多個階段。</p></td>
   </tr>
   <tr>
   <td><strong>只需要一個決定（選擇性）</strong></td>
   <td>第一個做出決定的人會完成階段。</td>
   </tr>
   <tr>
   <td><strong>到期日（選擇性）</strong></td>
   <td>每個路徑的第一階段支援絕對到期日期。 路徑中的每個後續階段都支援相對到期日 — 從該階段開啟的天數。 使用者及團隊會透過電子郵件在到期日前72小時及24小時收到通知。</td>
   </tr>
   <tr>
   <td><strong>新增自訂訊息（選擇性）</strong></td>
   <td>在<strong>新增自訂訊息</strong>文字方塊中輸入訊息。 該訊息會顯示在核准電子郵件通知和Workfront的「核准」索引標籤中。<p>新增第二個階段時，預設會選取<strong>在所有階段顯示此訊息</strong>。 將其保留為選取狀態，以便在每個階段中使用相同的訊息。 若要對每個階段使用不同的訊息，請清除<strong>在所有階段顯示此訊息</strong>，然後在每個階段的<strong>新增自訂訊息</strong>文字方塊中輸入階段專屬訊息。</p></td>
   </tr>
   </table>

1. （選擇性）按一下&#x200B;**新增階段**&#x200B;以新增另一個階段至路徑。 路徑中的階段會依其列出的順序執行。 您可以在路徑內重新排序階段，但無法將階段從一個路徑移動到另一個路徑。 每個路徑可以有不同的階段數量。


1. （選擇性）在&#x200B;**平行路徑**&#x200B;下，按一下&#x200B;**新增路徑**&#x200B;以新增其他路徑。 新路徑會從一個空白階段開始，成為選取的路徑。 若要重新命名路徑，請將游標停留在路徑標籤上，按一下鉛筆圖示，然後輸入新名稱。

1. （選用）若要移除路徑，請將游標移至路徑標籤，然後按一下垃圾桶圖示。 **路徑1**&#x200B;無法移除，且路徑無法重新排序。 只有在路徑中沒有鎖定或完成的階段時，才能移除其他路徑。

   ![具有平行路徑的進階模式](assets/request-approval-advanced.jpeg)

1. （選擇性）若要清除所有路徑和階段並重新開始，請按一下右上方的&#x200B;**重設**。

1. 按一下&#x200B;**要求核准**。

</div>



<!--
## Resubmit an approval on a new version

Document approval decisions are not automatically reset when you upload a new version. For example, if your document is approved with changes, the decision will show "changes" as the decision, even if you upload a new version with the specified changes. You can clear the decision on a new version if you manually resubmit the approval.

1. Go to the project, task, or issue that contains the document, then select **Documents**.
1. Find the document you need.

1. Scroll down to the **Approvals** section in the Summary, click the More icon, then click Resubmit.

   ![Resubmit approval](assets/nwe-resubmit-approval-350x149.png)
-->