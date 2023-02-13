---
content-type: overview;how-to-procedural
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: system-information
title: 預覽沙箱測試環境 —  [!DNL Workfront Proof]
description: 「預覽沙箱」是測試環境，可作為即時環境的復本，並每週末重新整理一次 [!DNL Workfront Proof].
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: cdf269c6-39b1-477a-b9ea-03edf2de77f0
source-git-commit: 088570f516bbea2e6fd81b1f711151d8941ca71e
workflow-type: tm+mt
source-wordcount: '436'
ht-degree: 0%

---

# 預覽沙箱測試環境 —  [!DNL Workfront Proof]

>[!IMPORTANT]
>
>本文說明獨立產品中的功能 [!DNL Workfront Proof]. 有關內部校對的資訊 [!DNL Adobe Workfront]，請參閱 [校對](../../../review-and-approve-work/proofing/proofing.md).

「預覽沙箱」是測試環境，可作為即時環境的復本，並每週末重新整理一次 [!DNL Workfront Proof].

## 了解預覽沙箱

「預覽沙箱」可作為您組織中的使用者在不影響生產環境的情況下，安全地測試及處理來自生產環境的資料。 它是運行培訓課程、測試新功能和確定安裝功能的理想選擇。

此外，新產品功能會先上傳至「預覽沙箱」環境，再傳送至「生產」環境。 您的使用者可以在此試用新功能，而不會影響其在生產環境中的一般工作流程。

預覽沙箱包含您的實際生產資料。 資料會從「生產」流至「預覽」，而非相反。 它每個週末都會重新整理，因此資料最多可比生產環境落後一週。 自上次重新整理後建立的項目會在「預覽沙箱」環境中，直到後續重新整理為止。

## 存取預覽沙箱

依預設，身為系統管理員，您可以存取「預覽沙箱」環境。 如果您無法如本節所述存取「預覽沙箱」環境，請連絡您的 [!DNL Workfront] 管理員或我們的支援團隊。

* [以獨立方式存取預覽沙箱 [!DNL Workfront Proof] 客戶](#accessing-the-preview-sandbox-as-a-stand-alone-workfront-proof-customer)
* [以 [!DNL Workfront]+[!DNL Workfront Proof] 客戶](#accessing-the-preview-sandbox-as-a-workfrontworkfront-proof-customer)

### 以獨立方式存取預覽沙箱 [!DNL Workfront Proof] 客戶

1. 導覽至此URL:  `https://preview.proofhq.com`.
1. 使用您的預覽憑證登入。\
   除非您在預覽重新整理後在生產環境中變更，否則預覽認證應與生產認證相同。 只有在每週末都會進行重新整理時，才會同步登入。 不會自動同步。

### 以 [!DNL Workfront+Workfront] 證明客戶

身為系統管理員，您可以存取 [!DNL Workfront Proof] 透過 [!DNL Workfront] 介面。

若要存取 [!DNL Workfront Proof] 預覽沙箱：

1. 登入 [!DNL Workfront] 環境。
1. 按一下 **[!UICONTROL 設定]** 欄中。
1. 按一下 **[!UICONTROL 系統]** >**[!UICONTROL 偏好設定]**.

1. 在 **[!UICONTROL 測試環境]** ，按一下 **[!UICONTROL 沙箱預覽]**.

1. 使用您的預覽憑證登入。\
   除非您在預覽重新整理後在生產環境中變更，否則預覽憑證應與生產憑證相同。 只有在重新整理發生時，登入才會同步。 不會自動同步。
1. 按一下 [!DNL Workfront Proof] 表徵圖。\
   ![proof_access_proofhq.png](assets/proof-access-proofhq-350x39.png)\
   此 [!DNL Workfront Proof] 預覽環境隨即顯示。

## 從預覽沙箱接收電子郵件

不會從 [!DNL Workfront Proof] 預覽環境。
