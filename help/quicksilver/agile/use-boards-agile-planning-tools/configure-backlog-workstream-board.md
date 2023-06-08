---
filename: configure-backlog-workstream-board.md
content-type: reference
navigation-topic: boards
title: 在工作流程展示板上設定待處理專案
description: 您可以選擇在工作流程中的展示板上顯示未交訂單欄位，並為從工作流程卡清單提取到展示板未交訂單中的卡片定義查詢。
author: Lisa
exl-id: fd2f6eeb-a565-4461-a153-0504ad3c07d7
source-git-commit: fffbf47e75e5ff1b6cd7ce37e0198a07459006da
workflow-type: tm+mt
source-wordcount: '472'
ht-degree: 0%

---

# 在工作流程展示板上設定待處理專案

您可以選擇在工作流程中的展示板上顯示未交訂單欄位，並為從工作流程卡清單提取到展示板未交訂單中的卡片定義查詢。

>[!NOTE]
>
>如果您在待處理專案欄中新增不符合查詢條件的新卡片，當展示板重新整理時，卡片會從待處理專案消失，而且只能用於卡片清單中。 您可以隨時變更查詢，以調整哪些卡片會顯示在待處理專案欄中。

未交訂單欄和查詢無法在獨立面板上使用。 如需有關將輸入欄新增至獨立展示板的資訊，請參閱 [將輸入欄新增到展示板](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md).

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
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 授權*</strong></td> 
   <td> <p>[！UICONTROL Request]或更高版本</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有哪些計畫、授權型別或存取權，請聯絡您的 [!DNL Workfront] 管理員。

## 在工作流程展示板上設定待處理專案

{{step1-to-boards}}

1. 開啟您要使用的工作流程。 若要開啟工作流程，請按一下 [!UICONTROL **檢視工作流程**].
1. 按一下工作流程中的任何展示板以開啟。
1. 按一下 [!UICONTROL **設定**] 以開啟「設定」面板。
1. 開啟 [!UICONTROL **在此展示板上加入待處理專案欄**].

   待處理專案欄會新增在展示板的左側。 在您對其套用查詢之前，它會保持空白。

1. 展開 [!UICONTROL **待處理專案查詢**].

   >[!NOTE]
   >
   >預設查詢可能已套用至待處理專案，顯示卡片清單中所有具有狀態且狀態為「未完成」的工作專案。

1. 按一下 [!UICONTROL **新增條件**] ，然後按一下「空白」欄位。
1. 選取查詢依據的欄位。

   您可以選擇的欄位是卡片上的預設欄位。

1. 選取查詢修正因子。

   修飾元選項視其可套用的欄位而定。 例如，「name」欄位不以「大於」或「小於」作為修飾詞選擇，因為這些修飾詞僅適用於數字。

1. 選取值。

   當您使用「exists」或「not exists」作為修飾元時，值不可用。

   例如，如果您選擇「到期日」和「存在」，則待處理專案會顯示具有指定到期日的卡片。 任何沒有到期日的卡片都不會提取到待處理專案中。

1. （可選）按一下 [!UICONTROL **新增條件**] 以新增其他條件至查詢。

   ![待辦項目查詢](assets/backlog-query-wrkstrm-board.png)

1. （可選）按一下 [!UICONTROL **建立群組**] 使用OR運運算元新增連線到第一個條件的一組條件。
1. 按一下 [!UICONTROL **儲存查詢**].

   會套用查詢，符合條件的卡片會出現在待處理專案欄中。
