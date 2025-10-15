---
product-area: workfront-integrations
navigation-topic: workfront-for-slack
title: 接收 [!DNL Adobe Workfront] 中的 [!DNL Slack]通知
description: 接收 [!DNL Adobe Workfront] 中的 [!DNL Slack]通知
author: Becky
feature: Workfront Integrations and Apps
exl-id: bc1ce4ea-58be-4cd7-ab59-7dddb82949b9
source-git-commit: 6178cabbf021fbf92bd8795c5c2bd0346801d64d
workflow-type: tm+mt
source-wordcount: '584'
ht-degree: 1%

---

# 在[!DNL Adobe Workfront]中接收[!DNL Slack]個通知

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: *** Linked to Accessing Workfront from Slack.***Some of this information is duplicating in Accessing Workfront from Slack (also screen shots))</p>
-->

安裝[!DNL Adobe Workfront for Slack]之後，您可以在[!DNL Workfront]中接收[!DNL Slack]個通知。\
如需有關安裝[!DNL Workfront for Slack]的資訊，請參閱[設定 [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md)。

您可以啟用顯示在[!UICONTROL 介面的通知泡泡中的]通知[!DNL Workfront]的選取數目，以便在[!DNL Slack]中傳送。

電子郵件通知與[!DNL Workfront]介面通知獨立運作。 您或您的[!DNL Workfront]管理員可以停用電子郵件通知，而介面通知無法在[!DNL Workfront]中停用。\
但是，如果您只想在[!DNL Workfront]介面中關注這些通知，您可以停用可能會在[!DNL Slack]中收到的[!DNL Workfront]通知。

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
   <td> <p>任何</p>
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先決條件

您必須先在[!DNL Workfront]中接收[!DNL Slack]個通知

* 設定[!DNL Workfront for Slack]\
   如需設定[!DNL Workfront for Slack]的說明，請參閱[設定 [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md)。

## 設定[!DNL Workfront]的[!DNL Slack]通知 {#configure-workfront-notifications-for-slack}

1. （視條件而定）將[!DNL Workfront]新增至您的[!DNL Slack]執行個體後，從[!DNL Workfront]登入[!DNL Slack]。\
   如需有關從[!DNL Workfront]登入[!DNL Slack]的資訊，請參閱[存取 [!DNL Adobe Workfront] 從 [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md)。

1. 從任何頻道，開始在訊息欄位中輸入以下命令之一：

   `/workfront settings`

   或

   `/wf settings`

1. 預設會啟用所有通知。\
   停用下列任何通知：

   * [!UICONTROL 我被指派到一個新任務或問題]
   * [!UICONTROL 我的團隊已指派給新任務或問題]
   * [!UICONTROL 我收到新的核准或存取要求]
   * [!UICONTROL 有人將我加入定向更新]
   * [!UICONTROL 有人對我所在的執行緒發表評論]
   * [!UICONTROL 我訂閱的任務、問題或專案已更新]
   * [!UICONTROL 有人對我其中一個工作專案發表評論]
   * [!UICONTROL 有人對我的說明要求發表評論]

   您對[!UICONTROL 通知]選項所做的變更會立即生效。\
   您啟用的通知已在[!DNL Workfront] [!DNL Slack]頻道中傳遞。 當您在此停用通知時，只會針對[!DNL Slack]停用通知，不會針對[!DNL Workfront]介面停用通知。 您會在介面右上角的[!DNL Workfront]通知泡泡中繼續收到這些通知。

## 管理來自[!DNL Workfront]的[!DNL Slack]通知

您可以從[!DNL Workfront]接收及回應[!DNL Slack]個通知。

您可以停用您在[!DNL Slack]中啟用的通知的電子郵件通知，以確保您不會收到重複的通知。\
如需設定電子郵件通知的詳細資訊，請參閱[修改您自己的電子郵件通知](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md)。

在[!DNL Workfront]中啟用或停用[!DNL Slack]通知不會影響您在[!DNL Workfront]介面中收到的通知。\
無法停用[!DNL Workfront]介面中的通知。

若要管理[!DNL Workfront]的[!DNL Slack]通知：

1. 登入[!UICONTROL Slack]。
1. 從[!DNL Workfront]登入[!DNL Slack]。\
   如需有關從[!DNL Workfront]登入[!DNL Slack]的資訊，請參閱[!DNL Workfront]Access[!DNL Slack]from[中的「從 [!DNL Adobe Workfront] 登入 [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md)」區段。

1. 確保已啟用您[!DNL Workfront]的[!DNL Slack]通知。\
   如需有關哪些[!DNL Workfront]通知可設定為也傳送至[!DNL Slack]的詳細資訊，請參閱[設定 [!DNL Workfront] 的 [!DNL Slack]](#configure-workfront-notifications-for-slack-configure-workfront-notifications-for-slack)通知。

1. 前往&#x200B;**[!DNL Workfront]**&#x200B;頻道尋找您的[!DNL Workfront]通知。
1. （條件式與選擇式）執行下列任一項作業：

   * 按一下&#x200B;**[!UICONTROL 處理它]**&#x200B;以接受處理任務。

   * （有條件且選擇性）按一下&#x200B;**[!UICONTROL 在[!DNL Workfront]]**&#x200B;中回覆以回覆回應、輸入您的回覆，然後按一下&#x200B;**[!UICONTROL 回覆]**。

   * （有條件且選擇性）按一下「**[!UICONTROL 核准]**」或「**[!UICONTROL 拒絕]**」以核准或拒絕擱置您核准的任務、問題或專案。

   * （有條件且選擇性）按一下&#x200B;**[!UICONTROL 核准]**、**[!UICONTROL 變更]**&#x200B;或&#x200B;**[!UICONTROL 拒絕]**，以核准、核准變更，或拒絕檔案。

     您也可以將滑鼠移到檔案的縮圖上，然後按一下放大鏡圖示，在核准檔案之前檢視檔案的較大預覽。\
      只能預覽核准的Slack [檔案型別](https://api.slack.com/types/file)。

   * （條件式及選擇性）按一下&#x200B;**[!UICONTROL 授予]**&#x200B;或&#x200B;**[!UICONTROL 忽略]**&#x200B;以授予或忽略其他使用者要求更多存取許可權的要求。\

     對於您在通知中所做的每項決定，您會收到動作已在[!DNL Workfront]內完成的確認。
