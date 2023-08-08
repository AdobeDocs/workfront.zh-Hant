---
content-type: overview
product-area: user-management
navigation-topic: configure-your-user-profile
title: 在中設定個人休假 [!DNL Adobe Workfront]
description: Adobe Workfront的設計目的，並非為了複製或取代您現有的系統，以管理、產生和追蹤個人休假。 不過，請務必指明核准的休假何時發生，因為這會影響您的排程，並影響指派給您之任務的規劃完成日期。
author: Lisa
feature: Get Started with Workfront
exl-id: e7710495-c418-47b1-8598-725580054fc5
source-git-commit: 91eb8770c07396b5772029e9d2370f0b1f10d4a1
workflow-type: tm+mt
source-wordcount: '442'
ht-degree: 0%

---

# 在中設定個人休假 [!DNL Adobe Workfront]

[!DNL Adobe Workfront] 並非設計用來複製或取代您現有的系統，以管理、累積及追蹤個人休假。

不過，請務必指明核准的休假何時發生，因為這會影響您的排程並影響 [!UICONTROL 計畫完成日期] 指派給您的任務。

例如，如果您被指派給一項排程為兩週的任務，而您計畫在此期間休假3天， [!DNL Workfront] 將三天新增至任務時間表，以說明休假。

「資源管理」工具也會使用您的個人休假來指示您何時可以排程工作。

>[!NOTE]
>
>為了確保排程休假的日期不會出現不一致的情況，我們建議您使用者設定檔的時區與排程的時區相符。 如需詳細資訊，請參閱下列文章：
>
>* [建立排程](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)
>* [編輯使用者設定檔](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)
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
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 計劃*</strong></td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 授權*</strong></td> 
   <td>[！UICONTROL Work]或更高版本（用來設定您的個人休假）</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>存取層級設定*</strong></td> 
   <td>具有[！UICONTROL Edit User]存取權的[！UICONTROL Manager] （變更其他使用者的休假行事曆）<br>
   <strong>注意：</strong> 如果管理員編輯其他使用者的個人休假行事曆，則所有專案都會顯示在使用者的時區，而不是管理員的時區。</td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的 [!DNL Workfront] 管理員。

## 在中設定個人休假 [!DNL Workfront]

1. 按一下 **[!UICONTROL 主要功能表]** 圖示 ![主要功能表](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下個人資料圖片旁的使用者名稱。 或者（如果有的話），按一下頂端導覽區域中您的個人資料圖片，然後按一下 **[!UICONTROL Workfront設定檔]**.
1. 在左側面板中，按一下 **[!UICONTROL 休假]**.
1. 選取您個人休假的所需日期。

   ![個人休假行事曆](assets/personal-time-off-calendar.png)

1. 選取 **[!UICONTROL 全天]**，請休一整天的假。

   如果您休假不到一整天，並標註休假的開始和結束時間，請將其保留為未選取狀態。

1. 按一下&#x200B;**[!UICONTROL 儲存]**。

   您的休假現在可以在以下位置看到： [!DNL Workfront] 系統，位於資源管理工具，例如資源規劃工具和工作負載平衡器。 當您在這段期間被指派工作時，會出現工具提示，通知使用者您已排程休假。
