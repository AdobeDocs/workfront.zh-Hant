---
product-area: projects
navigation-topic: financials
title: 設定效能索引方法(PIM)
description: 項目的效能指數方法(PIM)控制Adobe Workfront用於計算項目效能度量的方法，如成本效能指數(CPI)、成本計畫效能指數(CSI)、計畫效能指數(SPI)和完成時估計(EAC)。
author: Alina
feature: Work Management
exl-id: de628881-c016-4521-bc33-3bcfba19a88f
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '472'
ht-degree: 1%

---

# 設定效能索引方法(PIM)

項目的效能指數方法(PIM)控制Adobe Workfront用於計算項目效能度量的方法，如成本效能指數(CPI)、成本計畫效能指數(CSI)、計畫效能指數(SPI)和完成時估計(EAC)。

Workfront會使用下列項目計算這些值：

* 時數
* 成本

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

## 關於Workfront中PIM的思考

* 您的Workfront管理員或組管理員設定預設值，以確定效能索引方法(PIM)應基於小時還是基於成本。 效能量度的計算會根據此預設值的設定方式而改變。 有關如何更改PIM的預設值的詳細資訊，請參見 [配置系統範圍的項目首選項](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).
* 項目經理還可以在項目級別更改項目「財務」子標籤中個別項目的PIM設定。 您必須具有項目的「管理」權限，才能編輯項目的「財務」子標籤。

## 設定項目的效能索引方法(PIM)

1. 轉到您是的所有者的項目。

   >[!IMPORTANT]
   >
   >您需要專案的「管理」權限，才能執行下列步驟。 我們還建議只有項目所有者才應對項目的「財務」區域進行更改。

1. 按一下 **專案詳細資料** 在左側面板中，然後前往 **金融** 的上界。
1. 連按兩下 **效能索引方法** 欄位來編輯。
1. 在 **效能索引方法** 欄位：

   | 基於小時 | Workfront在計算項目的CPI和EAC時使用「計畫小時數」，而項目的EAC以小時數顯示。 |
   |---|---|
   | 基於成本 | Workfront在計算項目的CPI和EAC時使用「計畫人工成本」，EAC顯示為貨幣值。 選擇此選項時，請確保任務分配者（職務角色或用戶）與成本比率相關聯。 |

   {style=&quot;table-layout:auto&quot;}

1. 按一下 **儲存** **變更**.
