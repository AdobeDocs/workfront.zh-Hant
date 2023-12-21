---
content-type: overview
product-area: projects
navigation-topic: approvals
title: 核准流程總覽
description: 您可以建立核准程式並將其附加至物件，以確保指定的使用者在物件進行之前先檢閱某些變更。
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: dd0822b6-80f1-4a2e-bf6a-0c425984f4d0
source-git-commit: e4de185f172b173dcc3ad966afa69ffb3bc479eb
workflow-type: tm+mt
source-wordcount: '1752'
ht-degree: 0%

---

# 核准流程總覽

<!-- Audited: 12/2023 -->

您可以建立核准程式並將其附加至物件，以確保指定的使用者在物件進行之前先檢閱某些變更。

這適用於Adobe Workfront中的下列物件型別：

* 工作專案（專案、任務或問題、範本、範本任務）
* 文件
* 證明

本文包含與工作專案相關之核准流程的一般資訊。
如需建立核准程式的說明，請參閱 [建立工作專案的核准流程](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

## 工作專案的核准流程型別

如果您是Adobe Workfront管理員或具有核准流程管理存取權的使用者，則可以為專案、任務和問題建立以下核准流程：

* **系統層級的全域核准程式**：使用者可以將這些連結附加到下列任一專案：

   * 核准區段中的專案、任務或問題
   * 在編輯專案方塊中的任務預設核准流程區域
   * 在預設核准流程區域中專案的佇列詳細資訊或佇列主題區段中。 專案必須啟用為請求佇列。

* **群組層級全域核准流程**：使用者可以將這些連結附加到下列專案：

   * 屬於「核准」區段中與核准流程相關聯之群組的專案、任務或問題
   * 在任務預設核准流程區域中屬於與核准流程相關聯之群組的專案的「編輯專案」方塊中
   * 在預設核准流程區域中專案的佇列詳細資訊或佇列主題區段中。 專案必須啟用為請求佇列，且必須屬於與核准流程關聯的群組。

  如需有關建立系統層級或群組層級核准流程的資訊，請參閱 [建立工作專案的核准流程](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

* **單次使用核准程式**：用於單一專案、任務、問題、範本或範本任務。 此型別的核准程式只會影響與其關聯的物件，而無法與任何其他物件關聯。

  如需有關建立單一使用核准流程的資訊，請參閱 [將新的或現有的核准流程與工作建立關聯](../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

>[!NOTE]
>
>本文使用「全域核准流程」一詞來區分「單次使用核准流程」。 全域核准流程可重複使用。
>
>「群組層級全域核准流程」一詞是指可重複用於專案的核准流程，其狀態僅與特定群組相關聯。

如需有關建立系統層次核准流程或群組層次核准流程的資訊，請參閱 [建立工作專案的核准流程](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

## 關於核准流程的考量事項

* 您必須先建立專案、任務、問題、範本或範本任務，核准流程才能與它們相關聯。
* 核准程式一律與兩個基本專案相關聯：

   * 每個核准流程都會對應至Workfront系統中的特定工作專案狀態。 當您變更工作專案的狀態時，該狀態的附加核准需要先確認狀態變更，然後才能將新狀態指派給專案。

     >[!TIP]
     >
     >
     >   
     >   
     >   * 您可以將群組層級核准與全域或群組層級狀態建立關聯。
     >   * 您無法使用核准程式將專案的狀態變更為與核准程式相關聯的狀態以外的狀態。
     >   
     >   
     >     例如，如果您有一個與進行中狀態相關聯的任務核准，則當核准被授予時，任務會自動將其狀態變更為進行中。 它無法自動將其狀態變更為「已完成」或任何其他與核准無關聯的狀態。
     >   
     >   
     >

   * 與核准流程關聯的實體可以是使用者、工作角色或團隊。 使用者最終需負責接受或拒絕核准。 您可以將核准指派給在專案上履行特定角色的使用者。 例如，您可以將核准指派給專案所有者或贊助者。 如需詳細資訊，請參閱 [建立工作專案的核准流程](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

     存在下列情況：

      * 當您指派核准給工作角色時，專案團隊中與工作角色相關聯的任何使用者都可以對核准做出決定。 與核准關聯的角色可以是其主要角色或任何其他角色。

        如需有關專案團隊的資訊，請參閱 [專案團隊概述](../../manage-work/projects/planning-a-project/project-team-overview.md).

      * 當您將核准指派給團隊時，該團隊的任何成員都可以對核准做出決定。 與核准相關聯的團隊可以是他們的主團隊或他們的任何其他團隊。

        如需有關使用者角色和團隊的資訊，請參閱 [編輯使用者設定檔](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* 當您建立工作專案時，它不會自動附加核准流程。 如果要使用一個，則必須手動附加。 如需有關將核准流程附加至專案的資訊，請參閱 [將新的或現有的核准流程與工作建立關聯](../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).
* Workfront管理員或具有核准流程管理存取權的使用者可以建立系統層級的全域核准流程，以供整個系統使用。 擁有核准流程管理存取權的群組管理員可以建立群組層級全域核准流程，僅供其管理的特定群組使用。
* 如果您不想對工作專案使用預先定義的系統層次或群組層次全域核准流程，則當您對要附加核准流程的物件具有「管理」許可權時，可以建立並附加單一使用核准流程。

  >[!NOTE]
  >
  您只能針對建立該程式的特定專案使用一次單一使用核准程式。 您可以為專案、任務、問題、範本和範本任務的一次性使用核准程式建立全域狀態和群組層級狀態的關聯。

* 當使用群組層級自訂狀態將群組層級核准流程附加至專案時，變更專案群組可能會在先前群組的核准狀態與系統層級現有的核准狀態之間產生衝突。 在更新群組之前，請考慮移除專案的群組層級核准流程，或其任務或問題。 如需有關建立群組層次核准流程的資訊，請參閱 [群組層級核准流程](../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-groups-approval-processes.md). 如需有關建立自訂群組狀態的資訊，請參閱 [建立或編輯群組狀態](../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md). 如需有關更新專案群組的資訊，請參閱 [編輯專案](../../manage-work/projects/manage-projects/edit-projects.md).

## 核准流程工作流程

本節說明下列核准工作專案的相關資訊：

* [核准程式依賴狀態的方式](#how-approval-processes-rely-on-statuses)
* [典型工作流程如何使用核准流程](#how-a-typical-workflow-uses-an-approval-process)

### 核准程式依賴狀態的方式 {#how-approval-processes-rely-on-statuses}

將狀態附加至核准程式，可確保料號以正確的順序在部門間移動。

**範例：** 您可以將核准處理附加至需要財務部門核准的行銷部門狀態。 然後，當有人將工作專案的狀態變更為「行銷部門」時，除非財務部門簽核該專案，否則該專案無法移至該部門。

如需工作專案狀態的詳細資訊，請參閱下列文章：

* [存取系統專案狀態清單](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md)
* [存取系統工作狀態清單](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/task-statuses.md)
* [存取系統問題狀態清單](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md)

### 典型工作流程如何使用核准流程 {#how-a-typical-workflow-uses-an-approval-process}

下列案例說明核准程式如何協助使用者核准工作，因為Workfront物件會依此順序透過包含數個步驟的工作流程進行：

1. Workfront管理員或具有核准流程管理存取權的使用者會為專案、任務或問題建立核准流程。

   >[!NOTE]
   >
   您可以將專案核准流程附加至範本，將任務核准流程附加至範本任務。 執行此動作後，當有人使用範本建立專案時，核准流程就會分別變成專案或任務核准流程。 附加到範本或範本任務的一次性使用核准流程仍然是專案和任務的一次性使用核准流程。

1. 擁有專案、任務或問題管理許可權的使用者會將核准流程附加到專案，或建立專案的單次使用核准。
1. 指定給工作專案的使用者會將其狀態變更為啟動核准流程的狀態，而核准流程隨即開始。 （建立核准程式的人定義了狀態與核准程式之間的關係。）
1. 指定的核准者會收到有關未決核准流程的通知，並複查工作專案。
1. 核准程式會在指定的核准者核准該程式的所有步驟後結束。 或者，如果他們拒絕步驟，則狀態會重設為預先定義的狀態，或建立問題。 （建立核准流程的人會定義在拒絕後要執行哪些自動步驟。）

**範例：** 廣告團隊已建立名為「準備列印」的狀態，以及名為「設計人員/撰稿人簽章」的核准程式，該程式與其狀態相關聯。 此核准流程已設定為：

* 需要團隊的設計師和撰稿人的核准
* 當有人將工作專案的狀態變更為準備列印時啟動

傳單專案所有者會將設計人員/撰稿人簽章核准程式附加至傳單專案。

當專案上的人員將狀態變更為「準備列印」時，撰稿人和設計人員會收到通知，要求他們核准或拒絕該專案。 在核准程式中，當他們考慮是否核準時，專案狀態將顯示為準備列印 — 未決核准。

他們在Workfront中核准傳單後，專案狀態會變更為「準備列印」。

## 檔案核准流程

檔案核准用於更一般的核准。 意見反應會以聊天格式擷取在「更新」索引標籤上。 您可以使用核准按鈕來核准、拒絕或核准變更。

若要在檔案上傳至Workfront後新增核准者，請參閱 [請求檔案核准](../../review-and-approve-work/manage-approvals/request-document-approvals.md).

## 校訂核准流程

校訂核准用於更深入的審查，通常包括更複雜的工作流程。 意見是透過校訂檢視器中的標籤工具擷取。 您可以使用核准按鈕來核准、拒絕或核准變更。

若要將自動化工作流程新增至檔案校訂，並將工作流程中的某些使用者指定為校訂的核准者，請參閱 [使用自動化工作流程建立進階校訂](../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md).

## 配置工作專案核准流程的設定

作為Workfront管理員，您可以為系統中的工作專案核准流程設定全域設定。 這些設定會決定核准流程的各種規則，例如核准決定應該允許保持開啟的時間長短，或者您如何在系統中管理核准委派。 如需核准流程設定的詳細資訊，請參閱 [設定全域核准設定](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md).
