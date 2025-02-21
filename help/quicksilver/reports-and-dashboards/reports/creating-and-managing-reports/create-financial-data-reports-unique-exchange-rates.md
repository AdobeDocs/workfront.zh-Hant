---
product-area: reporting
navigation-topic: create-and-manage-reports
title: 建立具有唯一匯率的財務資料報表
description: 如果已在Adobe Workfront中設定多個匯率，您可以在報表和清單中設定財務值，以顯示預設貨幣以外的貨幣。
author: Nolan
feature: Reports and Dashboards
exl-id: a0837c70-8330-4c38-98dc-8cf2e7e2e4bd
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '984'
ht-degree: 0%

---

# 建立具有唯一匯率的財務資料報表

<!-- Audited: 11/2024 -->

如果已在Adobe Workfront中設定多個匯率，您可以在報表和清單中設定財務值，以顯示預設貨幣以外的貨幣。

>[!IMPORTANT]
>
>如果您在檢視中選取預設貨幣以外的貨幣，您不會再在專案清單底部看到連結&#x200B;**新增更多工**&#x200B;和&#x200B;**新增更多問題**。

如需有關如何變更特定專案預設貨幣的資訊，請參閱[變更專案貨幣](../../../manage-work/projects/project-finances/change-project-currency.md)。

如果報表中有單一貨幣的專案，則分組的總和也會以系統預設貨幣顯示。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

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
   <td> 
      <p>新增：</p>
         <ul>
         <li><p>標準</p></li>
         </ul>
      <p>目前：</p>
         <ul>
         <li><p>規劃</p></li>
         </ul>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>編輯報告、儀表板、行事曆的存取權</p> <p>編輯對篩選器、檢視、群組的存取權</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權*</td> 
   <td> <p>管理報表的許可權</p></td> 
  </tr> 
 </tbody> 
</table>

*如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先決條件

在您可以檢視本節所述的替代貨幣之前，Workfront管理員必須先在Workfront的「設定」區域中啟用並設定多種貨幣。 如需詳細資訊，請參閱[設定匯率](../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md)。

## 套用財務值至報表 {#apply-financial-values-to-a-report}

若要在使用報表時轉換幣別間的財務值，請執行下列動作：

1. 移至您要轉換財務值為不同貨幣的報表。
1. 按一下&#x200B;**檢視**&#x200B;下拉式清單，按一下&#x200B;**變更貨幣**，然後選取下列您要顯示財務值的貨幣之一：

   * 專案原始貨幣
   * 任何其他貨幣

     >[!TIP]
     >
     >您只能選擇先前在「設定」中選取的貨幣。

   使用此選項可讓您快速轉換報表中費率值之間的財務值。

   ![變更貨幣](assets/qs-change-currency-2022-350x257.png)

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver,QuicksilverOrClassic.Draft mode">(NOTE: drafted this tip because I think this is confusing; this is in the step above.)</p>
   -->

   <!--
   <note type="tip">
   You can also select the Change Currency option to convert financial values in other lists.
   <br>
   <img src="assets/nwe-change-currency-new-lists-350x219.png" style="width: 350;height: 219;" data-mc-conditions="QuicksilverOrClassic.Quicksilver">
   <br>
   <br>
   </note>
   -->

## 使用不同幣別顯示多個專案中的預設幣別

當您在專案層級自訂貨幣，並且想要在同一報表中顯示所有專案的資訊時，會出現下列情況：

* 如果您建立的報表會從套用不同貨幣的兩個或多個專案中帶入財務資訊，則依預設，群組摘要會反映Workfront管理員所選取的系統預設貨幣。
* 如果您為具有相同貨幣的兩個或多個專案建立報表，但它們與系統的預設貨幣不同，則使用系統預設貨幣顯示分組中的總和。
* 如果您為兩個或多個專案建立報表，而這些專案具有與貨幣修訂相關聯的工作角色指派，則Workfront會將財務資訊從工作角色的修訂貨幣匯率轉換為專案的貨幣（當您在檢視中選取專案的原始貨幣時），或轉換為您在檢視報表時選取的任何其他貨幣。 如需有關覆寫工作角色的貨幣資訊，請參閱[建立和管理工作角色](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md)。

若要在報表中顯示兩個使用自訂貨幣的專案：

1. 建立套用不同貨幣的兩個專案。

   ![貨幣](assets/qs-currency-350x217.png)

1. 在兩個專案上記錄時數。

   如需記錄時間的詳細資訊，請參閱[記錄時間](../../../timesheets/create-and-manage-timesheets/log-time.md)。

1. 按一下&#x200B;**主功能表**&#x200B;圖示![主功能表圖示](assets/main-menu-icon.png)，然後按一下&#x200B;**報表**。
1. 按一下&#x200B;**新報告**，然後按一下&#x200B;**專案報告**。
1. 在&#x200B;**欄（檢視）**&#x200B;索引標籤中，新增&#x200B;**實際成本**&#x200B;欄，並以&#x200B;**總和**&#x200B;加以彙總。

   如需有關如何建立欄的資訊，請參閱[Adobe Workfront中的檢視總覽](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)。

1. 在&#x200B;**群組**&#x200B;索引標籤中，套用&#x200B;**規劃完成日期**&#x200B;群組。

   有關如何建立群組的資訊，請參閱Adobe Workfront中的[群組概觀](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)。

1. 在&#x200B;**篩選器**&#x200B;索引標籤中，新增&#x200B;**專案名稱**&#x200B;的篩選器，並選取兩個使用不同貨幣的專案。

   如需如何建立篩選的詳細資訊，請參閱[篩選總覽](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)。

1. 按一下「**儲存並關閉**」。

   **實際成本**&#x200B;的總計使用系統預設貨幣顯示在「群組」中，無論報告中的專案貨幣為何。

   如果兩個專案的幣別不同，系統預設幣別也會顯示在報表的「群組」中。

## 在專案層級的報表中顯示專案幣別

如果分組套用於專案內的任務或小時清單，則分組的總和會以專案的貨幣顯示。

1. 使用不同於系統預設貨幣的自訂貨幣建立專案。
1. 前往專案，並確認其中包含已記錄任務的小時數。

   如需記錄時間的詳細資訊，請參閱[記錄時間](../../../timesheets/create-and-manage-timesheets/log-time.md)。

   >[!NOTE]
   >
   >任務應指派給具有每小時費率成本費率的使用者或工作角色。

1. 按一下&#x200B;**工作**。
1. 展開&#x200B;**檢視**&#x200B;下拉式功能表，然後選取&#x200B;**新增檢視**。
1. 在新檢視中新增&#x200B;**實際成本**&#x200B;作為新欄，並以&#x200B;**總和**&#x200B;彙總。
1. 按一下&#x200B;**完成**，然後按一下&#x200B;**儲存檢視**。
1. 展開&#x200B;**群組**&#x200B;下拉式功能表，並選取&#x200B;**新增群組**。
1. 將&#x200B;**實際完成日期**&#x200B;新增至新群組作為新欄位，然後按一下&#x200B;**儲存群組**。

   **實際成本**&#x200B;欄彙總於新的群組中，並以專案的貨幣顯示總計。

## 編輯具有唯一貨幣的報告

報表中的財務欄位不可編輯，除非您將報表設定變更為顯示專案的原始貨幣。

若要在報表中內聯編輯財務欄位：

1. 導覽至報表。

   >[!NOTE]
   >
   >如果預設貨幣未在任何其他區域為清單顯示，您可以編輯檢視以顯示預設貨幣。\
   >如需如何在檢視中變更貨幣的相關資訊，請參閱本文[套用財務值至報表](#apply-financial-values-to-a-report)一節。

1. 按一下&#x200B;**報告動作**，然後選取&#x200B;**編輯**。
1. 按一下&#x200B;**報表設定**。
1. 按一下&#x200B;**預設貨幣**&#x200B;下拉式清單，然後選取&#x200B;**專案的原始貨幣**。

   ![預設貨幣](assets/qs-report-settings-default-currency-350x370.png)

1. 按一下&#x200B;**完成**。
