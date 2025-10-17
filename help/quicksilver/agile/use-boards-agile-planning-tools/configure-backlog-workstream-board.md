---
filename: configure-backlog-workstream-board.md
content-type: reference
navigation-topic: boards
title: 設定工作流程展示板上的待處理專案
description: 您可以選擇在工作流程中的展示板上顯示待處理資料欄，並為從工作流程卡片清單提取到展示板待處理資料中的卡片定義查詢。
author: Jenny
feature: Agile
exl-id: fd2f6eeb-a565-4461-a153-0504ad3c07d7
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '487'
ht-degree: 0%

---

# 在工作流程展示板上設定待處理專案

>[!IMPORTANT]
>
>工作串流僅適用於特定客戶群組。

您可以選擇在工作流程中的展示板上顯示待處理資料欄，並為從工作流程卡片清單提取到展示板待處理資料中的卡片定義查詢。

>[!NOTE]
>
>如果您在待處理專案欄中新增不符合查詢條件的卡片，當展示板重新整理時，該卡片將從待處理專案中消失，並且只能在卡片清單中使用。 您可以隨時變更查詢，以調整哪些卡片會出現在待處理專案欄中。

待處理專案欄和查詢在獨立面板上無法使用。 如需將輸入資料行新增至獨立展示板的資訊，請參閱[將輸入資料行新增至展示板](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md)。

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
   <td> 
   <p>投稿人或以上</p> 
   <p>要求或更高版本</p>
   </td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 在工作流程展示板上設定待處理專案

{{step1-to-boards}}

1. 開啟您要使用的工作流。 若要開啟工作流程，請按一下[檢視工作流程]。[!UICONTROL ****]
1. 按一下工作流程中的任何展示板以開啟。
1. 按一下主機板右側的&#x200B;[!UICONTROL **[設定]**]&#x200B;以開啟[設定]面板。
1. 開啟&#x200B;[!UICONTROL **在此展示板上包含待處理專案欄**]。

   待處理專案欄會新增在展示板的左側。 在您對其套用查詢之前，它保持空白。

1. 展開&#x200B;[!UICONTROL **待處理專案查詢**]。

   >[!NOTE]
   >
   >預設查詢可能已套用至待處理專案，顯示卡片清單中所有具有狀態且狀態為未完成的工作專案。

1. 按一下&#x200B;[!UICONTROL **新增條件**]，然後按一下[空白]欄位。
1. 選取查詢依據的欄位。

   您可以選擇的欄位是卡片上的預設欄位。

1. 選取查詢修正因子。

   修飾元選項取決於可套用的欄位。 例如，「名稱」欄位沒有「大於」或「小於」作為修飾詞選擇，因為這些修飾詞僅適用於數字。

1. 選取值。

   當您使用「exists」或「not exists」作為修飾元時，無法使用值。

   例如，如果您選擇「到期日」和「存在」，待處理專案會顯示具有指派到期日的卡片。 沒有到期日期的任何卡片都不會提取到待處理專案。

1. （選擇性）按一下&#x200B;[!UICONTROL **新增條件**]&#x200B;以新增其他條件至查詢。

   ![待處理專案查詢](assets/backlog-query-wrkstrm-board.png)

1. （選擇性）按一下&#x200B;[!UICONTROL **建立群組**]，新增連線到第一個條件且運運算元為OR的條件群組。
1. 按一下&#x200B;[!UICONTROL **儲存查詢**]。

   會套用查詢，且符合條件的卡片會出現在待辦專案欄中。
