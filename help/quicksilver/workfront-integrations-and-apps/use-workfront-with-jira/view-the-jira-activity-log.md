---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-jira
title: 檢視Jira活動記錄
description: 作為 [!DNL Jira] 管理員，您可以在活動記錄檔中檢視同步處理或建立 [!DNL Adobe Workfront] 與 [!DNL Jira] 之間票證期間發生的例外狀況與錯誤。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 3e66c8e3-94b7-4153-abbb-32b872b9402b
source-git-commit: b1b55b8046aa771abb2cceda333940ccf827356a
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 0%

---

# 檢視[!UICONTROL [!DNL Jira]活動記錄]

>[!IMPORTANT]
>
>為了提供更穩定且更可擴充的整合，我們改用現代、彈性的整合方法，即使用Workfront自動化與整合(Fusion)。 在此轉換過程中，Jira整合的Workfront在&#x200B;**2026年2月28日**&#x200B;後將無法使用。
>
>根據貴組織與Jira的整合需求，我們建議使用Workfront自動化和整合。
>
>如需Workfront自動化與整合的概觀，請參閱[Adobe Workfront Fusion概觀](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview)。
>
>如需Jira的Workfront自動化與整合模組特定功能的相關資訊，請參閱[Jira軟體模組](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/jira-software-modules)。

<!--

>[!IMPORTANT]
>
>To deliver more stable and scalable integrations, we're shifting to a modern, flexible integration approach using Workfront Automation and Integration (Fusion). As part of this transition process, the Workfront for Jira integration will not be available after **February 28, 2026**. 
>
>We recommend using Workfront Automation and Integration for your organization's integration needs with Jira. 
>
>Eight ready-to-use Workfront Automation and Integration templates for Jira will be available by August to help replicate common workflows and accelerate implementation. Templates are fully customizable to meet specific business needs and can be extended as requirements evolve. 
> 
>For an overview of Workfront Automation and Integration, see [Adobe Workfront Fusion overview](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview). 
>
>For information about the specific capabilities of the Workfront Automation and Integration modules for Jira, see [Jira Software modules](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/jira-software-modules). 

-->

作為[!DNL Jira]管理員，您可以在[!DNL Adobe Workfront]活動記錄檔[!DNL Jira]中檢視同步處理或建立[!UICONTROL 與]之間票證期間發生的例外狀況與錯誤。

您最多可在活動記錄中看到500個專案，這些專案會從最近的專案開始列出。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront套件</td> 
   <td><p>任何</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td><p>標準 </p>
       <p>規劃 </p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Jira存取</td> 
   <td> <p>系統管理員存取權</p> <p>重要：建議您在Jira和Workfront中建立個別系統管理員帳戶，以專門用於此整合，而不使用可能附加至使用者的現有帳戶。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>您必須是Workfront管理員。</p> </td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先決條件

在[!DNL Workfront]和[!DNL Jira]之間連結專案之前，您必須

* 安裝[!DNL Workfront for Jira]

  如需安裝[!DNL Workfront for Jira]的說明，請參閱[安裝 [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md)。

## 存取[!UICONTROL [!DNL Jira]活動記錄]：

1. 以系統管理員身分登入Jira。
1. 在主&#x200B;**[!UICONTROL 功能表中按一下]**&#x200B;設定[!DNL Jira]。
1. 按一下&#x200B;**[!UICONTROL 附加元件]**，然後按一下&#x200B;**[!UICONTROL 管理附加元件]**。

1. 展開&#x200B;**[!DNL Workfront]**&#x200B;附加元件。
1. 按一下&#x200B;**[!UICONTROL 設定]**。
1. 以系統管理員身分登入[!DNL Workfront]。
1. 選取&#x200B;**[!UICONTROL 活動記錄]**&#x200B;標籤。

   檢視建立專案或同步兩個應用程式之間欄位期間發生的例外和錯誤相關資訊。

   記錄檔包含下列欄位：

   * 發生日期
   * Jira中的使用者名稱
   * Jira問題編號
   * 所發生錯誤的簡短說明。
