---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 「檢視與分組：顯示依分組中平均值彙總的專案實際期間」
description: 您可以在專案報表中新增下列欄，以顯示分組中彙總為平均的實際期間。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 31794fe9-a04a-437d-8d2e-40e0cb6e6104
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '350'
ht-degree: 1%

---

# 檢視與分組：顯示依分組中平均值彙總的專案實際期間

您可以在專案報表中新增下列欄，以顯示分組中彙總為平均的實際期間。

![project_with_aggregate_actual_duration_in_grouping_view.png](assets/project-with-aggregate-actual-duration-in-grouping-view-350x65.png)

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

如果您還是沒有存取權，請詢問您的Workfront管理員，他們是否在您的存取層級中設定其他限制。 如需Workfront管理員如何修改存取層級的詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>。</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理報表的許可權</p> <p>如需請求其他存取權的資訊，請參閱<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求物件</a>的存取權。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的Workfront管理員。

## 顯示依分組中平均值彙總的專案實際期間

若要將此欄新增至專案檢視：

1. （建議）為獲得最佳結果及檢視實際期間彙總的平均值，您必須將分組新增至您的專案清單或報表。\
   如需建立群組的詳細資訊，請參閱文章[ Adobe Workfront中的群組概觀](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)。

1. 前往現有的專案檢視。
1. 展開[檢視]下拉式功能表，然後選取&#x200B;**自訂檢視**。
1. 按一下&#x200B;**新增資料行**。
1. 按一下&#x200B;**切換到文字模式**。
1. 將滑鼠移至此資料行&#x200B;**區域中的**&#x200B;顯示，然後按一下&#x200B;**按一下以編輯文字**。

1. 移除「文字模式」方塊中的所有文字，並以下列程式碼取代：
   <pre>aggregator.displayformat=compound <br>aggregator.function=AVG <br>aggregator.namekey=view.relatedcolumn <br>aggregator.namekeyargkey=actualduration <br>aggregator.valuefield=actualDurationMinutes <br>aggregator.valueformat=val <br>displayname=專案實際期間<br>durationunitfield=durationUnit.value <br>linkedname=project <br>linkedname=project <br>namenamicalduration namicationActualDuration numation namicationNamication實際期間{9實際期間{9實際期間{1Actual<br>namicationquerysort{querysort DurationMinutes <br>textmode=true <br>valuefield=actualDurationMinutes <br>valueformat=compound#M：D <br>viewalias=actualduration</pre>

1. 按一下「**儲存視圖**」。
