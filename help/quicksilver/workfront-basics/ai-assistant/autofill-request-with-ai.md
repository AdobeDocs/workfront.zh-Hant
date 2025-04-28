---
title: 使用AI自動填寫請求
content-type: reference
description: 您可以使用AI自動填寫請求欄位。
author: Becky
feature: Get Started with Workfront
hide: true
hidefromtoc: true
source-git-commit: 9e1a5718092092bb9ca98cf92ddd2a1a07f32f51
workflow-type: tm+mt
source-wordcount: '443'
ht-degree: 0%

---

# 使用AI自動填寫請求

AI可協助您自動填寫請求欄位。 它可以根據先前的請求建議欄位值，或從文字（例如電子郵件）剖析欄位值。

您可以在提交請求之前核准或拒絕這些提交。

自動填寫不會覆寫您已填寫的任何欄位。

## 填寫表單時取得建議

自動填寫可在您填寫表單時建議欄位值。 當您在請求欄位中輸入值時，Workfront會將這些值與先前的請求進行比較。 如果輸入的值與先前請求中類似內容中的其他欄位值緊密相關，Workfront會建議這些值。

例如，如果診所一律使用相同的計費代碼，Workfront會在輸入診所名稱時，建議在適當的欄位中輸入計費代碼。

若要根據先前的請求使用建議：

1. 開始建立請求。

   如需指示，請參閱[建立及提交要求](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md)。

1. 開始填寫欄位。

   當您填寫欄位時，其他欄位可能會顯示建議。

1. 對於每個欄位建議，請在該欄位下方選取&#x200B;**接受**&#x200B;或&#x200B;**拒絕**。

   或

   在頁面頂端選取「**全部接受**」或「**全部拒絕**」以接受或拒絕所有建議。

## 從文字提示取得建議

自動填寫可根據文字（例如電子郵件）建議欄位值。 您貼入文字區塊，Workfront便已處理文字，根據文字建議欄位值。

例如，如果電子郵件包含「此到期日為6月1日」，而請求表單有到期日的欄位，則Workfront會建議該欄位值在6月1日。

此型別的建議也會檢查先前是否有類似內容的請求。 例如，如果提示指出請求是針對特定使用者端，Workfront可以根據先前的請求，自動尋找並輸入該使用者端的帳單地址。

您可以貼上文字以套用至整個表單或表單的單一區段。

若要根據貼上的文字提示使用建議：

1. 開始建立請求。

   如需指示，請參閱[建立及提交要求](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md)。

1. 若要將文字提示套用至整個表單，請按一下熒幕右上角的&#x200B;**使用AI自動填滿**。

   或

   若要套用單一區段的文字提示，請按一下區段名稱旁的AI圖示![AI圖示](assets/request-prompt-icon.png)。

1. 將文字貼到提示方塊中。
1. 按一下&#x200B;**填寫表單**。

   Workfront會產生表單的建議。
1. 對於每個欄位建議，請在該欄位下方選取&#x200B;**接受**&#x200B;或&#x200B;**拒絕**。

   或

   在頁面頂端選取「**全部接受**」或「**全部拒絕**」以接受或拒絕所有建議。

