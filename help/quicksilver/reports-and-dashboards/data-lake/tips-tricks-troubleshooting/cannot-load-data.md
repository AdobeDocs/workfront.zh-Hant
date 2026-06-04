---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data connect
title: Tableau案頭無法建立連線
description: 當您嘗試將Tableau案頭連線到Data Connect時，您會收到錯誤。
author: Courtney
feature: Reports and Dashboards
exl-id: 2a25d99a-a05e-4f60-ae1a-51ee137ad5f3
TQID: https://experienceleague.adobe.com/-V1TT-X0FjMm2PIKDy0JVFkvt-A-a7f8fRbVzGzy1jg
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: c1579802-ddd4-4214-8a91-97b2066abe11id: d095671a-1355-40aa-8b5f-06c33c68080b
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 253
ht-degree: 0%

---

# Tableau案頭無法建立連線

## 問題

當您嘗試將Tableau案頭連線到Data Connect時，您會看到以下錯誤：

`Cannot load data into PowerBI. Receiving an HY000 [Microsoft][Snowflake] (25) message`

## 原因

此錯誤是由本機電腦上的Proxy設定所造成，該設定會阻止從Data Connect載入資料。

Data Connect透過協力廠商Snowflake雲端服務提供。 Tableau需要開啟網路才能與Snowflake通訊。

## 解決方案

您可以嘗試下列步驟來解決此問題：

* **停用您的保全性工具以進行疑難排解**：請關閉您的保全性工具，例如Zscaler或Cisco，檢視它是否可解決連線問題。 如果這樣可解決連線問題，請確保您的安全工具已升級至最新版本，並與您的內部網路團隊將Data Connect (Snowflake) IP位址新增至VPN允許清單。

* **新增IP位址至允許清單**：請確定您的防火牆設定允許Data Connect使用的IP位址。 使用命令`SYSTEM$ALLOWLIST()`取得IP位址，然後您可以在VPN中將其列入允許清單。

* **檢查防火牆和Proxy設定**：檢查網路上的任何防火牆或Proxy設定是否封鎖對Snowflake端點的存取。 您可能需要連絡網路管理員，將必要的Snowflake IP位址和連線埠新增至貴公司的允許清單。

* **因應措施選項**：從工作表熒幕（而非Tableau中的Data Source窗格）建立擷取。 連線沒有遺失，擷取程式也已完成。
