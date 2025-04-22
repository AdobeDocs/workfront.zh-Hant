---
title: 共用任務
product-area: projects
navigation-topic: grant-and-request-access-to-objects
description: 當您的Adobe Workfront管理員指派存取層級時，可以授予您檢視或編輯任務的存取權。 如需授與工作存取權的詳細資訊，請參閱授與工作存取權。
author: Courtney
feature: Get Started with Workfront
exl-id: 45da15cb-8880-41f7-a0de-939882c1f154
source-git-commit: eb4bf18407562b88bf0c946c905b202e5b62a5fe
workflow-type: tm+mt
source-wordcount: '1201'
ht-degree: 1%

---

# 共用任務

當您的Adobe Workfront管理員指派存取層級時，可以授予您檢視或編輯任務的存取權。 如需授與工作存取權的詳細資訊，請參閱[授與工作存取權](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md)。

除了授予使用者的存取層級外，您還可以授予他們檢視、貢獻或管理您有權共用之特定工作的許可權。

許可權專屬於Workfront中的一個專案，可定義使用者可對該專案執行的動作。


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

## 共用任務時的注意事項

除了下列考量事項外，另請參閱[物件共用許可權概觀](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)。

* 任務的建立者預設擁有其「管理」許可權。
* 您可以個別共用工作，也可以一次大量共用數個工作。\
  共用工作與共用其他物件相同。 如需在Workfront中共用專案的詳細資訊，請參閱[共用物件](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md)。

* 您可以將下列許可權授與工作： 

   * 檢視
   * 管理
   * 參與
* 當您共用任務時，使用者預設會繼承與任務相關的所有子物件的相同許可權。 例如，他們會對附加到任務的子任務、問題和檔案繼承相同許可權。\
  如需Workfront中物件階層的詳細資訊，請參閱  [瞭解Adobe Workfront中的物件](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)。

  Workfront管理員可以指定檔案是否應該繼承使用者存取層級中較高物件的許可權。 如需有關限制檔案繼承許可權的詳細資訊，請參閱[建立或修改自訂存取層級](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)。

* 您可以從任務中移除繼承的許可權。\
  如需有關從物件移除繼承許可權的詳細資訊，請參閱  [從物件移除許可權](../../workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md)。

## 共用任務的方法

您可以透過下列方式共用任務：

* 手動（個別或大量）。

* 自動，執行下列動作：

   * 指定任務之任何父系物件的許可權：專案、方案或投資組合。 任務會從其父物件繼承許可權。 如需有關檢視物件繼承許可權的資訊，請參閱[檢視物件的繼承許可權](../../workfront-basics/grant-and-request-access-to-objects/view-inherited-permissions-on-objects.md)。
   * 在用來建立任務所在專案的範本上，將實體新增至專案共用。 如需從範本共用專案的詳細資訊，請參閱[共用範本](../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md)。

   * 編輯專案時，請指定專案中所有任務的許可權。 如需有關根據使用者對專案的許可權管理專案上任務存取許可權的資訊，請參閱文章[編輯專案](../../manage-work/projects/manage-projects/edit-projects.md)中的[](../../manage-work/projects/manage-projects/edit-projects.md#access)區段。

  >[!TIP]
  >
  >如果您未指定將使用者指派給專案中的任務時，您希望使用者擁有哪些任務許可權，預設情況下，他們會獲得與專案相同的許可權。

## 共用任務

1. 導覽至您要共用的工作。

1. 在工作名稱的右側，按一下&#x200B;**共用**。 **共用[工作名稱]**&#x200B;對話方塊開啟。

   ![共用工作按鈕](assets/share-task-button.png)

1. 在&#x200B;**授與任務存取權**&#x200B;欄位中，開始輸入您要與其共用任務的使用者、團隊、角色、群組或公司名稱，然後在其出現在下拉式清單中時按一下該名稱。

   >[!TIP]
   >
   >您只能與作用中使用者、團隊、角色或公司共用任務。


1. （選擇性）選取&#x200B;**擁有存取權**&#x200B;下拉式清單，並選取工作的存取層級：

   * **只有受邀者才能存取：**&#x200B;只有受邀參與工作的使用者才能存取（預設）。
   * **系統中的每個人都可以檢視**：系統中的所有使用者都可以在沒有邀請的情況下檢視工作。

1. 按一下使用者名稱右側的下拉式清單，並選取他們對於此工作的許可權層級：

   * **檢視**：使用者可以檢閱並共用工作。
   * **Contribute**：使用者可以更新、記錄資訊、進行微幅編輯及共用工作（也包含所有檢視許可權）。
   * **管理**：使用者擁有工作的完整存取權，但沒有管理許可權，這些許可權是在存取層級授與的（也包含所有檢視和貢獻許可權）。

1. （可選）按一下您已授與的許可權層級旁的進階選項圖示，以設定工作的特定許可權。

   ![已設定的進階許可權選項](assets/advanced-permission-options.png)

1. （選擇性）若要關閉工作子物件的繼承許可權，請按一下&#x200B;**關閉**&#x200B;內嵌&#x200B;**繼承許可權**。

1. （選擇性）若要使用連結快速共用工作，請按一下[複製連結] **，然後將其轉寄給收件者。**

1. 按一下「**儲存**」。


## 大量共用任務

1. 導覽至包含您要共用之任務的專案。

1. 在專案頁面的「**任務**」標籤中，選取您要共用之每個任務左側的方塊，然後按一下頁面頂端的「**共用**」圖示「![共用」圖示](assets/share-icon.png)。 共用強制回應視窗隨即開啟。

   ![大量共用工作](assets/bulk-share-tasks.png)

1. 在&#x200B;**將任務存取權授予**&#x200B;欄位中，開始輸入您要與其共用任務的使用者、團隊、角色、群組或公司的名稱，然後在其出現在下拉式清單中時按一下該名稱。

   >[!TIP]
   >
   >您只能與作用中使用者、團隊、角色或公司共用任務。


1. （選擇性）選取&#x200B;**誰有存取權**&#x200B;下拉式清單，並選取工作的存取層級：

   * **只有受邀者才能存取：**&#x200B;只有受邀參與工作的使用者才能存取（預設）。
   * **系統中的每個人都可以檢視**：系統中的所有使用者都可以檢視沒有邀請的工作。


1. 按一下使用者名稱右側的下拉式清單，並選取其工作的許可權層級：

   * **檢視**：使用者可以檢閱和共用工作。
   * **Contribute**：使用者可以更新、記錄資訊、進行微幅編輯及共用工作（也包含所有檢視許可權）。
   * **管理**：使用者擁有無管理許可權之工作的完整存取權，這些許可權是在存取層級授與的（也包含所有檢視和貢獻許可權）。

1. （可選）按一下您已授與的許可權層級旁的進階選項圖示，以設定作業的特定許可權。

   ![已設定的進階許可權選項](assets/advanced-permission-options.png)

1. 按一下「**儲存**」。

## 任務許可權

下表顯示當允許使用者檢視、貢獻或管理任務時，您可以授予使用者哪些許可權：

<table border="2" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>動作</strong> </th> 
   <th><strong>管理</strong> </th> 
   <th><strong>貢獻</strong> </th> 
   <th><strong>檢視</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="row">新增任務</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">新增前置任務</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">新增問題</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">刪除任務</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row"> <p>一般任務編輯<br></p> </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">變更任務狀態</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">編輯任務限制</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">檢視任務</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">新增檔案</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">複製任務*</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">移動任務*</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">記錄時數</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">修改計畫日期</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">接受指派</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">進行指派</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">附加自訂表單</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">編輯自訂欄位</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">建立核准流程</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">核准任務</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">編輯財務*</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">新增/編輯費用</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">檢視財務</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">更新/評論</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">共用</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">全系統共用</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

&#42;由存取層級和專案的許可權所控制。
