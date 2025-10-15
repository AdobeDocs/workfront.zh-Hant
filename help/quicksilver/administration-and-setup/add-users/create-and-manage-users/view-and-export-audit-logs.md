---
title: 檢視和匯出稽核記錄
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: 您可以檢視系統中的所有稽核記錄，或符合特定篩選條件的稽核記錄。 您也可以匯出稽核記錄。 稽核記錄列出過去90天內系統中觸發的使用者變更。
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: b04e8ba5-c3f2-4838-8df1-35e90de5c7bd
source-git-commit: c8987d036e1c1324618cb53ebcbb8fd7e4bcc6a4
workflow-type: tm+mt
source-wordcount: '413'
ht-degree: 1%

---

# 檢視和匯出稽核記錄

<!--Audited: 08/2025-->

<!--
**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **
-->

您可以檢視系統中的所有稽核記錄，或符合特定篩選條件的稽核記錄。 您也可以將稽核記錄匯出至CSV檔案。

稽核記錄列出過去90天內系統中觸發的使用者變更。

如需有關所有稽核記錄型別及其產生原因的資訊，請參閱[稽核記錄概觀](../../../administration-and-setup/add-users/create-and-manage-users/audit-logs.md)。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront套件</td> 
   <td><p>任何</p></td> 
  </tr> 
  <tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td><p>標準</p>
       <p>規劃</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td><p>系統管理員</p></td>
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

<!--Old: 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td><p>Any</p></td> 
  </tr> 
  <tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td><p>Standard</p>
       <p>Plan</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td><p>System Administrator</p></td>
  </tr> 
 </tbody> 
</table>-->

## 檢視稽核記錄

{{step-1-to-setup}}

1. 在左側面板中，按一下&#x200B;**系統>稽核記錄**。
1. 在&#x200B;**動作型別**&#x200B;下拉式清單中，選取您要檢視的稽核型別。

   >[!NOTE]
   >
   >「動作型別」下拉式功能表中的選項會依選取的稽核記錄而有所不同。

1. 在&#x200B;**記錄型別**&#x200B;下拉式功能表中，選取您要檢視的稽核記錄型別。

   依預設會選取&#x200B;**所有記錄型別**。

   如需您可以檢視的所有稽核記錄型別及其包含資訊的清單，請參閱[稽核記錄概觀](../../../administration-and-setup/add-users/create-and-manage-users/audit-logs.md)。

1. （選用）為下列欄位設定任何可用的篩選器：

   * **使用者**：輸入進行變更的使用者名稱。
   * **從**：進行變更的時間範圍開始日期。
   * **至**：進行變更時時間範圍的結束日期。

   ![稽核記錄](assets/audit-logs.png)

1. 按一下&#x200B;**套用**。
1. （選擇性）按一下&#x200B;**清除**&#x200B;以重設對篩選器所做的變更。

## 匯出稽核記錄

{{step-1-to-setup}}

1. 在左側面板中，按一下&#x200B;**系統** > **稽核記錄**。

1. 在&#x200B;**記錄型別**&#x200B;下拉式功能表中，選取稽核記錄。

   依預設會選取&#x200B;**所有記錄型別**。

1. 設定任何可用的篩選器，然後按一下&#x200B;**套用**。

   >[!IMPORTANT]
   >
   >您無法一次匯出超過50,000個記錄。 Workfront會根據您設定的篩選器匯出記錄，而不是根據頁面上顯示的記錄數量。 您可以在頁面的右下角檢視篩選的記錄總數。

1. 按一下&#x200B;**匯出**。

   儲存檔案方塊開啟，您可以將匯出的檔案儲存在電腦上。

   您只能將稽核記錄儲存為CSV格式。

   完成儲存匯出的檔案。 您現在可以在電腦上找到它，並與他人共用。
