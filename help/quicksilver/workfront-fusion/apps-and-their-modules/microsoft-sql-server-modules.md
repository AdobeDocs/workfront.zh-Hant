---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 聯結器
navigation-topic: apps-and-their-modules
title: Microsoft SQL Server模組
description: 您可以使用 [!DNL Adobe Workfront Fusion] 以連線至Microsoft SQL Server。
author: Becky
feature: Workfront Fusion
exl-id: d79cf00d-a81e-4d88-ac4a-f80b7b5a92b3
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '391'
ht-degree: 1%

---

# [!DNL Microsoft SQL Server] 模組

您可以使用 [!DNL Adobe Workfront Fusion] 以連線到 [!UICONTROL Microsoft SQL Server].

## 存取需求

您必須具有下列存取權才能使用本文中的功能：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計劃*</td>
  <td> <p>[！UICONTROL Pro]或更高版本</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權*</td>
   <td> <p>[！UICONTROL計畫]，[！UICONTROL工作]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] 授權**</td> 
   <td>
   <p>目前授權需求：否 [!DNL Workfront Fusion] 授權需求。</p>
   <p>或</p>
   <p>舊版授權需求： [！UICONTROL [!DNL Workfront Fusion] 適用於工作自動化與整合] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>
   <p>目前產品需求：如果您有[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Adobe Workfront] 計畫，您的組織必須購買 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文所述功能。 [!DNL Workfront Fusion] 包含在[！UICONTROL Ultimate]中 [!DNL Workfront] 計畫。</p>
   <p>或</p>
   <p>舊版產品需求：貴組織必須購買 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文所述功能。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

若要瞭解您擁有哪些計畫、授權型別或存取權，請聯絡您的 [!DNL Workfront] 管理員。

有關以下專案的資訊： [!DNL Adobe Workfront Fusion] 授權，請參閱 [[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 使用 [!DNL Microsoft SQL Server] 模組

您可以透過預存程式，直接在資料庫伺服器上執行自訂邏輯。 [!DNL Adobe Workfront Fusion] 會動態載入輸入/輸出引數和記錄集的介面，以便每個引數或值可以個別對應。 開始設定案例之前，請確定您用來連線至資料庫的帳戶擁有讀取許可權 `INFORMATION_SCHEMA.ROUTINES` 和 `INFORMATION_SCHEMA.PARAMETERS` 檢視。

時間 [!DNL Fusion] 建立與的連線 [!DNL SQL server] 目的地， [!DNL Fusion] 使用者會識別主機（託管伺服器的網域名稱或IP位址）和連線埠。 [!DNL Fusion] 可以連線到任何可用的主機和連線埠。

瞭解使用者所使用的特定IP位址 [!DNL Workfront Fusion]，請參閱 [用於存取的IP位址 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/get-started/ip-addresses-for-fusion.md)

若要進一步瞭解如何建立預存程式，請參閱 [!DNL Microsoft SQL Server] 說明檔案。

>[!NOTE]
>
>[!DNL Workfront Fusion] 不支援多個記錄集。 系統只會處理第一個專案。

## 疑難排解錯誤 [!UICONTROL ER_LOCK_WAIT_TIMEOUT：超過鎖定等待逾時；請嘗試重新啟動交易]

使用多個模組修改相同資料時，會發生此錯誤。 這是由SQL交易所造成。

執行任何SQL模組時，它會啟動交易。 交易在案例完全執行後完成。

如果另一個模組嘗試存取相同的資料，則必須等到前一個交易完成。 由於第一個交易將在案例完成後完成，第二個交易永遠無法開始。

### 解決方案：

開啟自動提交。 自動認可會在模組執行完成後立即完成（認可）每個交易。

1. 按一下 [!UICONTROL 案例設定] 圖示 ![](assets/scenario-settings-icon.png)在熒幕底部。
1. 按一下 **[!UICONTROL 自動認可]** 核取方塊。
1. 按一下 **[!UICONTROL 確定]** 以儲存情境設定。
