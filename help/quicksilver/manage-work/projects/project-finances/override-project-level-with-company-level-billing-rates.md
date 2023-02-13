---
product-area: projects
navigation-topic: financials
title: 用公司層開單費率改寫項目層開單費率
description: 用公司層開單費率改寫項目層開單費率
author: Alina
feature: Work Management
exl-id: 02ea4c7c-0473-4cc4-913c-3baa613767b7
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '485'
ht-degree: 0%

---

# 用公司層開單費率改寫項目層開單費率

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: THIS IS LINKED TO THE UI IN THE EDIT PROJECT MODAL)</p>
-->

您可以將專案設定為使用公司層級的計費費率，而非專案層級的計費費率。

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

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
   <td> <p>計劃 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯對項目和財務資料的訪問</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>使用管理財務的權限管理項目的權限</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 啟用公司層開單費率改寫選項

當公司與項目關聯並啟用此選項時，對公司層開單費率所做的更改將覆蓋項目上設定的開單費率。

當用戶手動重新計算項目的財務時，將應用對公司層開單費率的任何更改。 除非將歷史收入計算標籤為開單，否則也會改寫它們。

1. 前往專案。
1. 按一下 **更多** 功能表 ![](assets/qs-more-icon-on-an-object.png) 在標題中專案名稱旁，按一下 **編輯**.
1. 在 **金融** 部分，啟用 **允許公司層開單費率改寫項目層開單費率**.

   >[!CAUTION]
   >
   >啟用此選項會覆寫歷史收入計算，除非標示為已計費。 您可以建立開單記錄，以保留歷史收入計算。 如需詳細資訊，請參閱文章 [建立計費記錄](../../../manage-work/projects/project-finances/create-billing-records.md)

1. 按一下 **儲存變更**.

## 更新公司層開單費率，並將其應用於項目

在您啟用了項目上的公司層開單費率改寫選項後，每當重新計算財務時，對公司開單費率所做的更改都將應用於項目。

>[!NOTE]
>
>使用者必須在其存取層級中擁有公司的存取權，才能更新公司層級的計費率。

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **設定**.
1. 按一下 **公司**.
1. 按一下與項目關聯的公司名稱，您為其啟用了公司層開單費率改寫。
1. 按一下 **計費率** 中。
1. 在 **公司帳單率** 欄位，然後按Enter。
1. 要更新一個或多個項目的公司費率，請執行以下操作之一：

   * 多個專案：
   1. 前往專案清單。
   1. 選取符合您要更新專案的核取方塊。
   1. 按一下 **編輯**.
   1. 在「設定」區段中，啟用 **重新計算成本和收入** 選項。
   1. 按一下 **儲存變更**.
   * 單一專案：

      1. 轉到啟用公司層開單費率改寫的項目。
      1. 按一下 **更多** 功能表 ![](assets/qs-more-icon-on-an-object.png) 在標題中專案名稱旁，按一下 **重新計算財務**.
