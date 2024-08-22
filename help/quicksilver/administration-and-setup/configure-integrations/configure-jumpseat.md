---
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
title: 設定 JumpSeat 整合
description: 您可以整合 [!DNL JumpSeat] 與 [!DNL Workfront] 以建立自訂的產品內指南。
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
author: Nolan, Becky
exl-id: 23edb48b-8cad-47be-8ace-5238a5869677
source-git-commit: 55c8a3e5d0041a0e975bfd979a2d2e38930fea8d
workflow-type: tm+mt
source-wordcount: '258'
ht-degree: 4%

---

# 設定 JumpSeat 整合

您可以整合[!DNL JumpSeat]與[!DNL Workfront]，以建立自訂的產品內指南。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計畫*</td> 
   <td> <p>[！UICONTROL Enterprise] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權*</td> 
   <td>[！UICONTROL計畫]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>您必須擁有使用中的[!DNL JumpSeat]計畫。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p> 您必須是[!DNL Workfront]管理員。 如需[!DNL Workfront]管理員的相關資訊，請參閱<a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予使用者完整管理存取權</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的[!DNL Workfront]管理員。

+++

## 先決條件

開始之前，您必須

* 在[!DNL JumpSeat]中新增並啟動[!DNL Workfront]作為應用程式。 如需詳細資訊，請參閱[如何新增或刪除應用程式](https://support.jumpseat.io/article/how-to-add-an-application/)。

## 設定[!DNL JumpSeat]整合

我們建議您在預覽和生產環境中設定[!DNL JumpSeat]整合。

>[!TIP]
>
>您需要在[!DNL JumpSeat]中新增並啟用兩個不同的[!DNL Workfront]應用程式 — 一個用於預覽，一個用於生產。 如需詳細資訊，請參閱[如何新增或刪除應用程式](https://support.jumpseat.io/article/how-to-add-an-application/)。

若要設定[!DNL JumpSeat]整合：

{{step-1-to-setup}}

1. 在左側面板中，按一下&#x200B;**[!UICONTROL 系統]** > **[!UICONTROL [!DNL JumpSeat]整合]**。
1. 輸入您的&#x200B;**[!UICONTROL [!DNL JumpSeat]URL]**，您可在[!DNL JumpSeat]中的擴充功能圖示上找到。

   **範例：** [!DNL https]：//{mycompanyname}.jumpseat.io

1. 輸入&#x200B;**[!UICONTROL [!DNL JumpSeat]整合權杖]**。 您可以在[!DNL JumpSeat]的&#x200B;**[!UICONTROL 組態]**&#x200B;頁面上找到此專案。

   **範例：** $2y$10$BevsKeQ8....OYR.LurSg2U64O

1. 按一下&#x200B;**[!UICONTROL 測試組態]**。
1. 選擇您要整合為&#x200B;**[!UICONTROL 作用中]**&#x200B;或&#x200B;**[!UICONTROL 非作用中]**。

   >[!IMPORTANT]
   >
   >在步驟5中執行的設定測試必須通過，才能啟用整合。

   ![JumpSeat整合頁面](assets/jumpseat-integration-page.png)

1. 按一下「**[!UICONTROL 儲存]**」。

>[!TIP]
>
>如需設定[!DNL JumpSeat]整合的詳細資訊，請參閱[JumpSeat+Workfront](https://jumpseat.io/landing-page/jumpseat-workfront/)的[!DNL JumpSeat]檔案。
