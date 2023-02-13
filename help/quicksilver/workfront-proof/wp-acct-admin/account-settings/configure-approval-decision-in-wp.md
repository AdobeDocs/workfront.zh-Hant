---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: account-settings-workfront-proof
title: 在 [!DNL Workfront Proof]
description: As a [!DNL Workfront Proof] 管理員使用「選擇」或「特優」版本計畫，您可以通過以下方式配置由 [!DNL Workfront Proof] 組織中的使用者 — 編輯我。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 9e1c2a4e-0641-4334-8ff9-dbb203ccbc82
source-git-commit: a6cd3fe793c197308105da27369191d84cb59377
workflow-type: tm+mt
source-wordcount: '624'
ht-degree: 0%

---

# 在 [!DNL Workfront Proof]

>[!IMPORTANT]
>
>本文說明獨立產品中的功能 [!DNL Workfront Proof]. 有關內部校對的資訊 [!DNL Adobe Workfront]，請參閱 [校對](../../../review-and-approve-work/proofing/proofing.md).

As a [!DNL Workfront Proof] 管理員使用「選擇」或「特優」版本計畫，您可以通過以下方式配置由 [!DNL Workfront Proof] 組織中的使用者：

* 更改決策的名稱
* 變更校對檢視器中顯示的決策順序
* 決定應顯示哪些決策

本文說明下列內容：

## 配置決策設定

1. 按一下 **[!UICONTROL 帳戶設定]**.
1. 開啟 **[!UICONTROL 決策]** 標籤。
1. 進行下列任一變更：

   * 要隱藏決策，請按一下 **[!UICONTROL 隱藏]** 你不需要的決定權。
   * 要更名決策，請按一下決策名稱，對其進行編輯，然後按一下框外的（或按Enter）。 [!DNL Workfront Proof] 更新系統中所有現有校樣的決策名稱。

      >[!IMPORTANT]
      >
      >重新命名決策時，請保留該邏輯。 例如，預設決定「已拒絕」可更改為「需要新版本」，但不應更改為「發送到打印機」)。

      如果您想回到 [!DNL Workfront Proof] 預設值，您可以按一下「還原預設決策」 。

>[!NOTE]
>
>* 如果有多個不同層級的決策，則決策背後的邏輯用於計算證明工作流程的整體狀態。
>* 「已核准」和「已核准且變更」決策會觸發自動工作流程的下一個階段。
>* 如果您重新命名決策，並想驗證邏輯，可以按一下 **[!UICONTROL 活動]** 在左側導覽面板中，檢查您的活動記錄，原始決策會以方括弧顯示。
>
>  ![2016-12-20_1921.png](assets/2016-12-20-1921-350x132.png)>

## 建立決策原因

決策原因是擷取關於證明的其他決策資訊的好方法。

1. 按一下 **[!UICONTROL 設定]** > **[!UICONTROL 帳戶設定]**.

1. 開啟 **[!UICONTROL 決策]** 標籤。
依預設，所有決策者都可依據您的證明找到原因，但您只能將原因限制在主要決策者。
您可以根據您的需求，允許選取多個原因，或將其設為單一選擇清單。 您也可以將理由設為必要理由，這表示審核者必須先挑選理由，才能獲准保存對證明的決定。
   ![Reacons_setup.png](assets/reasons-setup-350x121.png)

1. 在 **[!UICONTROL 原因]** ，按一下 **[!UICONTROL 新原因]**.
   ![New_reason.png](assets/new-reason-350x135.png)

1. 在顯示於下方的方塊中，輸入原因區段的標題 **[!UICONTROL 原因]**.
1. 如果要包括文本框，請選擇 **[!UICONTROL 包含文字方塊]**.
1. 按一下&#x200B;**[!UICONTROL 儲存]**。
   ![reacons_setup_2.png](assets/reasons-setup-2-350x146.png)
最重要的步驟是選取應顯示原因的決策。 如果您忘記這麼做，校樣上不會顯示原因。

1. 核取 **[!UICONTROL 顯示原因]** 欄。 您可以根據自己的原因選取一或多個決策。
   ![reacouns_-_decision_selection.png](assets/reasons---decision-selection-350x150.png)

## 建立貼文決策訊息

您可以建立貼文決策訊息，在審核者儲存其對校樣的決策後顯示。

1. 按一下 **[!UICONTROL 設定]** > **[!UICONTROL 帳戶設定]**.

1. 開啟 **[!UICONTROL 決策]** 標籤。
1. 在 **[!UICONTROL 貼文決策訊息]** ，按一下 **[!UICONTROL 編輯]** 在 **[!UICONTROL 訊息]** 行。
您也可以決定是否要向所有決策者顯示該消息，或者是否將其限制為主要決策者。
   ![post_decision_message_set_up.png](assets/post-decision-message-set-up-350x125.png)

1. 在 **[!UICONTROL 顯示訊息]** 欄，指定此訊息應顯示的決策。
如果您未選取至少一個決策，訊息將不會顯示在您的校樣上。 請務必勾選此欄中至少一個方塊。
   ![post_decision_message_set_up_2.png](assets/post-decision-message-set-up-2-350x151.png)
