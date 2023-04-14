---
filename: configure-backlog-workstream-board.md
content-type: reference
navigation-topic: boards
title: 配置工作流板上的積壓
description: 您可以選擇在工作流中的展示板上顯示積壓列，並為從工作流卡片清單提取到展示板積壓中的卡片定義查詢。
author: Lisa
exl-id: fd2f6eeb-a565-4461-a153-0504ad3c07d7
source-git-commit: 75bb5af9564947a39e1cb46f9d6be2c03eb07acc
workflow-type: tm+mt
source-wordcount: '416'
ht-degree: 0%

---

# 配置工作流板上的積壓

您可以選擇在工作流中的展示板上顯示積壓列，並為從工作流卡片清單提取到展示板積壓中的卡片定義查詢。 獨立展示板上不提供這些選項。 有關向獨立主板添加進氣列的資訊，請參見 [向展示板新增進紙欄](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md).

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 計劃*</strong></td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 授權*</strong></td> 
   <td> <p>[!UICONTROL Request]或更高版本</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的 [!DNL Workfront] 管理員。

## 配置工作流板上的積壓

{{step1-to-boards}}

1. 開啟您要使用的工作流。 若要開啟工作流，請按一下 [!UICONTROL **檢視工作流**].
1. 按一下工作流中的任何展示板以開啟它。
1. 按一下 [!UICONTROL **設定**] ，開啟「設定」面板。
1. 開啟 [!UICONTROL **在此板上包含積壓工作列**].

   積壓欄會新增在展示板左側。 在您將查詢套用至查詢之前，它會保留空白。

1. 展開 [!UICONTROL **積壓查詢**].

   >[!NOTE]
   >
   >預設查詢可能已應用於積壓，顯示卡清單中不屬於小版本且未處於「完成」狀態的所有工作項。

1. 按一下 [!UICONTROL **新增條件**] 然後按一下「空白」欄位。
1. 選擇要查詢的欄位。

   您可以選擇的欄位是卡片上的預設欄位。

1. 選擇查詢修改量。

   修飾詞選項取決於可套用的欄位。 例如，「名稱」欄位沒有「大於」或「小於」作為修飾詞選擇，因為這些修飾詞只適用於數字。

1. 選取值。

   當您使用「exists」或「not exists」作為修飾詞時，此值不可用。

   例如，如果您選擇「到期日」和「存在」，積壓工作將顯示具有指派到期日的卡片。 任何沒有到期日的卡都不會被提取至積壓工作。

1. （選用）按一下 [!UICONTROL **新增條件**] 以新增其他條件至查詢。

   ![待辦項目查詢](assets/backlog-query-wrkstrm-board.png)

1. （選用）按一下 [!UICONTROL **建立群組**] 新增一組以OR運算子連線至第一個條件的條件。
1. 按一下 [!UICONTROL **保存查詢**].

   系統會套用查詢，且符合條件的卡片會出現在積壓欄中。
