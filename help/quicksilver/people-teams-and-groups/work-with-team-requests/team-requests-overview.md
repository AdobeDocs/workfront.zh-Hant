---
content-type: reference
product-area: user-management;agile-and-teams
navigation-topic: people-teams-and-groups
title: 團隊請求概觀
description: 團隊請求可在主功能表的團隊區域中找到。
author: Jenny
feature: People Teams and Groups
exl-id: c131c021-8bc0-4a48-a873-9ee0e189bcab
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '469'
ht-degree: 0%

---

# 團隊請求概觀

## 瞭解團隊請求

在[!UICONTROL 主要功能表]的[!UICONTROL 團隊]區域找到團隊請求。 按一下左側面板中的[!UICONTROL 團隊請求]圖示![請求圖示](assets/request-icon.png)以檢視團隊請求。

>[!NOTE]
>
>敏捷團隊沒有團隊請求。

[!UICONTROL 團隊要求]索引標籤會顯示目前於下拉式清單中選取之團隊等待指派的要求。 括弧內的數字表示有多少專案已準備好處理。

團隊請求代表未指派給特定使用者的擱置工作專案。 而是將其指派給一個團隊，該團隊的任何成員都可以自願接受對該專案的責任。 如果使用者自願處理團隊請求，則使用者將接受工作指派作為其自己的工作指派。 除了專案團隊外，任務還會指派給個別使用者。

>[!NOTE]
>
>團隊請求不應用於合作任務指派。 如果您需要指派多位使用者一起處理一項任務，請透過[!UICONTROL 進階工作分派]而不是透過團隊請求來執行此操作。 如需詳細資訊，請參閱[建立進階工作分派](../../manage-work/tasks/assign-tasks/create-advanced-assignments.md)。

## 瞭解[!UICONTROL 準備開始]和[!UICONTROL 全部]選項

團隊請求區段頂端有兩個選項： [!UICONTROL 準備開始]和[!UICONTROL 全部]。

[!UICONTROL 準備開始]選項只會顯示符合以下所有條件的任務和問題：

* 所有前置任務均已符合其前置任務相依性型別的條件。\
  例如，如果前置任務關係的型別是[!UICONTROL 完成 — 開始] （前置任務必須先完成，相依任務才能開始），前置任務必須標籤為[!UICONTROL 完成]。 （如需前置任務相依性型別的詳細資訊，請參閱[任務相依性型別概觀](../../manage-work/tasks/use-prdcssrs/task-dependency-types.md)。）

* 登入使用者是指派給這些任務和問題（針對工作請求）的人員，或所選團隊指派給這些任務和問題（針對團隊請求）。
* 專案狀態為[!UICONTROL 目前]。
* [!UICONTROL 預計開始日期]或[!UICONTROL 計劃開始日期]已經過或排程在今天日期後的兩週內開始（或尚未定義[!UICONTROL 預計開始日期]或[!UICONTROL 計劃開始日期]）。
* [!UICONTROL 移交日期]已經發生，或將在目前日期後的兩週內發生。

>[!NOTE]
>
>如果任務符合前三個條件並在目前日期後兩週內有移交日期，則即使計畫/預計日期超過兩週，也會顯示為[!UICONTROL 準備開始]。 如果任務沒有移交日期，則計畫/預計日期必須在目前日期的兩週內。

[!UICONTROL 全部]選項會顯示目前專案上指派給登入使用者的所有任務和問題，或指派給團隊的所有任務或問題。
