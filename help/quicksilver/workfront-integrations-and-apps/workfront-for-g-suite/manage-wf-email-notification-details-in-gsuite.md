---
product-area: workfront-integrations
keywords: google，doc，檔案，工作表，幻燈片
navigation-topic: workfront-for-g-suite
title: 管理 [!DNL Adobe Workfront] 來自G Suite的通知詳細資料
description: 在G Suite中，當您開啟通知電子郵件Adobe [!DNL Workfront] 已傳送，您無需離開收件匣即可檢視相關工作專案詳細資訊和回應。 如果有可用動作（例如核准請求），您可以直接從Workfront for G Suite執行這些動作。
author: Becky
feature: Workfront Integrations and Apps
exl-id: d5ca31d8-3667-4405-a523-3dc248a94746
source-git-commit: 4b95828dc3e6a67c4dbefb46f173303c519643a9
workflow-type: tm+mt
source-wordcount: '480'
ht-degree: 1%

---

# 管理 [!DNL Adobe Workfront] 通知詳細資料來源 [!DNL G Suite]

>[!NOTE]
>
>Google適用的Adobe Workfront外掛程式最新版本已於2023年6月26日發行。

在 [!DNL G Suite]，當您開啟通知電子郵件時 [!DNL Adobe Workfront] 已傳送，您可以檢視相關工作專案詳細資料且無需離開即可回應 [!UICONTROL 收件匣]. 如果有動作（例如核准請求），您可以直接從執行這些動作 [!DNL Workfront for G Suite].

>[!NOTE]
>
> [!DNL Workfront for G Suite] 支援您收到的幾乎所有電子郵件通知型別 [!DNL Workfront] （大約120種不同的型別）。 [!UICONTROL 每日摘要] 電子郵件傳送自 [!DNL Workfront] 未出現在 [!DNL Workfront for G Suite]. 如需關於以下專案的資訊： [!DNL Workfront] 電子郵件通知型別，請參閱 [啟用或停用您自己的事件通知](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

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

在您管理通知詳細資料之前，請前往 [!DNL G Suite]，您必須

* 安裝 [!DNL Workfront for G suite]\
   如需指示，請參閱 [安裝 [!DNL Adobe Workfront for G Suite]](../../workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md).

## 管理 [!DNL Adobe Workfront] 通知詳細資料來源 [!DNL G Suite]

1. 如果 [!DNL Workfront for G Suite] 面板未顯示，請按一下 [!DNL Workfront] 圖示 ![](assets/wf-lion-icon.png) 在 [!DNL G Suite] 頁面最右側的附加元件側欄。
1. 在 [!DNL G Suite]，開啟 [!DNL Workfront] 通知電子郵件。
1. 按一下 **[!UICONTROL 檢視所有更新]** 如果顯示在面板頂端附近。
1. 按一下 **[!UICONTROL 詳細資料]**.
1. 按一下任何可用選項。

   可能顯示的選項與您已開啟的電子郵件通知型別有關。 例如，如果是要求您核准任務的電子郵件通知，您會看到 **[!UICONTROL 核准]** 和 **[!UICONTROL 拒絕]** 而不是下列選項 **[!UICONTROL 處理它]** 或 **[!UICONTROL 完成]**：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>電子郵件通知型別</th> 
      <th>動作</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td>任務或問題</td> 
      <td><strong>[！UICONTROL核准]</strong> 它， <strong>[！UICONTROL拒絕]</strong> 它， <strong>[！UICONTROL授予]</strong> 存取它， <strong>[！UICONTROL忽略]</strong> 要求存取它， <strong>[！UICONTROL處理它]</strong>，或按一下選項以表示您已 <strong>[！UICONTROL完成]</strong> 使用它</td> 
     </tr> 
     <tr> 
      <td>專案</td> 
      <td><strong>[！UICONTROL核准]</strong> 它， <strong>[！UICONTROL拒絕]</strong> 它， <strong>[！UICONTROL授予]</strong> 存取它，或 <strong>[！UICONTROL忽略]</strong> 要求存取它</td> 
     </tr> 
     <tr> 
      <td>文件</td> 
      <td><strong>[！UICONTROL核准]</strong> 它， <strong>[！UICONTROL拒絕]</strong> 它， <strong>[！UICONTROL授予]</strong> 存取它，或 <strong>[！UICONTROL忽略]</strong> 要求存取它</td> 
     </tr> 
     <tr> 
      <td>更新 </td> 
      <td> <p>檢視專案更新完整清單的任何部分，以便擁有您需要的內容 <strong>[！UICONTROL貼文]</strong> 新的更新或 <strong>[！UICONTROL回覆]</strong>. 您可以按一下 <strong>[！UICONTROL Notify]</strong> 以提醒特定使用者您的回覆。 </p> <p>如需詳細資訊，請參閱 <a href="../../workfront-integrations-and-apps/workfront-for-g-suite/reply-to-wf-update-notification-from-gsuite.md" class="MCXref xref">回覆 [!DNL Adobe Workfront] 更新通知來源 [!DNL G Suite]</a>.</p> </td> 
     </tr> 
     <tr> 
      <td>核准請求</td> 
      <td><strong>[！UICONTROL核准]</strong> 或 <strong>[！UICONTROL拒絕]</strong> 它（您可以按一下其他選項來改變主意）、下載、檢視其擁有者或檢視其參考號碼</td> 
     </tr> 
     <tr> 
      <td>專案狀態的變更</td> 
      <td> 檢視專案的所有目前資訊，包括任何自訂表格。 </td> 
     </tr> 
    </tbody> 
   </table>
