---
product-area: workfront-integrations
navigation-topic: workfront-for-outlook
title: 的權限級別 [!DNL Workfront] (Outlook)
description: 此 [!DNL Workfront for Outlook] 載入項需要讀/寫郵箱訪問權限。 此 [!DNL Workfront for Outlook] 整合需要最高級別的權限，因為它具有從Outlook exchange伺服器下載電子郵件附件並將其上傳到的功能 [!DNL Workfront]，即使用者從含有附件的電子郵件提交請求時。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 704da044-21ed-4ca1-be6f-0e0aa832e069
source-git-commit: 177bf9271dca0310653b73b9100607a82290c326
workflow-type: tm+mt
source-wordcount: '451'
ht-degree: 0%

---

# 的權限級別 [!DNL Workfront for Outlook]

[!DNL Workfront for Outlook] 需要中允許的四個層級中的最高權限 [!DNL Outlook] 增益集。

如需中權限的詳細資訊，請參閱 [!DNL Outlook] 增益集，請參閱 [的隱私權、權限和安全性 [!DNL Outlook] 增益集](https://docs.microsoft.com/en-us/office/dev/add-ins/outlook/privacy-and-security) 在 [!DNL Microsoft] 檔案。

此 [!DNL Workfront for Outlook] 載入需要讀/寫郵箱訪問(`ReadWriteMailbox`)，即最高權限範圍。
此 [!DNL Workfront for Outlook] 整合需要最高層級的權限，因為它具備從 [!DNL Outlook] exchange伺服器上傳至 [!DNL Workfront]，即使用者從含有附件的電子郵件提交請求時。 為了讓此功能發揮作用， [!DNL Workfront for Outlook] 使用函式 `mailbox.getCallbackTokenAsync()` 從 [!DNL Office] 附加元件JavaScript API可取得Token，並使用該API從Exchange伺服器下載電子郵件附件。 唯一允許使用該函式的權限是 `ReadWriteMailbox`. 如需詳細資訊，請參閱 [Outlook載入項的隱私權、權限和安全性](https://docs.microsoft.com/en-us/office/dev/add-ins/outlook/privacy-and-security) 在Microsoft檔案中。

此 [!DNL Workfront for Outlook] 此外，外掛程式也需要 `ReadWriteItem` 權限(包含 `ReadWriteMailbox`)，用於讀取電子郵件內文及讀取/更新電子郵件中繼資料：

* 閱讀電子郵件內文：

   [!DNL Workfront for Outlook] 使用者提交請求時讀取電子郵件內文，或將電子郵件內文作為更新傳送至 [!DNL Adobe Workfront] 物件。
* 讀取/更新電子郵件元資料：

   [!DNL Workfront for Outlook] 當使用者從電子郵件提交請求時，會更新電子郵件標題。 這是為了儲存有關已提交的資訊 [!DNL Adobe Workfront] 物件，因此下次使用者開啟相同電子郵件的增益集時，就會顯示該電子郵件先前動作的相關資訊。

[!DNL Workfront for Outlook] 僅當用戶在附加元件內執行操作時才訪問用戶的郵箱。 它沒有任何背景功能。 Workfront for Outlook僅在下列情況下會存取使用者的信箱：

* 使用者嘗試提交請求、建立任務，或傳送電子郵件作為更新來源 [!DNL Workfront for Outlook] （開啟載入項並選取動作）
   * [!DNL Workfront for Outlook] 讀取要在載入項內填入表單中的電子郵件內文。
   * [!DNL Workfront for Outlook] 讀取電子郵件中繼資料，以顯示關於增益集的資訊，關於使用相同電子郵件在增益集中執行的先前動作。
* 當使用者提交請求、建立任務或傳送電子郵件作為更新時， [!DNL Workfront for Outlook] (按一下 [!UICONTROL 提交] 按鈕):
   * [!DNL Workfront for Outlook] 讀取電子郵件內文，以要求說明或留言的形式將其傳送至Workfront。
   * [!DNL Workfront for Outlook] 更新電子郵件中繼資料，以儲存有關已提交請求或已更新物件的資訊。
   * [!DNL Workfront for Outlook] 從exchange伺服器下載電子郵件附件，以上傳至已提交的請求、已建立的任務或已更新的對象。
