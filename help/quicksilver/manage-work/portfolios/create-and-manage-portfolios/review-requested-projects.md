---
product-area: portfolios;projects
navigation-topic: create-and-manage-portfolios
title: 檢閱請求的專案
description: 專案請求在Adobe Workfront中顯示為[!UICONTROL 已請求]狀態的專案。 本文會介紹如何稽核專案請求。
author: Alina
feature: Work Management, Strategic Planning
exl-id: 1acfb885-0da3-495d-ba66-e80e339e90de
source-git-commit: cf3466759a7263c446525b97dd2748ad17d0f7a6
workflow-type: tm+mt
source-wordcount: '479'
ht-degree: 0%

---

# 檢閱請求的專案

當提交多個專案請求以供稽核時，專案管理辦公室或專案組合委員會可以開會以稽核提交的請求，並決定專案請求核准。 專案請求在[!DNL Adobe Workfront]中顯示為狀態為[!UICONTROL 已請求]的專案。

您可以執行下列其中一項作業來提交專案請求以供複查：

* 將專案狀態變更為&#x200B;**[!UICONTROL 已要求]**。
* 完成專案的[!UICONTROL 業務案例]，並提交核准。\
   如需有關完成專案商業案例的詳細資訊，請參閱[建立專案的商業案例](../../../manage-work/projects/define-a-business-case/create-business-case.md)。

您可以在[!DNL Adobe Workfront]的下列區域中檢閱請求的專案：

* 在專案報告中
* 在投資組合內

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計畫*</td> 
   <td> <p>[！UICONTROL Business]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權*</td> 
   <td> <p>[！UICONTROL計畫] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>[！UICONTROL View]或更高版本的Portfolio存取權</p> <p>[！UICONTROL Edit]專案的存取權</p> <p>注意：如果您還是沒有存取權，請詢問您的[!DNL Workfront]管理員是否對您的存取層級設定了其他限制。 如需[!DNL Workfront]管理員如何變更您的存取層級的詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>投資組合上的[！UICONTROL View]許可權或更高</p> <p>[！UICONTROL Manage]專案許可權可更新其狀態</p> <p>如需請求其他存取權的資訊，請參閱<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求物件</a>的存取權。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的[!DNL Workfront]管理員。

## 在專案報告中檢閱請求的專案

您可以建立專案報告，以檢視哪些專案具有[!UICONTROL 已要求]的狀態。

如需有關建立專案報告以核准專案請求的詳細資訊，請參閱[核准業務案例](../../../manage-work/projects/define-a-business-case/approve-business-case.md)中的[[!UICONTROL 建立專案報告以核准業務案例]](../../../manage-work/projects/define-a-business-case/approve-business-case.md#build-a-report)區段。 

## 檢閱投資組合中請求的專案

1. 前往您要檢閱其請求專案的投資組合。
1. 按一下左側面板中的&#x200B;**[!UICONTROL 專案]**
1. 從&#x200B;**[!UICONTROL 篩選器]**&#x200B;下拉式功能表中，選取&#x200B;**[!UICONTROL 已要求]**。

   清單中只會顯示狀態為&#x200B;**[!UICONTROL 已要求]**&#x200B;的專案。

   >[!TIP]
   >
   > 除了具有&#x200B;**[!UICONTROL 已要求]**&#x200B;的狀態外，專案還必須與選取的Portfolio相關聯，才能顯示在此清單中。

1. 按一下清單中專案的名稱以開啟。
1. 按一下左側面板中的&#x200B;**[!UICONTROL 專案詳細資料]**。
1. 執行下列任一項作業：

   * 按一下&#x200B;**[!UICONTROL 業務案例]**，然後按一下[!UICONTROL 業務案例摘要]區域中的&#x200B;**[!UICONTROL 核准]**&#x200B;或&#x200B;**[!UICONTROL 拒絕]**，以核准或拒絕業務案例。

     ![approve_or_reject_business_case.png](assets/approve-or-reject-business-case-350x563.png)

     若業務案例已核准，專案狀態會變更為&#x200B;**[!UICONTROL 已核准]**。

     若業務案例被拒絕，專案狀態會變更為&#x200B;**[!UICONTROL 已拒絕]**。

     >[!NOTE]
     >
     >沒有通知可提醒提交業務案例核准的使用者其專案請求是否核准或拒絕。 

     或

   * 在&#x200B;**[!UICONTROL 狀態]**&#x200B;下拉式功能表中，將專案狀態變更為任何其他狀態。

     ![](assets/project-status-change-from-drop-down-in-header-nwe-350x294.png)
 

 
