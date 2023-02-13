---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 連接器
navigation-topic: apps-and-their-modules
title: Microsoft SQL Server模組
description: 您可以使用 [!DNL Adobe Workfront Fusion] 連接到Microsoft SQL Server。
author: Becky
feature: Workfront Fusion
exl-id: d79cf00d-a81e-4d88-ac4a-f80b7b5a92b3
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '343'
ht-degree: 0%

---

# [!DNL Microsoft SQL Server] 模組

您可以使用 [!DNL Adobe Workfront Fusion] 連接到 [!UICONTROL Microsoft SQL Server].

## 存取需求

您必須具備下列存取權才能使用本文中的功能：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計劃*</td>
  <td> <p>[!UICONTROL Pro]或更高版本</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權*</td>
   <td> <p>[!UICONTROL計畫]、[!UICONTROL工作]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] 許可**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] （工作自動化和整合） </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>貴組織必須購買 [!DNL Adobe Workfront Fusion] 和 [!DNL Adobe Workfront] 以使用本文所述的功能。</td> 
  </tr> 
 </tbody> 
</table>

若要了解您擁有的計畫、授權類型或存取權，請聯絡您的 [!DNL Workfront] 管理員。

如需 [!DNL Adobe Workfront Fusion] 許可證，請參閱 [[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 使用 [!DNL Microsoft SQL Server] 模組

您可以通過儲存過程直接在資料庫伺服器上執行自定義邏輯。 [!DNL Adobe Workfront Fusion] 動態載入輸入/輸出參數和記錄集的介面，以便每個參數或值可以單獨映射。 開始配置方案之前，請確保您用來連接到資料庫的帳戶具有對的讀取訪問權限 `INFORMATION_SCHEMA.ROUTINES` 和 `INFORMATION_SCHEMA.PARAMETERS` 檢視。

當 [!DNL Fusion] 建立與 [!DNL SQL server] 目的地， [!DNL Fusion] 用戶標識主機（托管伺服器的域名或IP地址）和埠。 [!DNL Fusion] 可以連接到任何可用的主機和埠。

如需所使用之特定IP位址的相關資訊， [!DNL Workfront Fusion]，請參閱 [用於存取的IP位址 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/get-started/ip-addresses-for-fusion.md)

要了解有關建立儲存過程的詳細資訊，請參閱 [!DNL Microsoft SQL Server] 檔案。

>[!NOTE]
>
>[!DNL Workfront Fusion] 不支援多個記錄集。 只會處理第一個。

## 疑難排解錯誤 [!UICONTROL ER_LOCK_WAIT_TIMEOUT:超過鎖定等待超時；重新啟動事務]

使用多個模組修改相同資料時，會發生此錯誤。 它是由SQL事務造成的。

執行任何SQL模組時，它將啟動事務。 完全執行情境後，交易會完成。

如果其他模組嘗試存取相同的資料，則必須等待到上一個交易完成。 由於第一個交易會在方案完成後完成，因此第二個交易永遠無法開始。

### 解決方案：

開啟自動提交。 自動提交會在模組執行完成後立即完成（提交）每個事務。

1. 按一下 [!UICONTROL 藍本設定] 圖示 ![](assets/scenario-settings-icon.png)在螢幕底部。
1. 按一下 **[!UICONTROL 自動提交]** 核取方塊。
1. 按一下 **[!UICONTROL 確定]** 儲存案例設定。
