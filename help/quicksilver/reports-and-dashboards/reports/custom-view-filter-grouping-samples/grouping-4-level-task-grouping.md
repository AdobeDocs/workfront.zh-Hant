---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 「群組：Portfolio擁有者、方案擁有者、專案擁有者和專案狀態的4層級作業群組」
description: 此作業「群組」提供4個層次的「群組」。 在此情況下，任務會依Portfolio所有者、方案所有者、專案所有者和專案狀態分組。 使用標準介面，您最多只能有3個層級的「群組」。 若要新增第四個層級，您必須使用文字模式。 您無法同時依照超過4個准則將報表分組。
author: Nolan
feature: Reports and Dashboards
exl-id: a1780a57-b94c-4d3a-b526-9bf45dba21f1
source-git-commit: 7b25d3b5fe69f610e245db5ada116ea967f22c7b
workflow-type: tm+mt
source-wordcount: '379'
ht-degree: 0%

---

# 群組：Portfolio擁有者、方案擁有者、專案擁有者和專案狀態的4層作業群組

<!--Audited: 10/2024-->

此作業「群組」提供4個層次的「群組」。 在此情況下，任務會依Portfolio所有者、方案所有者、專案所有者和專案狀態分組。 使用標準介面，您最多只能有3個層級的「群組」。 若要新增第四個層級，您必須使用文字模式。 您無法同時依照超過4個准則將報表分組。

![four_tier_grouping_for_tasks.png](assets/four-tier-grouping-for-tasks-350x239.png)

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> 
    <p>新增：</p>
   <ul><li><p>修改篩選器的貢獻者 </p></li>
   <li><p>用於修改報告的標準</p></li> </ul>

<p>目前：</p>
   <ul><li><p>請求修改篩選器 </p></li>
   <li><p>計畫修改報表</p></li> </ul></td> 
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

*如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 為Portfolio擁有者、方案擁有者、專案擁有者和專案狀態建立4層級任務群組

若要套用此群組：

1. 前往工作清單。
1. 從&#x200B;**群組**&#x200B;下拉式功能表中，選取&#x200B;**新群組**。

1. 按一下&#x200B;**切換到文字模式**。
1. 移除&#x200B;**將您的報告分組**&#x200B;區域中的文字。
1. 使用下列程式碼取代方塊中的文字：
   <pre>group.0.linkedname=project<br>group.0.name=Portfolio所有者<br>group.0.notime=false<br>group.0.valuefield=project:portfolio:owner：name<br>group.0.valueformat=string<br>group.1.linkedname=project<br>group.1.name=Program Owner<br>group.1.notime=false<br>group.1.valuefield=project:program:owner：name<br>group.1.valueformat=string<br>group.2.linkedname=projectOwnerOwnerMM <br>GROUP.2.LISTGROUINGPARSEDMETHOD=NESTED(PROJECT)。NESTED(OWNER)。STRING(NAME)<br>GROUP.2.NAMEKEY=PROJECTOWNERMM<br>GROUP.2.NOTIME=FALSE<br>GROUP.2.VALUEFIELD=PROJECTOWNERMM：name<br>group.2.valueformat=string<br>group.3.enumclass=com.attask.common.constants.ProjectStatusEnum<br>group.3.linkedname=project<br>group.3.group.3 namekey=view.relatedcolumn<br>group.3.namekeyargkey.0=project<br>group.3.namekeyargkey.1=status<br>group.3.notime=false<br>group.3.valuefield=project：status<br>group.3.valueformat=val</pre>

1. 按一下&#x200B;**完成**，然後按一下&#x200B;**儲存群組**。
1. （選擇性）更新群組的名稱，然後按一下&#x200B;**儲存群組**。
