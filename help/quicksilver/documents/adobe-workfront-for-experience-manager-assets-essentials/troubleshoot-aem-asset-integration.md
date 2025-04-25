---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: 疑難排解Adobe Experience Manager整合
description: 問題： Assets未儲存至Adobe Experience Manager
author: Becky
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: f7e31e20-01e3-462d-9020-005e155f0259
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '231'
ht-degree: 0%

---

# 疑難排解Adobe Experience Manager整合

## 問題： Assets未儲存至Adobe Experience Manager

當使用者選擇要匯出到Experience Manager Assets的資產或資料夾並按一下選取，選擇器視窗會關閉，但資產未儲存到Experience Manager Assets。 Workfront中沒有顯示資產未儲存至Experience Manager Assets。

### 原因

由於Adobe Cloud Manager中的允許清單，因此可能會發生這種情況。 如果組織的Adobe Cloud Manager允許清單為空，則IP位址不受限制，且Workfront可以存取組織在Adobe Experience Manager中的資料夾和資產。 但是，如果即使將單一IP位址新增到Cloud Manager允許清單，允許清單會假設不允許清單上沒有的任何IP位址。 因此，如果Cloud Manager允許清單包含任何IP位址，也必須將Workfront IP位址新增至允許清單，才能讓Workfront將資產傳送至Experience Manager Assets。

### 解決方案：

將Workfront IP位址新增至Adobe Cloud Manager允許清單。

* 如需將IP位址新增至Adobe Cloud Manager的說明，請參閱Adobe Experience Manager檔案中的[IP允許清單簡介](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/implementing/using-cloud-manager/ip-allow-lists/introduction)。
* 如需新增至允許清單的Workfront IP位址清單，請參閱[設定防火牆](/help/quicksilver/administration-and-setup/get-started-wf-administration/configure-your-firewall.md)。
