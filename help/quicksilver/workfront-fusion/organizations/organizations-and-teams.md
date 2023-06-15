---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;user-management
navigation-topic: organizations
title: Adobe Workfront Fusion組織和團隊
description: Adobe Workfront Fusion的「組織」和「團隊」功能讓企業能夠控制Fusion中情景和其他功能的存取權。
author: Becky
feature: Workfront Fusion
exl-id: 601e937f-0286-4557-9a87-59aa9c0c22f1
source-git-commit: 392eee3c7b1aacf92d7877f07a8154924f3926a0
workflow-type: tm+mt
source-wordcount: '1111'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion] 組織和團隊

[!DNL Adobe Workfront Fusion]的「組織」和「團隊」功能讓企業能夠控制對Fusion中情境和其他功能的存取。

## 存取需求

您必須具有下列存取權才能使用本文中的功能：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] 計劃*</td> 
   <td> <p>[!DNL Pro] 或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Adobe Workfront Fusion]授權**</td> 
   <td> <p>Workfront Fusion for Work Automation and Integration，</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>貴組織必須購買 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文所述功能。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">存取層級設定*</td> 
   <td> 
     <p>您必須是 [!DNL Workfront Fusion] 您組織的管理員。</p>
     <p>您必須是 [!DNL Workfront Fusion] 您的團隊管理員。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

若要瞭解您擁有哪些計畫、授權型別或存取權，請聯絡您的 [!DNL Workfront] 管理員。

<p>**如需以下專案的資訊： [!DNL Adobe Workfront Fusion] 授權，請參閱 <a href="../../workfront-fusion/get-started/license-automation-vs-integration.md" class="MCXref xref">[!DNL Adobe Workfront Fusion] 授權</a></p>


## 組織

[!DNL Workfront Fusion] 使用者屬於一個組織。 您的 [!DNL Fusion] 授權會決定您的組織中有多少可用的使用中案例和聯結器。

[!DNL Fusion] 授權會決定組織可用的作用中案例和使用中應用程式數量。 [!DNL Fusion] 在組織儀表板上顯示目前的「作用中案例」和「作用中應用程式」計數。

* [組織角色](#organization-roles)
* [邀請使用者加入組織](#inviting-users-to-an-organization)
* [在組織之間切換](#switch-between-organizations)

### 組織角色

使用者在組織中擁有下列其中一種角色：

* **[!UICONTROL 所有者]**：擁有者擁有組織中可用的所有許可權。
* **[!UICONTROL 管理員]**：管理員角色可讓使用者建立和管理組織的團隊和使用者。
* **[!UICONTROL 會員]**：成員可以使用 [!DNL Workfront Fusion] 但無法進行組織變更。
* **[!UICONTROL 會計]**：會計師角色只允許使用者在組織儀表板上檢視授權資訊。
* **[!UICONTROL 應用程式開發人員]**：此角色的功能目前無法使用，且將在不久的將來提供。 我們目前不建議將使用者指派給此角色。

### 邀請使用者加入組織

依預設，組織所有者（或授權的使用者）可以邀請其他人加入其組織。

若要邀請使用者加入組織：

1. 按一下 **[!UICONTROL 變更詳細資料]** 在熒幕的右上角。
1. 選取 **[!UICONTROL 邀請新使用者]**.

   ![](assets/fusion-organization-invite-user-350x199.png)

1. 填寫使用者的電子郵件地址和名稱。
1. 選取使用者的角色。 有關角色的詳細資訊，請參閱 [組織角色](#organization-roles) 於本檔案中。
1. （選用）新增附註。 此附註會顯示在使用者收到的邀請電子郵件中。
1. 按一下&#x200B;**[!UICONTROL 儲存]**。

[!DNL Fusion] 傳送一封包含特定組織邀請的電子郵件，並 [!UICONTROL 接受角色] 按鈕。

![](assets/accept-the-role.png)

收件者按一下按鈕後，系統會將他們重新導向至邀請頁面，以便他們接受邀請。

邀請將於一天後過期。

>[!NOTE]
>
>如果使用者是初次使用 [!DNL Fusion]， [!DNL Fusion] 自動為他們建立帳戶，並傳送一封包含臨時密碼的電子郵件，指示新使用者登入並變更其密碼。

### 在組織之間切換

您可能屬於Fusion中的多個組織。 資源不會在組織之間共用。

您可以按一下右上角的組織名稱，然後從下拉式選單中選取新組織，在Adobe整合式體驗中切換組織。 即使您是Adobe中其他組織的成員，下拉式清單中仍只會顯示具有Fusion帳戶的組織。

## 團隊

團隊是共用特定資源存取許可權的使用者群組。 這些資源可能包括：

* 情景
* 連線
* Webhook
* 金鑰
* 資料存放區
* 資料結構
* 電子郵件通知設定

>[!NOTE]
>
>由於專案團隊可控制對資源的存取，因此專案團隊只有一名成員有時很實用。 例如，訓練中的使用者可以建立與其個人的連線 [!DNL Google] 帳戶。 任何團隊成員也可以連線到個人 [!DNL Google] 帳戶，所以在這種情況下，最好讓使用者成為培訓團隊的唯一成員。

組織可以擁有所需數量的團隊，使用者可以屬於一個或多個團隊。

使用者可以從左側導覽面板的下拉式清單中選取其團隊。 使用者只會看見他們所屬的團隊。 選取團隊將允許使用者存取該團隊的資源。

* [團隊角色](#team-roles)
* [團隊管理](#team-management)

### 團隊角色

使用者在每個團隊中具有以下角色之一：

* **[!UICONTROL 團隊管理員]**：除了其他專案團隊角色的功能，管理員角色還允許使用者新增、移除或更改專案團隊成員的角色。
* **[!UICONTROL 團隊成員]**：團隊成員角色可讓使用者建立和執行情境。
* **[!UICONTROL 團隊監視]**：此 [!UICONTROL 監視] 角色可讓使用者存取情境的執行資訊，但他們無法設計情境或變更其「作用中」狀態。
* **[!UICONTROL 團隊操作員]**：此 [!UICONTROL 運運算元] 角色可讓使用者檢視執行資料並變更案例的「作用中」狀態。
* **[!UICONTROL 團隊受限制的成員]**：此角色的功能目前無法使用，且將在不久的將來提供。 我們目前不建議將使用者指派給此角色。

### 團隊管理

* [建立團隊](#create-a-team)
* [設定團隊通知選項](#set-team-notification-options)

#### 建立團隊

組織擁有者和管理員能夠建立團隊。

若要建立專案團隊：

1. 在左側導覽面板中，按一下 **[!UICONTROL 組織]**
1. 選取 **[!UICONTROL 團隊]** 標籤。
1. 按一下 **[!UICONTROL 新增團隊]** 在團隊清單下。
1. 輸入新團隊的名稱，然後按一下 **新增**.

#### 設定團隊通知選項

電子郵件通知選項是在團隊層級上設定的。

1. 在左側導覽面板中，按一下 **[!UICONTROL 團隊]**
1. 選取 **[!UICONTROL 通知選項]** 標籤。
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
      <td><p>當案例停用時收到電子郵件。</p><p><b>注意：</b> 只有在案例因錯誤而自動停用時，您才會收到案例停用的通知。 您不會收到有關手動停用案例的通知。</p><p>在某些情況下，情境可能會被 [!DNL Workfront Fusion] 工程團隊，因為此情境會導致效能或其他問題。 在這些情況下，您不會收到以下專案的通知： [!DNL Workfront Fusion]. </p></td>

</tr>
</tbody>
</table>

自動儲存通知選項的變更

#### 在群組之間切換

您可能屬於Fusion中的多個群組。 由於團隊不共用資源，因此您可能需要切換團隊以存取特定案例或其他資源。

如果您的組織不在Adobe統一體驗中，您可以按一下左側導覽中的團隊名稱，然後從下拉式選單中選取團隊來切換團隊。

如果您的團隊在Adobe統一體驗，您可以按一下標題中的團隊名稱，然後從下拉式選單中選取團隊來選取新團隊。 此選項適用於特定團隊的所有頁面，例如案例頁面或「連線」頁面。

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/organization-add-team-350x181.png" style="width: 350;height: 181;"> </p>
-->