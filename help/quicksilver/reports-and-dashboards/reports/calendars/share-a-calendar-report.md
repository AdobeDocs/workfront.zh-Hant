---
product-area: calendars
navigation-topic: calendars-navigation-topic
title: 共用行事曆報告
description: 您可以與其他使用者共用行事曆，也可以公開行事曆，讓沒有 [!DNL Adobe Workfront] 授權的人檢視行事曆。
author: Lisa
feature: Reports and Dashboards
exl-id: 77eed0fe-2d47-40c4-a03d-590f7fa17dbe
source-git-commit: 0606dab832753543ceef4b5b505413967176aec4
workflow-type: tm+mt
source-wordcount: '606'
ht-degree: 0%

---

# 共用行事曆報告


您可以與其他使用者共用行事曆，也可以公開使用，讓沒有[!DNL Adobe Workfront]授權的人檢視行事曆。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront plan]</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權</td> 
   <td><p>新增：淺色</p>
       <p>或</p>
       <p>目前：檢閱</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>[!UICONTROL 檢視]或更高許可權可存取[!UICONTROL 報表]、[!UICONTROL 儀表板]和[!UICONTROL 行事曆]</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td>[!UICONTROL 檢視]或行事曆報告的更高許可權（可存取共用）</td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 與[!DNL Workfront]個使用者共用行事曆 {#share-a-calendar-with-workfront-users}

共用行事曆與共用其他物件類似。 如需在[!DNL Adobe Workfront]中共用物件的詳細資訊，請參閱[物件共用許可權簡介](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)。

與您共用的行事曆會在行事曆名稱旁邊顯示星號(&#42;)。

若要在[!DNL Workfront]內共用行事曆：

1. 移至您要共用的行事曆。
1. 按一下行事曆名稱旁的&#x200B;**更多**&#x200B;功能表，然後按一下&#x200B;**共用**。
   ![行事曆更多功能表](assets/more-menu-calendar.png)
1. 在&#x200B;**[!UICONTROL 授與行事曆存取權]**&#x200B;欄位中，開始輸入您要共用行事曆的使用者、團隊、角色、群組或公司名稱，然後按一下顯示在下拉式清單中的名稱。\
   若要瞭解如何設定許可權，請參閱[物件許可權共用概述](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)。

1. （可選）針對您想要授與行事曆存取權的每個使用者、團隊、角色或群組，重複步驟3。
1. 按一下下拉式功能表，為您在步驟3中新增的每個使用者、團隊、角色、群組或公司指定許可權，然後選取您要授與的許可權層級：

   * **[!UICONTROL 檢視]：**&#x200B;使用者可以檢閱和共用行事曆。

     ![共用行事曆以檢視存取權](assets/view-calendar.png)

   * **[!UICONTROL 管理]：**&#x200B;使用者擁有行事曆的完整存取權，減去在存取層級授與的管理許可權，再加上所有檢視許可權。

     ![共用行事曆以管理存取權](assets/manage-calendar.png)

     >[!NOTE]
     >
     >[!DNL Workfront]管理員和行事曆建立者可以從這些實體移除許可權。

1. （選擇性）視使用者的角色而定，您可以按一下&#x200B;**[!UICONTROL 進階選項]**，然後按一下&#x200B;**[!UICONTROL 共用]**&#x200B;，讓使用者與其他使用者共用行事曆。

   如需許可權層級的詳細資訊，請參閱[物件共用許可權總覽](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)。

1. （選擇性）若要讓行事曆可供所有[!DNL Workfront]使用者使用，請按一下齒輪圖示，然後在下拉式功能表中按一下&#x200B;**[!UICONTROL 讓此物件在整個系統內可見]**，讓物件可供所有[!DNL Workfront]使用者使用。\
   所有使用者都可以根據您設定的許可權檢視物件。

1. 按一下「**[!UICONTROL 儲存]**」。

## 與公開連結共用行事曆

您可以公開行事曆，並與沒有[!DNL Workfront]授權的人共用連結。

1. 移至您要共用的行事曆。
1. 按一下&#x200B;**[!UICONTROL 行事曆動作]**，然後按一下&#x200B;**[!UICONTROL 共用]**。
1. 按一下行事曆名稱旁的&#x200B;**更多**&#x200B;功能表。
   ![行事曆更多功能表](assets/more-menu-calendar.png)
按一下&#x200B;**複製公開連結**。
1. 按一下「**[!UICONTROL 儲存]**」。

## 與私人連結共用行事曆

您可以與[!DNL Workfront]個使用者共用私人行事曆連結。 使用者需要登入才能在使用連結時檢視行事曆。

1. 移至您要共用的行事曆。
1. 按一下行事曆名稱旁的&#x200B;**更多**&#x200B;功能表，然後按一下&#x200B;**[!UICONTROL 取得可共用的連結]**。
   ![行事曆更多功能表](assets/more-menu-calendar.png)

   >[!NOTE]
   >
   >[!DNL Workfront]使用者必須擁有行事曆的存取權，才能透過連結存取行事曆。 若要授與存取權，請參閱[與 [!DNL Workfront] 使用者共用行事曆](#share-a-calendar-with-workfront-users)。\
   >如果使用者沒有存取權，他們可以在將連結貼入瀏覽器後要求。
