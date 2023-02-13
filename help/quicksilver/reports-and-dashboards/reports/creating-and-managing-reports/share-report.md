---
product-area: reporting
navigation-topic: create-and-manage-reports
title: 在Adobe Workfront中共用報表
description: 您的Adobe Workfront管理員會在使用者指派存取層級時，授予其檢視或編輯報表的存取權。 有關授予對問題的訪問權限的詳細資訊，請參閱授予對報告、控制面板和日曆的訪問權限。
author: Nolan
feature: Reports and Dashboards
exl-id: 225e815a-0354-493d-bbcf-59304ef77570
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '807'
ht-degree: 0%

---

# 在Adobe Workfront中共用報表

您的Adobe Workfront管理員會在使用者指派存取層級時，授予其檢視或編輯報表的存取權。 如需授與問題存取權的詳細資訊，請參閱 [授予對報表、控制面板和日曆的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

除了授予使用者的存取層級之外，您也可以授予使用者檢視或管理您有權共用之特定報表的權限。 如需存取層級和權限的詳細資訊，請參閱 [存取層級與權限如何搭配運作](../../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md).

權限是Workfront中一個項目專屬的權限，並定義可對該項目採取的動作。

>[!NOTE]
>
>Workfront管理員可以為所有使用者新增或移除系統中任何項目的權限，而不是這些項目的擁有者。

## 存取需求

您必須具備以下條件才能共用物件：

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
   <td> <p>審核或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>檢視報表、控制面板、日曆的存取權或更高版本</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>檢視權限或更高報表</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 共用報表的考量事項

除了下列考量事項外，另請參閱 [共用報表、控制面板和日曆](../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md).

* 您可以與其他個人、團隊、群組、工作角色或公司共用您建立的報表。 您也可以共用其他人建立和已與您共用的報表。
* 您也可以將這些區段共用給整個組織或公開。 將報表設為公用會產生可與其他人共用的URL。
* 您可以共用個別報表，或從報表清單共用多個報表。

## 共用報表的方式

您可以透過下列方式在Workfront中共用報表：

* 手動，如 [共用報表](#share-a-report) 一節。
* 從包含已共用報表的控制面板繼承檢視權限，自動執行。 有關查看對象繼承的權限的資訊，請參見 [查看對象的繼承權限](../../../workfront-basics/grant-and-request-access-to-objects/view-inherited-permissions-on-objects.md).

## 共用報表 {#share-a-report}

從清單中共用一或多個報表完全相同。

1. 前往報表清單，選取一或多個報表，然後按一下 **共用**.

   或

   按一下一個報表的名稱，然後按一下**報表動作>****共用**.

   ![](assets/qs-report-actions-sharing.png)

1. 在顯示的方塊中， **新增人員、團隊、角色、群組或公司……** 欄位開始鍵入要與其共用報告的用戶、團隊、職務角色、組或公司的名稱，然後按 **輸入** 名稱時顯示。

1. 要調整所添加名稱的訪問級別，請按一下名稱右側的下拉菜單，然後選擇以下選項之一。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">檢視它</td> 
      <td> <p>可讓收件者存取在 <strong>報表</strong> <img src="assets/reports-in-main-menu.png"> 並運行。</p> <p>您可以按一下 <strong>進階設定</strong> 指定您要讓使用者或使用者 <strong>共用</strong> 和系統裡的任何人。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">管理它</td> 
      <td> <p>允許收件者完全編輯報表的存取權。</p> <p>您可以按一下 <strong>進階設定</strong> 指定您要讓使用者或使用者 <strong>刪除</strong> 來自系統和 <strong>共用</strong> 和系統裡的任何人。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. （可選）重複前2個步驟，將其他名稱新增至清單並設定其選項。
1. （選用）按一下 **齒輪** 圖示 ![](assets/gear-icon-settings-with-dn-arrow.jpg) 在共用方塊的右上角，然後選取下列其中一個選項：

   * **將此設定公開給外部使用者：** 選取此選項可產生可與其他人共用的URL。 任何具有URL的人都可以存取報表，不需要Adobe Workfront授權。

      >[!CAUTION]
      >
      >建議您在與外部使用者共用包含機密資訊的物件時，務必小心。 這可讓使用者檢視資訊，而不需要是Workfront使用者或您組織的一員。

      >[!NOTE]
      >
      >如果報表有提示，而您公開共用，則執行報表的使用者必須登入Workfront，才能使用提示執行報表。 如果無法登入Workfront，則會在未套用提示的情況下看到報表。 有關限制與提示共用報表的詳細資訊，請參閱一節 [共用提示報表的限制](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md#limitations-of-running-public-prompted-reports) 在文章中 [新增提示至報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

   * **使此系統範圍可見：** 選取此選項，讓Workfront中有權存取報表的所有人都能查看報表。

1. 按一下&#x200B;**儲存**。
