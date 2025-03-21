---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data connect
title: Tableau案頭無法建立連線
description: 當您嘗試將Tableau案頭連線到Data Connect時，您會收到錯誤。
author: Courtney
feature: Reports and Dashboards
source-git-commit: e8b1d553ac4761e2b6eae79ae384956105939d90
workflow-type: tm+mt
source-wordcount: '252'
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

* **因應措施選項**：從工作表熒幕(而非Tableau中的Data Source窗格)建立擷取。 連線沒有遺失，擷取程式也已完成。

