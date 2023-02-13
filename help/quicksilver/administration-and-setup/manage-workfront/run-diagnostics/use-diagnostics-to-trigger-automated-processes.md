---
user-type: administrator
product-area: system-administration
navigation-topic: run-diagnostics
title: 使用診斷程式觸發自動化流程
description: 您可以使用診斷來手動觸發自動化進程，例如基於時間的指令碼、重新計算或電子郵件通知。
feature: System Setup and Administration
role: Admin
exl-id: 9243ee60-006b-4628-bde7-5b037dde7511
source-git-commit: 5d36c2c959dbfd00920eaf0a16409102b99de042
workflow-type: tm+mt
source-wordcount: '329'
ht-degree: 6%

---

# 使用診斷程式觸發自動化流程

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

您可以使用診斷來手動觸發自動化進程，例如基於時間的指令碼、重新計算或電子郵件通知。

## 存取需求

您必須具備下列條件才能執行本文所述步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">Adobe Workfront計畫</a> </td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront授權概觀</a> </td> 
   <td> <p>計劃 </p>您必須是Workfront管理員。 如需Workfront管理員的相關資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予使用者完整的管理存取權</a>.</td> 
  </tr> 
 </tbody> 
</table>

## 使用診斷觸發自動化進程

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **設定** ![](assets/gear-icon-settings.png).

1. 展開 **系統**，然後按一下 **診斷**.
1. 從下列任一選項中選取：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">傳送逾期通知</td> 
      <td> <p>手動傳送逾期任務和問題的自動提醒通知。 </p> <p>有關設定自動提醒的詳細資訊，請參閱 <a href="../../../administration-and-setup/manage-workfront/emails/setting-up-automatic-reminders.md" class="MCXref xref">設定自動提醒</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">傳送早期通知</td> 
      <td> <p>手動傳送任務和即將到期問題的自動提醒通知。</p> <p>有關設定自動提醒的詳細資訊，請參閱 <a href="../../../administration-and-setup/manage-workfront/emails/setting-up-automatic-reminders.md" class="MCXref xref">設定自動提醒</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">傳送提示通知</td> 
      <td> <p>手動傳送提醒通知。 </p> <p>有關設定提醒通知的詳細資訊，請參閱 <a href="../../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md" class="MCXref xref">設定提醒通知</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">檢查所有 POP 帳戶</td> 
      <td> <p>檢查是否有新電子郵件已傳送至連結至Workfront的POP帳戶。 </p> <!--
        <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information about Workfront and POP account integrations, see and <a href="../../../manage-work/requests/create-and-manage-request-queues/queue-details-tab-overview.md" class="MCXref xref">Overview of the Queue Details tab in a project</a>.</p>
       --> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">重新計算時間表</td> 
      <td> <p>重新計算處於「目前」狀態的Workfront中所有專案的時間表。 </p> <p>如需自動或手動計算專案時間軸的詳細資訊，請參閱 <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref">重新計算項目時間表</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">恢復預設客戶報告</td> 
      <td>還原原本透過Workfront傳送的預設報表，以便顯示在 <strong>報表</strong> 區段。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">生成時程表</td> 
      <td>根據用戶的定期工時單配置檔案為用戶生成工時單。 只有在將時間表配置檔案分配給用戶後，並且只有在刪除當前和將來的任何時間表後，時間表配置檔案已發生顯著更改時，才需要運行此選項。</td> 
     </tr> 
    </tbody> 
   </table>
