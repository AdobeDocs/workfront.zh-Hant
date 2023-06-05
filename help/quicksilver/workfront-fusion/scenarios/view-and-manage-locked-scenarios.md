---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: 在中管理鎖定的情境 [!DNL Adobe Workfront Fusion]
description: 在中管理鎖定的情境 [!DNL Adobe Workfront Fusion]
author: Becky
feature: Workfront Fusion
exl-id: 014434dc-7548-42d1-bacd-89ddf627b647
source-git-commit: 9050684504f2335f5631f63978a9f65c25fd8d5f
workflow-type: tm+mt
source-wordcount: '333'
ht-degree: 0%

---

# 在中管理鎖定的情境 [!DNL Adobe Workfront Fusion]

在某些情況下，情境可能會被暫時鎖定 [!DNL Workfront Fusion]. 鎖定的執行將在2-4小時內自動解鎖。 您也可以手動解除鎖定案例。

>[!IMPORTANT]
>
>手動解鎖情境可能會導致情境執行出錯。

## 存取需求

您必須具有下列存取權才能使用本文中的功能：

<table style="table-layout:auto">  
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] 計劃*</td> 
   <td> <p>[!DNL Pro] 或更高</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權*</td> 
   <td> <p>[！UICONTROL計畫]，[！UICONTROL工作]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Adobe Workfront Fusion]授權**</td> 
  <td> <p>[！UICONTROL [!DNL Workfront Fusion] 適用於工作自動化與整合] </p><p>[！UICONTROL [!DNL Workfront Fusion] 工作自動化專用] </p>  </td>    </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>貴組織必須購買 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文所述功能。</td> 
  </tr> 
 </tbody> 
</table>

若要瞭解您擁有哪些計畫、授權型別或存取權，請聯絡您的 [!DNL Workfront] 管理員。

有關以下專案的資訊： [!DNL Adobe Workfront Fusion] 授權，請參閱 [[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 瞭解鎖定的情況

出於多種原因，情境可能會被鎖定。

Workfront Fusion不支援並行處理排程情境。 這些情境會在情境執行開始時鎖定，並在完成時解除鎖定。 如果執行中斷，情境可能不會解鎖。 當使用者手動強制停止情景或發生系統問題時，可能會發生這種情況。

此外，Workfront Fusion工程團隊可能會鎖定情境，因為它會導致效能或其他問題。

無論鎖定案例的原因為何，該案例將在鎖定後2-4小時自動解鎖。

## 解鎖鎖定的案例

鎖定的情境將從鎖定時起2-4小時解鎖。 在排程自動解鎖案例之前，您可以手動解鎖案例。

手動解鎖情境可能會導致情境執行出錯。 我們建議僅在情境因在設計情境時執行和停止執行而被鎖定時，手動解鎖情境。 在其他情況下，我們建議您等待案例自動解鎖。

>[!IMPORTANT]
>
>手動解鎖情境可能會導致情境執行出錯。

1. 前往鎖定案例的「案例詳細資訊」頁面。
1. 按一下 **[!UICONTROL 選項]** 在熒幕的右上角。
1. 選取 **[!UICONTROL 解鎖執行]**.
1. 按一下 **[!UICONTROL 解鎖]**.
