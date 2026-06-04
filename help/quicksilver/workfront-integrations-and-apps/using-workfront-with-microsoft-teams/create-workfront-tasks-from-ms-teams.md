---
product-area: workfront-integrations;agile-and-teams;user-management
navigation-topic: workfront-for-microsoft-teams
title: 建立來自 [!DNL Microsoft] 團隊的 [!DNL Adobe Workfront] 工作
description: 如果團隊擁有者已為您的團隊安裝和設定 [!DNL Workfront] 的Adobe，且您從Microsoft Teams登入Microsoft Teams，您就可以從Microsoft Teams在Workfront [!DNL Workfront] 中建立個人工作。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 31b86c8d-967a-446a-86f2-3d38e44c45e1
TQID: https://experienceleague.adobe.com/EGXeEO-HU8813eA-dyVAuKSv6rAQg8tsDiDT5leVee0
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
subfeature_v2:
  - id: a7ef0b24-c866-4849-a368-53678af2dfe5
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 449
ht-degree: 4%

---

# 從[!DNL Microsoft Teams]建立[!DNL Adobe Workfront]個任務

>[!IMPORTANT]
>
>隨著[Microsoft轉換至「新團隊」使用者端](https://learn.microsoft.com/en-us/microsoftteams/teams-classic-client-end-of-availability)，傳統團隊使用者端在2025年7月1日之後將不再可用。 若要繼續使用Microsoft Teams和Workfront等整合式應用程式，客戶必須在此日期之前轉換至新Teams使用者端。
>
>更新的Workfront整合現在可供使用，並且與新團隊體驗完全相容。 在大多數情況下，使用者轉換後，Workfront會自動顯示。 如果不適用，可從Microsoft Teams App Store手動安裝整合。 若要在New Teams使用者端中安裝或驗證Workfront整合，請參閱[為Microsoft Teams](/help/quicksilver/workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md)安裝 [!DNL Adobe Workfront] 。



## 存取權要求

+++ 展開以檢視這篇文章中所述功能的存取權要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 封裝</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td> <p>標準</p>
   <p>工作或更高層級</p> </td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先決條件

如果符合下列條件，您可以從[!DNL Microsoft Teams]在[!DNL Adobe Workfront]中建立個人工作：

* 團隊擁有者已為您的團隊安裝和設定[!DNL Workfront for Microsoft Teams]。
* 您已從[!DNL Microsoft Teams]登入[!DNL Workfront]。

>[!NOTE]
>
>[!DNL Microsoft Teams]不再支援[!DNL Internet Explorer]。 若要使用[!DNL Adobe Workfront for Microsoft Teams]整合，您必須使用[!DNL Internet Explorer]以外的網頁瀏覽器。

如需有關安裝[!DNL Workfront for Microsoft Teams]以及從[!DNL Microsoft Teams]登入[!UICONTROL Workfront]的資訊，請參閱[安裝 [!DNL Adobe Workfront for Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md)。

## 從[!DNL Microsoft Teams]建立個人任務

1. 從[!DNL Microsoft Teams]登入[!DNL Workfront]。

   如需有關登入[!DNL Workfront]的資訊，請參閱[安裝 [!DNL Adobe Workfront for Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md)。

1. 若要開啟&#x200B;**[!UICONTROL 新工作]**&#x200B;卡片：

   * 如果您在[!DNL Workfront]機器人聊天頻道，請在[!UICONTROL 交談]欄位中輸入&#x200B;**[!UICONTROL 新任務]**&#x200B;以建立新任務。
   * 如果您在[!DNL Workfront]機器人聊天頻道以外的聊天頻道：

      * 開始在[!UICONTROL 交談]欄位中輸入&#x200B;**[!DNL @workfront]**，然後選取您想要的[!DNL Workfront]機器人頻道。
      * 繼續在[!UICONTROL 交談]欄位中輸入&#x200B;**[!UICONTROL 新工作]**&#x200B;以建立新工作。

        [!UICONTROL 新任務]卡片會顯示在[!DNL Workfront]機器人頻道中。

        ![ms_teams_new_task_card.png](assets/ms-teams-new-task-card-350x181.png)

1. 在[!UICONTROL Workfront]機器人頻道中，在[!UICONTROL 新增工作]卡片上指定下列資訊：

   * **[!UICONTROL 中的任務名稱撰寫任務的標題]**&#x200B;欄位。
   * 在&#x200B;**[!UICONTROL 寫入任務的描述]**&#x200B;欄位中的任務描述。
   * 必須在&#x200B;**[!UICONTROL 到期日]**&#x200B;欄位中完成工作的日期。

1. 按一下&#x200B;**[!UICONTROL 儲存]。**

   新的個人任務建立於[!DNL Workfront]。 [!UICONTROL 參考號碼]已指派給它，並顯示在[!UICONTROL 新任務]卡片上。

   如需參考編號的相關資訊，請參閱[瞭解 [!DNL Adobe Workfront]](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)文章中的物件[[!UICONTROL 參考編號]物件](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-reference-numbers-of-objects)區段。

1. （選擇性）按一下&#x200B;**[!UICONTROL 編輯]**&#x200B;以進一步編輯工作資訊。
1. （選擇性）按一下「**[!UICONTROL 在[!DNL Workfront]]**&#x200B;中檢視」以在「[!DNL Workfront]」的新索引標籤中開啟工作，並進一步編輯工作、將其移至專案或將其指派給其他人。
