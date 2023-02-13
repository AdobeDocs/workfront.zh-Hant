---
title: 查看和導出審核日誌
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: 您可以檢視系統中的所有稽核記錄，或符合特定篩選條件的稽核記錄。 您也可以匯出稽核記錄。 稽核記錄會列出過去90天內，在系統中觸發的使用者變更。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: b04e8ba5-c3f2-4838-8df1-35e90de5c7bd
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '322'
ht-degree: 0%

---

# 查看和導出審核日誌

<!--
**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **
-->

您可以檢視系統中的所有稽核記錄，或符合特定篩選條件的稽核記錄。 您也可以匯出稽核記錄。

稽核記錄會列出過去90天內，在系統中觸發的使用者變更。

有關所有審核日誌類型及其生成內容的資訊，請參見 [稽核記錄](../../../administration-and-setup/add-users/create-and-manage-users/audit-logs.md).

## 存取需求

您必須具備下列條件才能執行本文所述步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td> <p>計劃 </p> <p>您必須是Workfront管理員。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 查看審核日誌

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **設定** ![](assets/gear-icon-settings.png).

1. 在左側面板中，按一下 **系統>審核日誌**.
1. 在 **記錄類型** 下拉式功能表，選取您要檢視的稽核記錄類型。

   **所有日誌類型** 預設為選取。

   有關您可以查看的所有審核日誌類型及其包含的資訊的清單，請參見 [稽核記錄](../../../administration-and-setup/add-users/create-and-manage-users/audit-logs.md).

1. （選用）設定任何可用的篩選器。

   >[!NOTE]
   >
   >「動作類型」下拉式功能表中的選項會依所選稽核記錄而有所不同。

   ![](assets/audit-logs.jpg)

1. 按一下 **套用**.
1. （選用）按一下 **清除篩選器** 重設對篩選器所做的變更。

## 導出審核日誌

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **設定** ![](assets/gear-icon-settings.png).

1. 在左側面板中，按一下 **系統>審核日誌**.

1. 在 **記錄類型** 下拉式功能表，選取稽核記錄。

   **所有日誌類型** 預設為選取。

1. 設定任何可用的篩選器，然後按一下 **套用**.

   >[!IMPORTANT]
   >
   >一次無法匯出超過50,000個日誌。 Workfront會根據您設定的篩選器匯出記錄檔，而非頁面上顯示的記錄檔數。 您可以在頁面的右下角檢視經過篩選記錄的總數。

1. 按一下 **匯出**.
