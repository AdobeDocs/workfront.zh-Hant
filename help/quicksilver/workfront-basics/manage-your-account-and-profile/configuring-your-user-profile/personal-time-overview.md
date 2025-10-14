---
content-type: overview
product-area: user-management
navigation-topic: configure-your-user-profile
title: 設定個人休假
description: 請務必在Adobe Workfront中指明核准的休假何時發生，因為這會影響您的排程，並影響您指派至之任務的規劃完成日期。
author: Becky
feature: Get Started with Workfront
exl-id: e7710495-c418-47b1-8598-725580054fc5
source-git-commit: f10b0a4897d6250f0c4decf1fad069c598536a38
workflow-type: tm+mt
source-wordcount: '428'
ht-degree: 0%

---

# 設定個人休假

<!-- Audited: 12/2023 -->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview Sandbox environment, and is being released in a phased rollout to Production.</span>-->

[!DNL Adobe Workfront]的設計目的並非複製或取代您現有的系統，以管理、累積及追蹤個人休假。

不過，請務必指明核准的休假何時發生，因為這會影響您的排程以及您指派給之任務的[!UICONTROL 規劃完成日期]。

例如，如果您被指派給一項排程為兩週的工作，而您計畫在這段時間內休假3天，則[!DNL Workfront]會在工作時間表上新增3天，以考慮該休假。

「資源管理」工具也會使用您的個人休假來指示您何時可以排程工作。

>[!NOTE]
>
>為了確保排程休假的日期不會出現不一致的情況，我們建議您使用者設定檔的時區與排程的時區相符。 如需詳細資訊，請參閱下列文章：
>
>* [建立排程](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)
>* [編輯使用者的設定檔](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)
>

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計劃</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權</td> 
   <td> <p>新增：標準（設定個人休假）</p>
        <p>或</p>
        <p>目前：工作或更高（以設定您的個人休假）</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td>具有[!UICONTROL Edit User]存取權的[!UICONTROL Manager] （變更其他使用者的休假行事曆）<br>
   <strong>注意：</strong>如果管理員編輯其他使用者的個人休假行事曆，所有專案都會以使用者的時區顯示，而非管理員的時區顯示。</td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

## 在[!DNL Workfront]中設定個人休假

{{step1-click-profile-pic}}

>[!NOTE]
>
>如果您在Adobe整合式體驗中，可以按一下頂端導覽區域中的Adobe帳戶選單（您的設定檔圖片），然後選擇Workfront設定檔來存取您的Workfront設定檔。
>
>![workfront設定檔](assets/aue-profile.png)

1. 在左側面板中，按一下&#x200B;**[!UICONTROL 休假]**。
1. 選取您個人休假的所需日期。

   <!--<span class="preview">Sample image in the Preview environment:</span>
   ![Personal time off calendar](assets/personal-time-off-calendar-0925.png)-->

   <!--Sample image in the Production environment:-->
   ![個人休假行事曆](assets/personal-time-off-calendar.png)

1. 如果您要休一整天的假，請選取&#x200B;**[!UICONTROL 全天]**。

   如果您休假不到一整天，請保持此核取方塊為空白，並指出休假的開始和結束時間。

1. 按一下「**[!UICONTROL 儲存]**」。

   您的休假現在可以在整個[!DNL Workfront]系統的資源管理工具（例如資源規劃工具和工作負載平衡器）中看到。 在此期間為您指派工作時，工具提示會通知使用者您已排程休假。
