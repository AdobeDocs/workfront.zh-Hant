---
title: AI助理總覽
content-type: reference
description: AI助理總覽
author: Becky
feature: Get Started with Workfront
exl-id: e5f2408b-2c29-4257-8bdc-bf20880de265
source-git-commit: b00032517f2bf048c50fbaf22b79c011017980ea
workflow-type: tm+mt
source-wordcount: '701'
ht-degree: 1%

---

# AI助理總覽

Workfront的AI助理可在自然語言對話中提供應用程式內資訊和建議，協助您完成工作。 AI助理可以透過以下方式為您提供更流暢的工作體驗

* 摘要工作專案或檔案
* 搜尋工作處理的指示或參考原物料
* 產生或檢查計算欄位的公式

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td><p>新增：任何</p>
       <p>或</p>
       <p>目前：無法使用</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td><p>新增：標準</p>
       <p>或</p>
       <p>目前：無法使用</p></td>
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

## AI助理的必要條件

若要為您的組織啟用AI助理，必須套用下列&#x200B;**所有**：

* 貴組織必須已移轉至Adobe IMS (Identity Management系統)
* 必須啟用Adobe統一體驗
* 貴組織必須有Select、Prime或Ultimate Workfront計畫
* Adobe必須有已簽署的檔案AdobeGen AI合約

  如需簽署合約的詳細資訊，請參閱本文中的[簽署AdobeGen AI合約](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement)。

## AI助理的考量事項

* AI助理對於您已開啟的頁面而言是前後關聯感應式的。 例如，在專案頁面的AI助理中輸入「摘要此專案」會傳回該特定專案的摘要。
* Workfront管理員必須為貴組織中的使用者啟用AI助理。 AI助理是透過存取層級啟用。

  如需詳細資訊，請參閱[啟用或停用AI助理](/help/quicksilver/workfront-basics/ai-assistant/enable-or-disable-assistant.md)。

* Workfront Planning AI Assistant與Workfront AI Assistant的功能不同。

  如需Workfront規劃中AI助理的詳細資訊，請參閱[Adobe Workfront規劃AI助理概述](/help/quicksilver/planning/general/planning-ai-assistant-overview.md)。

* AI助理目前僅提供英文版。


## AI助理中可用的功能

AI助理目前提供下列功能：

* 摘要專案、任務、問題或檔案。

  如需詳細資訊，請參閱[使用AI助理摘要](/help/quicksilver/workfront-basics/ai-assistant/summarize-this.md)。

* 提供從Adobe Experience League上的Workfront檔案提取的指示或參考資訊。

  如需詳細資訊，請參閱[從AI助理取得說明](/help/quicksilver/workfront-basics/ai-assistant/use-ai-to-retrieve-instructions.md)。

* 在Workfront中尋找特定專案。

  如需詳細資訊，請參閱[使用AI助理來處理專案、任務和問題](/help/quicksilver/workfront-basics/ai-assistant/work-with-pti-through-ai-assisant.md)。

* 產生或修訂已計算自訂欄位的公式。

  >[!NOTE]
  >
  >此功能僅適用於Prime或Ultimate Workfront計畫上的組織。

  如需詳細資訊，請參閱[使用AI助理產生或修訂計算欄位公式](/help/quicksilver/workfront-basics/ai-assistant/use-ai-assistant-to-check-formulas.md)。

* 在以下時間範圍內概述專案的更新、上傳的檔案和其他顯著變更：優先順序中的24小時、3天、7天。

如需詳細資訊，請參閱[在優先順序](/help/quicksilver/workfront-basics/priorities/catch-me-up.md)中趕上工作。


## AI助理可用的物件型別

如果使用者在Workfront中擁有有效許可權，AI助理可以查詢與下列物件型別相關聯的資料：

* 專案組合
* 計劃
* 專案
* 任務
* 問題
* 自訂表單
* 使用者
* Workfront Planning記錄


## 存取AI助理

1. 在任何Workfront頁面頂端，按一下AI助理圖示![](/help/quicksilver/workfront-basics/ai-assistant/assets/ai-assistant-icon.png)。
1. 在熒幕右側的面板中輸入您的問題或提示。

   如果您無法在此面板中輸入，表示貴組織沒有已簽署的檔案AdobeGen AI合約。

1. 如果AI助理沒有提供您需要的答案，請調整您的提示，然後再試一次。

## 簽署AdobeGen AI合約

如果您的組織沒有已簽署的AdobeGen AI檔案協定，則無法為您的組織啟用AI助理。

如果使用者嘗試在AdobeGen AI協定尚未簽署時使用AI助理，他們會看到一則訊息：

* 使用者：使用者會收到未為其組織啟用AI助理的通知，得知他們可以聯絡Workfront管理員，為其組織請求該服務。
* 管理員：管理員會收到沒有已簽署AdobeGen AI合約的通知，並可要求傳送合約副本以供簽署。

若要請求AdobeGen AI合約：

1. 身為Workfront管理員，按一下AI助理圖示![](/help/quicksilver/workfront-basics/ai-assistant/assets/ai-assistant-icon.png)。
1. 開始在AI助理面板中輸入。
1. 當AdobeGen AI合約訊息出現時，請按一下&#x200B;**檢閱合約**。
1. 輸入貴組織將簽署AdobeGen AI合約之個人的名稱和電子郵件地址。

   合約將傳送給此人簽署。 簽署並傳回之後，就會為貴組織啟用AI小幫手。
