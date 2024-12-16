---
user-type: administrator
content-type: overview;how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: 環境提升疑難排解
description: 疑難排解環境升級的常見問題。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 830dd573-d954-4ba2-a1d3-d1645b3fbac8
source-git-commit: c3c9a423bd60b26b2605a1b52bd706c9bc6acdec
workflow-type: tm+mt
source-wordcount: '328'
ht-degree: 0%

---

# 環境提升疑難排解

本文介紹如何疑難排解環境升級。

## 問題：環境升級套件延遲或失敗

如果您的環境升級套件發生延遲或失敗，請嘗試下列步驟：

* 如果封裝安裝在10-15分鐘後停止，或封裝安裝失敗，請重新組裝現有封裝或建立新封裝。

* 如果封裝安裝失敗，則可能有一或多個物件有問題。 檢查錯誤訊息，其可識別物件並可協助識別問題。 解決物件的問題後，請重新組裝套件並重新嘗試安裝。

* 如果您仍然遇到安裝問題，請嘗試在不同的目標環境中複製安裝。 儘可能接近原始安裝，包括選取的物件和安裝動作。

* 我們建議您在組裝封裝後，一律檢查封裝內容，以確認它包含您期望的物件。


## 問題：自訂表單無法提升

發生此狀況是因為自訂表單包含計算欄位。 如果計算欄位參照的欄位未在自訂表單中參照，則包含此表單的套件不會提升，且使用者可能會看到以下訊息：

「下列欄位無效：無效的自訂運算式無效運算式：無效的自訂運算式。」

當參照未附加至目標環境中任何自訂表單的現有欄位或新建立的欄位時，可能會出現此問題。

若要解決此問題，請執行下列任一項作業：

* 使用包含參考欄位的專案型別自訂表單建立套件。 將此套件升級至目標環境後，請升級包含計算欄位的原始預期套件。
* 在目標環境中手動建立引用的欄位，並將其與專案型別的自訂表單相關聯。 完成此操作後，將會識別欄位，並且您可以在不會遇到錯誤的情況下升級套件。
