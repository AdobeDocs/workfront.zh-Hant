---
content-type: tips-tricks-troubleshooting
product-previous: workfront-proof
product-area: documents;system-administration;user-management
navigation-topic: tips-tricks-and-troubleshooting-workfront-proof-users-and-contacts
title: 大量編輯使用者的其他群組
description: 當大量編輯時，我嘗試將單一其他群組新增到許多使用者。 儲存變更後，會移除所有現有的其他群組，而只保留新的其他群組。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: f2402830-3263-4204-ba8a-9028ef937577
source-git-commit: 1a85f2a214036b62d13cb01f0b7a77392648a5fd
workflow-type: tm+mt
source-wordcount: '187'
ht-degree: 0%

---

# 大量編輯使用者的其他群組

>[!IMPORTANT]
>
>本文提及獨立產品[!DNL Workfront Proof]中的功能。 有關[!DNL Adobe Workfront]內部校訂的資訊，請參閱[校訂](../../../review-and-approve-work/proofing/proofing.md)。

## 問題：

當大量編輯時，我嘗試將單一其他群組新增到許多使用者。
儲存變更後，會移除所有現有的其他群組，而只保留新的其他群組。

## 回答：

產生的行為取決於所選使用者目前的群組成員資格：

* 如果所有選取的使用者「其他群組」成員資格完全相符……
在您選取使用者並選取[!UICONTROL 編輯]後，[!UICONTROL 其他群組]欄位將會顯示完整清單
這些使用者所屬的所有群組。

* 如果選取的使用者擁有不同的「其他群組」成員資格……
在您選取使用者並按一下[編輯] 之後，[!UICONTROL [其他群組] ]欄位將會空白。

當您按一下&#x200B;**[!UICONTROL 儲存變更]**&#x200B;時，其他群組欄位中顯示的內容都會儲存。

欄位先前的內容會被覆寫。
