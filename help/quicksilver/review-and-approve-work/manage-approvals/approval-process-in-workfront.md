---
content-type: overview
product-area: projects
navigation-topic: approvals
title: 核准流程概述
description: 您可以建立核准程式並將其附加至物件，以確保指定的使用者在物件執行前檢閱特定變更。
author: Courtney
feature: Work Management
exl-id: dd0822b6-80f1-4a2e-bf6a-0c425984f4d0
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '1747'
ht-degree: 0%

---

# 核准流程概述

您可以建立核准程式並將其附加至物件，以確保指定的使用者在物件執行前檢閱特定變更。

這適用於Adobe Workfront中的下列類型物件：

* 工作項（項目、任務或問題、模板、模板任務）
* 文件
* 校訂

如需建立核准程式的指示，請參閱 [建立工作項的審批流程](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

本文包含與工作項關聯的審批流程的一般資訊。

## 核准程式類型

如果您是Adobe Workfront管理員，或具有核准程式之管理存取權的使用者，您可以針對專案、任務和問題建立下列核准程式：

* **系統級全局批准流程**:使用者可將下列任一項附加：

   * 「核准」區段中的專案、任務或問題
   * 在「編輯項目」框中，「任務預設審批流程」區域
   * 在項目的「隊列詳細資訊」或「隊列主題」部分的「預設批准流程」區域中。 必須以請求佇列的形式啟用專案。

* **組級全局批准流程**:使用者可將下列項目附加至：

   * 屬於「批准」部分中與批准流程關聯的組的項目、任務或問題
   * 在「編輯項目」框中，屬於與審批流程關聯的組的項目的「任務預設審批流程」區域
   * 在項目的「隊列詳細資訊」或「隊列主題」部分的「預設批准流程」區域中。 項目必須作為請求隊列啟用，並且必須屬於與批准流程關聯的組。

   有關建立系統級或組級審批流程的資訊，請參閱 [建立工作項的審批流程](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

* **一次性使用的核准程式**:用於單個項目、任務、問題、模板或模板任務。 此類審批流程僅影響與其關聯的對象，不能與任何其他對象關聯。

   如需建立一次性核准程式的相關資訊，請參閱 [將新審批流程或現有審批流程與工作關聯](../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

>[!NOTE]
>
>本文使用「全域核准程式」一詞，來區分「單一使用核准程式」。 可重複使用全域核准程式。
>
>「組級全局審批流程」一詞是指可重複用於項目且狀態僅與特定組關聯的審批流程。

有關建立系統級審批流程或組級審批流程的資訊，請參閱 [建立工作項的審批流程](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

## 核准程式的考量事項

* 您必須先建立項目、任務、問題、模板或模板任務，然後審批流程才能與它們關聯。
* 核准程式一律與兩個基本項目相關聯：

   * 每個核准程式都對應至Workfront系統中的特定工作項目狀態。 當您更改工作項的狀態時，該狀態的附加批准要求在可以將新狀態分配給該項之前確認狀態更改。

      >[!TIP]
      >
      >
      >   
      >   
      >   * 您可以將組級別審批與全局或組級別狀態關聯。
      >   * 您不能使用審批流程將物料的狀態更改為與審批流程相關聯的狀態以外的狀態。

         >   
         >   
         >     例如，如果任務批准與「正在進行」狀態關聯，則在批准時，任務會自動將其狀態更改為「正在進行」。 它無法自動將其狀態更改為「已完成」或與批准無關的任何其他狀態。


   * 與核准程式相關聯的實體可以是使用者、工作角色或團隊。 使用者最終須負責接受或拒絕核准。 您可以為在專案上履行特定角色的使用者指派核准。 例如，您可以為項目所有者或贊助商分配批准。 如需詳細資訊，請參閱 [建立工作項的審批流程](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

      存在下列情況：

      * 將批准分配給職務角色時，項目團隊中與職務角色關聯的任何用戶都可以對批准做出決策。 與核准相關聯的角色可以是其主要角色或任何其他角色。

         如需專案團隊的相關資訊，請參閱 [專案團隊概觀](../../manage-work/projects/planning-a-project/project-team-overview.md).

      * 當您將批准分配給某個團隊時，該團隊的任何成員都可以對批准做出決策。 與核准相關聯的團隊可以是其主團隊或任何其他團隊。

         如需使用者角色和團隊的相關資訊，請參閱 [編輯使用者的設定檔](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* 建立工作項時，它不會自動附加審批流程。 如果要使用，則必須手動附加。 有關將審批流程附加到項目的資訊，請參閱 [將新審批流程或現有審批流程與工作關聯](../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).
* Workfront管理員或具有核准程式之管理存取權的使用者，可以建立系統層級的全域核准程式，以便在整個系統中使用。 具有核准程式管理存取權的群組管理員可以建立群組層級的全域核准程式，以便僅供其管理的特定群組使用。
* 如果您不想對工作項使用預定義的系統級別或組級別全局審批流程，則當您對要附加審批流程的對象具有「管理」權限時，可以建立一次性審批流程並將其附加。

   >[!NOTE]
   您只能對建立該流程的特定項目使用一次一次性審批流程。 您可以為項目、任務、問題、模板和模板任務的一次性審批流程建立全局狀態和組級狀態的關聯。

* 使用組層自定義狀態將組層審批流程附加到項目時，更改項目組可能會在上一組的審批狀態和系統層的現有審批狀態之間產生衝突。 在更新組之前，請考慮刪除項目上的組級審批流程，或刪除其任務或問題。 如需建立群組層級核准程式的相關資訊，請參閱 [組級審批流程](../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-groups-approval-processes.md). 如需建立自訂群組狀態的相關資訊，請參閱 [建立或編輯群組狀態](../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md). 如需更新專案群組的相關資訊，請參閱 [編輯專案](../../manage-work/projects/manage-projects/edit-projects.md).

## 核准流程工作流程

本節將說明有關批准工作項的以下內容：

* [審批流程如何依賴狀態](#how-approval-processes-rely-on-statuses)
* [典型工作流程如何使用核准程式](#how-a-typical-workflow-uses-an-approval-process)

### 審批流程如何依賴狀態 {#how-approval-processes-rely-on-statuses}

將狀態附加到審批流程可確保物料以正確的順序通過部門。

**範例：** 您可以將審批流程附加至需要財務部門審批的市場營銷部門狀態。 然後，當某人將工作項的狀態更改為「營銷部」時，該項在財務部簽名前無法移至該部。

有關工作項目狀態的詳細資訊，請參閱以下文章：

* [訪問系統項目狀態清單](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md)
* [訪問系統任務狀態清單](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/task-statuses.md)
* [訪問系統問題狀態清單](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md)

### 典型工作流程如何使用核准程式 {#how-a-typical-workflow-uses-an-approval-process}

下列案例說明當Workfront物件依照以下順序執行多個步驟的工作流程時，核准程式如何協助使用者核准工作：

1. Workfront管理員或具有核准流程管理存取權的使用者會為專案、任務或問題建立核准流程。

   >[!NOTE]
   您可以將項目批准流程附加到模板，並將任務批准流程附加到模板任務。 執行此操作後，當某人使用模板建立項目時，審批流程將分別變成項目或任務審批流程。 附加到模板或模板任務的一次性審批流程仍然是項目和任務的一次性審批流程。

1. 對項目、任務或問題具有「管理」權限的用戶會將審批流程附加至項目，或為項目建立一次性審批。
1. 分配給工作項的用戶將其狀態更改為啟動審批流程且審批流程開始的狀態。 （建立審批流程的人員定義了狀態與審批流程之間的關係。）
1. 指定的批准者接收有關待定批准流程的通知，並審閱工作項。
1. 批准流程在指定批准者批准流程的所有步驟後結束。 或者，如果他們拒絕步驟，則狀態會重設為預先定義狀態，或建立問題。 （建立批准流程的人員，定義了這些自動步驟中的哪些步驟在拒絕後發生。）

**範例：** 廣告團隊已建立一個狀態，稱為「準備打印」，並建立了一個稱為「設計器/複製者簽名」的批准過程，該過程與此狀態關聯。 此核准程式已設定為：

* 需要團隊的設計師和文案撰寫者批准
* 每當有人將工作項的狀態更改為「準備打印」時啟動

手冊項目所有者將設計人員/文案撰寫人簽發批准流程附加到手冊項目。

當項目中的某個人將狀態更改為「準備打印」時，複製者和設計者會收到通知，要求他們批准或拒絕它。 在審批過程中，當審議是否批准時，項目的狀態顯示為「準備打印 — 待批」。

在兩人核准Workfront中的手冊後，專案狀態會變更為「準備列印」。

## 文檔審批流程

文檔批准用於更一般的批准。 在「更新」頁簽上，以聊天格式捕獲反饋。 您可以使用核准按鈕來核准、拒絕或核准變更。

要將文檔上載到Workfront後添加批准者，請參閱 [請求文檔批准](../../review-and-approve-work/manage-approvals/request-document-approvals.md).

## 證明核准流程

校樣核准可用於更深入的審核，且通常包含更複雜的工作流程。 校對檢視器中會使用標籤工具擷取意見。 您可以使用核准按鈕來核准、拒絕或核准變更。

要將自動工作流添加到文檔校樣中，並指定工作流中的某些用戶作為校樣的批准者，請參閱 [使用自動化工作流程建立進階校樣](../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md).

## 配置工作項目審批流程的設定

身為Workfront管理員，您可以在系統中為工作項目核准程式配置全域設定。 這些設定會決定核准程式的各種規則，例如允許核准決定持續開放多久，或您在系統中管理核准委派的方式。 如需核准程式設定的詳細資訊，請參閱 [配置全局批准設定](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md).
