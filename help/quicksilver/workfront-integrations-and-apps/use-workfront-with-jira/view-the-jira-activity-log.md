---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-jira
title: 檢視Jira活動記錄
description: 作為 [!DNL Jira] 管理員，您可以在活動記錄檔中檢視同步處理或建立 [!DNL Adobe Workfront] 與 [!DNL Jira] 之間票證期間發生的例外狀況與錯誤。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 3e66c8e3-94b7-4153-abbb-32b872b9402b
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '307'
ht-degree: 0%

---

# 檢視[!UICONTROL [!DNL Jira]活動記錄]

作為[!DNL Jira]管理員，您可以在[!UICONTROL 活動記錄檔]中檢視同步處理或建立[!DNL Adobe Workfront]與[!DNL Jira]之間票證期間發生的例外狀況與錯誤。

您最多可在活動記錄中看到500個專案，這些專案會從最近的專案開始列出。

## 存取需求

您必須具備下列條件：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://business.adobe.com/products/workfront/pricing.html" target="_blank">[!DNL Adobe Workfront]計畫</a>*</td> 
   <td> <p>[！UICONTROL Pro]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe [!DNL Workfront]授權總覽</a>*</td> 
   <td> <p>[！UICONTROL計畫]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira] 存取</td> 
   <td> <p>系統管理員存取權</p> <p>重要：建議您在[!DNL Jira]和[!DNL Workfront]中建立個別的系統管理員帳戶以專用於此整合，而不使用可能附加至使用者的現有帳戶。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>您必須是[!DNL Workfront]管理員。 如需[!DNL Workfront]管理員的相關資訊，請參閱<a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予使用者完整管理存取權</a>。</p> <p>注意：如果您還是沒有存取權，請詢問您的[!DNL Workfront]管理員是否對您的存取層級設定了其他限制。 如需[!DNL Workfront]管理員如何修改存取層級的詳細資訊，請參閱<a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的[!DNL Workfront]管理員。

## 先決條件

在[!DNL Workfront]和[!DNL Jira]之間連結專案之前，您必須

* 安裝[!DNL Workfront for Jira]

  如需安裝[!DNL Workfront for Jira]的說明，請參閱[安裝 [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md)。

## 存取[!UICONTROL [!DNL Jira]活動記錄]：

1. 以系統管理員身分登入Jira。
1. 在主[!DNL Jira]功能表中按一下&#x200B;**[!UICONTROL 設定]**。
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
