---
title: 使用工作代理
content-type: reference
description: 瞭解如何使用工作代理程式、可指派給Workfront任務的AI共同作業人員。
author: Becky
feature: Work Management, Tasks
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
    internal-label: Work management
subfeature_v2:
  - id: b91c0848-76c4-4da4-8b81-3aade0518dd0
    internal-label: Tasks
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
source-git-commit: bc354886dc8c2f1dae24513f1d74e800e19fb3ab
workflow-type: tm+mt
source-wordcount: '1025'
ht-degree: 1%
---
# 使用工作代理

工作代理是可直接指派給Workfront任務的AI共同作業人員，除了現有的AI檢閱者用於檔案和資產檢閱外。 就像其他AI共同作業人員一樣，工作代理會在「設定」區域中設定，並像使用者一樣指派給任務。

工作代理會連線到您在Copilot Studio、Claude或Writer中設定的代理。

如需有關在Workfront中建立工作代理程式的資訊和指示，請參閱設定AI共同作業人員一文中的[設定工作代理程式](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md#configure-a-work-agent)。

## 存取權要求

+++ 展開以檢視這篇文章中所述功能的存取權要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] 封裝</td> 
   <td><p>選取、Prime或Ultimate</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] 授權</td> 
   <td><p>[！UICONTROL標準]</p>
  </tr> 
  <tr> 
   <td>存取層級設定</td> 
   <td>[！UICONTROL系統管理員]</td> 
  </tr> 
  </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先決條件

* 您必須先在Copilot、Claude或Writer.ai中設定代理程式，才能將其用作「工作代理程式」。

## 工作代理程式概述

工作代理是將MCP代理指派給Workfront中特定工作的方法。 您可以在Copilot Studio、Claude或Writer.ai等應用程式中設定代理程式，然後將該代理程式以工作代理程式身分連線至Workfront。 然後，您可以像指派使用者一樣將其指派給任務。

某些範例工作流程可能包括：

* 偵測已上傳至任務的影像、根據提供給代理程式的條件產生變數，並將新影像上傳至任務。
* 從工作說明產生復本、根據代理程式中設定的准則複查復本，並將復本張貼至更新流。
* 讀取事件的詳細資料、識別遺漏的詳細資料，以及在更新流中發佈有關遺漏詳細資料的問題。

>[!NOTE]
>
>* 有關代理程式職責和能力的特定詳細資訊是在建立代理程式的應用程式中設定，而不是在Workfront中設定。
>* Workfront MCP伺服器不需要新增至作為工作代理程式的代理程式，也不需要連線工作代理程式才能運作。
>* 工作代理目前支援在Copilot Studio、Claude和Writer.ai中建立的代理。
>* 在Copilot Studio中設定代理程式時，您必須將安全性設定為&#x200B;**無驗證**。
>* 如需有關在Workfront中建立工作代理程式的資訊和指示，請參閱設定AI共同作業人員一文中的[設定工作代理程式](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md#configure-a-work-agent)。

## 工作代理程式讀取的資訊

當「工作代理程式」開始處理任務時，會自動讀取下列任務資訊作為前後關聯：

* 任務標題
* 任務說明
* 任務更新流中的註解
* 附加到任務的任何自訂表單中的資訊

此資訊一律會讀取且無法設定為Workfront設定。

>[!TIP]
>
>為獲得最佳結果，我們建議：
>
>* 包括您希望代理程式直接在任務說明或相關自訂表格欄位中使用的任何背景資訊。
>* 確定任務符合指示代理程式執行的操作。 例如，如果指示您的代理將文字從英文翻譯成法文，請在工作說明中加入您要翻譯的文字。

## 工作代理程式啟動觸發程式

當工作代理程式被指派給任務時，它會在滿足以下任何情況時開始工作：

* 「工作代理程式」已指派給準備開始的任務。 （例如，如果任務具有前置任務，則前置任務為完成。）
* 工作代理程式和使用者會指派給任務，而工作代理程式會先指派。
* 工作代理已被指派為已準備好開始的工作，且工作代理是唯一的或主要受指派人。 （例如，如果任務具有前置任務，則前置任務為完成。）
* 工作代理程式和使用者已被指派的任務已準備好開始，且工作代理程式已先指派或為主要受指派人。 （例如，如果任務具有前置任務，則前置任務為完成。）
* 將使用者與工作代理指派給任務，並移除使用者。
* 使用者和「工作代理程式」被指派給任務，而「工作代理程式」被設定為任務的「主要受指派人」。

下列情況不會導致Work Agent開始處理工作：

* 「工作代理程式」會指派給已指派使用者的任務。
* 工作代理程式@mentioned在任務中。
* 「工作代理程式」會指派給已指派「工作代理程式」的工作。 在這種情況下，指派的第一個工作代理程式將已開始工作，而第二個工作代理程式將不會執行任何動作。
* 「工作代理程式」被指派給未準備好開始的任務。 （例如，如果任務具有前置任務，則前置任務尚未完成。）

## 將工作代理指派至任務

工作代理的指派方式與使用者的指派方式相同。

當您在可用受指派人清單中搜尋「工作代理程式」時，「工作代理程式」的名稱僅為名字。

如需指示，請參閱[指派工作](/help/quicksilver/manage-work/tasks/assign-tasks/assign-tasks.md)。

>[!NOTE]
>
>無法指派工作代理以檢閱或核准檔案。

## 疑難排解工作代理

如果您的工作代理程式未傳回回應或輸出，請檢查下列專案：

* 請確定您的代理程式已發佈在AI平台提供者端。
* 請確定您有足夠的代理程式平台的AI積分。
* 確定對任務採取的操作不需要特定的存取層級。
* 如果您使用Copilot作為代理程式提供者，請確定您使用的是「無驗證」設定。
* 如果您使用Copilot，請確定您的代理程式已設定在全球環境中。 Work Agent功能目前不支援Copilot Studio的區域版本。
* 請確定共同作業人員是任務的主要受指派人。
* 請確定工作代理程式所指派的任務可以開始。 例如，檢查該任務的所有前置任務是否已完成。

>[!TIP]
>
>您也可以前往代理程式提供者平台，要求代理程式在平台內執行工作。 如果代理程式無法在平台內執行工作，則工作代理程式在Workfront中也會遇到問題。
