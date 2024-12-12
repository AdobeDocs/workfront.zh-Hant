---
product-area: projects
navigation-topic: financials
title: 設定績效指數方法(PIM)
description: 專案的績效指數方法(PIM)控制Adobe Workfront用來計算專案績效指標的方法，例如成本績效指數(CPI)、成本排程績效指數(CSI)、排程績效指數(SPI)以及完工估算(EAC)。
author: Lisa
feature: Work Management
exl-id: de628881-c016-4521-bc33-3bcfba19a88f
source-git-commit: 6afa65f921864403c10541d283ef717dce81aed7
workflow-type: tm+mt
source-wordcount: '434'
ht-degree: 1%

---

# 設定績效指數方法(PIM)

專案的績效指數方法(PIM)控制Adobe Workfront用來計算專案績效指標的方法，例如成本績效指數(CPI)、成本排程績效指數(CSI)、排程績效指數(SPI)以及完工估算(EAC)。

Workfront會使用下列方法計算這些值：

* 時數
* 成本

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

## Workfront中PIM的考量事項

* 您的Workfront管理員或群組管理員會設定績效指數方法(PIM)是以小時為基礎或以成本為基礎的預設值。 績效量度的計算會根據此預設值的設定方式而改變。 如需有關如何變更計算PIM預設值的詳細資訊，請參閱[設定系統範圍的專案偏好設定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)。
* 專案經理也可以在專案的「財務」子頁標中，針對個別專案在專案層級變更PIM的設定。 您必須擁有專案的管理許可權才能編輯專案的財務子標籤。

## 設定專案的績效指數方法(PIM)

1. 前往您擁有的專案。

   >[!IMPORTANT]
   >
   >您需要專案的管理許可權才能執行以下步驟。 我們也建議只有專案所有者應該對專案的財務區域進行變更。

1. 按一下左側面板中的&#x200B;**專案詳細資料**，然後移至&#x200B;**財務**&#x200B;區域。
1. 連按兩下&#x200B;**績效指數方法**&#x200B;欄位中的值即可進行編輯。
1. 從&#x200B;**績效指數方法**&#x200B;欄位中的下列選項中選取：

   | 基於小時 | Workfront使用計畫時數來計算專案的CPI和EAC，而專案的EAC顯示為數字（以時數表示）。 |
   |---|---|
   | 基於成本 | Workfront使用計畫勞力成本來計算專案的CPI和EAC，而EAC會顯示為貨幣值。 選取此選項時，請確定您的任務受指派人（職務角色或使用者）與成本費率相關聯。 |

   {style="table-layout:auto"}

1. 按一下&#x200B;**儲存** **變更**。
