---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 「檢視：透過縮排任務來顯示任務中的父子關係」
description: 您可以在匯出的工作清單中維持父子關係的差異，方法是在工作清單中加入自訂檢視，並確保在您匯出清單之前已選取此檢視。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 4987501f-a1d9-47cd-bfbe-83acfc225204
source-git-commit: 0483230c5d8b7d33f420c6c5f09c4a5aafe37f37
workflow-type: tm+mt
source-wordcount: '299'
ht-degree: 2%

---

# 檢視：透過縮排任務來顯示任務中的父子關係

您可以在匯出的工作清單中維持父子關係的差異，方法是在工作清單中加入自訂檢視，並確保在您匯出清單之前已選取此檢視。

![](assets/parent-child-indented-custom-view-350x94.png)

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>請求修改檢視 </p>
   <p>計畫修改報表</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>編輯報告、儀表板、行事曆的存取權以修改報告</p> <p>編輯對篩選器、檢視、群組的存取權以修改檢視</p> <p><b>附註</b>

如果您還是沒有存取權，請詢問您的Workfront管理員，他們是否在您的存取層級中設定其他限制。 如需有關Workfront管理員如何修改您的存取層級的資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理報表的許可權</p> <p>如需請求其他存取許可權的詳細資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">要求物件的存取權 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的Workfront管理員。

## 透過縮排任務來顯示任務中的父子關係

1. 前往含有您要匯出之工作清單的專案。
1. 按一下 **檢視** 下拉式功能表，然後選取 **新檢視**.

1. 在熒幕左上角為篩選器命名。
1. 按一下 **任務名稱** 欄標題。

1. 選取 **切換到文字模式** 在右上角。
1. 按一下文字方塊中的任意位置以編輯文字，並移除所有現有文字。
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

1. 按一下「**儲存**」。
1. 按一下「**儲存視圖**」。
