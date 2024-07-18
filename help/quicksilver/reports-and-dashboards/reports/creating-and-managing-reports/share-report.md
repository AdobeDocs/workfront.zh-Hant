---
product-area: reporting
navigation-topic: create-and-manage-reports
title: 在Adobe Workfront中共用報表
description: 當使用者指派存取層級時，您的Adobe Workfront管理員會授予他們檢視或編輯報告的存取權。 如需授與問題存取權的詳細資訊，請參閱授與報告、控制面板和行事曆的存取權。
author: Nolan
feature: Reports and Dashboards
exl-id: 225e815a-0354-493d-bbcf-59304ef77570
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '808'
ht-degree: 0%

---

# 在Adobe Workfront中共用報表

當使用者指派存取層級時，您的Adobe Workfront管理員會授予他們檢視或編輯報告的存取權。 如需授與問題存取權的詳細資訊，請參閱[授與報告、儀表板和行事曆的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md)。

除了授予使用者的存取層級之外，您還可以授予他們檢視或管理您有權共用之特定報告的許可權。 如需存取層級和許可權的詳細資訊，請參閱[存取層級和許可權如何搭配運作](../../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md)。

許可權專屬於Workfront中的一個專案，可定義使用者可對該專案執行的動作。

>[!NOTE]
>
>Workfront管理員可以新增或移除系統中所有使用者的任何專案許可權，而無需擁有這些專案。

## 存取需求

您必須具備下列專案才能共用物件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>任何 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>評論或以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>檢視報表、儀表板、行事曆的存取權或以上專案</p> <p>注意：如果您還是沒有存取權，請詢問您的Workfront管理員，他們是否在您的存取層級中設定其他限制。 如需Workfront管理員如何修改存取層級的詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>檢視許可權或更高的報告</p> <p>如需請求其他存取權的資訊，請參閱<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求物件</a>的存取權。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的Workfront管理員。

## 關於共用報表的考量事項

除了下列考量事項外，另請參閱[共用報告、儀表板和行事曆](../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md)。

* 您可以與其他個人、團隊、群組、職位角色或公司共用您建立的報表。 您也可以共用他人建立並與您共用的報表。
* 您也可以將它們與整個組織共用或公開。 將報表設為公開會產生可與其他人共用的URL。
* 您可以共用個別報表，也可以從報表清單共用多個報表。

## 共用報表的方式

您可以透過下列方式在Workfront中共用報表：

* 手動，如以下[共用報表](#share-a-report)區段中所述。
* 從包含已共用報表的控制面板繼承檢視許可權，以自動執行。 如需有關檢視物件繼承許可權的資訊，請參閱[檢視物件的繼承許可權](../../../workfront-basics/grant-and-request-access-to-objects/view-inherited-permissions-on-objects.md)。

## 共用報表 {#share-a-report}

從清單共用一個報表或多個報表的方式相同。

1. 移至報告清單，並選取一或多個報告，然後按一下[共用]。****

   或

   按一下其中一個報表的名稱，然後按一下**「報表動作>****共用**」。

   ![](assets/qs-report-actions-sharing.png)

1. 在顯示的方塊中，在&#x200B;**新增人員、團隊、角色、群組或公司……**&#x200B;欄位中，開始輸入您要與其共用報表的使用者、團隊、工作角色、群組或公司的名稱，然後在名稱顯示時按&#x200B;**Enter**。

1. 若要調整所新增名稱的存取層級，請按一下名稱右側的下拉式功能表，然後選擇下列其中一個選項。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">檢視它</td> 
      <td> <p>允許您的收件者存取，以便在<strong>報告</strong> <img src="assets/reports-in-main-menu.png">區域檢視並執行報告。</p> <p>您可以按一下<strong>進階設定</strong>，指定您是否要讓使用者能夠與系統中的任何人共用<strong>共用</strong>。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">管理它</td> 
      <td> <p>允許收件者完整編輯報告存取權。</p> <p>您可以按一下<strong>進階設定</strong>，指定您是否要讓使用者從系統<strong>刪除</strong>報告，並與系統中的任何人共用<strong>共用</strong>。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. （可選）重複上述兩個步驟，將其他名稱新增至清單並設定其選項。
1. （選擇性）按一下共用方塊右上角的&#x200B;**齒輪**&#x200B;圖示![](assets/gear-icon-settings-with-dn-arrow.jpg)，然後選取下列其中一個選項：

   * **將此設為公開給外部使用者：**&#x200B;選取此選項可產生可與其他人共用的URL。 擁有URL的任何人都可以存取報表，無需擁有Adobe Workfront授權。

     >[!CAUTION]
     >
     >建議您將包含機密資訊的物件與外部使用者共用時務必謹慎。 這可讓他們檢視資訊，而不需要身為Workfront使用者或屬於您的組織。

     >[!NOTE]
     >
     >如果報告有提示且您公開共用，則執行報告的使用者必須登入Workfront，才能使用提示執行報告。 如果他們無法登入Workfront，將會看到未套用提示的報告。 如需有關共用具有提示之報表的限制的詳細資訊，請參閱文章[新增提示至報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)中的[共用提示之報表的限制](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md#limitations-of-running-public-prompted-reports)小節。

   * **讓此在整個系統內可見：**&#x200B;選取此選項，讓Workfront中可存取報告的所有人都可以看到報告。

1. 按一下「**儲存**」。
