---
product-area: projects
navigation-topic: approvals
title: 檢視核准
description: 核准流程提供了為專案、任務和問題建立多步驟核准的靈活性。 Adobe Workfront管理員會定義核准程式，以提供整個系統的一致性。
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: 1071e456-f111-4c52-b13a-ac1113f69cec
source-git-commit: 95679dd71ef7e4991853e63573a387f26321159d
workflow-type: tm+mt
source-wordcount: '861'
ht-degree: 0%

---

# 檢視核准

核准流程提供了為專案、任務和問題建立多步驟核准的靈活性。 Adobe Workfront管理員會定義核准程式，以提供整個系統的一致性。

如需有關建立核准流程的資訊，請參閱 [建立工作專案的核准流程](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

如需將核准與Workfront中的工作相關聯的資訊，請參閱 [將新的或現有的核准流程與工作建立關聯](../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>評論或以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>檢視與核准關聯的物件或更高的存取許可權</p> <p>注意：如果您還是沒有存取權，請詢問您的Workfront管理員，他們是否在您的存取層級中設定其他限制。 如需有關Workfront管理員如何修改您的存取層級的資訊，請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>檢視與核准相關聯的物件或更高許可權</p> <p>如需請求其他存取許可權的詳細資訊，請參閱 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">要求物件的存取權 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的Workfront管理員。

## 在Adobe Workfront中尋找核准

您可以從Workfront的多個區域檢視或管理核准。 如需有關如何管理不同區域之核准的資訊，請參閱 [核准工作](../../review-and-approve-work/manage-approvals/approving-work.md).

您可以從下列區域檢視或管理核准：

* 在「首頁」區域中

   * 當您選取檢視全部或核準時，所有等待您核准的專案、任務、問題、時程表、檔案和存取權都會顯示在首頁區域中。
   * 您自己提交的核准也會顯示在首頁區域，在工作清單的「我已提交的核准」區段。 如需詳細資訊，請參閱 [在[首頁]區域中檢閱您提交核准的工作](#review-work-you-submit-for-approval-in-the-home-area) 一節。
   * 當關聯的專案、任務或問題標籤為「已解決」、「保留」、「已關閉」或「已取消」時，核准會從「首頁」區域移除。

  如需有關使用「首頁」的資訊，請參閱 [開始使用首頁](../../workfront-basics/using-home/using-the-home-area/get-started-with-home.md).

* 在專案、任務、問題、檔案或校訂的標題中
* 在專案、任務或問題的核准區段中
* 在報表中

  >[!NOTE]
  >
  >您無法對報表的核准做出決定。

  您可以建立包含核准資訊的專案、任務、問題或檔案核准報告。

  如需建立報表的相關資訊，請參閱 [建立自訂報表](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## 在[首頁]區域中檢閱您提交核准的工作 {#review-work-you-submit-for-approval-in-the-home-area}

1. 按一下 **首頁** 圖示 ![](assets/home-icon-30x29.png) Adobe Workfront左上角。

   >[!NOTE]
   >
   >您的Workfront管理員可能會對您環境中的「首頁」圖示進行下列變更：
   >
   >* 以自訂的影像取代，以說明您的組織。 在此情況下，圖示看起來將會與本文中顯示的有所不同。
   >* 使用其他頁面取代連結至該頁面的頁面。 在此情況下，請按一下 **主要功能表** ![](assets/main-menu-icon.png) 然後按一下「 」 **首頁**.

1. 選取 **工作清單**，然後按一下 **篩選** 下拉式功能表並選取 **核准**.
1. 展開 **我已提交的核准** 區段，並尋找您提交的核准。

   ![](assets/approvals-submitted-section-in-home-nwe-350x401.png)

## 檢視物件的核准狀態

您可以在物件的下列區段中檢視物件的核准狀態：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">更新 </td> 
   <td> <p>發生時顯示所有核准狀態。 核准狀態會與其他狀態一起顯示於 <strong>更新</strong> 區段。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">核准</td> 
   <td> <p>顯示核准流程的更多詳細資訊，例如核准流程的每個階段以及核准者是否已授予核准。</p> </td> 
  </tr> 
 </tbody> 
</table>

* [使用更新區域檢視核准狀態](#use-the-updates-area-to-view-an-approval-status)
* [使用核准區域檢視核准狀態](#use-the-approvals-area-to-view-an-approval-status)

### 使用更新區域檢視核准狀態 {#use-the-updates-area-to-view-an-approval-status}

對專案、任務或問題啟動核準時，狀態會顯示在 **更新** 物件的索引標籤，指示核准狀態。 每當物件透過核准程式轉換時，就會顯示新狀態。 這包含下列事件：

* 對物件啟動核准流程。 當狀態變更時，會啟動核准流程。
* 物件已拒絕
* 物件已核准 

>[!TIP]
>
>如果將核准套用至任務，則核准更新會顯示在任務的「更新」標籤上，而不是顯示在任務所在專案的「更新」標籤上。

### 使用核准區域檢視核准狀態 {#use-the-approvals-area-to-view-an-approval-status}

您可以檢視您目前正在處理的任務或問題在核准流程中的位置。 您可以看到下列資訊：

* 核准流程的階段
* 哪些核准者已核准它
* 哪些核准者尚未核准此專案

若要檢視任務或問題在核准流程中的目前狀態：

1. 前往與核准相關聯的專案、任務或問題。
1. 在左側面板中，按一下 **核准**. 您可能需要先按一下 **顯示更多**.

   「核准」標籤會顯示所有過去核准路徑和階段的完整資訊。 您可以檢視確切的核准決策者，或核准是針對團隊、工作角色或使用者所設定。

   ![](assets/approvals-tab-expanded-on-issue-nwe-350x320.png)

   如需有關建立核准流程的資訊，請參閱 [建立工作專案的核准流程](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).
