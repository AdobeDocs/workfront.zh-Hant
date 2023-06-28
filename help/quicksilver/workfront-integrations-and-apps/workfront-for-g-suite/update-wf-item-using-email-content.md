---
product-area: workfront-integrations;projects
keywords: google，doc，檔案，工作表，幻燈片
navigation-topic: workfront-for-g-suite
title: 更新 [!DNL Adobe Workfront] 使用電子郵件內容的G Suite專案
description: 您可以使用非Adobe Workfront電子郵件中的資訊更新現有的專案、任務或問題。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 2ac392f5-98a3-4ab6-a0e3-cda378f0f68b
source-git-commit: 4b95828dc3e6a67c4dbefb46f173303c519643a9
workflow-type: tm+mt
source-wordcount: '649'
ht-degree: 0%

---

# 更新 [!DNL Adobe Workfront] 專案來源 [!DNL G Suite] 使用電子郵件內容

>[!NOTE]
>
>Google適用的Adobe Workfront外掛程式最新版本已於2023年6月26日發行。

您可以使用非的資訊更新現有的專案、任務或問題。[!DNL Adobe Workfront] 電子郵件。

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

更新之前 [!DNL Workfront] 使用來自的電子郵件內容的專案 [!DNL G Suite]，您必須

* 安裝 [!DNL Workfront for G suite]\
   如需指示，請參閱 [安裝 [!DNL Adobe Workfront for G Suite]](../../workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md).

## 更新 [!DNL Workfront] 使用來自的電子郵件內容的專案 [!DNL G Suite]

1. 如果 [!UICONTROL 適用於G Suite的Workfront] 面板未顯示，請按一下Workfront圖示 ![](assets/wf-lion-icon.png) 在 [!DNL G Suite] 頁面最右側的附加元件側欄。
1. 當電子郵件訊息開啟於 [!DNL G Suite]，按一下 **[!UICONTROL 發佈為新更新]** 在 [!DNL G Suite] 面板。
1. 下 **[!UICONTROL 型別]**，按一下下拉式箭頭，然後按一下您要新增更新的物件型別。
1. 按一下 **[!UICONTROL 搜尋]** 選項，開始輸入您要新增更新的物件名稱，然後選取出現在以下清單中的專案。

   此選項會依您在步驟3中所選取的專案而有所不同。 可能是 **[!UICONTROL 搜尋專案]**， **[!UICONTROL 搜尋任務]**，或 **[!UICONTROL 搜尋問題]**.

   >[!NOTE]
   >
   >當您輸入任務名稱時，臨時個人任務會從下面顯示的名稱清單中排除。

1. 進行下列任一項選擇性變更：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[！UICONTROL更新]</td> 
      <td>編輯此文字的任何部分，這些部分取自電子郵件的主旨行與內文。</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[！UICONTROL包含電子郵件附件]</td> 
      <td><p>（只有在電子郵件至少包含一個附件時才可用。） 按一下此選項，將附件儲存在任務或問題的[！UICONTROL檔案]索引標籤中。 </p><p>如果您不想儲存附件，請按一下附件名稱右側的X。 </p><p>如果電子郵件包含檔案的連結 [!DNL Google Drive]，連結會儲存至您建立之任務或問題的[！UICONTROL概觀]索引標籤。 </p><p>重要： <span style="color: #ff1493;"><span style="color: #000000;">為了讓此功能發揮作用，您的</span></span>[!DNL Workfront] 管理員<span style="color: #ff1493;"><span style="color: #000000;"> 必須授權 [!DNL Google Drive] 使用 [!DNL Workfront]</span></span></p>
      <p>如果啟用此選項，則轉換為任務、問題和更新的其他電子郵件仍會啟用此選項。</p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">通知</td> 
      <td>按一下 <strong>[！UICONTROL Notify]</strong>，按一下 <strong>[！UICONTROL搜尋使用者或團隊]</strong> 選項，然後開始輸入人員或團隊的名稱，並在它出現於以下清單中時按一下它。 對您要新增的每個人和團隊重複此步驟，然後按一下 <strong>[！UICONTROL儲存]</strong>.</td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下 **[!UICONTROL 更新]**.

   當您重新整理瀏覽器時，會出現一則訊息，其底部會有連結 [!DNL Workfront for G Suite] 面板會確認您已將電子郵件轉換為更新：

   您可以按一下連結，前往 [!UICONTROL 更新] 定位於 [!DNL Workfront] 您於步驟4中指定的物件。

   您可以重複這些步驟，將相同的電子郵件轉換為更新、任務和問題(請參閱 [使用電子郵件內容在[！DNL G Suite]中建立Adobe Workfront問題](../../workfront-integrations-and-apps/workfront-for-g-suite/create-wf-issue-in-g-suite-using-email-content.md))。 當您重新整理瀏覽器或在其他時間返回電子郵件時，您為電子郵件建立的所有連結都會列在 [!UICONTROL 適用於G Suite的Workfront] 面板。

1. （選用）繼續使用中的更新 [!DNL Workfront] 執行下列任一項作業，即可使用附加元件面板：

   * 若要在上新增另一個更新 **[!UICONTROL 更新]** 標籤，按一下 **[!UICONTROL 開始新的更新]** 並輸入資訊。

   * 若要回覆 **[!UICONTROL 更新]** 標籤，按一下 **[!UICONTROL 回覆]** 並輸入您的回覆。

     對於上述兩個選項，您可以按一下 **[!UICONTROL 通知]** 以指定回覆的收件者，如步驟5所示。 準備就緒後，按一下 **[!UICONTROL Post]** 以新增更新或回覆。

   * 按一下 **[!UICONTROL 詳細資料]** 標籤以檢視新專案、任務或問題的詳細資訊。
