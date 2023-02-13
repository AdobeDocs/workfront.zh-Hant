---
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
title: 配置JumpSeat整合
description: 您可以整合 [!DNL JumpSeat] with [!DNL Workfront] 建立自訂的產品內指引。
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
exl-id: 23edb48b-8cad-47be-8ace-5238a5869677
source-git-commit: 2f840ea68c9efb78acb4c24346c6775671ed0334
workflow-type: tm+mt
source-wordcount: '245'
ht-degree: 2%

---

# 配置JumpSeat整合

您可以整合 [!DNL JumpSeat] with [!DNL Workfront] 建立自訂的產品內指引。

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 計劃*</strong></td> 
   <td> <p>[!UICONTROL Enterprise] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 授權*</strong></td> 
   <td>[!UICONTROL計畫]</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>產品</strong></td> 
   <td>您必須具有活動 [!DNL JumpSeat] 計畫。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>訪問級別配置*</strong></td> 
   <td> <p> 您必須是 [!DNL Workfront] 管理員。 如需 [!DNL Workfront] 管理員請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予使用者完整的管理存取權</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的 [!DNL Workfront] 管理員。

## 必要條件

開始之前，您必須

* 新增及啟用 [!DNL Workfront] 作為 [!DNL JumpSeat]. 如需詳細資訊，請參閱 [如何新增或刪除應用程式](https://support.jumpseat.io/article/how-to-add-an-application/).

## 設定 [!DNL JumpSeat] 整合

建議您設定 [!DNL JumpSeat] 與預覽和生產環境的整合。

>[!TIP]
>
>您需要新增和啟動兩個不同的 [!DNL Workfront] 應用程式 [!DNL JumpSeat] — 一個用於預覽，一個用於生產。 請參閱 [如何新增或刪除應用程式](https://support.jumpseat.io/article/how-to-add-an-application/) 以取得更多資訊。

若要設定 [!DNL JumpSeat] 整合：

1. 按一下 **[!UICONTROL 主菜單]** 圖示 ![](assets/main-menu-icon.png) 在 [!DNL Adobe Workfront]，然後按一下 **[!UICONTROL 設定]**.
1. 在左側面板中，按一下 **[!UICONTROL 系統]** > **[!UICONTROL [!DNL JumpSeat]整合]**.
1. 輸入 **[!UICONTROL [!DNL JumpSeat]URL]**.

   **範例：** [!DNL https]://{mycompanyname}.jumpseat.io

1. 輸入 **[!UICONTROL [!DNL JumpSeat]整合Token]**. 您可以在 **[!UICONTROL 設定]** 頁面 [!DNL JumpSeat].

   **範例：** $2y$10$BevsKeQ8....OYR.LurSg2U64O

1. 按一下 **[!UICONTROL 測試配置]**.
1. 選擇是否希望整合 **[!UICONTROL 作用中]** 或 **[!UICONTROL 非作用中]**.

   >[!IMPORTANT]
   >
   >在步驟5中執行的設定測試必須通過，才能啟動整合。

   ![JumpSeat整合頁面](assets/jumpseat-integration-page.png)

1. 按一下&#x200B;**[!UICONTROL 儲存]**。
