---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: 篩選按鈕不會顯示在頁首中
description: 請參閱本文，疑難排解未在頁面標題中顯示的篩選按鈕。
feature: Get Started with Workfront
author: Lisa and Alina
exl-id: 327564ed-60df-441a-a38b-a17a8c57adb0
source-git-commit: 210ca2e82286ff904bc7defb7b8c9c2559489d66
workflow-type: tm+mt
source-wordcount: '276'
ht-degree: 1%

---

# 篩選按鈕不會顯示在頁首中

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 計劃</strong></td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe [!DNL Workfront] 授權</strong></td> 
   <td> <p>[!UICONTROL計畫] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>訪問級別配置</strong></td> 
   <td> <p>[!UICONTROL系統管理員]</p> </td> 
  </tr> 
 </tbody> 
</table>

## 問題

下列篩選按鈕不會顯示在其各自的區域中：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>[!DNL Adobe Workfront] 區域</strong></td> 
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
     <li> <p><span>[!UICONTROL我的時間表批准]</span> </p> </li> 
     <li> <p><span>[!UICONTROL我的工時單]</span> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## 解決方案

中的篩選按鈕 [!UICONTROL 項目和工時單] 不會顯示區域，因為對應的篩選器未包含在套用至使用者的版面範本中。 此 [!DNL Workfront] 管理員必須指派包含篩選器的配置範本。

>[!NOTE]
>
>有時候篩選器會從 [!UICONTROL 清單控制項] 區域 [!UICONTROL 設定]. 此 [!DNL Workfront] 管理員必須將它們納入此區域的清單中，才能在版面範本中使用。

1. 確認版面範本顯示下列篩選器：

   * [!UICONTROL 正在執行的項目] 和 [!UICONTROL 我擁有的專案] 在 [!UICONTROL 專案] 區域
   * [!UICONTROL 我的時間表批准] 和 [!UICONTROL 我的工時單] 在 [!UICONTROL 工時單] 區域

   要執行此操作：

   1. 存取版面範本。
   1. 選擇 **[!UICONTROL 清單]** 在 **[!UICONTROL 自訂使用者看見的項目]**.
   1. 選擇 **[!UICONTROL 專案]** 或 **[!UICONTROL 工時單]** 在 **[!UICONTROL 選取要自訂的清單]**.
   1. 在 **[!UICONTROL 篩選]** 部分，驗證 **[!UICONTROL 正在執行的項目]**, **[!UICONTROL 我擁有的專案]** （專案）及 **[!UICONTROL 我的時間表批准]** 和 **[!UICONTROL 我的工時單]** （對於工時單）。
   1. 按一下&#x200B;**[!UICONTROL 儲存]**。

   如需詳細資訊，請參閱 [使用版面範本自訂篩選器、檢視和群組](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md).

1. 將版面範本指派給正確的使用者、工作角色、團隊或群組。 如需詳細資訊，請參閱 [將使用者指派至版面範本](../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md).
