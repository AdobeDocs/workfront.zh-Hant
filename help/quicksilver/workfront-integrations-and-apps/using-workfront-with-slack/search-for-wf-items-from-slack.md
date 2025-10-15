---
product-area: workfront-integrations
navigation-topic: workfront-for-slack
title: 搜尋來自 [!DNL Adobe Workfront] 的 [!DNL Slack]個專案
description: 您可以從已安裝的 [!DNL Adobe Workfront] 應用程式搜尋 [!DNL Slack], if your instance of Slack has had the [!DNL Workfront] 專案。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 85821f21-d4fd-4f28-bd7a-0c109a4433a8
source-git-commit: 6178cabbf021fbf92bd8795c5c2bd0346801d64d
workflow-type: tm+mt
source-wordcount: '213'
ht-degree: 6%

---

# 從[!DNL Adobe Workfront]搜尋[!DNL Slack]個專案

如果您的[!DNL Adobe Workfront]執行個體已安裝[!DNL Slack]應用程式，您可以從[!DNL Slack]搜尋[!DNL Workfront]專案。

如需使用[!DNL Workfront]設定[!DNL Slack]的詳細資訊，請參閱[為 [!DNL Adobe Workfront] 設定 [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md)。

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

您必須先從[!DNL Workfront]搜尋[!DNL Slack]個專案

* 為[!DNL Workfront]設定[!DNL Slack]\
   如需設定[!DNL Workfront for Slack]的說明，請參閱[設定 [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md)。

## 從[!DNL Workfront]搜尋[!DNL Slack]個專案：

1. 登入您的[!DNL Slack]執行個體並從[!DNL Workfront]登入[!DNL Slack]。\
   如需有關從[!DNL Workfront]登入[!DNL Slack]的詳細資訊，請參閱[!DNL Workfront]Access[!DNL Slack]from[中的「從 [!DNL Adobe Workfront] 登入 [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md)」區段。

1. 從任何頻道，開始在訊息欄位中輸入以下任一命令：

   `/workfront search <keyword>`

   或

   `/wf search <keyword>`

   >[!NOTE]
   >
   >命令區分大小寫。 關鍵字不區分大小寫，而且輸入時必須不含括弧或引號。

1. 在出現的欄位中，從下列選項中選取物件型別：

   * 專案
   * 任務
   * 問題
   * 報表
   * 人員
   * 範本
   * 文件
   * 產品組合
   * 方案
   * 控制面板
   * 公司
   * 備註

     您一次只能選取一個物件型別。\
      符合搜尋條件的專案清單隨即顯示。

1. 按一下專案名稱，在新的瀏覽器分頁中於[!DNL Workfront]開啟它。
