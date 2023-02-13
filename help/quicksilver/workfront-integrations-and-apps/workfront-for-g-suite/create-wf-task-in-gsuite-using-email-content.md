---
product-area: workfront-integrations;projects
keywords: google,doc，文檔，工作表，幻燈片
navigation-topic: workfront-for-g-suite
title: 建立 [!DNL Adobe Workfront] 使用電子郵件內容在G套裝中執行任務
description: 您可以轉換外部電子郵件(非由Adobe產生) [!DNL Workfront])轉至Workfront任務。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 6bbb4301-2791-4d72-bad8-fef63d6e892a
source-git-commit: 04782dfdb8c1ed24bb9c7399a01511c0cbd2dec3
workflow-type: tm+mt
source-wordcount: '915'
ht-degree: 0%

---

# 建立 [!DNL Adobe Workfront] 任務 [!DNL G Suite] 使用電子郵件內容

您可以轉換外部電子郵件(非由 [!DNL Adobe Workfront]) [!DNL Workfront] 任務。

您也可以將外部電子郵件轉換為現有任務的更新。 如需詳細資訊，請參閱 [更新 [!DNL Adobe Workfront] 來自[!DNL G Suite]的項目（使用電子郵件內容）](../../workfront-integrations-and-apps/workfront-for-g-suite/update-wf-item-using-email-content.md).

如需使用的相關資訊 [!DNL G Suite] 使用由傳送的通知電子郵件 [!DNL Workfront]，請參閱 [管理 [!DNL Adobe Workfront] 來自[!DNL G Suite]的通知詳細資料](../../workfront-integrations-and-apps/workfront-for-g-suite/manage-wf-email-notification-details-in-gsuite.md).

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計劃*</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權*</td> 
   <td> <p>[!UICONTROL工作], [!UICONTROL計畫]</p> </td> 
  </tr> 
   </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的 [!DNL Workfront] 管理員。

## 必要條件

建立 [!DNL Workfront] 任務 [!DNL G Suite]，您必須

* 安裝 [!DNL Workfront for G suite]\
   如需指示，請參閱 [安裝 [!DNL Adobe Workfront for G Suite]](../../workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md).

## 建立 [!DNL Adobe Workfront] 任務 [!DNL G Suite] 使用電子郵件內容

1. 若 [!UICONTROL Workfront for G Suite] 面板時，按一下 [!DNL Workfront] 圖示 ![](assets/wf-lion-icon.png) 在 [!DNL G Suite] 頁面最右側的附加元件側欄。
1. 在中開啟電子郵件訊息 [!DNL G Suite]，按一下 [!DNL Workfront for G Suite] 將電子郵件轉換為新 [!DNL Workfront] 任務。

   ![](assets/convert-email-task-issue-update.png)

1. 選取 **[!UICONTROL 新建]** 選項，指明任務是屬於項目的一部分，還是獨立於項目的個人任務。
1. 如果要將任務附加到父項目，請按一下 **[!UICONTROL 專案名稱]**，開始鍵入要執行任務的項目名稱，然後在項目名稱出現在下面的清單中時按一下。
1. 進行下列任一變更：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL任務名]</td> 
      <td>編輯此文字的任何部分，該部分取自電子郵件的主旨行。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL描述]</td> 
      <td>編輯此文字的任何部分，此部分取自電子郵件內文。</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL指派給]</td> 
      <td>按一下 <strong>[!UICONTROL指派給]</strong>，按一下 <strong>[!UICONTROL將此指派給]</strong> 選項，然後開始鍵入人員的名稱，並在其下清單中出現時按一下。 對每個要新增的人員重複執行此步驟，然後按一下 <strong>[!UICONTROL保存]</strong>.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL計畫持續時間]</td> 
      <td> <p>按一下 <strong>[!UICONTROL計畫持續時間]</strong>，然後輸入任務需要的天數。 </p> <p>注意：您可以透過不同方式為您的組織設定此選項。 例如，對於您的組織，您可能需要輸入小時數，而非天數。 如果您需要更多資訊，請參閱 [!DNL Workfront] 管理員。 如果要指定設定的預設值以外的時段，請輸入 <strong>m</strong>, <strong>h</strong>, <strong>d</strong>, <strong>w</strong>，或 <strong>mo</strong> 在數字之後表示分鐘、小時、天、周或月。</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL優先順序]</td> 
      <td>按一下下拉箭頭，然後按一下您要執行任務的優先順序。</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL包含電子郵件附件]</td> 
      <td> <p>（只有在電子郵件至少包含一個附件時才可用。） 按一下此選項可將電子郵件中的附件保存到任務的[!UICONTROL Documents]區域中。 </p> <p>如果不想保存附件，請按一下其名稱右側的X。 </p> <p>如果電子郵件包含 [!DNL Google Drive]，則會將它們儲存至您所建立任務的[!UICONTROL概述]標籤。 </p> <p>重要：為了讓這能發揮作用，您的 [!DNL Workfront] 管理員必須授權 [!DNL Google Drive] 在 [!DNL Workfront]，如一節所述 <a href="../../administration-and-setup/configure-integrations/configure-document-integrations.md#configur" class="MCXref xref">配置整合以管理文檔</a> 在文章中 <a href="../../administration-and-setup/configure-integrations/configure-document-integrations.md" class="MCXref xref">配置文檔整合</a>.</p> <p>如果您啟用此選項，系統仍會對您轉換為工作、問題和更新的其他電子郵件啟用此選項。</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL包含電子郵件檔案]</td> 
      <td> <p>按一下此選項，將原始電子郵件儲存為電子郵件(EML)檔案 <span>到[!UICONTROL文檔]區域</span> 任務。 從那裡，您可以連按兩下檔案，以開啟電子郵件應用程式中的電子郵件。</p> <p>如果您啟用此選項，系統仍會對您轉換為工作、問題和更新的其他電子郵件啟用此選項。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下 **[!UICONTROL 建立任務]**.

   此 **[!UICONTROL 詳細資料]** 頁簽中的 [!DNL Workfront for G Suite] 中。 您可以按一下 **[!UICONTROL 更新]** 並立即開始與共同作業人員溝通，而不需將您留在盒子裡。

   在 **[!UICONTROL 詳細資料]** ，您也可以按一下 **[!UICONTROL 檢視[!DNL Workfront]]** 去Workfront的新任務。

   重新整理瀏覽器時，會顯示位於 [!DNL Workfront for G Suite] 面板會確認您已將電子郵件轉換為任務：

   ![](assets/email-was-converted.png)

   您可以按一下連結，前往 [!DNL Workfront for G Suite] 面板中，選擇「已建立的任務」。

   您可以重複這些步驟，將相同的電子郵件轉換為多個工作。 當您重新整理瀏覽器或在其他時間返回電子郵件時，您為電子郵件建立的所有連結都會列在 [!UICONTROL Workfront for G Suite] 中。

1. （選用）繼續處理 [!DNL Workfront for G Suite] 面板，執行下列任一操作：

   * 在 **[!UICONTROL 更新]** 按一下 **[!UICONTROL 開始新更新]** 並輸入更新。

   * 回覆 **[!UICONTROL 更新]** 按一下 **[!UICONTROL 回覆]** 並輸入您的回復。

      對於上述兩個動作，您可以通知特定使用者您的意見。 按一下 **[!UICONTROL 通知]**，開始輸入使用者的名稱，然後在下拉式清單中出現時按一下名稱。 對要通知的其他用戶重複此過程，然後按一下 **[!UICONTROL 貼文]**.

   * 按一下 **[!UICONTROL 檔案]** 頁簽，查看隨任務保存的任何文檔。

您可以重複這些步驟，將相同的電子郵件轉換為多個工作。 當您重新整理瀏覽器或在其他時間返回電子郵件時，您為電子郵件建立的所有連結都會列在 [!DNL Workfront for G Suite] 中。
