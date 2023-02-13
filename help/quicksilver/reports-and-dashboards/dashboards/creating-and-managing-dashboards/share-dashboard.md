---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: 共用控制面板
description: 您的Adobe Workfront管理員會在控制面板的使用者指派存取層級時，授予他們檢視或編輯控制面板的存取權。 除了授予使用者的存取層級之外，您也可以授予使用者檢視或管理您有權共用的特定控制面板的權限。
author: Nolan
feature: Reports and Dashboards
exl-id: 21bd531f-8732-4d6c-b91f-990887285447
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '542'
ht-degree: 0%

---

# 共用控制面板

您的Adobe Workfront管理員會在控制面板的使用者指派存取層級時，授予他們檢視或編輯控制面板的存取權。 如需授與問題存取權的詳細資訊，請參閱 [授予對報表、控制面板和日曆的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

除了授予使用者的存取層級之外，您也可以授予使用者檢視或管理您有權共用的特定控制面板的權限。 如需存取層級和權限的詳細資訊，請參閱 [存取層級與權限如何搭配運作](../../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md).

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
   <td role="rowheader"><strong>Adobe Workfront計畫*</strong></td> 
   <td> <p>任何 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront授權*</strong></td> 
   <td> <p>審核或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>訪問級別配置*</strong></td> 
   <td> <p>檢視報表、控制面板、日曆的存取權或更高版本</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>物件權限</strong></td> 
   <td> <p>檢視控制面板的權限或更高</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 必要條件

必須先建立控制面板，才能共用它。

如需建立控制面板的詳細資訊，請參閱 [建立控制面板](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

## 共用控制面板的考量事項

除了下列考量事項外，另請參閱 [共用報表、控制面板和日曆](../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md).

* 控制面板的建立者預設具有其「管理」權限。

* 您可以與其他個人、團隊、群組、工作角色或公司共用您建立的控制面板。 您也可以共用已建立和已與您共用的控制面板。
* 您也可以讓整個組織在整個系統內皆可檢視，以便與其共用。
* 您可以共用個別控制面板，或從清單共用多個控制面板。
* 共用控制面板時，依預設，使用者會繼承控制面板上所有報表物件的檢視權限。

   如需Workfront中物件階層的詳細資訊，請參閱 [了解Adobe Workfront中的物件](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

   如需檢視繼承權限的相關資訊，請參閱 [查看對象的繼承權限](../../../workfront-basics/grant-and-request-access-to-objects/view-inherited-permissions-on-objects.md).

## 共用控制面板

從清單共用一個控制面板或數個控制面板是相同的。

1. 前往控制面板清單，選取一或多個控制面板，然後按一下 **共用** ![](assets/share-icon.png).

   或

   按一下某個控制面板的名稱，然後按一下**控制面板動作>****共用**.

   ![](assets/qs-dashboard-actions-menu-350x318.png)

1. 在 **新增人員、團隊、角色、群組或公司……** 欄位中，開始輸入要共用控制面板的使用者、團隊、角色、群組或公司名稱，然後在下拉式清單中出現時按一下名稱。
1. （可選）若要讓系統中的所有使用者都能存取控制面板，請按一下 **設定** 表徵圖，然後選擇 **使此可見系統範圍**.

1. 按一下&#x200B;**儲存**。
