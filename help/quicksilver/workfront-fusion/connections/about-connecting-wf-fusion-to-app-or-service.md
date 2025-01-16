---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: connections-annd-webhooks
title: 連線總覽
description: Adobe Workfront Fusion檔案已移至新位置。 本文已棄用，但包含新文章的連結，內容涵蓋此功能。
author: Becky
feature: Workfront Fusion
exl-id: 2d5cf083-9893-45e8-8f7d-0f8f5a74eef3
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '665'
ht-degree: 0%

---

# 連線總覽

>[!IMPORTANT]
>
>Adobe Workfront Fusion檔案已移至新位置。
>
>本文資訊可在以下文章中找到：
>
>* [連線總覽](https://experienceleague.adobe.com/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/connection-overview.html)
>* [管理連線](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/connect-to-applications/manage-connections.html)
>
>請更新任何書籤。
>
>本文已不再更新，將於不久將來移除。

<!-- Audited: 3/2024-->

對於大多數應用程式而言，[!DNL Workfront Fusion]需要連線，以便根據特定情境的設定與指定的協力廠商服務通訊。

例如，如果您想要建立從[!DNL Workfront]擷取資訊的案例，您必須授予[!DNL Workfront Fusion]存取許可權以存取您的[!DNL Workfront]帳戶。

連線代表Fusion用來存取應用程式的授權和許可權。 您可以為每個應用程式建立一或多個連線，並可以在多個模組或案例中使用相同的連線。

大部分的連線只用於單一應用程式。 例如，[!DNL Workfront]連線不能在[!UICONTROL Salesforce]模組中使用。 有些[!DNL Adobe]應用程式可以共用連線。 如需詳細資訊，請參閱[應用程式及其模組](/help/quicksilver/workfront-fusion/apps-and-their-modules/apps-and-their-modules.md)中列出的這些應用程式的文章。

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
   <p>目前：無[!DNL Workfront Fusion]授權需求。</p>
   <p>或</p>
   <p>舊版：任何 </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>
   <p>新增：</p> <ul><li>[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Workfront]計畫：您的組織必須購買[!DNL Adobe Workfront Fusion]。</li><li>已包含[！UICONTROL Ultimate] [!DNL Workfront]計畫： [!DNL Workfront Fusion]。</li></ul>
   <p>或</p>
   <p>目前：您的組織必須購買[!DNL Adobe Workfront Fusion]。</p>
   </td> 
  </tr>
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

如需[!DNL Adobe Workfront Fusion]授權的相關資訊，請參閱[[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md)。

## 存取許可權

對於每個連線，[!DNL Workfront Fusion]只需要成功完成特定案例所需的存取許可權。 例如，如果您建立案例以從[!DNL Google Docs]列出檔案，[!DNL Workfront Fusion]不會要求取得檔案內容的許可權。 稍後，如果您發現需要存取檔案的內容，可以更新連線或建立可以存取該內容的新連線。

並非所有服務都允許您限制對特定任務的存取。 在這些情況下，[!DNL Workfront Fusion]必須要求完整的存取許可權。 如需有關如何限制[!DNL Workfront Fusion]存取您註冊這些服務的帳戶的詳細資訊，請參閱[應用程式及其模組](/help/quicksilver/workfront-fusion/apps-and-their-modules/apps-and-their-modules.md)中列出的應用程式特定檔案。

## 管理連線

您可以從[!UICONTROL 連線]區域管理所有連線。

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

1. 若要開啟[!UICONTROL 連線]區域，請按一下左側導覽中的<b>[!UICONTROL 連線]</b>。
1. （可選）按一下「環境和型別」(Environment and Type)下拉式清單並選取一個選項，以指出環境和連線型別。
1. （選擇性）若要檢視連線授予[!DNL Workfront Fusion]的許可權，請按一下[檢視]圖示![檢視該連線的連線許可權](assets/view-connection-permissions.png)。
1. （選擇性）若要重新命名連線，請反白連線名稱並輸入新名稱。
1. （選擇性）若要重新授權連線，請按一下該連線的&#x200B;**重新授權**。
1. （選擇性）若要刪除連線，請按一下該連線的&#x200B;**刪除**。
1. （選擇性）若要驗證與服務的連線是否已成功建立，請按一下連線的[驗證]。****



## 更新連線

[!DNL Workfront Fusion]通常會在無限制的時間內取得特定服務的存取權。 某些應用程式需要在一段時間後更新存取許可權。 在這些情況下，[!DNL Workfront Fusion]會在存取權到期前不久透過電子郵件通知您。

若要更新連線：

1. 按一下&#x200B;**[!UICONTROL 連線]**&#x200B;區域中的&#x200B;**[!UICONTROL 重新授權]**&#x200B;按鈕。
