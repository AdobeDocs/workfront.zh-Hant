---
product-area: workfront-integrations
navigation-topic: workfront-for-outlook
title: 適用於Outlook的 [!DNL Workfront] 許可權層級
description: ' [!DNL Workfront for Outlook] 增益集需要讀取/寫入信箱存取權。  [!DNL Workfront for Outlook] 整合需要最高層級的許可權，因為它具有從Outlook Exchange伺服器下載電子郵件附件，並在使用者從具有附件的電子郵件提交請求時將其上傳到 [!DNL Workfront]的功能。'
author: Becky
feature: Workfront Integrations and Apps
exl-id: 704da044-21ed-4ca1-be6f-0e0aa832e069
source-git-commit: 793c8c940c8cb7ac53169edf21ddf28af2554120
workflow-type: tm+mt
source-wordcount: '486'
ht-degree: 0%

---

# [!DNL Workfront for Outlook]的許可權層級

>[!IMPORTANT]
>
>[Microsoft已停用對舊版Exchange Online權杖](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens)的支援，這些權杖是由Workfront Outlook增益集用於驗證。 Microsoft的這項變更會分階段推出，並於2025年10月1日完成。
>
>**由於Microsoft已停用這些權杖，適用於Microsoft Outlook整合的Workfront已停止運作。**

[!DNL Workfront for Outlook]需要[!DNL Outlook]增益集所允許之四個許可權等級中的最高者。

如需[!DNL Outlook]增益集許可權的相關詳細資訊，請參閱[檔案中的 [!DNL Outlook] ](https://docs.microsoft.com/en-us/office/dev/add-ins/outlook/privacy-and-security)增益集的隱私、許可權和安全性[!DNL Microsoft]。

[!DNL Workfront for Outlook]增益集需要讀取/寫入信箱存取權(`ReadWriteMailbox`)，這是最高的許可權範圍。
[!DNL Workfront for Outlook]整合需要最高層級的許可權，因為它具有從[!DNL Outlook] Exchange伺服器下載電子郵件附件，並在使用者從具有附件的電子郵件提交請求時將其上傳到[!DNL Workfront]的功能。 為了讓此功能運作，[!DNL Workfront for Outlook]會使用來自`mailbox.getCallbackTokenAsync()`增益集JavaScript API的功能[!DNL Office]來取得Token，並使用該功能從Exchange伺服器下載電子郵件附件。 唯一允許使用該函式的許可權是`ReadWriteMailbox`。 如需詳細資訊，請參閱Microsoft檔案中的[Outlook增益集的隱私、許可權和安全性](https://docs.microsoft.com/en-us/office/dev/add-ins/outlook/privacy-and-security)。

[!DNL Workfront for Outlook]增益集也需要`ReadWriteItem`許可權（包含在`ReadWriteMailbox`中），此許可權用於讀取電子郵件內文及讀取/更新電子郵件中繼資料：

* 讀取電子郵件內文：

  當使用者提交要求或傳送電子郵件內文作為[!DNL Workfront for Outlook]物件的更新時，[!DNL Adobe Workfront]會讀取電子郵件內文。
* 讀取/更新電子郵件中繼資料：

  當使用者提交電子郵件中的請求時，[!DNL Workfront for Outlook]會更新電子郵件標題。 這麼做是為了儲存已提交[!DNL Adobe Workfront]物件的相關資訊，所以下次使用者為同一封電子郵件開啟增益集時，會顯示該電子郵件中先前動作的相關資訊。

[!DNL Workfront for Outlook]只有在使用者在附加元件內執行動作時，才會存取使用者的信箱。 它沒有任何背景功能。 適用於Outlook的Workfront僅在下列情況下存取使用者的信箱：

* 使用者嘗試從[!DNL Workfront for Outlook]提交請求、建立任務或傳送電子郵件作為更新（開啟增益集並選取動作）
   * [!DNL Workfront for Outlook]讀取要填入增益集內表單的電子郵件內文。
   * [!DNL Workfront for Outlook]會讀取電子郵件中繼資料，以在增益集上顯示增益集中使用相同電子郵件完成之先前動作的相關資訊。
* 當使用者提交請求、建立任務或從[!DNL Workfront for Outlook]傳送電子郵件作為更新時（按一下增益集上的[!UICONTROL 提交]按鈕）：
   * [!DNL Workfront for Outlook]會讀取電子郵件內文，以要求說明或註解的形式傳送給Workfront。
   * [!DNL Workfront for Outlook]會更新電子郵件中繼資料，以儲存有關已提交請求或已更新物件的資訊。
   * [!DNL Workfront for Outlook]會從exchange伺服器下載電子郵件附件，以上傳至已提交的請求、已建立的任務或已更新的物件。
