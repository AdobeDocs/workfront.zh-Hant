---
product-area: workfront-integrations;projects
keywords: google，doc，檔案，工作表，幻燈片
navigation-topic: workfront-for-g-suite
title: 使用電子郵件內容在Google Workspace中建立 [!DNL Adobe Workfront] 問題
description: 您可以將 [!DNL Adobe Workfront)] 未產生的外部電子郵件轉換為 [!DNL Workfront] 問題。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 7a15f557-67d8-4be8-8538-4bce06536c0a
source-git-commit: 494c7bf8aaf3570d4a01b5e88b85410ee3f52f18
workflow-type: tm+mt
source-wordcount: '770'
ht-degree: 0%

---

# 使用電子郵件內容在[!DNL Google Workspace]中建立[!DNL Adobe Workfront]問題

>[!NOTE]
>
>Google適用的Adobe Workfront外掛程式最新版本已於2023年6月26日發行。

您可以將外部電子郵件（非[!DNL Adobe Workfront]產生）轉換為[!DNL Workfront]問題。

您也可以將外部電子郵件轉換為現有問題的更新。 如需詳細資訊，請參閱[使用電子郵件內容](../../workfront-integrations-and-apps/workfront-for-g-suite/update-wf-item-using-email-content.md)從 [!DNL Google Workspace] 更新 [!DNL Adobe Workfront] 專案。

如需使用[!DNL Google Workspace]處理[!DNL Workfront]所傳送之通知電子郵件的相關資訊，請參閱[管理 [!DNL Adobe Workfront] 來自 [!DNL Google Workspace]](../../workfront-integrations-and-apps/workfront-for-g-suite/manage-wf-email-notification-details-in-gsuite.md)的通知詳細資料。

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計畫*</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權*</td> 
   <td> <p>[！UICONTROL Work]， [！UICONTROL計畫]</p> </td> 
  </tr> 
   </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的[!DNL Workfront]管理員。

## 先決條件

在您可以從[!DNL Google Workspace]建立問題之前，您必須

* 安裝[!DNL Workfront for Google Workspace]\
   如需指示，請參閱[安裝 [!DNL Adobe Workfront for Google Workspace]](../../workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md)。

## 使用電子郵件內容在[!DNL Google Workspace]中建立[!DNL Adobe Workfront]問題

1. 如果未顯示Google Workspace]的[!UICONTROL Workfront面板，請按一下頁面最右側[!DNL Google Workspace]附加元件側邊欄中的[!DNL Workfront]圖示![Workfront圖示](assets/wf-lion-icon.png)。
1. 在[!DNL Google Workspace]中開啟電子郵件訊息後，按一下[!DNL Workfront for Google Workspace]中的選項以將電子郵件轉換為新的[!DNL Workfront]問題。

   ![轉換電子郵件](assets/convert-email-task-issue-update.png)

1. 如果您想要將問題附加到父專案，請按一下&#x200B;**[!UICONTROL 專案名稱]**，開始輸入您要問題的專案名稱，然後在下方清單中出現時按一下專案名稱。
1. 進行下列任一變更：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[！UICONTROL問題名稱]</td> 
      <td>編輯此文字的任何部分，這部分取自電子郵件的主旨列。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL說明]</td> 
      <td>編輯此文字的任何部分，這些部分取自電子郵件的內文。</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[！UICONTROL指派給]</td> 
      <td>按一下<strong>[！UICONTROL指派給]</strong>，按一下出現的<strong>[！UICONTROL將此指派給]</strong>選項，然後開始輸入人員名稱，並在人員名稱出現在以下清單中時按一下該名稱。 對您要新增的每個人重複此動作，然後按一下<strong>[！UICONTROL儲存]</strong>。</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[！UICONTROL優先順序]</td> 
      <td>按一下下拉箭頭，然後按一下您要問題的優先順序。</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[！UICONTROL包含電子郵件附件]</td> 
      <td> <p>（只有在電子郵件至少包含一個附件時才可用。） 按一下此選項，將電子郵件中的附件儲存至問題的[！UICONTROL檔案]區域。 </p> <p>如果您不想儲存附件，請按一下附件名稱右側的X。 </p> <p>如果電子郵件包含指向[!DNL Google Drive]中檔案的連結，則會將其儲存到您正在建立的問題的[！UICONTROL概觀]索引標籤。 </p> <p>重要：為了使其運作，您的[!DNL Workfront]管理員必須授權[!DNL Google Drive]使用[!DNL Workfront]中的檔案，如文章<a href="../../administration-and-setup/configure-integrations/configure-document-integrations.md" class="MCXref xref">設定檔案整合</a>中的<a href="../../administration-and-setup/configure-integrations/configure-document-integrations.md#configur" class="MCXref xref">設定整合以管理檔案</a>一節所述。</p> <p>如果啟用此選項，則對於您轉換為任務、問題和更新的其他電子郵件，此選項仍保持啟用狀態。</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">包含電子郵件檔案</td> 
      <td> <p>按一下此選項，將原始電子郵件儲存為電子郵件(EML) （電子郵件）檔案<span>至問題的[！UICONTROL檔案]區域</span>。 從那裡，您可以連按兩下檔案，以在電子郵件應用程式中開啟電子郵件。</p> <p>如果啟用此選項，則對於您轉換為任務、問題和更新的其他電子郵件，此選項仍保持啟用狀態。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下&#x200B;**[!UICONTROL 建立問題]**。

   新問題的&#x200B;**[!UICONTROL 詳細資料]**&#x200B;索引標籤會顯示在[!DNL Workfront for Google Workspace]面板中。 您可以按一下「**[!UICONTROL 更新]**」，立即開始與共同作業人員通訊，不必離開您的收件匣。

   在&#x200B;**[!UICONTROL 詳細資料]**&#x200B;標籤底部，您也可以按一下&#x200B;**[!UICONTROL 在Workfront中檢視]**，移至Workfront中的新問題。

   當您重新整理瀏覽器時，訊息會在[!UICONTROL Google Workspace的Workfront]面板底部顯示連結，以確認您已將此電子郵件轉換為問題：

   您可以按一下連結，針對您建立的問題，移至「[!DNL Workfront for Google Workspace]」面板內的「詳細資料」檢視。

   您可以重複這些步驟，將相同的電子郵件轉換為多個問題。 當您重新整理瀏覽器或在其他時間返回電子郵件時，您為電子郵件建立的所有連結都會列在[!UICONTROL Google Workspace的Workfront]面板底部。

1. （選用）執行下列任一項作業，繼續處理[!DNL Workfront for Google Workspace]面板中的問題：

   * 若要在&#x200B;**[!UICONTROL 更新]**&#x200B;標籤上新增更新，請按一下&#x200B;**[!UICONTROL 開始新的更新]**&#x200B;並輸入更新。

   * 若要回覆&#x200B;**[!UICONTROL 更新]**&#x200B;標籤上的更新，請按一下&#x200B;**[!UICONTROL 回覆]**，然後輸入您的回覆。

     對於上述兩個動作，您可以通知特定使用者您的評論。 按一下&#x200B;**[!UICONTROL 通知]**，開始輸入使用者的名稱，然後當名稱出現在下拉式清單中時，按一下該名稱。 對您要通知的其他使用者重複此程式，然後按一下&#x200B;**[!UICONTROL 發佈]**。

   * 按一下「**[!UICONTROL 檔案]**」標籤，檢視與問題一併儲存的任何檔案。
