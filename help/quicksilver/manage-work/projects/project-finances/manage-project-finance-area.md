---
product-area: projects
navigation-topic: financials
title: 管理專案財務領域的資訊
description: 您可以存取專案詳細資訊區段的財務區域，以檢視或編輯專案的財務資訊。
author: Lisa
feature: Work Management
exl-id: 147f5d55-a827-4cca-9ab0-afb03a4bcd5a
source-git-commit: e5a87b92bf1f6c2e0485ba8a2eb73e52c422b2fc
workflow-type: tm+mt
source-wordcount: '1285'
ht-degree: 2%

---

# 管理專案財務區域的資訊

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: some information in here is duplicated in Edit projects. If you need to update one of the fields in this area, do it in both places.)</p>
-->

您可以存取專案詳細資訊區段的財務區域，以檢視或編輯專案的財務資訊。 您可以在此區域中檢視或編輯的欄位數量有限。 如需有關編輯專案所有資訊的資訊，請參閱[編輯專案](../../../manage-work/projects/manage-projects/edit-projects.md)。

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
   <p>新增：淺色或更高</p>
   <p>或</p>
   <p>目前：檢閱或以上</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>檢視專案和財務資料的存取權或更高的存取權</p> <p>編輯對專案和財務資料的存取權以編輯專案的財務資訊</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>檢視專案或以上版本的許可權，其中包含檢視財務許可權</p> <p>管理專案的許可權，包括管理財務以編輯專案的財務資訊</p> </td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 財務領域概述

在「財務」區域中檢視或編輯資訊時，請考量下列事項：

* 您可以在「專案詳細資料」的「財務」區域中找到的財務資訊，代表從作業累計至專案層次的值，以及直接在專案上輸入的資訊。 某些財務資訊可在專案與作業層級管理。
* 您必須擁有專案的檢視許可權以及從存取層級存取財務資料，才能檢視專案的財務區域。
* 您必須擁有專案的管理許可權，以及從您的存取層級存取財務資料，才能編輯財務區域上的資訊。 不過，我們建議只有專案所有者應編輯此區域的資訊。

## 檢視專案的財務資訊

1. 前往專案。
1. 按一下左側面板中的&#x200B;**專案詳細資料**。
1. 按一下[詳細資料]區段右上角的&#x200B;**編輯**&#x200B;圖示![](assets/edit-icon.png)，然後按一下&#x200B;**財務**。

   ![](assets/finance-area-in-details-view-only-nwe-350x188.png)

   >[!NOTE]
   >
   >根據Workfront管理員設定版面配置範本的方式，概觀區段可能不會列在前，在此情況下會摺疊。 如需詳細資訊，請參閱[使用配置範本自訂詳細資料檢視](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md)。

1. 檢視專案之財務區域的下列欄位：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">績效指數方法</td> 
      <td> 控制Workfront用來計算「實現值」量度的方法。 可以是小時制，也可以是成本制。 <br>如需有關PIM的詳細資訊，請參閱文章<a href="../../../manage-work/projects/project-finances/set-pim.md" class="MCXref xref">設定績效指數方法(PIM)</a></td> 
     </tr> 
     <tr> 
      <td role="rowheader">CPI/SPI/CSI</td> 
      <td> <p>這些是顯示您的專案在指定時間的表現情形的專案績效量度。 其值是根據績效指數方法計算。<br>如需詳細資訊，請參閱下列文章： </p> 
       <ul> 
        <li> <p><a href="../../../manage-work/projects/project-finances/calculate-cpi.md" class="MCXref xref">計算成本績效指數(CPI)</a> </p> </li> 
        <li> <p><a href="../../../manage-work/projects/project-finances/calculate-spi.md" class="MCXref xref">計算排程績效指數(SPI) </a> </p> </li> 
        <li> <p><a href="../../../manage-work/projects/project-finances/calculate-csi.md" class="MCXref xref">計算成本排程績效指數(CSI)</a> </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">預估完成成本</td> 
      <td> 專案的預估總成本，如果績效指數方法(PIM)是以時數為基準，則以時數表示；如果績效指數方法(PIM)是以成本為基準，則以貨幣值表示。<br>如需有關計算完工估算的詳細資訊，請參閱文章<a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref">計算完工估算(EAC)</a></td> 
     </tr> 
     <tr> 
      <td role="rowheader">預算</td> 
      <td>這是專案的預算集。 這由專案所有者手動指定。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">固定成本</td> 
      <td>這些是專案的固定成本，與專案上的其他活動無關。 由專案所有者手動輸入。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">規劃成本</td> 
      <td>專案的估計成本，根據計畫時數以及與任務受指派人（工作角色或使用者）相關聯的費率。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">實際成本</td> 
      <td>專案的所有應計成本。 實際成本是所有實際成本的總和：勞力成本（根據實際時數以及與工作角色或記錄工作角色的使用者相關聯的費率）、費用及固定成本（可與專案或作業相關聯）。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">固定收入</td> 
      <td>根據專案排程設定預期收入。 固定收入由專案所有者手動指定。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">規劃收入</td> 
      <td>根據計畫時數以及與任務受指派人（工作角色或使用者）關聯的費率的預期收入。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">實際收入</td> 
      <td>根據實際時數以及與任務受指派人（職務角色或使用者）關聯的費率，從專案得到的實際收入。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">已計費收入</td> 
      <td> <p>記入帳單記錄中，向客戶或其他當事人記帳的收入。 如需有關付費記錄的詳細資訊，請參閱文章<a href="../../../manage-work/projects/project-finances/create-billing-records.md" class="MCXref xref">建立付費記錄</a>。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> </td> 
      <td> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> </td> 
      <td> </td> 
     </tr> 
    </tbody> 
   </table>

## 編輯專案的財務資訊

身為專案所有者，您可以編輯專案之「財務」子標籤上的資訊。

若要編輯「專案財務」子頁簽上的資訊，請執行下列動作：

1. 前往您擁有的專案。

   >[!NOTE]
   >
   >您需要專案的管理許可權才能執行以下步驟。 我們也建議只有專案所有者應該變更專案的財務子標籤。

1. 按一下左側面板中的&#x200B;**專案詳細資料**。
1. 按一下[詳細資料]區段右上角的&#x200B;**編輯**&#x200B;圖示![](assets/edit-icon.png)，然後按一下&#x200B;**財務**。 這將開啟「財務」區域以進行編輯。
1. 編輯任何可編輯的欄位，方法是按一下該欄位或按一下&#x200B;**+新增**&#x200B;將資訊新增至空白欄位。

   >[!TIP]
   >
   >如果欄位是由Workfront自動計算，或是您沒有編輯許可權，則無法加以編輯。

   ![](assets/edit-finance-area-in-project-details-nwe-350x275.png)

1. 更新以下任何欄位。

   >[!NOTE]
   >
   >根據您的Workfront管理員設定版面配置範本的方式，您環境中專案詳細資訊區段中的欄位可能會不同。 如需詳細資訊，請參閱[使用配置範本自訂詳細資料檢視](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md)。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">績效指數方法</td> 
      <td> <p>控制Workfront用來計算專案績效量度的方法。 這是由您的管理員在系統層級設定的，但您也可以在專案層級進行編輯。 請考慮選取下列其中一個選項：</p> 
       <ul> 
        <li><strong>小時型：</strong>Workfront使用計畫時數來計算專案的CPI和EAC，而專案的EAC顯示為數字（以小時為單位）。 </li> 
        <li><strong>以成本為基礎：</strong>Workfront使用計畫勞力成本來計算專案的CPI和EAC，而EAC會顯示為貨幣值。 選取此選項時，請確定您的任務受指派人（職務角色或使用者）與成本費率相關聯。</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">預估完成成本</td> 
      <td> <p>代表專案或任務完成時的預估總成本。 這是由您的管理員在系統層級設定的，但您也可以在專案層級進行編輯。 請考慮選取下列其中一個選項：</p> 
       <ul> 
        <li><strong>在專案層級計算</strong>：父系任務與專案的EAC是透過在EAC公式中輸入實際時數/實際勞力成本來決定。 此計算包括直接新增到父級任務或專案的實際時數/成本和費用。</li> 
        <li><strong>從任務/子任務累計</strong>：父任務和專案的EAC是由每個子任務的EAC相加所決定。 此計算不包括直接新增到父級任務或專案的實際時數/成本和費用。</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">預算</td> 
      <td>指定此專案的預算。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">固定成本</td> 
      <td>指定此專案的固定成本。 這不應包含任何人力或費用成本。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">固定收入</td> 
      <td> <p>指定此專案的固定收入。 這不應包括來自向合作夥伴或第三方計費的任何計費記錄的收入。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">專案貨幣</td> 
      <td> <p>如果貨幣與系統中的預設貨幣不同，請指定此專案的貨幣。 您系統中的預設貨幣由Workfront管理員定義。 如需有關在Workfront中設定匯率的詳細資訊，請參閱文章<a href="../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">設定匯率</a>。</p> </td> 
     </tr>
    </tbody> 
   </table>

1. 按一下「**儲存變更**」。
