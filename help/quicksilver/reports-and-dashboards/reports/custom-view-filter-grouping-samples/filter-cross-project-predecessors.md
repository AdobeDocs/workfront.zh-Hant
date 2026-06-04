---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 篩選器：顯示不完整的跨專案前置任務
description: 此任務篩選器傳回不完整的跨專案前置任務。
author: Lisa and Courtney
feature: Reports and Dashboards
exl-id: 7ee2432c-1d82-454e-a73a-f1f6b6a5c10d
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/Z1eiFj8bs-qj9Jxs3m7GnYDZE-bBPvGHE3VFEv3DOFM
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 199
ht-degree: 8%

---

# 篩選器：顯示不完整的跨專案前置任務

<!--Audited: 10/2024-->

此任務篩選器傳回不完整的跨專案前置任務。

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

## 篩選跨專案前置任務

若要套用此篩選：

1. 前往工作清單或工作報告。
1. 從&#x200B;**篩選器**&#x200B;下拉式功能表中，選取&#x200B;**新增篩選器**。

1. （視條件而定）如果您從清單存取篩選器，請按一下&#x200B;**文字模式**；如果您從報表存取篩選器，請按一下&#x200B;**切換至文字模式**。
1. 在新區域中，貼上下列程式碼：
   <pre>前置任務MM：projectID=FIELD：projectID<br>前置任務MM：projectID_Mod=ne<br>percentComplete=100<br>percentComplete_Mod=ne</pre>

1. （視條件而定）如果您從報表存取篩選器，請按一下&#x200B;**儲存篩選器**；如果您從工作清單存取篩選器，請按一下&#x200B;**套用**，然後按一下&#x200B;**另存為新篩選器**。
