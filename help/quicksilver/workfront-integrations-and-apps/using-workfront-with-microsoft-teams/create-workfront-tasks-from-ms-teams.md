---
product-area: workfront-integrations;agile-and-teams;user-management
navigation-topic: workfront-for-microsoft-teams
title: 建立 [!DNL Adobe Workfront] 任務來源 [!DNL Microsoft] 團隊
description: 您可以在Adobe中建立個人任務 [!DNL Workfront] 若群組擁有者已安裝並設定，則從Microsoft Teams [!DNL Workfront] 適用於您團隊的Microsoft Teams，且您已從Microsoft Teams登入Workfront。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 31b86c8d-967a-446a-86f2-3d38e44c45e1
source-git-commit: 1f2655c0e88a5cc918501e2a0ef830758111ded8
workflow-type: tm+mt
source-wordcount: '364'
ht-degree: 0%

---

# 建立 [!DNL Adobe Workfront] 任務來源 [!DNL Microsoft Teams]

>[!NOTE]
>
>適用於Microsoft Teams的Adobe Workfront整合目前僅支援傳統Microsoft Teams體驗。

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計畫*</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權*</td> 
   <td> <p>[！UICONTROL Work]， [！UICONTROL計畫]</p> </td> 
  </tr>
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的 [!DNL Workfront] 管理員。

## 先決條件

您可以在中建立個人工作 [!DNL Adobe Workfront] 從 [!DNL Microsoft Teams] 如果符合下列條件：

* 群組擁有者已安裝並設定 [!DNL Workfront for Microsoft Teams] 給您的團隊。
* 您已登入 [!DNL Workfront] 從 [!DNL Microsoft Teams].

>[!NOTE]
>
>[!DNL Microsoft Teams] 不再支援 [!DNL Internet Explorer]. 若要使用 [!DNL Adobe Workfront for Microsoft Teams] 整合，您必須使用 [!DNL Internet Explorer].

如需關於安裝的資訊 [!DNL Workfront for Microsoft Teams] 並登入 [!UICONTROL Workfront] 從 [!DNL Microsoft Teams]，請參閱 [安裝 [!DNL Adobe Workfront for Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md).

## 建立個人任務來源 [!DNL Microsoft Teams]

1. 登入 [!DNL Workfront] 從 [!DNL Microsoft Teams].

   有關登入的資訊 [!DNL Workfront]，請參閱 [安裝 [!DNL Adobe Workfront for Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md).

1. 若要開啟 **[!UICONTROL 新任務]** 卡片：

   * 如果您在 [!DNL Workfront] 機器人聊天頻道，型別 **[!UICONTROL 新任務]** 在 [!UICONTROL 交談] 欄位以建立新任務。
   * 如果您在以外的聊天頻道 [!DNL Workfront] 機器人聊天頻道：

      * 開始輸入 **[!DNL @workfront]** 在 [!UICONTROL 交談] 欄位，然後選取 [!DNL Workfront] 您想要的機器人管道。
      * 繼續輸入 **[!UICONTROL 新任務]** 在 [!UICONTROL 交談] 欄位以建立新任務。

        此 [!UICONTROL 新任務] 卡片會顯示在 [!DNL Workfront] 機器人管道。

        ![ms_teams_new_task_card.png](assets/ms-teams-new-task-card-350x181.png)

1. 在 [!UICONTROL Workfront] 機器人管道，請在以下欄位中指定下列資訊： [!UICONTROL 新任務] 卡片：

   * 中的任務名稱 **[!UICONTROL 撰寫任務的標題]** 欄位。
   * 中的任務說明 **[!UICONTROL 撰寫工作的說明]** 欄位。
   * 必須完成任務的日期，在 **[!UICONTROL 到期日期]** 欄位。

1. 按一下 **[!UICONTROL 儲存].**

   新的個人任務建立於 [!DNL Workfront]. A [!UICONTROL 參考號碼] 已指派給它並在以下位置顯示： [!UICONTROL 新任務] 卡片。

   如需參考號碼的詳細資訊，請參閱 [[!UICONTROL 參考號碼] 個物件](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-reference-numbers-of-objects) 中的區段 [瞭解中的物件 [!DNL Adobe Workfront]](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md) 文章。

1. （選用）按一下 **[!UICONTROL 編輯]** 以進一步編輯任務資訊。
1. （選用）按一下 **[!UICONTROL 檢視位置[!DNL Workfront]]** 以開啟中新標籤的工作 [!DNL Workfront] 然後進一步編輯任務、將其移至專案，或將其指派給其他人員。
