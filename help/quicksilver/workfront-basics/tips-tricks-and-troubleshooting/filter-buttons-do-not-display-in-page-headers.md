---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: 篩選器按鈕不顯示在頁眉中
description: 閱讀本文以排除未在頁眉中顯示的篩選器按鈕故障。
feature: Get Started with Workfront
author: Nolan and Alina
exl-id: 327564ed-60df-441a-a38b-a17a8c57adb0
source-git-commit: 114d306d99ae9ba0a18abd63a6137ad0568ab202
workflow-type: tm+mt
source-wordcount: '276'
ht-degree: 1%

---

# 篩選器按鈕不顯示在頁眉中

## 訪問要求

您必須具有以下訪問權限才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 計劃</strong></td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe [!DNL Workfront] 許可證</strong></td> 
   <td> <p>[!UICONTROL計畫] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>訪問級別配置</strong></td> 
   <td> <p>[!UICONTROL系統管理員]</p> </td> 
  </tr> 
 </tbody> 
</table>

## 問題

以下濾鏡按鈕不顯示在其各自的區域中：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>[!DNL Adobe Workfront] 面積</strong></td> 
   <td><strong>篩選按鈕</strong></td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL項目] </p> </td> 
   <td> 
    <ul> 
     <li> <p>[！我正在執行的UICONTROL項目]</p> </li> 
     <li> <p>[！我擁有的UICONTROL項目]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td><span>[!UICONTROL時間表]</span> </td> 
   <td> 
    <ul> 
     <li> <p><span>[!UICONTROL我的時間表審批]</span> </p> </li> 
     <li> <p><span>[!UICONTROL我的時間表]</span> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## 解決方案

中的篩選器按鈕 [!UICONTROL 項目和工時單] 不顯示區域，因為應用於用戶的佈局模板中不包含相應的篩選器。 的 [!DNL Workfront] 管理員必須分配包含篩選器的佈局模板。

>[!NOTE]
>
>有時，從 [!UICONTROL 清單控制項] 區域 [!UICONTROL 設定]。 的 [!DNL Workfront] 管理員必須將它們包括在此區域的清單中，才能在佈局模板中使用它們。

1. 驗證佈局模板是否顯示以下篩選器：

   * [!UICONTROL 正在執行的項目] 和 [!UICONTROL 我擁有的項目] 的 [!UICONTROL 項目] 面積
   * [!UICONTROL 我的時間表審批] 和 [!UICONTROL 我的工時單] 的 [!UICONTROL 工時單] 面積

   要執行此操作：

   1. 訪問佈局模板。
   1. 選擇 **[!UICONTROL 清單]** 在 **[!UICONTROL 自定義用戶查看的內容]**。
   1. 選擇 **[!UICONTROL 項目]** 或 **[!UICONTROL 工時單]** 在 **[!UICONTROL 選擇要自定義的清單]**。
   1. 在 **[!UICONTROL 篩選]** 部分，驗證 **[!UICONTROL 正在執行的項目]**。 **[!UICONTROL 我擁有的項目]** （用於項目）及 **[!UICONTROL 我的時間表審批]** 和 **[!UICONTROL 我的工時單]** （對於工時單）。
   1. 按一下&#x200B;**[!UICONTROL 儲存]**。

   有關詳細資訊，請參見 [使用佈局模板自定義篩選器、視圖和分組](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)。

1. 將佈局模板分配給正確的用戶、作業角色、團隊或組。 有關資訊，請參見 [將用戶分配到佈局模板](../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md)。
