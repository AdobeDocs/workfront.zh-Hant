---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 檢視：透過縮排任務來顯示任務中的父子關係
description: 您可以在匯出的工作清單中維持父子關係的差異，方法是在工作清單中加入自訂檢視，並確保在您匯出清單之前已選取此檢視。
author: Nolan
feature: Reports and Dashboards
exl-id: 4987501f-a1d9-47cd-bfbe-83acfc225204
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '260'
ht-degree: 0%

---

# 檢視：透過縮排任務來顯示任務中的父子關係

<!--Audited: 11/2024-->

您可以在匯出的工作清單中維持父子關係的差異，方法是在工作清單中加入自訂檢視，並確保在您匯出清單之前已選取此檢視。

![父子縮排](assets/parent-child-indented-custom-view-350x94.png)

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
   <td role="rowheader">Adobe Workfront授權</td> 
   <td> <p> 目前： 
   <ul>
   <li>請求修改檢視</li> 
   <li>計畫修改報表</li>
   </ul>
     </p>
     <p> 新增： 
   <ul>
   <li>修改檢視的貢獻者</li> 
   <li>用於修改報告的標準</li>
   </ul>
     </p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>編輯報告、儀表板、行事曆的存取權以修改報告</p> <p>編輯對篩選器、檢視、群組的存取權以修改檢視</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理報表的許可權</p> </td> 
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
