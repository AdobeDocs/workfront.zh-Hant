---
title: 共用自訂表格
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: 您可以設定自訂表單的存取權，以控制誰（人員、角色、群組、團隊、公司）可以檢視、共用及編輯該表單。
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: a264512f-54ab-426e-8dd7-5602ece81c57
source-git-commit: a7be72f0a594a21baed2592d8a2e467118ab1b7f
workflow-type: tm+mt
source-wordcount: '1531'
ht-degree: 0%

---

# 共用自訂表格

您可以設定自訂表單的存取權，以控制誰（人員、角色、群組、團隊、公司）可以檢視、共用及編輯該表單。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront計畫</p> </td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td>
   <p>新增：標準</p>
   <p>或</p>
   <p>目前：計畫</p></td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>管理自訂表單的存取權</p> </td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 存取自訂表格 {#access-to-custom-forms}

根據預設，當您建立新的自訂表單且有人將其附加到物件時，任何指派給該物件的使用者都可以檢視並填寫表單。 這包括擁有請求授權的使用者以及外部使用者。

但是，在尚未附加自訂表單的物件上，使用者（即使他們具有「規劃工具」存取層級）無法從「自訂Forms」下拉式選單中附加它，除非以下其中一項為True：

* 有人將自訂表單共用給使用者或其團隊、工作角色、群組或公司，授與至少檢視許可權並選取「附加至自訂資料」
* 使用者擁有計畫授權，其存取層級允許對自訂表單的管理存取權

## 從表單清單共用自訂表單

您可以為特定使用者、工作角色、群組、團隊和公司設定特定層級的表單存取權，而不需將自訂表單保留在預設共用狀態（本文中之[存取自訂表單](#access-to-custom-forms)的說明）。

{{step-1-to-setup}}

1. 在左側面板中，按一下&#x200B;**自訂Forms**。
1. 選取自訂表格，然後按一下![共用圖示](assets/share-icon.png)。
1. 在顯示的方塊中，在&#x200B;**將自訂表單存取權授予**&#x200B;下方，開始輸入您要與共用自訂表單的使用者、團隊、工作角色、群組或公司名稱，然後在名稱顯示時按&#x200B;**Enter**。
1. 若要調整您剛新增的使用者、團隊、工作角色、群組或公司的存取權，請按一下名稱右側的下拉式功能表，然後設定下列其中一個可用選項及其任何進階設定：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">檢視它</td> 
      <td> <p>此選項提供在物件上檢視和填寫自訂表單的功能。 在物件層級，使用者必須至少擁有Contribute存取權，並啟用<strong>編輯自訂表單</strong>進階設定。 例如，如果表單附加至專案，使用者必須擁有該專案的Contribute存取權，否則將無法填寫表單。</p>

   <p><b>注意</b>：對於擁有輕度授權和貢獻者授權（或工作、檢閱和請求授權）的使用者，這是最高的可用選項。</p>

   <p>按一下<strong>進階設定</strong>，指定是否要允許下列專案：</p> 
       <ul> 
        <li><strong>附加至自訂資料</strong>：能夠將自訂表單附加至他們具有「管理」存取權的專案、任務和問題</li> 
        <li> <p><strong>共用</strong>：能夠與系統中的其他人共用自訂表單</p> <p>具有輕度或貢獻者授權（或工作、檢閱或請求授權）的使用者只能透過API或自訂表單報表共用自訂表單。</p> </li>
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">管理它</td> 
      <td> <p>此選項僅適用於擁有Standard或Plan授權的使用者。 </p> <p>除了能夠將表單新增到他們有權編輯的物件之外，使用者還可以完全編輯自訂表單，包括新增、編輯和刪除欄位。</p> <p>按一下<strong>進階設定</strong>，指定是否要允許下列專案：</p> 
       <ul> 
        <li> <p><strong>附加至自訂資料</strong>：能夠將自訂表單附加至他們具有「管理」存取權的專案、任務和問題</p> </li> 
        <li><strong>刪除</strong>：從系統中刪除自訂表單</li> 
        <li><strong>共用</strong>：與系統中的其他人共用自訂表單</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. （可選）重複步驟4至5，將其他名稱新增至清單並設定其選項。
1. （選擇性）如果您想要將自訂表單（在其附加的物件上）的存取許可權制在您先前步驟中指定的物件上，請按一下共用方塊右上角的齒輪圖示![](assets/gear-icon-settings-with-dn-arrow.jpg)，然後按一下&#x200B;**移除系統範圍存取權**。

   如果您改變心意，可以按一下&#x200B;**讓此在整個系統內可見** （預設選項）。

   >[!NOTE]
   >
   >* 當您將自訂表單設定為全系統可見時，您僅允許使用者在指派給他們的物件上看見並填寫它，不允許將其附加到其他物件。 您可以使用步驟5中說明的「附加至自訂資料」選項，授與將自訂表單附加至物件的功能。
   >* 大多陣列織都想要確保系統中的每個人都可以填寫自訂表單，將其附加到他們工作的物件上，並在報表中檢視其資料。 如果您的組織是這種情況，建議您使用&#x200B;**讓此在整個系統內可見**。 以這種方式設定選項時，對話方塊中會顯示「系統範圍可見」：
   >   
   >![](assets/visible-system-wide-350x480.png)
   >   
   >如果您擔心自訂表單附加至特定物件時，使用者可能會輸入敏感資料，限制這些&#x200B;*物件*&#x200B;的共用可能比限制表單本身的存取權更好。

1. 按一下「**儲存**」。

## 從表單設計工具共用自訂表單

{{step-1-to-setup}}

1. 在左側面板中，按一下&#x200B;**自訂Forms**。
1. 開啟自訂表單或建立新的自訂表單。
1. 當您準備共用表單時，請按一下表單設計工具右上角的&#x200B;**共用**。
1. 在顯示的方塊中，在&#x200B;**授與自訂表單存取權**&#x200B;下方，開始輸入您要與共用自訂表單的使用者、團隊、工作角色、群組或公司名稱，然後在名稱顯示時按&#x200B;**Enter**。
1. 若要調整您剛新增的使用者、團隊、工作角色、群組或公司的存取權，請按一下名稱右側的下拉式功能表，然後設定下列其中一個可用選項及其任何進階設定：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">檢視它</td> 
      <td> <p>此選項提供在物件上檢視和填寫自訂表單的功能。 在物件層級，使用者必須至少擁有Contribute存取權，並啟用<strong>編輯自訂表單</strong>進階設定。 例如，如果表單附加至專案，使用者必須擁有該專案的Contribute存取權，否則將無法填寫表單。</p>

   <p><b>注意</b>：對於擁有輕度授權和貢獻者授權（或工作、檢閱和請求授權）的使用者，這是最高的可用選項。</p> <p>按一下<strong>進階設定</strong>，指定是否要允許下列專案：</p> 
       <ul> 
        <li><strong>附加至自訂資料</strong>：能夠將自訂表單附加至他們具有「管理」存取權的專案、任務和問題</li> 
        <li> <p><strong>共用</strong>：能夠與系統中的其他人共用自訂表單</p> <p>具有輕度或貢獻者授權（或工作、檢閱或請求授權）的使用者只能透過API或自訂表單報表共用自訂表單。</p> </li>
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">管理它</td> 
      <td> <p>此選項僅適用於擁有Standard或Plan授權的使用者。 </p> <p>除了能夠將表單新增到他們有權編輯的物件之外，使用者還可以完全編輯自訂表單，包括新增、編輯和刪除欄位。</p> <p>按一下<strong>進階設定</strong>，指定是否要允許下列專案：</p> 
       <ul> 
        <li> <p><strong>附加至自訂資料</strong>：能夠將自訂表單附加至他們具有「管理」存取權的專案、任務和問題</p> </li> 
        <li><strong>刪除</strong>：從系統中刪除自訂表單</li> 
        <li><strong>共用</strong>：與系統中的其他人共用自訂表單</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. （可選）重複步驟5至6，將其他名稱新增至清單並設定其選項。
1. （選擇性）如果您想要將自訂表單（在其附加的物件上）的存取許可權制在您先前步驟中指定的物件上，請按一下「**誰有存取權**」下的下拉式箭頭，然後選取「**只有受邀者才能存取**」。

   如果您改變心意，可以選取&#x200B;**系統中的每個人都可以檢視**。

   >[!NOTE]
   >
   >* 當您將自訂表單設定為全系統可見時，您僅允許使用者在指派給他們的物件上看見並填寫它，不允許將其附加到其他物件。 您可以使用步驟6中說明的「附加至自訂資料」選項，授與將自訂表單附加至物件的功能。
   >* 大多陣列織都想要確保系統中的每個人都可以填寫自訂表單，將其附加到他們工作的物件上，並在報表中檢視其資料。 如果您的組織有此情況，建議您使用&#x200B;**系統中的每個人都可以檢視**。 以這種方式設定選項時，對話方塊中會顯示「系統範圍可見」：
   >   
   >![共用自訂表單](assets/share-custom-form-in-designer.png)
   >   
   >如果您擔心自訂表單附加至特定物件時，使用者可能會輸入敏感資料，限制這些&#x200B;*物件*&#x200B;的共用可能比限制表單本身的存取權更好。

1. 按一下「**儲存**」。

## 從表單清單中移除對自訂表單的存取權

{{step-1-to-setup}}

1. 在左側面板中，按一下&#x200B;**自訂Forms**。
1. 選取自訂表格，然後按一下![共用圖示](assets/share-icon.png)。
1. 在顯示的方塊中，按一下您不想再擁有表單特殊存取許可權的使用者、團隊、角色、群組或公司名稱右側的X。
1. （可選）對要移除的其他名稱重複上一步驟至。
1. 按一下「**儲存**」。
