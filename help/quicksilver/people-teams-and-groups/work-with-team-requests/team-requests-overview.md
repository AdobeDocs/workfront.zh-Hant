---
content-type: reference
product-area: user-management;agile-and-teams
navigation-topic: people-teams-and-groups
title: 團隊請求概觀
description: 團隊請求位於「主菜單」的「團隊」區域。
author: Lisa
feature: People Teams and Groups
exl-id: c131c021-8bc0-4a48-a873-9ee0e189bcab
source-git-commit: 9693ac3792fec3eca6218a228f2067519ed433ac
workflow-type: tm+mt
source-wordcount: '469'
ht-degree: 0%

---

# 團隊請求概觀

## 了解團隊請求

在 [!UICONTROL 團隊] 區域 [!UICONTROL 主菜單]. 按一下 [!UICONTROL 團隊請求] 圖示 ![請求圖示](assets/request-icon.png) ，檢視團隊請求。

>[!NOTE]
>
>敏捷團隊沒有團隊請求。

此 [!UICONTROL 團隊請求] 頁簽顯示當前在下拉清單中選擇的團隊的等待分配請求。 括弧中的數字表示有多少項目可供使用。

團隊請求表示未分配給特定用戶的待定工作項。 而是指派給一個團隊，該團隊的任何成員都可以自願承擔項目的責任。 如果用戶自願處理團隊請求，則用戶將接受工作分配作為自己。 除了團隊之外，還將任務分配給各個用戶。

>[!NOTE]
>
>不應將團隊請求用於協作任務分配。 如果您需要指派多個使用者以共同處理任務，請透過 [!UICONTROL 高級分配] 而非透過團隊要求。 如需詳細資訊，請參閱 [建立高級分配](../../manage-work/tasks/assign-tasks/create-advanced-assignments.md).

## 了解 [!UICONTROL 準備開始] 和 [!UICONTROL 全部] 選項

「團隊請求」區段頂端有兩個選項： [!UICONTROL 準備開始] 和 [!UICONTROL 全部].

此 [!UICONTROL 準備開始] 選項僅顯示符合下列所有條件的任務和問題：

* 所有前置任務都滿足其前置任務依賴類型的條件。\
   例如，如果前置關係的類型為 [!UICONTROL 完成開始] （前置任務必須在從屬任務開始之前完成），前置任務必須標籤為 [!UICONTROL 完成]. (如需先前相依性類型的詳細資訊，請參閱 [任務相關性類型概述](../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).)

* 登入的使用者是指派給這些工作和問題（針對工作請求）的人員，或指派給所選團隊給這些工作和問題（針對團隊請求）。
* 項目狀態為 [!UICONTROL 目前].
* 此 [!UICONTROL 預計開始日期] 或 [!UICONTROL 計劃開始日期] 已過，或已排程在今天日期後兩週內開始（或否） [!UICONTROL 預計開始日期] 或 [!UICONTROL 計劃開始日期] 已定義)。
* 此 [!UICONTROL 移交日期] 已發生或將在目前日期後兩週內發生。

>[!NOTE]
>
>如果任務滿足前三個標準，並且在當前日期後的兩週內有切換日期，則該任務將顯示為 [!UICONTROL 準備開始] 即使計畫/預計日期比兩週更遠。 如果任務沒有切換日期，則計畫/預計日期必須在當前日期後的兩週內。

此 [!UICONTROL 全部] 選項顯示分配給登錄用戶的當前項目上的所有任務和問題，或分配給團隊的所有任務或問題。
