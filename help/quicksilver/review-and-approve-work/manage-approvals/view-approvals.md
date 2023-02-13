---
product-area: projects
navigation-topic: approvals
title: 查看批准
description: 核准程式可靈活地為專案、任務和問題建立多步驟核准。 Adobe Workfront管理員定義核准程式，以提供整個系統的一致性。
author: Courtney
feature: Work Management
exl-id: 1071e456-f111-4c52-b13a-ac1113f69cec
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '861'
ht-degree: 0%

---

# 查看批准

核准程式可靈活地為專案、任務和問題建立多步驟核准。 Adobe Workfront管理員定義核准程式，以提供整個系統的一致性。

如需建立核准程式的相關資訊，請參閱 [建立工作項的審批流程](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

有關將批准與Workfront中的工作關聯的資訊，請參閱 [將新審批流程或現有審批流程與工作關聯](../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

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
   <td> <p>審核或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>查看或更高程度地訪問與批准關聯的對象</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>查看與批准關聯的對象的或更高權限</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 在Adobe Workfront中找出核准

您可以從Workfront的數個區域檢視或管理核准。 如需如何管理不同領域的核准的相關資訊，請參閱 [核准工作](../../review-and-approve-work/manage-approvals/approving-work.md).

您可以從以下區域檢視或管理核准：

* 在首頁

   * 當您選擇查看「全部」或「批准」時，等待批准的所有項目、任務、問題、時間表、文檔和訪問都顯示在「首頁」區域中。
   * 您自己提交的核准也會顯示在「工作清單」的「首頁」區域的「核准我已提交」區段中。 如需詳細資訊，請參閱 [在「首頁」區域審核您提交以供審批的工作](#review-work-you-submit-for-approval-in-the-home-area) 一節。
   * 將關聯的項目、任務或問題標籤為「已解決」、「暫掛」、「已關閉」或「已取消」時，系統會從「首頁」區域中刪除審批。

   有關使用首頁的資訊，請參閱 [開始使用首頁](../../workfront-basics/using-home/using-the-home-area/get-started-with-home.md).

* 在項目、任務、問題、文檔或校樣的標題中
* 在項目、任務或問題的「批准」部分
* 在報表中

   >[!NOTE]
   >
   >您無法對報表的核准作出決定。

   您可以建立包含審批資訊的項目、任務、發放或文檔審批報告。

   如需建立報表的相關資訊，請參閱 [建立自訂報表](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## 在「首頁」區域審核您提交以供審批的工作 {#review-work-you-submit-for-approval-in-the-home-area}

1. 按一下 **首頁** 圖示 ![](assets/home-icon-30x29.png) 在Adobe Workfront的左上角。

   >[!NOTE]
   >
   >您的Workfront管理員可能會對環境中的「首頁」圖示進行下列變更：
   >
   >* 以自訂的影像取代，以說明您的組織。 在此情況下，圖示看起來會與本文所顯示的不同。
   >* 將連結至該頁面的頁面取代為其他頁面。 在此情況下，按一下 **主菜單** ![](assets/main-menu-icon.png) 在頁面的右上角，然後按一下 **首頁**.


1. 選擇 **工作清單**，然後按一下 **篩選** 下拉式功能表，然後選取 **核准**.
1. 展開 **我提交的批准** 部分，並查找您提交的批准。

   ![](assets/approvals-submitted-section-in-home-nwe-350x401.png)

## 查看對象的批准狀態

您可以在對象的以下部分中查看對象的批准狀態：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">更新 </td> 
   <td> <p>在發生時顯示所有批准狀態。 核准狀態會與 <strong>更新</strong> 區段。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">核准</td> 
   <td> <p>顯示有關審批流程的更詳細資訊，如審批流程的每個階段以及審批人是否已授予審批。</p> </td> 
  </tr> 
 </tbody> 
</table>

* [使用「更新」區域查看批准狀態](#use-the-updates-area-to-view-an-approval-status)
* [使用「批准」區域查看批准狀態](#use-the-approvals-area-to-view-an-approval-status)

### 使用「更新」區域查看批准狀態 {#use-the-updates-area-to-view-an-approval-status}

當對項目、任務或問題啟動審批時，狀態將顯示在 **更新** 頁簽，指示批准狀態。 每當物件經過核准程式轉變時，就會顯示新狀態。 這包括下列事件：

* 在對象上啟動批准過程。 狀態更改時，將啟動審批流程。
* 對象被拒絕
* 對象已批准 

>[!TIP]
>
>如果將批准應用於任務，則批准更新會顯示在任務的「更新」頁簽上，而不是顯示在任務所在項目的「更新」頁簽上。

### 使用「批准」區域查看批准狀態 {#use-the-approvals-area-to-view-an-approval-status}

您可以清楚了解您目前處理的任務或問題在核准程式中的位置。 您可以看到下列資訊：

* 審批流程的階段
* 哪些批准者已批准了它
* 哪些批准者尚未批准

要查看任務或問題在審批流程中的當前狀態，請執行以下操作：

1. 轉到與批准關聯的項目、任務或問題。
1. 在左側面板中，按一下 **核准**. 您可能需要先按一下 **顯示更多**.

   「核准」索引標籤會顯示所有過去核准路徑和階段的完整資訊。 您可以確切看到誰對核准做出決策，或是針對團隊、工作角色或使用者設定核准。

   ![](assets/approvals-tab-expanded-on-issue-nwe-350x320.png)

   如需建立核准程式的相關資訊，請參閱 [建立工作項的審批流程](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).
