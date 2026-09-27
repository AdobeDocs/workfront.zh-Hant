---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: 疑難排解Adobe Experience Manager整合
description: 問題： Assets未儲存至Adobe Experience Manager
author: Becky
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: f7e31e20-01e3-462d-9020-005e155f0259
TQID: 'https://experienceleague.adobe.com/VaiQnZXQe39sYlnJOblWoea9UwOaujEU3ME-jh7-0EI'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
    internal-label: Integrations
  - id: a1f87682-0525-5459-aa06-3560bb4c3b2a
    internal-label: Workfront Integrations and Apps
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
    internal-label: Resource management
subfeature_v2:
  - id: b70a979b-965d-47a9-a360-e7ec2a19b8c1
    internal-label: Digital content and documents
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 4c642a8ef31f3b9a03288f2d74e704be6ee86c55
workflow-type: tm+mt
source-wordcount: '247'
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
