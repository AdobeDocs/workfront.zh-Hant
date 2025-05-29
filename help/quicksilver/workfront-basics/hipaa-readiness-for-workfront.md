---
content-type: reference
navigation-topic: get-started-with-workfront
title: Workfront的HIPAA整備
description: Workfront如HIPAA所定義，若客戶為Business Associate及/或Covered Entity (Business Associate代表其提供Adobe Workfront)，應使用下列指引設定Workfront以供HIPAA使用。
feature: Get Started with Workfront
author: Courtney
hide: true
hidefromtoc: true
source-git-commit: a984038eea41d249cb0ad0d2ec6ba47025c56a65
workflow-type: tm+mt
source-wordcount: '473'
ht-degree: 0%

---


# Workfront的HIPAA整備

Workfront如HIPAA所定義，若客戶為Business Associate及/或Covered Entity (Business Associate代表其提供Adobe Workfront)，應使用下列准則來設定Workfront以供HIPAA使用：


## 密碼需求

| **安全性設定** | **這是什麼？** | **需求** |
|----------------------|------------------|------------------|
| 協定的最小密碼強度 | 合約密碼的最低強度為何？ | 不少於8個字元 |
| 使用者密碼的最小密碼強度 | 使用者密碼的最低強度為何？ | 來自下列三個類別的字元：<br>*大寫字母（拉丁字母）<br>*小寫字母（拉丁字母）<br>*以10位數字為底<br>*非字母數字字元 |
| 密碼持續時間 | 密碼應該保留多久不變？ | 密碼應至少每90天變更一次 |
| 密碼歷程記錄 | 應該記住和禁止使用多少個過去的密碼？ | 不少於5個 |


## 登入要求

| **安全性設定** | **這是什麼？** | **需求** |
|----------------------|------------------|------------------|
| 登入失敗次數上限 | 有多少次失敗的登入嘗試造成使用者被鎖定？ | 在5分鐘期間內不超過5次嘗試；30分鐘後允許重試 |
| 最大SSO驗證失敗數 | 有多少失敗的SSO驗證嘗試會造成鎖定？ | 不超過5個（僅適用於使用SSO的客戶） |


## 工作階段需求

| **安全性設定** | **這是什麼？** | **需求** |
|----------------------|------------------|------------------|
| 工作階段逾時 | 閒置數分鐘導致登出？ | 不超過15分鐘 |

## 客戶責任

確保所有員工、代表及/或代理人都瞭解並瞭解各方所簽署之授權及/或服務協定（視適用情況而定）中與Workfront資料使用相關的條款。

特別是，應檢閱並傳達下列責任和義務： 

* 客戶需負責其所有使用者使用Workfront服務。 

* 客戶必須遵守其與Adobe合約的所有條款，包括禁止將資料元素上傳至Workfront的條款。 

* 任何敏感資料，包括但不限於ePHI，均由客戶自行承擔上傳風險。  客戶必須隨時負責所有客戶資料。 


## 資料保護與法規遵循

>[!IMPORTANT]
>
>Workfront並非設計作為電子健康記錄(EHR)的存放庫。 只有在Adobe明確授權書面內容時，才能處理ePHI。 

* 對於任何可以存取ePHI的Workfront資料庫，請確定已啟用&#x200B;**靜態加密(EAR)**。
   * 請聯絡您的客戶經理(AE)，確認您的Workfront購買包含EAR。
   * 設定可透過Workfront存取的系統/資料庫，以符合法規遵循義務。
* 確保ePHI未進行傳輸、連結或與其他Adobe解決方案共用。
* 確保透過Workfront處理的患者照片能夠安全地儲存，並且不會公開存取。