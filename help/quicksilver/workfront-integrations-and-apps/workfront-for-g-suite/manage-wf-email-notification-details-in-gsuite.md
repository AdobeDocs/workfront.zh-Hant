---
product-area: workfront-integrations
keywords: google,doc，文檔，工作表，幻燈片
navigation-topic: workfront-for-g-suite
title: 管理 [!DNL Adobe Workfront] 來自G Suite的通知詳細資料
description: 在G套裝中，當您開啟通知電子郵件Adobe [!DNL Workfront] 已發送，則您可以查看相關工作項的詳細資訊並做出響應，而無需離開收件箱。 如果有可用的動作（例如核准請求），您可以直接從G Suite的Workfront執行這些動作。
author: Becky
feature: Workfront Integrations and Apps
exl-id: d5ca31d8-3667-4405-a523-3dc248a94746
source-git-commit: 3143e5a4988b7234d8225da442f5af1d756d461d
workflow-type: tm+mt
source-wordcount: '465'
ht-degree: 1%

---

# 管理 [!DNL Adobe Workfront] 通知詳細資訊 [!DNL G Suite]

在 [!DNL G Suite]，當您開啟通知電子郵件時 [!DNL Adobe Workfront] 已傳送，則您可以檢視相關工作項目詳細資訊並回應，而不需離開 [!UICONTROL 收件匣]. 如果有可用動作（例如核准請求），您可以直接從 [!DNL Workfront for G Suite].

>[!NOTE]
>
> [!DNL Workfront for G Suite] 支援您幾乎可從 [!DNL Workfront] （約120種不同類型）。 [!UICONTROL 每日摘要] 寄送的電子郵件 [!DNL Workfront] 未出現在 [!DNL Workfront for G Suite]. 如需 [!DNL Workfront] 電子郵件通知類型，請參閱 [啟用或停用您自己的事件通知](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

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

管理通知詳細資訊之前，請先從 [!DNL G Suite]，您必須

* 安裝 [!DNL Workfront for G suite]\
   如需指示，請參閱 [安裝 [!DNL Adobe Workfront for G Suite]](../../workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md).

## 管理 [!DNL Adobe Workfront] 通知詳細資訊 [!DNL G Suite]

1. 若 [!DNL Workfront for G Suite] 面板時，按一下 [!DNL Workfront] 圖示 ![](assets/wf-lion-icon.png) 在 [!DNL G Suite] 頁面最右側的附加元件側欄。
1. 在 [!DNL G Suite]，開啟 [!DNL Workfront] 通知電子郵件。
1. 按一下 **[!UICONTROL 查看所有更新]** 如果它顯示在面板頂端附近。
1. 按一下 **[!UICONTROL 詳細資料]**.
1. 按一下任何可用選項。

   可能顯示的選項與您已開啟的電子郵件通知類型相關。 例如，如果這是要求您核准任務的電子郵件通知，您會看到 **[!UICONTROL 核准]** 和 **[!UICONTROL 拒絕]** 而非 **[!UICONTROL 努力]** 或 **[!UICONTROL 完成]**:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>電子郵件通知的類型</th> 
      <th>動作</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td>任務或問題</td> 
      <td><strong>[!UICONTROL批准]</strong> 它， <strong>[!UICONTROL拒絕]</strong> 它， <strong>[!UICONTROL授予]</strong> 訪問， <strong>[!UICONTROL忽略]</strong> 請求訪問它， <strong>[!UICONTROL用它]</strong>，或按一下選項以指出您是 <strong>[!UICONTROL完成]</strong> 用它</td> 
     </tr> 
     <tr> 
      <td>專案</td> 
      <td><strong>[!UICONTROL批准]</strong> 它， <strong>[!UICONTROL拒絕]</strong> 它， <strong>[!UICONTROL授予]</strong> 存取 <strong>[!UICONTROL忽略]</strong> 存取請求</td> 
     </tr> 
     <tr> 
      <td>文件</td> 
      <td><strong>[!UICONTROL批准]</strong> 它， <strong>[!UICONTROL拒絕]</strong> 它， <strong>[!UICONTROL授予]</strong> 存取 <strong>[!UICONTROL忽略]</strong> 存取請求</td> 
     </tr> 
     <tr> 
      <td>更新 </td> 
      <td> <p>查看項目整個更新清單中的任何部分，以便擁有所需的上下文 <strong>[!UICONTROL Post]</strong> 新更新或 <strong>[!UICONTROL回復]</strong>. 您可以按一下 <strong>[!UICONTROL Notify]</strong> 提醒特定使用者您的回覆。 </p> <p>如需詳細資訊，請參閱 <a href="../../workfront-integrations-and-apps/workfront-for-g-suite/reply-to-wf-update-notification-from-gsuite.md" class="MCXref xref">回覆 [!DNL Adobe Workfront] 更新通知 [!DNL G Suite]</a>.</p> </td> 
     </tr> 
     <tr> 
      <td>核准請求</td> 
      <td><strong>[!UICONTROL批准]</strong> 或 <strong>[!UICONTROL拒絕]</strong> 它（可以通過按一下其他選項來改變主意）、下載它、查看它的所有者或查看它的參考號</td> 
     </tr> 
     <tr> 
      <td>專案狀態的變更</td> 
      <td> 檢視專案的所有目前資訊，包括任何自訂表單。 </td> 
     </tr> 
    </tbody> 
   </table>
