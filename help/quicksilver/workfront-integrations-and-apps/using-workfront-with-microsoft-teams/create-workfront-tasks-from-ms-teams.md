---
product-area: workfront-integrations;agile-and-teams;user-management
navigation-topic: workfront-for-microsoft-teams
title: 建立來自 [!DNL Adobe Workfront] 團隊的 [!DNL Microsoft] 工作
description: 如果團隊擁有者已為您的團隊安裝和設定 [!DNL Workfront] 的Adobe，且您從Microsoft Teams登入Microsoft Teams，您就可以從Microsoft Teams在Workfront [!DNL Workfront] 中建立個人工作。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 31b86c8d-967a-446a-86f2-3d38e44c45e1
source-git-commit: 4cf780aa1b1221cd6ff8e6ce58fbb7d3621f7fa9
workflow-type: tm+mt
source-wordcount: '443'
ht-degree: 0%

---

# 從[!DNL Adobe Workfront]建立[!DNL Microsoft Teams]個任務

>[!IMPORTANT]
>
>隨著[Microsoft轉換至「新團隊」使用者端](https://learn.microsoft.com/en-us/microsoftteams/teams-classic-client-end-of-availability)，傳統團隊使用者端在2025年7月1日之後將不再可用。 若要繼續使用Microsoft Teams和Workfront等整合式應用程式，客戶必須在此日期之前轉換至新Teams使用者端。
>
>更新的Workfront整合現在可供使用，並且與新團隊體驗完全相容。 在大多數情況下，使用者轉換後，Workfront會自動顯示。 如果不適用，可從Microsoft Teams App Store手動安裝整合。 若要在New Teams使用者端中安裝或驗證Workfront整合，請參閱[為Microsoft Teams [!DNL Adobe Workfront] 安裝](/help/quicksilver/workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md)。



## 存取需求

+++ 展開以檢視本文中功能的存取需求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront套件</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td> <p>標準</p>
   <p>工作或更高</p> </td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先決條件

如果符合下列條件，您可以從[!DNL Adobe Workfront]在[!DNL Microsoft Teams]中建立個人工作：

* 團隊擁有者已為您的團隊安裝和設定[!DNL Workfront for Microsoft Teams]。
* 您已從[!DNL Workfront]登入[!DNL Microsoft Teams]。

>[!NOTE]
>
>[!DNL Microsoft Teams]不再支援[!DNL Internet Explorer]。 若要使用[!DNL Adobe Workfront for Microsoft Teams]整合，您必須使用[!DNL Internet Explorer]以外的網頁瀏覽器。

如需有關安裝[!DNL Workfront for Microsoft Teams]以及從[!UICONTROL 登入]Workfront[!DNL Microsoft Teams]的資訊，請參閱[安裝 [!DNL Adobe Workfront for Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md)。

## 從[!DNL Microsoft Teams]建立個人任務

1. 從[!DNL Workfront]登入[!DNL Microsoft Teams]。

   如需有關登入[!DNL Workfront]的資訊，請參閱[安裝 [!DNL Adobe Workfront for Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md)。

1. 若要開啟&#x200B;**[!UICONTROL 新工作]**&#x200B;卡片：

   * 如果您在[!DNL Workfront]機器人聊天頻道，請在&#x200B;**[!UICONTROL 交談]**&#x200B;欄位中輸入[!UICONTROL 新任務]以建立新任務。
   * 如果您在[!DNL Workfront]機器人聊天頻道以外的聊天頻道：

      * 開始在&#x200B;**[!DNL @workfront]**&#x200B;交談[!UICONTROL 欄位中輸入]，然後選取您想要的[!DNL Workfront]機器人頻道。
      * 繼續在&#x200B;**[!UICONTROL 交談]**&#x200B;欄位中輸入[!UICONTROL 新工作]以建立新工作。

        [!UICONTROL 新任務]卡片會顯示在[!DNL Workfront]機器人頻道中。

        ![ms_teams_new_task_card.png](assets/ms-teams-new-task-card-350x181.png)

1. 在[!UICONTROL Workfront]機器人頻道中，在[!UICONTROL 新增工作]卡片上指定下列資訊：

   * **[!UICONTROL 中的任務名稱撰寫任務的標題]**&#x200B;欄位。
   * 在&#x200B;**[!UICONTROL 寫入任務的描述]**&#x200B;欄位中的任務描述。
   * 必須在&#x200B;**[!UICONTROL 到期日]**&#x200B;欄位中完成工作的日期。

1. 按一下&#x200B;**[!UICONTROL 儲存]。**

   新的個人任務建立於[!DNL Workfront]。 [!UICONTROL 參考號碼]已指派給它，並顯示在[!UICONTROL 新任務]卡片上。

   如需參考編號的相關資訊，請參閱[[!UICONTROL 瞭解]文章中的物件](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-reference-numbers-of-objects)參考編號[物件 [!DNL Adobe Workfront]](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)區段。

1. （選擇性）按一下&#x200B;**[!UICONTROL 編輯]**&#x200B;以進一步編輯工作資訊。
1. （選擇性）按一下「**[!UICONTROL 在[!DNL Workfront]]**&#x200B;中檢視」以在「[!DNL Workfront]」的新索引標籤中開啟工作，並進一步編輯工作、將其移至專案或將其指派給其他人。
