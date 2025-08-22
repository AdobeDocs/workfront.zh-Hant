---
title: 設定 [!DNL Workfront] 與 [!DNL Frame.io] 整合
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
description: 身為 [!DNL Adobe Workfront] 管理員，您可以整合 [!DNL Workfront] 與 [!DNL Frame.io] ，並提供組織順暢的檢閱與核准資產方式。
author: Courtney
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
hide: true
hidefromtoc: true
exl-id: 7d909976-d3ff-4e60-9158-c3bffe498e6e
source-git-commit: 5a2df341a54d305807a1c9f175baf60b9007ffa2
workflow-type: tm+mt
source-wordcount: '421'
ht-degree: 0%

---

# 設定[!DNL Workfront]與[!DNL Frame.io]整合

Workfront管理員可啟用Workfront與Frame.io之間的整合，方法是在「設定」區域中設定預設Frame.io帳戶，然後在Workfront中指定Frame.io使用者。 如此一來，專案協調員就能使用Workfront專案來計畫及啟動工作，並可檢閱及核准工作流程。


## 存取需求

<!--DELETE THIS SECTION MARCH 2026-->
<!--
>[!IMPORTANT]
>
>This functionality is available only to organization that have been onboarded to the [!DNL Adobe Admin Console].-->

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

<table>
  <tr>
   <td>[!DNL Adobe Workfront] 計劃</td>
   <td>任何</td>
  </tr>
  <tr>
   <td>[!DNL Adobe Workfront] 授權
   </td>
   <td><p>目前： [！UICONTROL計畫]</p>
   <p>新增：[！UICONTROL Standard]</p></td>
  </tr>
  <tr>
   <td>存取層級設定
   </td>
   <td>您必須是[!DNL Workfront]管理員。
   </td>
  </tr>

</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 設定預設[!DNL Frame.io]帳戶[!BADGE 即將推出]{type=Informative}

設定預設的[!DNL Frame.io]帳戶後，在[!DNL Workfront]中建立的任何專案都會在Frame.io中建立映象專案。

>[!IMPORTANT]
>
>此功能即將推出。 目前，Frame.io帳戶是由Workfront團隊手動新增。 請聯絡您的Adobe客戶代表以尋求協助。

## 使用Workfront群組設定單一Frame.io帳戶

您可以使用與預設帳戶不同的單一Frame.io帳戶來連線單一Workfront群組。

若要使用Workfront群組設定單一Frame.io帳戶：

{{step-1-to-setup}}

1. 在左側面板中，按一下&#x200B;**群組**。
1. 選擇現有的群組，或按一下[建立群組] ****。
1. 在左側面板中，按一下&#x200B;**連線到Frame.io**。
1. 輸入API開發人員權杖。
1. 按一下&#x200B;**起始連線**。
1. （視條件而定）如果您是多個Frame.io帳戶的管理員，請選取您要使用的帳戶。

## 啟用Frame.io使用者

經常使用Frame.io的Workfront使用者應標示為Frame.io使用者。 Workfront管理員可以在Workfront使用者設定檔中指定Frame.io使用者。

>[!TIP]
>
>我們建議讓經常使用創意工具及上傳資產的使用者能夠以Frame.io使用者的身分檢閱和核准。

當使用者在Workfront中標示為Frame.io使用者並新增至專案時：

* 他們在Frame.io中新增為共同作業人員。<!--do we need to be more explicit about a frame license being provisioned for them?-->
* 他們可以從Frame.io將資產傳送到Workfront以進行正式檢閱和核准。
* 他們可以從Workfront在單向同步資料夾中檢視資訊。 [!BADGE 即將推出]{type=Informative}

若要啟用Frame.io使用者：

{{step-1-to-users}}

1. 選取一或多個使用者，然後按一下&#x200B;**編輯**&#x200B;圖示![編輯圖示](assets/edit-icon.png)。
1. 在「存取」區段中，啟用「新增至Frame.io中的專案」核取方塊，然後在下拉式選單中選取&#x200B;**是**。
   ![新增到框架專案](assets/add-to-frame-project.png)

   >[!NOTE]
   >
   >如果未核取此方塊，則使用者會保留對過去指派的存取權，並加入往後的Frame.io專案。<!-- If the user is deactivated, they lose all access to previous assignments and are removed from the Frame.io account.-->
