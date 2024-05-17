---
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
title: 設定JumpSeat整合
description: 您可以整合 [!DNL JumpSeat] 替換為 [!DNL Workfront] 以建立自訂的產品內指南。
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
exl-id: 23edb48b-8cad-47be-8ace-5238a5869677
source-git-commit: 530c4451f4720a1710350f8e822e343794b63e87
workflow-type: tm+mt
source-wordcount: '260'
ht-degree: 1%

---

# 設定JumpSeat整合

您可以整合 [!DNL JumpSeat] 替換為 [!DNL Workfront] 以建立自訂的產品內指南。

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 計畫*</strong></td> 
   <td> <p>[！UICONTROL Enterprise] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 授權*</strong></td> 
   <td>[！UICONTROL計畫]</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>產品</strong></td> 
   <td>您必須擁有使用中 [!DNL JumpSeat] 計畫。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>存取層級設定*</strong></td> 
   <td> <p> 您必須是 [!DNL Workfront] 管理員。 有關的資訊 [!DNL Workfront] 管理員，請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予使用者完整管理存取權</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的 [!DNL Workfront] 管理員。

## 先決條件

開始之前，您必須

* 新增並啟動 [!DNL Workfront] 作為中的應用程式 [!DNL JumpSeat]. 如需詳細資訊，請參閱 [如何新增或刪除應用程式](https://support.jumpseat.io/article/how-to-add-an-application/).

## 設定 [!DNL JumpSeat] 整合

我們建議設定 [!DNL JumpSeat] 在預覽和生產環境中整合。

>[!TIP]
>
>您需要新增並啟用兩個個別的 [!DNL Workfront] 中的應用程式 [!DNL JumpSeat] — 一個用於預覽，另一個用於生產。 另請參閱 [如何新增或刪除應用程式](https://support.jumpseat.io/article/how-to-add-an-application/) 以取得詳細資訊。

若要設定 [!DNL JumpSeat] 整合：

1. 按一下 **[!UICONTROL 主要功能表]** 圖示 ![](assets/main-menu-icon.png) 位於的右上角 [!DNL Adobe Workfront]，然後按一下 **[!UICONTROL 設定]**.
1. 在左側面板中，按一下 **[!UICONTROL 系統]** > **[!UICONTROL [!DNL JumpSeat]整合]**.
1. 輸入您的 **[!UICONTROL [!DNL JumpSeat]URL]**，您可至下列位置找到擴充功能圖示： [!DNL JumpSeat].

   **範例：** [!DNL https]：//{mycompanyname}.jumpseat.io

1. 輸入 **[!UICONTROL [!DNL JumpSeat]整合權杖]**. 您可在此頁面找到： **[!UICONTROL 設定]** 頁面位置 [!DNL JumpSeat].

   **範例：** $2y$10$BevsKeQ8....OYR.LurSg2U64O

1. 按一下 **[!UICONTROL 測試設定]**.
1. 選擇您是否希望整合 **[!UICONTROL 作用中]** 或 **[!UICONTROL 非使用中]**.

   >[!IMPORTANT]
   >
   >在步驟5中執行的設定測試必須通過，才能啟用整合。

   ![JumpSeat整合頁面](assets/jumpseat-integration-page.png)

1. 按一下「**[!UICONTROL 儲存]**」。

>[!TIP]
>
>如需關於設定您的 [!DNL JumpSeat] 整合，請參閱 [!DNL JumpSeat] 的檔案 [JumpSeat+Workfront](https://jumpseat.io/landing-page/jumpseat-workfront/).
