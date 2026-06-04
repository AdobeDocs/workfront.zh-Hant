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
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40cid: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 1473
ht-degree: 2%

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

## 從「生產」中舊版檔案區域的「摘要」面板建立核准工作流程

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

## 從「預覽」中舊版檔案區域的「摘要」面板建立核准工作流程

如果您的組織使用Workfront儲存空間，當您存取Workfront中的檔案時，將會看到舊版檔案區域。 如需Workfront儲存體的詳細資訊，請參閱[Adobe雲端儲存體與舊版Workfront儲存體之間的差異](/help/quicksilver/review-and-approve-work/esm-overview.md#differences-between-adobe-cloud-storage-and-legacy-workfront-storage)。

若要建立核准工作流程：

1. 前往包含檔案的專案、任務或問題，然後在左側面板中選取&#x200B;**檔案**。

1. 按一下您需要的檔案，該檔案的「檔案摘要」面板隨即開啟。

1. 在版本下拉式選單中，選取您要建立核准的檔案版本。 預設會選取最新版本。

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
   <td><strong>只需要一個決定（選擇性）</strong></td>
   <td>第一個做出決定的人會完成階段。</td>
   </tr>
   <tr>
   <td><strong>到期日（選擇性）</strong></td>
   <td>設定核准的到期日。 使用者與團隊會收到電子郵件通知，通知時間為指定到期日前72小時或24小時。</td>
   </tr>
   <tr>
   <td><strong>新增自訂訊息（選擇性）</strong></td>
   <td>在<strong>新增自訂訊息</strong>文字方塊中輸入訊息。該訊息會顯示在核准電子郵件通知和Workfront的「核准」索引標籤中。
   <p>新增第二個階段時，預設會選取<strong>在所有階段顯示此訊息</strong>。 將其保留為選取狀態，以便在每個階段中使用相同的訊息。 若要對每個階段使用不同的訊息，請清除<strong>在所有階段顯示此訊息</strong>，然後視需要在每個階段的<strong>新增自訂訊息</strong>文字方塊中輸入階段專屬訊息。</p></td>
   </tr>
   </table>

1. （選擇性）重複上一步驟，視需要新增其他階段。

   >[!NOTE]
   >
   >* 如果您新增多個階段，核准工作流程會依階段列出的順序進行。 完成所有必要的決定後，下一個階段會開始，而上一個階段會鎖定。
   >* 如果您在建立核准工作流程後編輯自訂訊息，則會傳送更新的電子郵件通知給所有現有參與者。 如果您稍後新增參與者，則自訂訊息會包含在其電子郵件通知中。

   ![新增自訂訊息至階段](assets/add-custom-message.jpeg)

</div>


## 從生產中新檔案區域的摘要面板建立核准工作流程

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

## 從預覽中的新檔案區域的摘要面板建立核准工作流程

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
   <td><strong>只需要一個決定（選擇性）</strong></td>
   <td>第一個做出決定的人會完成階段。</td>
   </tr>
   <tr>
   <td><strong>到期日（選擇性）</strong></td>
   <td>設定核准的到期日。 使用者與團隊會收到電子郵件通知，通知時間為指定到期日前72小時或24小時。</td>
   </tr>
   <tr>
   <td><strong>新增自訂訊息（選擇性）</strong></td>
   <td>在<strong>新增自訂訊息</strong>文字方塊中輸入訊息。該訊息會顯示在核准電子郵件通知和Workfront的「核准」索引標籤中。
   <p>新增第二個階段時，預設會選取<strong>在所有階段顯示此訊息</strong>。 將其保留為選取狀態，以便在每個階段中使用相同的訊息。 若要對每個階段使用不同的訊息，請清除<strong>在所有階段顯示此訊息</strong>，然後在每個階段的<strong>新增自訂訊息</strong>文字方塊中輸入階段專屬訊息。</p></td>
   </tr>
   </table>

1. （選擇性）重複上一步驟，視需要新增其他階段。

   >[!NOTE]
   >
   >* 如果您新增多個階段，核准工作流程會依階段列出的順序進行。 完成所有必要的決定後，下一個階段會開始，而上一個階段會鎖定。
   >* 如果您在建立核准工作流程後編輯自訂訊息，則會傳送更新的電子郵件通知給所有現有參與者。 如果您稍後新增參與者，則自訂訊息會包含在其電子郵件通知中。

   ![新增自訂訊息至階段](assets/add-custom-message.jpeg)

</div>



<!--
## Resubmit an approval on a new version

Document approval decisions are not automatically reset when you upload a new version. For example, if your document is approved with changes, the decision will show "changes" as the decision, even if you upload a new version with the specified changes. You can clear the decision on a new version if you manually resubmit the approval.

1. Go to the project, task, or issue that contains the document, then select **Documents**.
1. Find the document you need.

1. Scroll down to the **Approvals** section in the Summary, click the More icon, then click Resubmit.

   ![Resubmit approval](assets/nwe-resubmit-approval-350x149.png)
-->
