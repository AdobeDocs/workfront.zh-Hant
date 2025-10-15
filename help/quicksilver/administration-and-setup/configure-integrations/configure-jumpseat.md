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
source-git-commit: 85ccee879fd4ba5a80b6e885458839901f83d26e
workflow-type: tm+mt
source-wordcount: '257'
ht-degree: 6%

---

# 設定 JumpSeat 整合

您可以整合[!DNL JumpSeat]與[!DNL Workfront]，以建立自訂的產品內指南。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

<table>
  <tr>
   <td>Adobe Workfront套件
   </td>
    <p>Workflow Ultimate</p>
   <td> <p>Prime或Ultimate</p>
   </td>
  </tr>
    <tr>
   <td>Adobe Workfront授權
   </td>
   <td>標準
   <p>規劃</p>
   </td>
  </tr>
  </tr>
  <tr>
   <td>產品
   </td>
   <td>您必須擁有使用中的[!DNL JumpSeat]計畫。
   </td>
  </tr>
   <tr>
   <td>存取層級設定
   </td>
   <td>您必須是[!DNL Workfront]管理員。
   </td>
  </tr>
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先決條件

開始之前，您必須

* 在[!DNL Workfront]中新增並啟動[!DNL JumpSeat]作為應用程式。 如需詳細資訊，請參閱[如何新增或刪除應用程式](https://support.jumpseat.io/article/how-to-add-an-application/)。

>[!IMPORTANT]
>
>如果您在Adobe Unified Experience，則必須使用下列應用程式URL： `.workfront.adobe.com`。



## 設定[!DNL JumpSeat]整合

我們建議您在預覽和生產環境中設定[!DNL JumpSeat]整合。

>[!TIP]
>
>您需要在[!DNL Workfront]中新增並啟用兩個不同的[!DNL JumpSeat]應用程式 — 一個用於預覽，一個用於生產。 如需詳細資訊，請參閱[如何新增或刪除應用程式](https://support.jumpseat.io/article/how-to-add-an-application/)。

若要設定[!DNL JumpSeat]整合：

{{step-1-to-setup}}

1. 在左側面板中，按一下&#x200B;**[!UICONTROL 系統]** > **[!UICONTROL [!DNL JumpSeat]整合]**。
1. 輸入您的&#x200B;**[!UICONTROL [!DNL JumpSeat]URL]**，您可在[!DNL JumpSeat]中的擴充功能圖示上找到。

>[!BEGINSHADEBOX]

**範例：**

https://{mycompanyname}.jumpseat.io

>>

>[!ENDSHADEBOX]

1. 輸入&#x200B;**[!UICONTROL [!DNL JumpSeat]整合權杖]**。 您可以在&#x200B;**[!UICONTROL 的]**&#x200B;組態[!DNL JumpSeat]頁面上找到此專案。

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
>如需設定[!DNL JumpSeat]整合的詳細資訊，請參閱[!DNL JumpSeat]JumpSeat+Workfront[的](https://jumpseat.io/landing-page/jumpseat-workfront/)檔案。
