---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: 疑難排解Adobe Experience Manager整合
description: 「問題：資產未儲存至Adobe Experience Manager」
author: Becky
feature: Digital Content and Documents, Workfront Integrations and Apps
source-git-commit: a73ebfe8c735eb9e103b01a201a8f71d6ab7bda2
workflow-type: tm+mt
source-wordcount: '241'
ht-degree: 0%

---

# 疑難排解Adobe Experience Manager整合

## 問題：資產未儲存至Adobe Experience Manager

當使用者選擇要匯出到Experience Manager Assets的資產或資料夾並按一下選取，選擇器視窗會關閉，但資產未儲存到Experience Manager Assets。 Workfront中沒有顯示資產未儲存至Experience Manager Assets。

### 原因

由於Adobe Cloud Manager中的允許清單，可能會發生這種情況。 如果組織的AdobeCloud Manager允許清單為空，則IP位址不受限制，並且Workfront可以存取組織在Adobe Experience Manager中的資料夾和資產。 但是，如果即使將單一IP位址新增到Cloud Manager允許清單，允許清單會假設不允許清單上沒有的任何IP位址。 因此，如果Cloud Manager允許清單包括任何IP位址，也必須將Workfront IP位址新增到允許清單，以啟用Workfront將資產傳送到Experience Manager Assets。

### 解決方案：

將Workfront IP位址新增至Adobe Cloud Manager允許清單。

* 如需將IP位址新增到您的AdobeCloud Manager的說明，請參閱 [IP允許清單簡介](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/implementing/using-cloud-manager/ip-allow-lists/introduction.html?lang=en) (位於Adobe Experience Manager檔案中)。
* 如需新增至允許清單的Workfront IP位址清單，請參閱 [設定防火牆](/help/quicksilver/administration-and-setup/get-started-wf-administration/configure-your-firewall.md).


