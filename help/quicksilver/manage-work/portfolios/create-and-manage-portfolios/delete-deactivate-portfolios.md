---
product-area: portfolios
navigation-topic: create-and-manage-portfolios
title: 刪除和停用投資組合
description: Portfolio是Adobe Workfront中的專案或方案的集合。 如果您發現某個投資組合與您的系統無關，您可以將其刪除或停用。
author: Alina
feature: Work Management, Strategic Planning
exl-id: f88669d2-e8e9-4905-a771-1427b1fd32b2
source-git-commit: b774a74863bb35e3477a69ff11189c40a6d66437
workflow-type: tm+mt
source-wordcount: '417'
ht-degree: 0%

---

# 刪除和停用投資組合

Portfolio是中專案或方案的集合 [!DNL Adobe Workfront]. 如果您發現某個投資組合與您的系統無關，您可以將其刪除或停用。

我們建議停用不再需要與未來專案關聯的專案組合，而不是刪除它，以保留目前與專案組合及其方案關聯的專案上的歷史資訊。

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計劃*</td> 
   <td> <p>任何 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權*</td> 
   <td> <p>[！UICONTROL計畫] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>[！UICONTROL Edit]專案和Portfolio的存取權</p> <p>注意：如果您還是沒有存取權，請詢問您的 [!DNL Workfront] 管理員是否對您的存取層級設定其他限制。 如需瞭解如何 [!DNL Workfront] 管理員可以變更您的存取層級，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>投資組合的[！UICONTROL Manage]許可權 </p> <p>如需請求其他存取許可權的詳細資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">要求物件的存取權 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的 [!DNL Workfront] 管理員。

## 刪除和停用投資組合的概觀

在決定是否刪除或停用投資組合時，請考慮下列事項：

* 刪除投資組合會刪除與其關聯的計畫。

  >[!IMPORTANT]
  >
  >您不需要擁有程式的任何許可權就能刪除投資組合。

* 刪除投資組合不會刪除與其相關聯的專案。
* 您無法復原已刪除的投資組合。
* 停用專案組合可確保建立專案時，專案組合及其方案的名稱不再指派給專案。

## 停用投資組合

當您停用投資組合時，您仍然可以從以下位置存取它： [!UICONTROL Portfolio] 區域，但使用者嘗試將其新增至專案時，其不再顯示在投資組合清單中。

>[!NOTE]
>
>視您的 [!DNL Workfront] 或群組管理員設定您的配置範本， [!UICONTROL Portfolio] 區域可能不會顯示在 [!UICONTROL 主要功能表]. 如需詳細資訊，請參閱 [使用版面配置範本自訂主功能表](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md)

1. 按一下 **[!UICONTROL 主要功能表]** 圖示 ![](assets/main-menu-icon.png) 位於的右上角 [!DNL Adobe Workfront].

1. 按一下 **[!UICONTROL Portfolio]** .
1. 按一下投資組合的名稱。
1. 按一下「更多」功能表 ![](assets/more-icon.png) 投資組合名稱右側，然後按一下 **[!UICONTROL 停用Portfolio]**.

## 刪除投資組合

1. 按一下 **[!UICONTROL 主要功能表]** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角。

1. 按一下 **[!UICONTROL Portfolio]** .
1. 選取投資組合，然後按一下 **[!UICONTROL 刪除]**&#x200B;這&#x200B;個 [!UICONTROL 刪除] 圖示 ![](assets/delete.png).
1. 在出現的方塊中，按一下 **[!UICONTROL 是的，刪除]** 以確認。
