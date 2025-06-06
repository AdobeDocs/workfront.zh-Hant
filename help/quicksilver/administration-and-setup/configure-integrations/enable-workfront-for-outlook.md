---
title: '為Outlook啟用 [!DNL Adobe Workfront] '
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
description: 在使用者開始使用Outlook的 [!DNL Adobe Workfront] 之前，您必須先為您的系統啟用它。
author: Lisa, Becky
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
exl-id: be523b27-191f-46ca-9a87-d512f9a15a1e
source-git-commit: b4b45bbc8bb68dbac35488c1777fca85fa0cc7e3
workflow-type: tm+mt
source-wordcount: '312'
ht-degree: 1%

---

# 啟用 [!DNL Adobe Workfront for Outlook]

>[!IMPORTANT]
>
>[Microsoft正在停用對舊版Exchange Online權杖](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens)的支援，Workfront Outlook增益集目前使用這些權杖進行驗證。 Microsoft的這項變更已開始影響客戶，並將在2025年10月前持續分階段推出。
>
>* **在Microsoft完全停用這些Token後，適用於Microsoft Outlook整合的Workfront將無法繼續運作。**
>
>在這次變更中，Microsoft已決定變更代號重新啟用的方式。 在&#x200B;**2025年6月30日**&#x200B;之後，管理員將無法再自行重新啟用權杖 — 只有Microsoft支援可授予例外狀況。 **在2025年10月1日，所有租使用者的舊版代號將會關閉。 將不會授與例外。**


在使用者開始使用[!DNL Adobe Workfront for Outlook]之前，您必須先為您的系統啟用它。

如需如何在啟用[!DNL Workfront for Outlook]之後使用的資訊，請參閱[[!DNL Adobe Workfront for Outlook]](../../workfront-integrations-and-apps/using-workfront-with-outlook/workfront-for-outlook.md)。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具備下列專案才能執行本文所述的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計劃</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權</td> 
   <td>[！UICONTROL計畫]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>您必須是[!DNL Workfront]管理員。 如需[!DNL Workfront]管理員的相關資訊，請參閱<a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予使用者完整管理存取權</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的[!DNL Workfront]管理員。

+++

## 啟用[!DNL Workfront] [!DNL Outlook]增益集

1. 以系統管理員身分登入[!DNL Workfront]。

{{step-1-to-setup}}

1. 展開&#x200B;**[!UICONTROL 系統]**，然後按一下&#x200B;**[!UICONTROL 偏好設定]**。

1. 確定&#x200B;**[!UICONTROL 允許人員使用Workfront的行動應用程式，且已選取[!DNL Workfront] [!DNL Outlook]增益集]**。\
   除了允許使用[!DNL Workfront]行動應用程式之外，此設定也允許使用[!DNL Workfront] [!DNL Outlook]增益集。

   此選項預設為啟用。

1. 按一下「**[!UICONTROL 儲存]**」。

## 正在安裝[!DNL Workfront] [!DNL Outlook]增益集

如需有關使用[!DNL Outlook]的[!DNL Workfront]增益集的系統需求資訊，請參閱[為 [!DNL Outlook]](../../workfront-integrations-and-apps/using-workfront-with-outlook/set-up-workfront-for-outlook.md)設定Adobe Workfront中的[系統需求](../../workfront-integrations-and-apps/using-workfront-with-outlook/set-up-workfront-for-outlook.md#system-requirements-and-prerequisites)。

如需如何為[!DNL Outlook]安裝[!DNL Workfront]增益集的資訊，請參閱[在[設定 [!DNL Adobe Workfront for Outlook]](../../workfront-integrations-and-apps/using-workfront-with-outlook/set-up-workfront-for-outlook.md)中安裝增益集](../../workfront-integrations-and-apps/using-workfront-with-outlook/set-up-workfront-for-outlook.md#downloading-and-installing-the-add-in)。
