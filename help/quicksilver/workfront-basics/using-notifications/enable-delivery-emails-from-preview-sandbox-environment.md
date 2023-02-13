---
navigation-topic: notifications
title: 啟用從預覽沙箱環境傳送電子郵件
description: 如果您想要從「預覽沙箱」環境接收電子郵件通知，您必須在登入「預覽」時，在使用者設定中啟用此功能。
author: Lisa
feature: Get Started with Workfront
exl-id: e5c7e387-d08d-42f6-a9e6-f44e514ef902
source-git-commit: f3ba39e02d690dd3a0d50ecdb22af0c12a3d4ffb
workflow-type: tm+mt
source-wordcount: '517'
ht-degree: 0%

---

# 啟用從預覽沙箱環境傳送電子郵件

[!UICONTROL Adobe Workfront] 停用「預覽」和「自訂重新整理沙箱」環境中的所有電子郵件通訊。 如需預覽沙箱環境的相關資訊，請參閱 [Adobe Workfront預覽沙箱環境](../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md). 如需自訂重新整理沙箱環境的相關資訊，請參閱 [Adobe Workfront自訂重新整理沙箱環境](../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md).

如果您想要從「預覽沙箱」環境接收下列電子郵件通知，您必須在登入「預覽」時於使用者設定中啟用此功能：

* 由事件通知觸發的電子郵件通知
* 提醒通知
* 自動延遲或提前提醒通知
* 電子郵件邀請

您可以親自或為您有權編輯的任何使用者執行此操作。 如需編輯使用者所需存取權的詳細資訊，請參閱 [授予使用者存取權](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

>[!NOTE]
>
>在「預覽沙箱」環境中，行動應用程式一律會停用報表傳送和推播通知。 您和 [!DNL Workfront] 當您存取「預覽沙箱」環境時，管理員可以為行動應用程式啟用報表傳送或推播通知。
>
>如需報表傳送的相關資訊，請參閱 [報表傳送概觀](../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan*]</strong></td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 授權*</strong></td> 
   <td> <p>[!UICONTROL Request]或更高版本以更改您自己的設定</p> <p>[!UICONTROL計畫]可編輯其他用戶的設定</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>訪問級別配置*</strong></td> 
   <td> <p>您必須具備下列其中一項：</p> 
    <ul> 
     <li> <p>[!UICONTROL系統管理員]訪問級別。</p> <p> 有關此訪問級別的資訊，請參見 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予使用者完整的管理存取權</a>. </p> </li> 
     <li> <p>在訪問級別中，必須為[!UICONTROL用戶]設定選擇[!UICONTROL編輯]。 對於[!UICONTROL用戶]設定，在[!UICONTROL微調您的設定]下 <img src="assets/gear-icon-in-access-levels.png"> ，必須啟用[!UICONTROL建立]選項和兩個[!UICONTROL用戶管理]選項中的至少一個。 </p> <p>如果您使用「[!UICONTROL用戶管理員（組用戶）]」選項，則必須是用戶所屬組的組管理員。</p> <p> <img src="assets/access-req-users-350x101.png" style="width: 350;height: 101;"> </p> <p>如需存取層級中[!UICONTROL使用者]設定的相關資訊，請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">授予使用者存取權</a>.</p> </li> 
    </ul> <p>注意：如果您仍無法存取，請詢問您的 [!DNL Workfront] 管理員。 若要了解 [!DNL Workfront] 管理員可修改您的存取層級，請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的 [!DNL Workfront] 管理員。

## 啟用從預覽沙箱環境傳送電子郵件

1. 登入您的預覽沙箱環境。
1. 按一下 [!DNL Adobe Workfront]. 然後，按一下 **[!UICONTROL 更多]** 選取 **[!UICONTROL 編輯]**.

   或

   在 [!DNL Workfront] 並按一下其名稱。 然後，按一下 **[!UICONTROL 更多]** 選取 **[!UICONTROL 編輯]**.

   或

   若為多位使用者：按一下 **[!UICONTROL 主菜單]** 圖示 ![](assets/main-menu-icon.png) 在Workfront的右上角，然後按一下 **[!UICONTROL 使用者]** ![](assets/users-icon-in-main-menu.png).  然後，選取多個使用者，然後按一下 **[!UICONTROL 編輯]**.

1. 按一下 **[!UICONTROL 偏好設定]**.
1. 選擇 **[!UICONTROL 從此測試環境接收電子郵件]**.

   >[!NOTE]
   >
   >如果您位於生產環境，則無法使用此選項。

1. 按一下 **[!UICONTROL 儲存變更]**.
