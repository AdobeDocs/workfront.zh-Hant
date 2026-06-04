---
product-area: projects
navigation-topic: financials
title: 變更專案貨幣
description: 身為專案經理，您可以設定專案以使用Adobe Workfront系統預設貨幣以外的貨幣。 這可讓您在計算人力成本與收入時，以所需的貨幣顯示專案的財務資訊。
author: Lisa
feature: Work Management
exl-id: c496fe92-5c17-41a5-972b-1c063643bde3
TQID: https://experienceleague.adobe.com/oI3Fu9-AAnKYBbnaI-7BNWWd5Js6eUpvwVQtEWJVPiY
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 570
ht-degree: 3%

---

# 變更專案貨幣

身為專案經理，您可以設定專案以使用Adobe Workfront系統預設貨幣以外的貨幣。 這可讓您在計算人力成本與收入時，以所需的貨幣顯示專案的財務資訊。

在您能夠使用本節所述的替代貨幣之前，Workfront管理員必須先啟用並設定多個貨幣，如文章[設定匯率](../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md)中所述。

## 存取權要求

+++ 展開以檢視這篇文章中所述功能的存取權要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront 封裝</td> 
   <td>任何 </td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront授權</td> 
   <td>
   <p>標準</p>
   <p>規劃</p></td> 
  </tr> 
  <tr> 
   <td>存取層級設定</td> 
   <td>編輯專案的存取權</td> 
  </tr> 
  <tr> 
   <td>物件許可權</td> 
   <td>管理專案的許可權</td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 在Workfront中變更專案貨幣時的注意事項

* 如果專案中有任何財務資訊，則無法變更專案的貨幣。
* 費率用於人工成本、收入計算和報告目的。
* 如果您沒有為專案指定不同的貨幣，Workfront會假設專案的貨幣是系統的預設貨幣。 如需系統層級預設貨幣的資訊，請參閱[設定匯率](../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md)。
* 依預設，所有完整授權使用者都可檢視貨幣和匯率。 Workfront管理員需要授予&#x200B;**匯率**&#x200B;的其他管理存取權，才能讓使用者設定專案的特定匯率。
* Workfront中的匯率不是動態的。 值是由管理員所設定，當匯率發生變更時，必須更新。
* 如果將有效日期套用至貨幣及其匯率，則匯率可能會在專案存留期內變更。 如需有效日期匯率的資訊，請參閱[設定匯率](/help/quicksilver/administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md)。
* 建立報表以反映專案的貨幣時，所有報表預設都會依專案的預設貨幣分組。 如果您建立的報表包含具有不同匯率的多個專案，則套用至專案的任何群組都會反映系統層級的預設匯率。 如需詳細資訊，請參閱文章[建立具有唯一匯率的財務資料報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-financial-data-reports-unique-exchange-rates.md)。

## 設定專案的貨幣

1. 前往您要變更預設貨幣的專案。

   >[!TIP]
   >
   >確保專案沒有任何財務資訊。 例如，確保沒有與專案相關的計畫或實際成本。

1. 按一下左側面板中的&#x200B;**專案詳細資料**，然後移至&#x200B;**財務**&#x200B;區域。
1. 在&#x200B;**貨幣**&#x200B;欄位中按一下&#x200B;**新增**，然後選取您要做為專案預設貨幣的貨幣。 顯示您的Workfront管理員為您的Workfront執行個體設定的所有貨幣。

   專案![&#128279;](assets/currency-on-project.png)上的貨幣

1. （視條件而定）如果您選取的貨幣不是為Workfront系統設定的預設貨幣，請指定所選貨幣的匯率，因為該匯率與系統中設定為基本貨幣的貨幣相關。

   >[!NOTE]
   >
   >如果開啟此專案的&#x200B;**使用系統**&#x200B;日期有效匯率設定，則不允許匯率覆寫。 如需詳細資訊，請參閱[編輯專案](/help/quicksilver/manage-work/projects/manage-projects/edit-projects.md)。

1. 按一下「**儲存變更**」。
