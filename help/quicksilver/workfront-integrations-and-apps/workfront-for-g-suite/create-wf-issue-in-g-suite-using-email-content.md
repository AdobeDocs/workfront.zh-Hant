---
product-area: workfront-integrations;projects
keywords: google,doc，文檔，工作表，幻燈片
navigation-topic: workfront-for-g-suite
title: 建立 [!DNL Adobe Workfront] 使用電子郵件內容的G套裝問題
description: 您可以轉換外部電子郵件(非由 [!DNL Adobe Workfront)] 到 [!DNL Workfront] 問題。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 7a15f557-67d8-4be8-8538-4bce06536c0a
source-git-commit: 925e8f9d57d65fcb44068274800450d9db5c9d34
workflow-type: tm+mt
source-wordcount: '804'
ht-degree: 0%

---

# 建立 [!DNL Adobe Workfront] 問題 [!DNL G Suite] 使用電子郵件內容

>[!NOTE]
>
>有 [已知問題](https://experienceleague.adobe.com/docs/workfront-known-issues/issues/new-workfront-experience/wf-current/wf-integrations-error-when-opening-wf-for-gsuite.html?lang=en) 與 [!DNL Workfront for G Suite] 未如預期運作。 我們正在開發新版本，並預期會發佈至 [!DNL Google Marketplace] 在不久的將來。

您可以轉換外部電子郵件(非由 [!DNL Adobe Workfront]) [!DNL Workfront] 問題。

您也可以將外部電子郵件轉換為現有問題的更新。 如需詳細資訊，請參閱 [更新 [!DNL Adobe Workfront] 來自[!DNL G Suite]的項目（使用電子郵件內容）](../../workfront-integrations-and-apps/workfront-for-g-suite/update-wf-item-using-email-content.md).

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

建立問題之前，請先從 [!DNL G Suite]，您必須

* 安裝 [!DNL Workfront for G suite]\
   如需指示，請參閱 [安裝 [!DNL Adobe Workfront for G Suite]](../../workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md).

## 建立 [!DNL Adobe Workfront] 問題 [!DNL G Suite] 使用電子郵件內容

1. 若 [!UICONTROL Workfront for G Suite] 面板時，按一下 [!DNL Workfront] 圖示 ![](assets/wf-lion-icon.png) 在 [!DNL G Suite] 頁面最右側的附加元件側欄。
1. 在中開啟電子郵件訊息 [!DNL G Suite]，按一下 [!DNL Workfront for G Suite] 將電子郵件轉換為新 [!DNL Workfront] 問題。

   ![](assets/convert-email-task-issue-update.png)

1. 如果要將問題附加至父項目，請按一下 **[!UICONTROL 專案名稱]**，開始輸入您想要問題的專案名稱，然後在下方清單中顯示專案名稱時按一下。
1. 進行下列任一變更：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL問題名稱]</td> 
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
      <td role="rowheader">[!UICONTROL優先順序]</td> 
      <td>按一下下拉式箭頭，然後按一下您要解決問題的優先順序。</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL包含電子郵件附件]</td> 
      <td> <p>（只有在電子郵件至少包含一個附件時才可用。） 按一下此選項可將電子郵件中的附件保存到問題的[!UICONTROL Documents]區域。 </p> <p>如果不想保存附件，請按一下其名稱右側的X。 </p> <p>如果電子郵件包含 [!DNL Google Drive]，則會儲存至您所建立問題的[!UICONTROL概述]標籤。 </p> <p>重要：為了讓這能發揮作用，您的 [!DNL Workfront] 管理員必須授權 [!DNL Google Drive] 在 [!DNL Workfront]，如一節所述 <a href="../../administration-and-setup/configure-integrations/configure-document-integrations.md#configur" class="MCXref xref">配置整合以管理文檔</a> 在文章中 <a href="../../administration-and-setup/configure-integrations/configure-document-integrations.md" class="MCXref xref">配置文檔整合</a>.</p> <p>如果您啟用此選項，系統仍會對您轉換為工作、問題和更新的其他電子郵件啟用此選項。</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">包含電子郵件檔案</td> 
      <td> <p>按一下此選項，將原始電子郵件儲存為電子郵件(EML)（電子郵件）檔案 <span>到[!UICONTROL文檔]區域</span> 問題。 從那裡，您可以連按兩下檔案，以開啟電子郵件應用程式中的電子郵件。</p> <p>如果您啟用此選項，系統仍會對您轉換為工作、問題和更新的其他電子郵件啟用此選項。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下 **[!UICONTROL 建立問題]**.

   此 **[!UICONTROL 詳細資料]** 標籤中 [!DNL Workfront for G Suite] 中。 您可以按一下 **[!UICONTROL 更新]** 並立即開始與共同作業人員溝通，而不需將您留在盒子裡。

   在 **[!UICONTROL 詳細資料]** ，您也可以按一下 **[!UICONTROL 在Workfront中檢視]** 去Workfront的新刊。

   重新整理瀏覽器時，會顯示位於 [!UICONTROL Workfront for G Suite] 面板會確認您已將電子郵件轉換為問題：

   您可以按一下連結，前往 [!DNL Workfront for G Suite] 面板，以了解您建立的問題。

   您可以重複這些步驟，將相同的電子郵件轉換為多個問題。 當您重新整理瀏覽器或在其他時間返回電子郵件時，您為電子郵件建立的所有連結都會列在 [!UICONTROL Workfront for G Suite] 中。

1. （選用）繼續處理 [!DNL Workfront for G Suite] 面板，執行下列任一操作：

   * 在 **[!UICONTROL 更新]** 按一下 **[!UICONTROL 開始新更新]** 並輸入更新。

   * 回覆 **[!UICONTROL 更新]** 按一下 **[!UICONTROL 回覆]** 並輸入您的回復。

      對於上述兩個動作，您可以通知特定使用者您的意見。 按一下 **[!UICONTROL 通知]**，開始輸入使用者的名稱，然後在下拉式清單中出現時按一下名稱。 對要通知的其他用戶重複此過程，然後按一下 **[!UICONTROL 貼文]**.

   * 按一下 **[!UICONTROL 檔案]** 頁簽，查看隨問題保存的任何文檔。
