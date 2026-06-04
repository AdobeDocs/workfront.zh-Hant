---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 檢視：透過縮排任務來顯示任務中的父子關係
description: 您可以在匯出的工作清單中維持父子關係的差異，方法是在工作清單中加入自訂檢視，並確保在您匯出清單之前已選取此檢視。
author: Courtney
feature: Reports and Dashboards
exl-id: 4987501f-a1d9-47cd-bfbe-83acfc225204
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/QSBA40vOIbB8cm0YydDuJN9NS2X6SoXNF-dCBUHFniM
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 244
ht-degree: 6%

---

# 檢視：透過縮排任務來顯示任務中的父子關係

<!--Audited: 11/2024-->

您可以在匯出的工作清單中維持父子關係的差異，方法是在工作清單中加入自訂檢視，並確保在您匯出清單之前已選取此檢視。

![父子縮排](assets/parent-child-indented-custom-view-350x94.png)

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
   <p>投稿人或請求修改檢視 </p>
   <p>要修改報告的標準或計畫</p>
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>編輯報告、儀表板、行事曆的存取權以修改報告</p> <p>編輯對篩選器、檢視、群組的存取權以修改檢視</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理報表的許可權</p>  </td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。


+++

## 透過縮排任務來顯示任務中的父子關係

1. 前往含有您要匯出之工作清單的專案。
1. 按一下&#x200B;**檢視**&#x200B;下拉式功能表，然後選取&#x200B;**新增檢視**。
1. 在&#x200B;**工作名稱**&#x200B;欄標題中按一下。
1. 選取右上角的&#x200B;**切換至文字模式**。
1. 按一下&#x200B;**編輯文字模式**&#x200B;並移除所有現有文字。
1. 貼上下列文字：


   ```
   displayname=
   linkedname=direct
   namekey=name
   querysort=name
   textmode=true
   valueexpression=IF({indent}<1,{name},IF({indent}<2,CONCAT(" - ",{name}),IF({indent}<3,CONCAT(" - - ",{name}),IF({indent}<4,CONCAT(" - - - ",{name}),CONCAT(" - - - - ",{name})))))
   valueformat=HTML
   ```

1. 按一下&#x200B;**完成** > **儲存檢視**。
