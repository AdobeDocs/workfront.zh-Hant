---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: connections-annd-webhooks
title: 連線總覽
description: 對於大多數應用程式而言，必須建立連線，透過 [!DNL Adobe Workfront Fusion] 可依據特定情境的設定，與指定的協力廠商服務通訊。
author: Becky
feature: Workfront Fusion
exl-id: 2d5cf083-9893-45e8-8f7d-0f8f5a74eef3
source-git-commit: b90343eab40e91c6f5cddeaa960ce9c9c97b1d29
workflow-type: tm+mt
source-wordcount: '616'
ht-degree: 0%

---

# 連線總覽

<!-- Audited: 3/2024-->

針對大部分應用程式， [!DNL Workfront Fusion] 需要連線，才能根據特定情境的設定，與指定的協力廠商服務通訊。

例如，如果要建立從擷取資訊的情境 [!DNL Workfront]，您必須授與存取許可權給 [!DNL Workfront Fusion] 以存取您的 [!DNL Workfront] 帳戶。

連線代表Fusion用來存取應用程式的授權和許可權。 您可以為每個應用程式建立一或多個連線，並可以在多個模組或案例中使用相同的連線。

大部分的連線只用於單一應用程式。 例如， [!DNL Workfront] 連線不能用於 [!UICONTROL Salesforce] 模組。 部分 [!DNL Adobe] 應用程式可以共用連線。 如需詳細資訊，請參閱所列之這些應用程式的文章 [應用程式及其模組](/help/quicksilver/workfront-fusion/apps-and-their-modules/apps-and-their-modules.md).

連線是在群組層級上管理的。 團隊的所有成員都可以存取團隊的連線，而團隊外部的使用者無權存取團隊的連線。

## 存取需求

您必須具有下列存取權才能使用本文中的功能：

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計劃</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權</td> 
   <td> <p>新增：[！UICONTROL Standard]</p><p>或</p><p>目前： [！UICONTROL Work]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] 授權**</td> 
   <td>
   <p>目前：否 [!DNL Workfront Fusion] 授權需求。</p>
   <p>或</p>
   <p>舊版：任何 </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>
   <p>新增：</p> <ul><li>[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Workfront] 計畫：您的組織必須購買 [!DNL Adobe Workfront Fusion].</li><li>[！UICONTROL Ultimate] [!DNL Workfront] 計畫： [!DNL Workfront Fusion] 已包括在內。</li></ul>
   <p>或</p>
   <p>目前：您的組織必須購買 [!DNL Adobe Workfront Fusion].</p>
   </td> 
  </tr>
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱 [Workfront檔案中的存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

有關的資訊 [!DNL Adobe Workfront Fusion] 授權，請參閱 [[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 存取許可權

對於每個連線， [!DNL Workfront Fusion] 只需要成功完成特定情境所需的存取許可權。 例如，如果您建立案例以列出檔案 [!DNL Google Docs]， [!DNL Workfront Fusion] 不會要求取得檔案內容的許可權。 稍後，如果您發現需要存取檔案的內容，可以更新連線或建立可以存取該內容的新連線。

並非所有服務都允許您限制對特定任務的存取。 在這些情況下， [!DNL Workfront Fusion] 必須具備完整存取許可權。 如需如何限制的詳細資訊 [!DNL Workfront Fusion] 存取您在這些服務上註冊的帳戶，請參閱以下列出的應用程式特定檔案： [應用程式及其模組](/help/quicksilver/workfront-fusion/apps-and-their-modules/apps-and-their-modules.md).

## 管理連線

您可以從以下位置管理所有連線： [!UICONTROL 連線] 區域。

>[!NOTE]
>
>連線為團隊所擁有。 如果您找不到要尋找的連線，請檢查您檢視的群組是否正確。
>
>若要選取新專案團隊：
>
>* 按一下左側導覽中的專案團隊名稱，然後選取新的專案團隊。
>
>    或
>
>* 按一下左側導覽中的「團隊概述」 ，然後按一下頁面頂端附近的團隊名稱旁的下拉箭頭。 選取新團隊。

1. 若要開啟 [!UICONTROL 連線] 區域，按一下 <b>[!UICONTROL 連線]</b> ，位於左側導覽器中。
1. （可選）按一下「環境和型別」(Environment and Type)下拉式清單並選取一個選項，以指出環境和連線型別。
1. （選擇性）若要檢視授予哪些許可權 [!DNL Workfront Fusion] 若為連線，按一下「檢視」圖示 ![檢視連線許可權](assets/view-connection-permissions.png) 用於該連線。
1. （選擇性）若要重新命名連線，請反白連線名稱並輸入新名稱。
1. （選用）若要重新授權連線，請按一下 **重新授權** 用於該連線。
1. （選用）若要刪除連線，請按一下 **刪除** 用於該連線。
1. （選擇性）若要確認與服務的連線是否已成功建立，請按一下 **驗證** 用於連線。



## 更新連線

[!DNL Workfront Fusion] 通常會在無限制的時段內取得特定服務的存取權。 某些應用程式需要在一段時間後更新存取許可權。 在這些情況下， [!DNL Workfront Fusion] 在存取權到期前不久，會透過電子郵件通知您。

若要更新連線：

1. 按一下 **[!UICONTROL 重新授權]** 中的按鈕 **[!UICONTROL 連線]** 區域。
