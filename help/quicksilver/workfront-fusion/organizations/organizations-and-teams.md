---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;user-management
navigation-topic: organizations
title: Adobe Workfront Fusion組織和團隊
description: Adobe Workfront Fusion檔案已移至新位置。 本文已棄用，但包含新文章的連結，內容涵蓋此功能。
author: Becky
feature: Workfront Fusion
exl-id: 601e937f-0286-4557-9a87-59aa9c0c22f1
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '1300'
ht-degree: 1%

---

# [!DNL Adobe Workfront Fusion]組織和團隊

>[!IMPORTANT]
>
>Adobe Workfront Fusion檔案已移至新位置。
>
>本文資訊可在以下文章中找到：
>
>* [Adobe Workfront Fusion組織和團隊概觀](https://experienceleague.adobe.com/docs/workfront-fusion/using/set-up-and-manage-fusion/set-up-and-manage-orgs-and-teams/set-up-orgs-teams-and-users/org-and-team-overview.html)
>* [設定團隊通知選項](https://experienceleague.adobe.com/docs/workfront-fusion/using/set-up-and-manage-fusion/set-up-and-manage-orgs-and-teams/set-up-orgs-teams-and-users/set-team-notification-options.html)
>
>請更新任何書籤。
>
>本文已不再更新，將於不久將來移除。

[!DNL Adobe Workfront Fusion]的組織與團隊功能可讓企業控制Fusion中案例與其他功能的存取權。

## 存取需求

您必須具有下列存取權才能使用本文中的功能：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] 計畫*</td> 
   <td> <p>[!DNL Pro] 或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Adobe Workfront Fusion]授權**</td> 
   <td>
   <p>目前授權需求：無[!DNL Workfront Fusion]授權需求。</p>
   <p>或</p>
   <p>舊版授權需求： [！UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration]，[！UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>
   <p>目前產品需求：如果您有[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Adobe Workfront]計畫，您的組織必須購買[!DNL Adobe Workfront Fusion]及[!DNL Adobe Workfront]，才能使用本文所述的功能。 [!DNL Workfront Fusion]包含在[！UICONTROL Ultimate] [!DNL Workfront]計畫中。</p>
   <p>或</p>
   <p>舊版產品需求：您的組織必須購買[!DNL Adobe Workfront Fusion]及[!DNL Adobe Workfront]，才能使用本文所述的功能。</p>
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">存取層級設定*</td> 
   <td> 
     <p>您必須是組織的[!DNL Workfront Fusion]管理員。</p>
     <p>您必須是團隊的[!DNL Workfront Fusion]管理員。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的[!DNL Workfront]管理員。

<p>**如需[!DNL Adobe Workfront Fusion]授權的相關資訊，請參閱<a href="../../workfront-fusion/get-started/license-automation-vs-integration.md" class="MCXref xref">[!DNL Adobe Workfront Fusion]授權</a></p>


## 組織

[!DNL Workfront Fusion]個使用者屬於某個組織。

* [組織角色](#organization-roles)
* [邀請使用者加入組織](#inviting-users-to-an-organization)
* [在組織之間切換](#switch-between-organizations)

### 組織角色

使用者在組織中擁有下列其中一種角色：

* **[!UICONTROL 所有者]**：所有者擁有組織中可用的所有許可權。
* **[!UICONTROL 管理員]**：管理員角色可讓使用者建立和管理組織的團隊和使用者。
* **[!UICONTROL 成員]**：成員可以使用[!DNL Workfront Fusion]，但無法進行組織變更。
* **[!UICONTROL 會計]**：會計師角色只允許使用者在組織儀表板上檢視授權資訊。
* **[!UICONTROL 應用程式開發人員]**：此角色的功能目前無法使用，而且將在不久的將來提供。 我們目前不建議將使用者指派給此角色。

如需每個組織角色中使用者可用的特定動作資訊，請參閱[組織和團隊角色](/help/quicksilver/workfront-fusion/organizations/organization-roles.md)。

### 邀請使用者加入組織

依預設，組織擁有者（或授權的使用者）可以邀請其他人加入其組織。

若要邀請使用者加入組織：

1. 按一下畫面右上角的&#x200B;**[!UICONTROL 變更詳細資料]**。
1. 選取&#x200B;**[!UICONTROL 邀請新使用者]**。

   ![](assets/fusion-organization-invite-user-350x199.png)

1. 填寫使用者的電子郵件地址和名稱。
1. 選取使用者的角色。 如需角色的詳細資訊，請參閱本檔案中的[組織角色](#organization-roles)。
1. （選用）新增附註。 此附註會顯示在使用者收到的邀請電子郵件中。
1. 按一下「**[!UICONTROL 儲存]**」。

[!DNL Fusion]傳送一封電子郵件，其中包含特定組織的邀請及[!UICONTROL 接受角色]按鈕。

當收件者按一下按鈕時，系統會將他們重新導向至邀請頁面，讓他們接受邀請。

邀請將於一天後過期。

>[!NOTE]
>
>如果使用者是[!DNL Fusion]的新使用者，[!DNL Fusion]會自動為他們建立帳戶，並傳送一封包含臨時密碼的電子郵件，指示新使用者登入並變更其密碼。

### 在組織之間切換

您可能屬於Fusion中的多個組織。 資源不會在組織之間共用。

您可以按一下右上角的組織名稱，然後從下拉式選單中選取新組織，在Adobe統一體驗中切換組織。 即使您是Adobe中其他組織的成員，下拉式清單中仍只會顯示具有Fusion帳戶的組織。

## 團隊

團隊是共用特定資源存取許可權的使用者群組。 這些資源可能包括：

* 情境
* 連線
* Webhook
* 金鑰
* 資料儲存區
* 資料結構
* 電子郵件通知設定

>[!NOTE]
>
>由於專案團隊可控制對資源的存取，因此專案團隊只擁有一名成員有時相當實用。 例如，訓練中的使用者可以建立與其個別[!DNL Google]帳戶的連線。 任何團隊成員也可以連線至個別[!DNL Google]帳戶，因此在此情況下，最好讓使用者成為訓練團隊的唯一成員。

組織可以擁有任意所需數量的團隊，使用者可以屬於一個或多個團隊。

使用者可從左側導覽面板的下拉式清單中選取其團隊。 使用者只會看到他們所屬的團隊。 選取團隊將允許使用者存取該團隊的資源。

* [團隊角色](#team-roles)
* [團隊管理](#team-management)

### 團隊角色

使用者在其每個團隊中具有以下角色之一：

* **[!UICONTROL 團隊管理員]**：除了其他團隊角色的功能外，管理員角色還可讓使用者新增、移除或變更團隊成員的角色。
* **[!UICONTROL 團隊成員]**：團隊成員角色可讓使用者建立和執行案例。
* **[!UICONTROL 團隊監控]**： [!UICONTROL 監控]角色可讓使用者存取案例的執行資訊，但他們無法設計案例或變更其「作用中」狀態。
* **[!UICONTROL 團隊運運算元]**： [!UICONTROL 運運算元]角色可讓使用者檢視執行資料，並變更案例的「作用中」狀態。
* **[!UICONTROL 團隊受限制成員]**：此角色的功能目前無法使用，而且將在不久的將來提供。 我們目前不建議將使用者指派給此角色。

如需每個專案團隊角色中使用者可用的特定動作資訊，請參閱[組織和專案團隊角色](/help/quicksilver/workfront-fusion/organizations/organization-roles.md)。

### 團隊管理

* [建立團隊](#create-a-team)
* [設定團隊通知選項](#set-team-notification-options)

#### 建立團隊

組織擁有者和管理員能夠建立團隊。

若要建立專案團隊：

1. 在左側導覽面板中，按一下&#x200B;**[!UICONTROL 組織]**
1. 選取「**[!UICONTROL 團隊]**」標籤。
1. 按一下團隊清單下的&#x200B;**[!UICONTROL 新增團隊]**。
1. 輸入新團隊的名稱，然後按一下&#x200B;**新增**。

#### 設定團隊通知選項

>[!NOTE]
>
>如果您的組織已移至Unified Shell，您將會透過「Adobe通知」區域收到通知。 您必須使用Unified Shell體驗才能在Adobe通知區域中檢視通知。
>
>若要使用Unified Shell Experience (包括Adobe通知區域)，請按一下靠近頁面頂端的在Unified Experience中嘗試新的Fusion UI按鈕。 此按鈕僅在您的組織已移至Unified Shell時可用。
>
>如需詳細資訊，請參閱[在[!DNL Adobe Unified Experience]中存取[!DNL Workfront Fusion]的通知](/help/quicksilver/workfront-fusion/fusion-in-admin-console/fusion-unified-experience.md#access-your-notifications)。

在團隊層級設定電子郵件通知選項。

1. 在左側導覽面板中，按一下&#x200B;**[!UICONTROL 團隊]**
1. 選取&#x200B;**[!UICONTROL 通知選項]**&#x200B;標籤。
1. 啟用您希望團隊收到的通知。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">'[！UICONTROL案例執行中的警告]'</td> 
      <td> <p>當案例執行中有警告時收到電子郵件</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">情景執行中的[！UICONTROL錯誤]</td> 
      <td>當案例執行中發生錯誤時收到電子郵件。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[！UICONTROL案例停用]</p> </td> 
      <td><p>當案例停用時收到電子郵件。</p><p><b>注意：</b>只有在案例因錯誤而自動停用時，您才會收到案例停用的通知。 您沒有收到有關手動停用案例的通知。</p><p>在某些情況下，案例可能會由[!DNL Workfront Fusion]工程團隊停用，因為案例會導致效能或其他問題。 在這些情況下，您不會在[!DNL Workfront Fusion]中收到通知。 </p></td>

</tr>
</tbody>
</table>

通知選項的變更會自動儲存

#### 在團隊之間切換

您可能屬於Fusion中的多個群組。 由於專案團隊不共用資源，因此您可能需要切換專案團隊以存取特定案例或其他資源。

如果您的組織不在Adobe統一體驗中，您可以按一下左側導覽中的團隊名稱，然後從下拉式選單中選取團隊來切換團隊。

如果您的團隊在AdobeUnified Experience，您可以按一下標題中的團隊名稱並從下拉式選單中選取團隊來選取新團隊。 此選項適用於特定團隊的所有頁面，例如案例頁面或「連線」頁面。

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/organization-add-team-350x181.png" style="width: 350;height: 181;"> </p>
-->