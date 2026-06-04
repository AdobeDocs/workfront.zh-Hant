---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 篩選：當狀態與不同群組相關聯時，依相同名稱狀態顯示專案
description: 您可以將具有3個字母鍵NST的任務狀態指派給群組A （已命名的新狀態）。 您可能有另一個任務狀態指派給群組B，也命名為New Status ，帶有3個字母的索引鍵NES。 雖然2個狀態的名稱可以相同，但3個字母的程式碼永遠都是唯一的。 如需群組狀態的詳細資訊，請參閱建立或編輯群組狀態。
author: Courtney
feature: Reports and Dashboards
exl-id: 8ddcd8b1-44a9-4341-80c7-76ba70d2953b
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/qOu5WArxekdKKXAswMAtapaOHX36J9vGMpUom614lvE
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 479
ht-degree: 3%

---

# 篩選：當狀態與不同群組相關聯時，依相同名稱狀態顯示專案

<!--Audited: 10/2024-->

您可以讓任務狀態指派給群組A （名稱為&#x200B;*新狀態*，包含3個字母的索引鍵&#x200B;*NST*）。 您可能有另一個工作狀態指派給群組B，也命名為&#x200B;*新狀態*，含有3個字母的索引鍵&#x200B;*NES。* 雖然2個狀態的名稱可以相同，但3個字母的程式碼永遠都是唯一的。

如需群組狀態的詳細資訊，請參閱[建立或編輯群組狀態](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md)。

使用篩選產生器，您無法識別具有相同名稱的2個狀態。 您必須在自訂篩選器中使用文字模式，以區分2種狀態。

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
   <td> 
   <p>修改篩選器的貢獻者或請求 </p>
   <p>要修改報告的標準或計畫</p>
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>編輯報告、儀表板、行事曆的存取權以修改報告</p> <p>編輯篩選器、檢視和群組的存取權以修改篩選器</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理報表的許可權</p>  </td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 當狀態與不同群組相關聯時，依相同名稱狀態顯示專案

1. 例如，移至您要自訂工作清單之篩選器的&#x200B;**篩選器**&#x200B;下拉式清單。\
   這也適用於專案和問題。
1. 按一下&#x200B;**新增篩選器**。
1. 從左上角的第一個下拉式清單中，選取工作>狀態。
1. 選取修飾元的&#x200B;**等於**，然後選取您要報告的其中一個狀態。

   例如，在任務報告中，如果您只想顯示狀態為&#x200B;**新狀態**&#x200B;的任務，請新增&#x200B;**狀態等於新狀態**。

   >[!TIP]
   >
   >請注意，對於名為「新狀態」的狀態，您只有一個選項。

1. 按一下&#x200B;**文字模式**。\
   下列程式碼應顯示在提供的空白處：

   <pre>OR:1:狀態=NST<br>OR:1:狀態_模式=in </pre>

   >[!NOTE]
   >
   >此處只顯示一個狀態。 狀態行會顯示其中一個狀態的3個字母鍵之一。

1. 新增下列2行程式碼，以新增篩選器中缺少的狀態：

   <pre>OR:2:狀態=NES<br>OR:2:狀態_模式=in</pre>

1. 按一下&#x200B;**套用**，然後按&#x200B;**另存新檔**。

   清單會顯示群組A的「新狀態」狀態與群組B的「新狀態」狀態任務。
