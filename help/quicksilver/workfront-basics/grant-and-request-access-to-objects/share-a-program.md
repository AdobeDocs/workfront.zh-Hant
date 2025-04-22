---
title: 共用方案
product-area: projects
keywords: 共用，程式，許可權
navigation-topic: grant-and-request-access-to-objects
description: 指派存取層級時，您的Adobe Workfront管理員可授予您檢視或編輯方案的存取權。 您必須擁有計畫授權才能編輯計畫。
author: Courtney
feature: Get Started with Workfront
exl-id: bfa6ce97-24ad-44b3-9c2f-7fac6b748f94
source-git-commit: eb4bf18407562b88bf0c946c905b202e5b62a5fe
workflow-type: tm+mt
source-wordcount: '914'
ht-degree: 0%

---

# 共用方案


指派存取層級時，您的Adobe Workfront管理員可授予您檢視或編輯方案的存取權。 您必須擁有計畫授權才能編輯計畫。 如需詳細資訊，請參閱[授予程式的存取權](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-programs.md)。

除了授予您的存取層級之外，您還可以從可與您共用方案的使用者那裡獲得檢視或管理特定方案的許可權。 如需存取層級和許可權的詳細資訊，請參閱[存取層級和許可權如何搭配運作](../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md)。

許可權是Workfront中每個專案專屬的許可權，可定義使用者可對該專案執行的動作。


## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具備下列專案才能共用物件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td> <p>任何 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td> <p>新增：標準</p> 
   或
   <p>目前：工作或以上</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>檢視您要共用之物件的存取許可權或以上許可權</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>檢視您要共用之物件的許可權或更高的許可權</p></td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 關於共用方案的考量事項

除了下列考量事項外，另請參閱[物件共用許可權概觀](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)。

>[!NOTE]
>
>Workfront管理員可以新增或移除系統中所有使用者的任何專案許可權，而無需擁有這些專案。

* 依預設，方案的建立者擁有管理許可權。

* 您可以個別共用計畫，也可以一次共用多個計畫。

  如需在Workfront中共用專案的詳細資訊，請參閱[共用物件](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md)。

* 您只能授與程式的「檢視」或「管理」許可權：

* 當您共用方案時，使用者預設會繼承與該方案相關聯的所有子物件的相同許可權。

  如需Workfront中物件階層的詳細資訊，請參閱[瞭解Adobe Workfront中的物件](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)。

* 您可以從程式中移除繼承的許可權。 如需有關從物件移除許可權的詳細資訊，請參閱  [從物件移除許可權](../../workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md)。

## 共用方案

{{step1-to-programs}}

1. 在&#x200B;**程式**&#x200B;頁面上，選取您要共用的程式。 程式頁面隨即開啟。

1. 在程式名稱的右側，按一下&#x200B;**共用**。 **共用[程式名稱]**&#x200B;對話方塊開啟。

   ![共用方案按鈕](assets/share-program-button.png)

1. 在&#x200B;**授與方案存取權**&#x200B;欄位中，開始輸入您要共用方案的使用者、團隊、角色、群組或公司的名稱，然後當名稱出現在下拉式清單中時按一下該名稱。

   >[!TIP]
   >
   >您只能與作用中使用者、團隊、角色或公司共用方案。


1. （選擇性）選取&#x200B;**誰有存取權**&#x200B;下拉式清單，並選取程式的存取層級：

   * **只有受邀者才能存取：**&#x200B;只有受邀加入此程式的使用者才能存取（預設）。
   * **系統中的每個人都可以檢視**：系統中的所有使用者都可以檢視沒有邀請的程式。


1. 按一下使用者名稱右側的下拉式清單，並選取其對此程式的許可權層級：

   * **檢視**：使用者可以檢閱並共用程式。
   * **管理**：使用者擁有此程式的完整存取權，但沒有管理許可權，這些許可權是在存取層級授與的（也包含所有檢視許可權）。

1. （可選）按一下您已授與的許可權層級旁的進階選項圖示，以設定程式的特定許可權。

   ![已設定的進階許可權選項](assets/advanced-options-icon.png)

1. （選擇性）若要關閉程式子物件的繼承許可權，請按一下&#x200B;**關閉**&#x200B;內嵌&#x200B;**繼承許可權**。

1. （選擇性）若要使用連結快速共用程式，請按一下[複製連結] **，然後將它轉寄給收件者。**

1. 按一下「**儲存**」。

## 大量共用程式

{{step1-to-programs}}

1. 在&#x200B;**程式**&#x200B;頁面上，選取您要共用之每個程式左側的方塊，然後按一下頁面頂端的&#x200B;**共用**&#x200B;圖示![共用圖示](assets/share-icon.png)。 共用強制回應視窗隨即開啟。

   ![大量共用程式](assets/bulk-share-programs.png)

1. 在&#x200B;**授與程式存取權**&#x200B;欄位中，開始輸入您要與其共用程式的使用者、團隊、角色、群組或公司的名稱，然後當名稱出現在下拉式清單中時按一下該名稱。

   >[!TIP]
   >
   >您只能與作用中使用者、團隊、角色或公司共用方案。


1. （選擇性）選取&#x200B;**誰有存取權**&#x200B;下拉式清單，並選取程式的存取層級：

   * **只有受邀者才能存取：**&#x200B;只有受邀加入程式的使用者才能存取（預設）。
   * **系統中的每個人都可以檢視**：系統中的所有使用者都可以檢視沒有邀請的程式。


1. 按一下使用者名稱右側的下拉式清單，並選取其方案的許可權層級：

   * **檢視**：使用者可以檢閱和共用程式。
   * **管理**：使用者擁有無管理許可權程式的完整存取權，這些許可權是在存取層級授與的（也包含所有檢視許可權）。

1. （可選）按一下您已授與的許可權層級旁的進階選項圖示，以設定程式的特定許可權。

   ![已設定的進階許可權選項](assets/advanced-options-icon.png)

1. 按一下「**儲存**」。

## 程式許可權

下表顯示當允許使用者檢視或管理方案時，您可以授予他們哪些許可權：

| **動作** | **管理** | **檢視** |
|---|---|---|
| 編輯計畫詳細資料 | ✓ |   |
| 檢視計畫 | ✓ | ✓ |
| 刪除計畫 | ✓ |   |
| 附加自訂表格 | ✓ |   |
| 編輯自訂欄位 | ✓ |   |
| 新增或移除專案&#42; | ✓ |   |
| 核准專案 | ✓ |   |
| 新增檔案資料夾&#42; | ✓ | ✓ |
| 新增檔案 | ✓ | ✓ |
| 新增更新/評論 | ✓ | ✓ |
| 共用 | ✓ | ✓ |
| 共用系統範圍 |   | ✓ |

*這些許可權是由存取層級和其他物件（例如專案）的許可權所控制。


