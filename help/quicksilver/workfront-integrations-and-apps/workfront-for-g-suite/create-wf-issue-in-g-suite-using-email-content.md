---
product-area: workfront-integrations;projects
keywords: google，doc，檔案，工作表，幻燈片
navigation-topic: workfront-for-g-suite
title: 建立 [!DNL Adobe Workfront] G Suite使用電子郵件內容的問題
description: 您可以轉換外部電子郵件（非由產生） [!DNL Adobe Workfront)] 至 [!DNL Workfront] 問題。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 7a15f557-67d8-4be8-8538-4bce06536c0a
source-git-commit: 4b95828dc3e6a67c4dbefb46f173303c519643a9
workflow-type: tm+mt
source-wordcount: '776'
ht-degree: 0%

---

# 建立 [!DNL Adobe Workfront] 中的問題 [!DNL G Suite] 使用電子郵件內容

>[!NOTE]
>
>Google適用的Adobe Workfront外掛程式最新版本已於2023年6月26日發行。

您可以轉換外部電子郵件（非由產生） [!DNL Adobe Workfront])至 [!DNL Workfront] 問題。

您也可以將外部電子郵件轉換為現有問題的更新。 如需詳細資訊，請參閱 [更新 [!DNL Adobe Workfront] 使用電子郵件內容的[！DNL G Suite]專案](../../workfront-integrations-and-apps/workfront-for-g-suite/update-wf-item-using-email-content.md).

如需關於使用的資訊 [!DNL G Suite] 使用傳送的通知電子郵件 [!DNL Workfront]，請參閱 [管理 [!DNL Adobe Workfront] 來自[！DNL G Suite]的通知詳細資料](../../workfront-integrations-and-apps/workfront-for-g-suite/manage-wf-email-notification-details-in-gsuite.md).

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

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
   <td> <p>[！UICONTROL工作]，[！UICONTROL計畫]</p> </td> 
  </tr> 
   </tbody> 
</table>

&#42;若要瞭解您擁有哪些計畫、授權型別或存取權，請聯絡您的 [!DNL Workfront] 管理員。

## 必要條件

在建立問題之前，從 [!DNL G Suite]，您必須

* 安裝 [!DNL Workfront for G suite]\
   如需指示，請參閱 [安裝 [!DNL Adobe Workfront for G Suite]](../../workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md).

## 建立 [!DNL Adobe Workfront] 中的問題 [!DNL G Suite] 使用電子郵件內容

1. 如果 [!UICONTROL 適用於G Suite的Workfront] 面板未顯示，請按一下 [!DNL Workfront] 圖示 ![](assets/wf-lion-icon.png) 在 [!DNL G Suite] 頁面最右側的附加元件側欄。
1. 當電子郵件訊息開啟於 [!DNL G Suite]，按一下中的選項 [!DNL Workfront for G Suite] 若要將電子郵件轉換為新電子郵件 [!DNL Workfront] 問題。

   ![](assets/convert-email-task-issue-update.png)

1. 如果要將問題附加到父專案，請按一下 **[!UICONTROL 專案名稱]**，開始輸入您想要問題的專案名稱，然後在下方清單中出現時按一下專案名稱。
1. 進行下列任一變更：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[！UICONTROL問題名稱]</td> 
      <td>編輯此文字的任何部分，這部分取自電子郵件的主旨行。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL說明]</td> 
      <td>編輯此文字的任何部分，這些部分取自電子郵件的內文。</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[！UICONTROL指派給]</td> 
      <td>按一下 <strong>[！UICONTROL指派給]</strong>，按一下 <strong>[！UICONTROL將此指派給]</strong> 選項，然後開始輸入人員名稱，並在人員名稱出現在以下清單中時按一下該名稱。 對您要新增的每個人重複此動作，然後按一下 <strong>[！UICONTROL儲存]</strong>.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[！UICONTROL優先順序]</td> 
      <td>按一下下拉箭頭，然後按一下您想要的問題優先順序。</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[！UICONTROL包含電子郵件附件]</td> 
      <td> <p>（只有在電子郵件至少包含一個附件時才可用。） 按一下此選項，可將電子郵件中的附件儲存至問題的[！UICONTROL檔案]區域。 </p> <p>如果您不想儲存附件，請按一下附件名稱右側的X。 </p> <p>如果電子郵件包含檔案的連結 [!DNL Google Drive]，會儲存至您建立之問題的[！UICONTROL概觀]索引標籤。 </p> <p>重要：為了讓此功能發揮作用，請 [!DNL Workfront] 管理員必須授權 [!DNL Google Drive] 使用中的檔案 [!DNL Workfront]，如一節中所述 <a href="../../administration-and-setup/configure-integrations/configure-document-integrations.md#configur" class="MCXref xref">設定整合以管理檔案</a> 在文章中 <a href="../../administration-and-setup/configure-integrations/configure-document-integrations.md" class="MCXref xref">設定檔案整合</a>.</p> <p>如果啟用此選項，則轉換為任務、問題和更新的其他電子郵件仍會啟用此選項。</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">包含電子郵件檔案</td> 
      <td> <p>按一下此選項，將原始電子郵件儲存為電子郵件(EML) （電子郵件）檔案 <span>至[！UICONTROL檔案]區域</span> 問題。 從那裡，您可以連按兩下檔案，以在電子郵件應用程式中開啟電子郵件。</p> <p>如果啟用此選項，則轉換為任務、問題和更新的其他電子郵件仍會啟用此選項。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下 **[!UICONTROL 建立問題]**.

   此 **[!UICONTROL 詳細資料]** 新問題的標籤會顯示在 [!DNL Workfront for G Suite] 面板。 您可以按一下 **[!UICONTROL 更新]** 並且立即開始與共同作業人員通訊，無需離開您的收件匣。

   在底部 **[!UICONTROL 詳細資料]** 標籤，您也可以按一下 **[!UICONTROL 在Workfront中檢視]** 前往Workfront的新問題。

   當您重新整理瀏覽器時，會出現一則訊息，其底部會有連結 [!UICONTROL 適用於G Suite的Workfront] 面板會確認您已將電子郵件轉換為問題：

   您可以按一下連結，前往 [!DNL Workfront for G Suite] 面板，針對您已建立的問題。

   您可以重複這些步驟，將相同的電子郵件轉換為多個問題。 當您重新整理瀏覽器或在其他時間返回電子郵件時，您為電子郵件建立的所有連結都會列在 [!UICONTROL 適用於G Suite的Workfront] 面板。

1. （可選）繼續處理中的問題 [!DNL Workfront for G Suite] 執行下列任一項作業，即可使用panel：

   * 若要在上新增更新 **[!UICONTROL 更新]** 標籤，按一下 **[!UICONTROL 開始新的更新]** 並輸入更新。

   * 若要回覆 **[!UICONTROL 更新]** 標籤，按一下 **[!UICONTROL 回覆]** 並輸入您的回覆。

     對於上述兩個動作，您可以通知特定使用者您的評論。 按一下 **[!UICONTROL 通知]**，開始輸入使用者名稱，然後在其出現在下拉式清單中時按一下該名稱。 對您要通知的其他使用者重複此程式，然後按一下 **[!UICONTROL Post]**.

   * 按一下 **[!UICONTROL 檔案]** 索引標籤以檢視與問題一併儲存的任何檔案。
