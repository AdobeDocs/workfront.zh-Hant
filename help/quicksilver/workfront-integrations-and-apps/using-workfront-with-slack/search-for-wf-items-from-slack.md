---
product-area: workfront-integrations
navigation-topic: workfront-for-slack
title: 搜尋來自 [!DNL Slack]的 [!DNL Adobe Workfront] 個專案
description: 您可以從已安裝的 [!DNL Slack], if your instance of Slack has had the [!DNL Workfront] 應用程式搜尋 [!DNL Adobe Workfront] 專案。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 85821f21-d4fd-4f28-bd7a-0c109a4433a8
TQID: https://experienceleague.adobe.com/JulYq173XQa6mG93qzUwfBDn4TPVEafD2OVpcIAXxi8
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
subfeature_v2:
  - id: e4fedd42-4a54-4109-859f-13c7f0366a72
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 208
ht-degree: 15%

---

# 從[!DNL Slack]搜尋[!DNL Adobe Workfront]個專案

如果您的[!DNL Slack]執行個體已安裝[!DNL Workfront]應用程式，您可以從[!DNL Slack]搜尋[!DNL Adobe Workfront]專案。

如需使用[!DNL Slack]設定[!DNL Workfront]的詳細資訊，請參閱[為 [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md)設定 [!DNL Adobe Workfront] 。

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
   <td> <p>任何</p>
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先決條件

您必須先從[!DNL Slack]搜尋[!DNL Workfront]個專案

* 為[!DNL Slack]設定[!DNL Workfront]\
   如需設定[!DNL Workfront for Slack]的說明，請參閱[設定 [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md)。

## 從[!DNL Slack]搜尋[!DNL Workfront]個專案：

1. 登入您的[!DNL Slack]執行個體並從[!DNL Slack]登入[!DNL Workfront]。\
   如需有關從[!DNL Slack]登入[!DNL Workfront]的詳細資訊，請參閱[Access [!DNL Adobe Workfront] from [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md)中的「從[!DNL Slack]登入[!DNL Workfront]」區段。

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
   * 報告
   * 人員
   * 範本
   * 文件
   * 專案組合
   * 方案
   * 儀表板
   * 公司
   * 備註

     您一次只能選取一個物件型別。\
      符合搜尋條件的專案清單隨即顯示。

1. 按一下專案名稱，在新的瀏覽器分頁中於[!DNL Workfront]開啟它。
