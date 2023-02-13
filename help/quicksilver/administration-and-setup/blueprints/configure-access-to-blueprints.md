---
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: best-practices-catalog
title: 配置對Blueprint的訪問
description: 作為系統管理員，您可以通過設定請求隊列來儲存請求，為用戶啟用請求安裝藍圖的訪問權限。 您可在該處取得單一位置以追蹤及更新請求。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: d85f363f-2ab4-45cb-b851-a7f33e1ca905
source-git-commit: d46eb98c443a421f340b1021972ddb89eda1966b
workflow-type: tm+mt
source-wordcount: '510'
ht-degree: 0%

---

# 配置對Blueprint的訪問

全部 [!DNL Adobe Workfront] 用戶可以瀏覽藍圖目錄。

身為系統管理員，您可以：

* 新增 [!UICONTROL 藍圖] 至版面範本的主功能表，並將版面範本指派給使用者或群組。 如需詳細資訊，請參閱 [自訂 [!UICONTROL 主菜單] 使用版面範本](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md) 和 [將使用者指派至版面範本](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md).

   >[!NOTE]
   >
   >* 未指派配置範本的使用者將看到 [!UICONTROL 藍圖] 圖示 [!UICONTROL 主菜單].
   >* 建立新版面範本時， [!UICONTROL 藍圖] 圖示包含在 [!UICONTROL 作用中項目] 清單 [!UICONTROL 主菜單] 依預設。



* 通過設定請求隊列來儲存請求，為用戶請求安裝藍圖啟用訪問權限。 您可在該處取得單一位置以追蹤及更新請求。 如需詳細資訊，請依照下列程式操作。
* 安裝藍圖。 如需詳細資訊，請參閱 [安裝Blueprint](../../administration-and-setup/blueprints/blueprints-install.md).

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 計劃</strong></td> 
   <td> <p> 任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe [!DNL Workfront] 授權</strong></td> 
   <td>[!UICONTROL計畫]</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>訪問級別配置</strong></td> 
   <td> <p>[!UICONTROL系統管理員]</p> </td> 
  </tr> 
 </tbody> 
</table>

## 必要條件 {#prerequisites}

* 您必須使用現有請求佇列來儲存Blueprint請求。 專案必須儲存為請求佇列，且必須位於 [!UICONTROL 目前] 狀態。
* 請求佇列必須為公用。 在請求隊列詳細資訊中，「[!UICONTROL 誰可以將請求新增到此佇列？]&quot;必須設定為 **[!UICONTROL 任何人]**.

>[!TIP]
>
>如果要為Blueprint請求建立新請求隊列，應在配置Blueprint訪問之前建立該隊列。 如需建立請求佇列的相關資訊，請參閱 [建立請求佇列](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

## 選取要儲存Blueprint請求的請求佇列

用戶必須先為這些請求選擇請求隊列，然後才能請求安裝Blueprint。 在定義請求隊列之前，用戶只能瀏覽Blueprint目錄。

1. 按一下 **[!UICONTROL 主菜單]** 圖示 ![](assets/main-menu-icon.png) 在 [!DNL Adobe Workfront]，然後按一下 **[!UICONTROL 藍圖]**.
1. 按一下 **[!UICONTROL 設定Blueprint請求]** 在目錄畫面的右上角。

   <!--
   <li value="3" data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>In the <strong>Configure blueprints</strong> dialog, ensure that the <strong>Configure request queues</strong> tab is selected.</p> </li>
   -->

1. 在 **[!UICONTROL 配置Blueprint]** 對話框，開始鍵入活動請求隊列的名稱，並在搜索結果中顯示時選擇該名稱。

   >[!IMPORTANT]
   >
   >此清單中只顯示公共請求隊列。 若要將請求佇列設為公用，請參閱 [必要條件](#prerequisites) 一節。

   請求佇列偏好設定已設定，使用者現在可以請求Blueprint安裝。

   ![設定請求佇列](assets/Blueprints_access_setup_request_queue.png)

1. （選用）若要變更實際請求佇列，請按一下「 **[!UICONTROL 編輯此請求佇列]**.

   請求佇列專案會在新的瀏覽器標籤中開啟，您可以視需要更新。

1. （選用）如果請求佇列包含主題群組或佇列主題，您可以從清單中選取。
1. 要返回Blueprint目錄，請按一下 **[!UICONTROL 關閉]**.

>[!NOTE]
>
>安裝請求的Blueprint時，應將問題狀態變更為 **[!UICONTROL 已關閉]** 或 **[!UICONTROL 已解決]** 在請求佇列中，以通知請求者。 如需安裝Blueprint的相關資訊，請參閱 [安裝Blueprint](../../administration-and-setup/blueprints/blueprints-install.md).
