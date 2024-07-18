---
content-type: overview;how-to-procedural
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: system-information
title: 預覽Sandbox測試環境 —  [!DNL Workfront Proof]
description: 預覽沙箱是測試環境，可作為您即時環境的復本，並在每個週末由 [!DNL Workfront Proof]重新整理。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: cdf269c6-39b1-477a-b9ea-03edf2de77f0
source-git-commit: 088570f516bbea2e6fd81b1f711151d8941ca71e
workflow-type: tm+mt
source-wordcount: '434'
ht-degree: 0%

---

# 預覽Sandbox測試環境 — [!DNL Workfront Proof]

>[!IMPORTANT]
>
>本文提及獨立產品[!DNL Workfront Proof]中的功能。 有關[!DNL Adobe Workfront]內部校訂的資訊，請參閱[校訂](../../../review-and-approve-work/proofing/proofing.md)。

預覽沙箱是測試環境，可作為您即時環境的復本，並在每個週末由[!DNL Workfront Proof]重新整理。

## 瞭解預覽沙箱

「預覽沙箱」可作為環境，讓您組織中的使用者可在此環境中安全地測試及處理來自生產環境的資料，而不會影響生產環境。 它非常適合用於執行訓練課程、測試新功能和判斷設定功能。

此外，新產品功能在傳送到生產環境之前，會先上傳到預覽沙箱環境。 您的使用者可以在那裡試用新功能，而不會影響他們在生產環境中的正常工作流程。

預覽沙箱包含您的實際生產資料。 資料會從生產環境流向預覽環境，而不會反向流動。 它每週末都會重新整理，因此資料最多可在生產環境後一週內運作。 自上次重新整理時間以來建立的專案會位於預覽沙箱環境中，直到後續重新整理為止。

## 存取預覽沙箱

依預設，作為系統管理員，您有權存取預覽沙箱環境。 如果您無法存取本節所述的預覽沙箱環境，請聯絡您的[!DNL Workfront]管理員或我們的支援團隊。

* [以獨立 [!DNL Workfront Proof] 客戶的身分存取預覽沙箱](#accessing-the-preview-sandbox-as-a-stand-alone-workfront-proof-customer)
* [以 [!DNL Workfront]+[!DNL Workfront Proof] 客戶的身分存取預覽沙箱](#accessing-the-preview-sandbox-as-a-workfrontworkfront-proof-customer)

### 以獨立[!DNL Workfront Proof]客戶身分存取預覽沙箱

1. 瀏覽至此URL： `https://preview.proofhq.com`。
1. 使用您的預覽憑證登入。\
   您的預覽認證應與生產認證相同，除非您在預覽重新整理發生後，於生產環境中變更了這些認證。 只有在每週末進行重新整理時，才會同步登入。 它們不會自動同步。

### 以[!DNL Workfront+Workfront]校訂客戶身分存取預覽沙箱

作為系統管理員，您可以透過[!DNL Workfront]介面存取[!DNL Workfront Proof]預覽沙箱。

若要存取[!DNL Workfront Proof]預覽沙箱：

1. 登入您的[!DNL Workfront]環境。
1. 按一下全域導覽列中的&#x200B;**[!UICONTROL 設定]**。
1. 按一下&#x200B;**[!UICONTROL 系統]** >**[!UICONTROL 偏好設定]**。

1. 在&#x200B;**[!UICONTROL 測試環境]**&#x200B;區段中，按一下&#x200B;**[!UICONTROL 沙箱預覽]**。

1. 使用您的「預覽」憑證登入。\
   您的預覽認證應與生產認證相同，除非您在預覽重新整理發生後，於生產環境中變更了這些認證。 登入只有在重新整理發生時才進行同步處理。 它們不會自動同步。
1. 按一下全域導覽列中的[!DNL Workfront Proof]圖示。\
   ![proof_access_proofhq.png](assets/proof-access-proofhq-350x39.png)\
   [!DNL Workfront Proof]預覽環境隨即顯示。

## 從預覽Sandbox接收電子郵件

絕不會從[!DNL Workfront Proof]預覽環境觸發電子郵件通知。
