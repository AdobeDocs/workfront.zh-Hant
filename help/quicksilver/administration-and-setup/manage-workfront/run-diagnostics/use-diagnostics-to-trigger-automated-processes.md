---
user-type: administrator
product-area: system-administration
navigation-topic: run-diagnostics
title: 使用診斷來觸發自動化流程
description: 您可以使用診斷手動觸發自動化程式，例如以時間為基礎的指令碼、重新計算或電子郵件通知。
feature: System Setup and Administration
role: Admin
author: Lisa
exl-id: 9243ee60-006b-4628-bde7-5b037dde7511
source-git-commit: 379772f6bd1ed9448e6fd5feee956a931f65f69e
workflow-type: tm+mt
source-wordcount: '350'
ht-degree: 9%

---

# 使用診斷來觸發自動化流程

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

您可以使用診斷手動觸發自動化程式，例如以時間為基礎的指令碼、重新計算或電子郵件通知。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td><p>新增：標準</p>
       <p>或</p>
       <p>目前：計畫</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td>[!UICONTROL 系統管理員]</td>
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 使用診斷來觸發自動化流程

1. 按一下Adobe Workfront右上角的&#x200B;**主功能表**&#x200B;圖示![主功能表圖示](assets/main-menu-icon.png)，然後按一下&#x200B;**設定** ![齒輪設定圖示](assets/gear-icon-settings.png)。

1. 展開&#x200B;**系統**，然後按一下&#x200B;**診斷**。
1. 從下列任一選項中選取：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">傳送逾期通知</td> 
      <td> <p>手動傳送逾期任務和問題的自動提醒通知。 </p> <p>如需設定自動提醒的詳細資訊，請參閱<a href="../../../administration-and-setup/manage-workfront/emails/setting-up-automatic-reminders.md" class="MCXref xref">設定自動提醒</a>。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">傳送臨近通知</td> 
      <td> <p>手動針對即將到期的任務和問題傳送自動提醒通知。</p> <p>如需設定自動提醒的詳細資訊，請參閱<a href="../../../administration-and-setup/manage-workfront/emails/setting-up-automatic-reminders.md" class="MCXref xref">設定自動提醒</a>。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">傳送提醒通知</td> 
      <td> <p>手動傳送提醒通知。 </p> <p>如需設定提醒通知的詳細資訊，請參閱<a href="../../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md" class="MCXref xref">設定提醒通知</a>。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">檢查所有 POP 帳戶</td> 
      <td>檢查已傳送至連結至Workfront之POP帳戶的新電子郵件。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">重新計算時間軸</td> 
      <td> <p>針對Workfront中所有處於目前狀態的專案，重新計算其時間表。 </p> <p>如需自動或手動計算專案時間表（一次一個專案）的詳細資訊，請參閱<a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref">重新計算專案時間表</a>。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">還原預設客戶報告</td> 
      <td>還原原本透過Workfront傳送的預設報告，以便所有使用者都能在<strong>報告</strong>區段中看到這些報告。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">產生時程表</td> 
      <td>根據使用者的週期性時程表設定檔產生使用者的時程表。 只有在時程表設定檔指派給使用者後，以及只有在刪除任何目前和未來的時程表後，才需要執行此選項。</td> 
     </tr> 
    </tbody> 
   </table>
