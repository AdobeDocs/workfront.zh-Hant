---
product-area: projects
navigation-topic: financials
title: 以公司層級的收費率覆寫專案層級的收費率
description: 以公司層級的收費率覆寫專案層級的收費率
author: Lisa
feature: Work Management
exl-id: 02ea4c7c-0473-4cc4-913c-3baa613767b7
source-git-commit: b983a780198743a2b87b4b48cf4d6afdf1cee437
workflow-type: tm+mt
source-wordcount: '476'
ht-degree: 1%

---

# 以公司層級的收費率覆寫專案層級的收費率

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: THIS IS LINKED TO THE UI IN THE EDIT PROJECT MODAL)</p>
-->

您可以將專案設定為使用公司層級的收費率，而非專案層級的收費率。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

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
   <td>
   <p>新增：標準</p>
   <p>或</p>
   <p>目前：計畫</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td>編輯專案與財務資料的存取權</td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td>管理具有管理財務之許可權的專案許可權</td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 啟用公司層級收費率覆寫選項

當公司與專案相關聯且啟用此選項時，對公司層級計費率所做的變更將會覆寫專案上設定的計費率。

當使用者手動重新計算專案的財務時，將套用公司層級計費率的任何變更。 除非標籤為已記帳，否則也會覆寫歷史收入計算。

1. 前往專案。
1. 按一下標題中專案名稱旁的&#x200B;**更多**&#x200B;功能表![更多](assets/qs-more-icon-on-an-object.png)，然後按一下&#x200B;**編輯**。
1. 在&#x200B;**財務**&#x200B;區段中，啟用&#x200B;**允許公司層級的收費率以覆寫專案層級的收費率**。

   >[!CAUTION]
   >
   >啟用此選項會覆寫歷史收入計算，除非將其標籤為已記帳。 您可以建立付費記錄，以保留歷史收入計算。 如需詳細資訊，請參閱文章[建立付費記錄](../../../manage-work/projects/project-finances/create-billing-records.md)

1. 按一下「**儲存變更**」。

## 更新公司層級收費率，並將其套用至專案

在您啟用專案的公司層級收費率覆寫選項後，對公司收費率所做的變更會在任何時候重新計算財務時套用至專案。

>[!NOTE]
>
>使用者必須擁有存取層級中公司的存取權，才能更新公司層級的計費費率。

{{step-1-to-setup}}

1. 按一下&#x200B;**公司**。
1. 按一下與您啟用公司層級收費率覆寫之專案相關聯的公司名稱。
1. 按一下左側面板中的&#x200B;**收費率**。
1. 更新現有職務角色的&#x200B;**公司收費率**&#x200B;和開始/結束日期，然後按Enter鍵。

   若要新增生效日期的公司收費率，請選取工作角色的收費率，然後按一下[編輯]。**** 如需日期有效公司收費率的詳細資訊，請參閱[覆寫公司層級的工作角色收費率](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/override-job-role-billing-rates-company-level.md)。

1. 若要更新一或多個專案的公司費率，請執行下列其中一項作業：

   * 多個專案：

      1. 前往專案清單。
      1. 勾選與您要更新專案相符的核取方塊。
      1. 按一下&#x200B;**編輯**。
      1. 在設定區段中，啟用&#x200B;**重新計算成本和收入**&#x200B;選項。
      1. 按一下「**儲存變更**」。

   * 單一專案：

      1. 移至您已啟用公司層級收費率覆寫的專案。
      1. 按一下標題中專案名稱旁的&#x200B;**更多**&#x200B;功能表![更多](assets/qs-more-icon-on-an-object.png)，然後按一下&#x200B;**重新計算財務**。
