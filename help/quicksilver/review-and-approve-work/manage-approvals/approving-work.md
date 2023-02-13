---
product-area: projects
navigation-topic: approvals
title: 核准工作
description: 核准工作
author: Courtney
feature: Work Management
exl-id: 6e43edbb-14dd-493d-a76b-84be6c3bef82
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '1134'
ht-degree: 0%

---

# 核准工作

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;From&nbsp;Courtney: Linked to Training sites/ articles , don't change title and link)</p>
-->

如果您被設定為核准者，則應定期複查等待核准的工作。

如需建立核准程式的相關資訊，請參閱 [建立工作項的審批流程](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

有關將批准與Workfront中的工作關聯的資訊，請參閱 [將新審批流程或現有審批流程與工作關聯](../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>審核或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>查看或更高程度地訪問與批准關聯的對象</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>查看與批准關聯的對象的或更高權限</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 在Adobe Workfront中找出核准

您可以在Workfront的各個區域中檢視及管理核准。

有關查看等待批准的項目或您已提交供批准的項目的詳細資訊，請參閱 [查看批准](../../review-and-approve-work/manage-approvals/view-approvals.md).

## 從首頁批准工作

1. 按一下 **首頁** 圖示 ![](assets/home-icon-30x29.png) 在Adobe Workfront的左上角。

   >[!NOTE]
   >
   >您的Workfront管理員可能會對環境中的「首頁」圖示進行下列變更：
   >
   >   
   >* 以自訂的影像取代，以說明您的組織。 在此情況下，圖示看起來會與本文所顯示的不同。
   >* 將連結至該頁面的頁面取代為其他頁面。 在此情況下，按一下 **主菜單** ![](assets/main-menu-icon.png) 在頁面的右上角，然後按一下 **首頁**.


1. 按一下 **篩選** 下拉式功能表。

   ![](assets/displaying-work-items-filters-nwe-350x401.png)

1. 選擇 **核准**.\
   顯示需要您批准的所有工作項目。 

   >[!NOTE]
   >
   >指派給「工作角色」或「群組」的核准不會顯示在「首頁」中。 分配給「團隊」的批准將顯示在「工作清單」的「團隊請求」分組中。

1. （可選）更改顯示批准的順序，如文章「按日期、項目或優先順序分組和排序」部分所述 [在「首頁」區域的「工作清單」中顯示項](../../workfront-basics/using-home/using-the-home-area/display-items-in-home-work-list.md).
1. 選擇要作出審批決策的物料。

   ![](assets/task-approval-home-350x127.png)

1. 在右側面板中做出核准決策時，按一下其中一個可用選項。 視您要核准的項目類型而定，下列選項會顯示在頁面的右上角：

   * **專案：** 按一下 **核准** 或 **拒絕**.

   * **任務：** 按一下 **核准** 或 **拒絕** .

   * **問題：** 按一下 **核准** 或 **拒絕** .

   * **工時單：** 按一下 **核准** 或 **拒絕** .

   * **文檔：** 按一下 **核准**, **拒絕**，或 **變更**.\
       檢視核準時，請考量下列事項：

      * 當使用者與您分享校樣時，校樣核准便會顯示在此處，如文章的「共用校樣連結」一節所述 [在Adobe Workfront內共用證明](../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).
      * 只有在您的Workfront環境與Workfront Proof Premium帳戶整合時，校對核准才會顯示在首頁區域。 如果您無法如此處所述使用校對功能，請聯絡您的Workfront管理員。
      * 您會收到應用程式內通知，並通知您校對核准。\
         如需應用程式內通知的詳細資訊，請參閱 [檢視及管理應用程式內通知](../../workfront-basics/using-notifications/view-and-manage-in-app-notifications.md).

      * 請求批准的用戶名將顯示在「首頁」區域的縮圖影像旁，並帶有以下文本：\
         &quot;*使用者A* 希望你同意……」

         <!--      
        <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">      
        (NOTE:&nbsp;From&nbsp;Courtney: Is this true?)      
        </MadCap:conditionalText>      
        -->

         如果用戶名不可用，將顯示以下文本：\
         「校樣的新版本已可供檢視」
      * 若要對校樣做出核准決定，請按一下 **前往校樣**，按一下 **完成審核**，然後按一下任一可用選項。 核准校樣時的可用選項為： **已核准**, **已核准並變更**, **需要的更改**，和 **無關**.

      * 對校樣做出決定後，校樣會保留在「我的核准」標籤中並附上文字「Decision Made」，直到您按一下 **重新整理** 按鈕，或直到您重新整理瀏覽器頁面為止。

         如需檢閱校樣的詳細資訊，請參閱 [在Adobe Workfront中檢閱校樣](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-proofs-in-wf.md).
   * **訪問：** 在 **變更存取** 下拉式功能表，然後按一下 **授予存取權**. 或者，按一下 **忽略**.


## 直接從專案、任務或問題核准工作

當項目、任務或問題處於待批准狀態時，您可以直接從項目、任務或問題批准或拒絕批准。 您也可以檢視有關核准程式的詳細資訊。

要直接從項目、任務或問題批准工作，請執行以下操作：

1. 轉到需要您批准的項目、任務或問題。

   有關項目、任務或問題的當前審批流程的審批資訊顯示在項目的題頭中。

   ![](assets/current-approval-process-in-project-header-with-stages-nwe-350x92.png)

   提供下列核准資訊：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">狀態</td> 
      <td>項目、任務或問題的當前狀態。 這是待批准項目的當前狀態。 狀態在審批流程的每個階段獲得批准後即被批准。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">核准階段</td> 
      <td>審批流程的階段。 <br>待批准的當前階段顯示為「待批准」。 已核准的階段會顯示為已核准；尚未核准的階段會顯示為未開始。</td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下 **核准** 或 **拒絕**，具體取決於您要批准還是拒絕批准流程。\
   等待批准的批准階段現在已獲得批准，並且批准過程將移至下一個階段。 所有階段都經過核准後，狀態才會核准。

## 直接從檔案核准檔案 

1. 轉到包含需要您批准的文檔的文檔區域。
1. 選擇文檔，然後按一下 **核准**, **變更**，或 **拒絕**.\
   ![](assets/approval-approve-document-350x215.png)\
   ![](assets/document-approval-350x199.png)

1. （可選）如果已為文檔生成校樣，則可以在校樣介面中批准文檔，如 [從校樣核准檔案](#approve-a-document-from-a-proof).

## 從核准通知電子郵件核准檔案

根據您的通知設定，您可能會收到電子郵件，通知您其他使用者需要您做出核准決定的檔案。 當您收到包含 **做出批准決策** 按鈕，您可以直接從電子郵件啟動核准程式：

1. 在電子郵件中，按一下 **做出批准決策** 開啟校樣的「檔案詳細資料」頁面。
1. 執行下列任一操作以審閱文檔：

   * 查看有關文檔的元資料。
   * 如果已建立校樣以檢閱帶有標籤和注釋的文檔，請按一下 **開啟校樣** ![](assets/open-proof-icon-qs.png) 在右上角附近，查看校樣。

      <!--   
     <span style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">[Andrzej, does it make sense to leave this here if it's s document approval?&nbsp;Would there never be a proof in that situation?]</span>   
     -->

      如需檢閱校樣的相關資訊，請參閱 [在Adobe Workfront中檢閱校樣](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-proofs-in-wf.md).

1. 按一下 **決策** 選項，以核准、核准變更或拒絕檔案。

## 從校樣核准檔案 {#approve-a-document-from-a-proof}

您可以在校對檢視器中核准檔案。 如需詳細資訊，請參閱 [在校對檢視器中決定校樣](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md) 在文章中 [在校對檢視器中決定校樣](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md).
