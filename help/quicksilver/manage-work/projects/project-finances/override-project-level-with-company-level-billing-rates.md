---
product-area: projects
navigation-topic: financials
title: 以公司層級的收費率覆寫專案層級的收費率
description: 以公司層級的收費率覆寫專案層級的收費率
author: Alina
feature: Work Management
exl-id: 02ea4c7c-0473-4cc4-913c-3baa613767b7
source-git-commit: 8dbb48e6aa2df874caa816468cf2e3ad408ebf7e
workflow-type: tm+mt
source-wordcount: '550'
ht-degree: 0%

---

# 以公司層級的收費率覆寫專案層級的收費率

{{highlighted-preview}}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: THIS IS LINKED TO THE UI IN THE EDIT PROJECT MODAL)</p>
-->

您可以將專案設定為使用公司層級的收費率，而非專案層級的收費率。

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
   <td> <p>計劃 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>編輯對專案和財務資料的存取權</p> <p>注意：如果您仍然沒有存取權，請詢問您的Workfront管理員是否對您的存取層級設定了其他限制。 如需有關Workfront管理員如何修改您的存取層級的資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理具有管理財務許可權之專案的許可權</p> <p>如需請求其他存取許可權的詳細資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">要求物件的存取權 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的Workfront管理員。

## 啟用公司層級收費率覆寫選項

當公司與專案相關聯且啟用此選項時，對公司層級計費率所做的變更會覆寫專案上設定的計費率。

當使用者手動重新計算專案的財務時，會套用對公司層級計費率所做的任何變更。 除非標籤為已記帳，否則也會覆寫歷史收入計算。

1. 前往專案。
1. 按一下 **更多** 功能表 ![](assets/qs-more-icon-on-an-object.png) 在標題中專案名稱旁邊，然後按一下 **編輯**.
1. 在 **財務** 區段，啟用 **允許公司層級收費率覆寫專案層級收費率**.

   >[!CAUTION]
   >
   >啟用此選項會覆寫歷史收入計算，除非將其標籤為已記帳。 您可以建立付費記錄，以保留歷史收入計算。 如需詳細資訊，請參閱文章 [建立付費記錄](../../../manage-work/projects/project-finances/create-billing-records.md)

1. 按一下 **儲存變更**.

## 更新公司層級收費率並將其套用至專案

在您啟用專案的公司層級收費率覆寫選項後，對公司收費率所做的變更會在任何時候重新計算財務時套用至專案。

>[!NOTE]
>
>使用者必須在其存取層級中擁有對公司的存取權，才能更新公司層級的計費費率。

1. 按一下 **主要功能表** 圖示 ![](assets/main-menu-icon.png) Adobe Workfront右上角，然後按一下 **設定**.
1. 按一下 **公司**.
1. 按一下與您啟用公司層級收費率覆寫之專案相關聯的公司名稱。
1. 按一下 **收費率** 在左側面板中。
1. 在生產環境中，為中的現有職務角色輸入新的收費率 **公司收費率** 欄位，然後按Enter。

   或

   <div class="preview">

   在預覽環境中，更新 **公司收費率** 以及現有職務角色的開始/結束日期，然後按Enter鍵。

   若要新增新的生效日期公司收費率，請選取工作角色的收費率，然後按一下編輯。 如需生效日期的公司帳單費率的詳細資訊，請參閱 [覆寫公司層級的工作角色收費率](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/override-job-role-billing-rates-company-level.md).

   </div>

1. 若要更新一或多個專案的公司費率，請執行下列任一項作業：

   * 多個專案：

   1. 前往專案清單。
   1. 選取符合您要更新專案的核取方塊。
   1. 按一下 **編輯**.
   1. 在設定區段中，啟用 **重新計算成本和收入** 選項。
   1. 按一下 **儲存變更**.

   * 單一專案：

      1. 前往您啟用公司層級收費率覆寫的專案。
      1. 按一下 **更多** 功能表 ![](assets/qs-more-icon-on-an-object.png) 在標題中專案名稱旁邊，然後按一下 **重新計算財務**.
