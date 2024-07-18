---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 「群組：任務百分比劃分2」
description: 「在此自訂任務分組中，您可以顯示按任務完成百分比值範圍分組的任務。 劃分會以10%的增量顯示完成百分比值：1-10%、11-20%等
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 7d5a40dd-d451-48c7-9323-af52aa387709
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '355'
ht-degree: 0%

---

# 群組：任務百分比劃分2

在此自訂任務分組中，您可以顯示按任務完成百分比值範圍分組的任務。 劃分會以10%的增量顯示完成百分比值：1-10%、11-20%等。

下列群組會依完成百分比值將專案組織為下列其中一個群組：

* 0%
* 1-10%
* 11-20%
* 21-30%
* 31-40%
* 41-50%
* 51-60%
* 61-70%
* 71-80%
* 81-90%
* 91-99%
* 100%

![task_10__breakdown_grouping.png](assets/task-10--breakdown-grouping-350x547.png)

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
   <td> <p>請求修改分組 </p>
   <p>計畫修改報表</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>編輯報告、儀表板、行事曆的存取權以修改報告</p> <p>編輯對篩選器、檢視、群組的存取權以修改群組</p> <p><b>附註</b>

如果您還是沒有存取權，請詢問您的Workfront管理員，他們是否在您的存取層級中設定其他限制。 如需Workfront管理員如何修改存取層級的詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>。</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理報表的許可權</p> <p>如需請求其他存取權的資訊，請參閱<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求物件</a>的存取權。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的Workfront管理員。

## 依任務百分比劃分分組

若要套用此群組：

1. 前往工作清單。
1. 從&#x200B;**群組**&#x200B;下拉式功能表中，選取&#x200B;**新群組**。

1. 按一下&#x200B;**切換到文字模式**。
1. 移除&#x200B;**將您的報告分組**&#x200B;區域中的文字。
1. 將文字取代為下列程式碼：
   <pre>group.0.linkedname=direct<br>group.0.name=Percent Breakdown<br>group.0.notime=false<br>group.0.valueexpression=IF({percentComplete}=0，"0 %"，IF({percentComplete}&lt;=11，"1-10 %"，IF({percentComplete}&lt;=21，"11-20 %"，IF({percentComplete}&lt;=31，"21-30 %"，IF({percentComplete}&lt;41，"31-40 %"，IF( 8}&lt;51，"41-50 %"，IF({percentComplete}&lt;61，"51-60 %"，IF({percentComplete}&lt;71，"61-70 %"，IF({percentComplete}&lt;81，"71-80 %"，IF({percentComplete}&lt;91，"81-90 %"，IF({percentComplete}&lt;100，"91-99 %"，"100 %"))))))))))<br>textmode=true{percentComplete}</pre>

1. 按一下&#x200B;**儲存群組**。
