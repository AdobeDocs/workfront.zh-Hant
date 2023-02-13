---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;user-management
navigation-topic: organizations
title: Adobe Workfront Fusion組織和團隊
description: Adobe Workfront Fusion的組織和團隊功能使企業能夠控制對Fusion中方案和其他功能的訪問。
author: Becky
feature: Workfront Fusion
exl-id: 601e937f-0286-4557-9a87-59aa9c0c22f1
source-git-commit: e58ff769015b8c4e34b34eea653f55a296eea371
workflow-type: tm+mt
source-wordcount: '922'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion] 組織和團隊

[!DNL Adobe Workfront Fusion]組織和團隊功能使企業能夠控制對Fusion中方案和其他功能的訪問。

## 存取需求

您必須具備下列存取權才能使用本文中的功能：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] 計劃*</td> 
   <td> <p>[!DNL Pro] 或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion]授權**</td> 
   <td> <p>Workfront Fusion for Work Automation and Integration,</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>貴組織必須購買 [!DNL Adobe Workfront Fusion] 和 [!DNL Adobe Workfront] 以使用本文所述的功能。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> 
     <p>您必須是 [!DNL Workfront Fusion] 管理員。</p>
     <p>您必須是 [!DNL Workfront Fusion] 管理員。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

若要了解您擁有的計畫、授權類型或存取權，請聯絡您的 [!DNL Workfront] 管理員。

<p>**有關 [!DNL Adobe Workfront Fusion] 許可證，請參閱 <a href="../../workfront-fusion/get-started/license-automation-vs-integration.md" class="MCXref xref">[!DNL Adobe Workfront Fusion] 授權</a></p>


## 組織

[!DNL Workfront Fusion] 使用者屬於某個組織。 您的 [!DNL Fusion] 授權可決定貴組織有多少個使用中案例和連接器。

[!DNL Fusion] 授權會決定組織可用的作用中案例和作用中應用程式數目。 [!DNL Fusion] 在組織控制面板上顯示目前的「作用中案例」和「作用中應用程式」計數。

* [組織角色](#organization-roles)
* [邀請使用者加入組織](#inviting-users-to-an-organization)

### 組織角色

使用者在組織中具有下列其中一個角色：

* **[!UICONTROL 擁有者]**:擁有者擁有組織中可用的所有權限。
* **[!UICONTROL 管理]**:管理員角色可讓使用者建立及管理組織的團隊和使用者。
* **[!UICONTROL 會員]**:成員可以使用 [!DNL Workfront Fusion] 但無法進行組織變更。
* **[!UICONTROL 會計]**:會計角色只允許用戶查看組織儀表板上的許可證資訊。
* **[!UICONTROL 應用程式開發人員]**:此角色的功能目前無法使用，並將於近期提供使用。 目前不建議將使用者指派給此角色。

### 邀請使用者加入組織

依預設，組織擁有者（或授權使用者）可邀請其他人加入其組織。

若要邀請使用者加入組織：

1. 按一下 **[!UICONTROL 變更詳細資訊]** 在螢幕的右上角。
1. 選擇 **[!UICONTROL 邀請新使用者]**.

   ![](assets/fusion-organization-invite-user-350x199.png)

1. 填寫使用者的電子郵件地址和名稱。
1. 為用戶選擇角色。 如需角色的詳細資訊，請參閱 [組織角色](#organization-roles) 在此文檔中。
1. （選用）新增附註。 此附註會顯示在使用者收到的邀請電子郵件中。
1. 按一下&#x200B;**[!UICONTROL 儲存]**。

[!DNL Fusion] 傳送電子郵件並附上邀請給特定組織，並 [!UICONTROL 接受角色] 按鈕。

![](assets/accept-the-role.png)

收件者按一下按鈕後，會重新導向至邀請頁面，以便接受邀請。

邀請將在一天後過期。

>[!NOTE]
>
>如果使用者是新使用者 [!DNL Fusion], [!DNL Fusion] 會自動為使用者建立帳戶，並傳送包含暫時密碼的電子郵件，引導新使用者登入並變更其密碼。

## 團隊

團隊是共用特定資源存取權的使用者群組。 這些資源可能包括：

* 情景
* 連線
* Webhook
* 金鑰
* 資料儲存
* 資料結構
* 電子郵件通知設定

>[!NOTE]
>
>由於團隊控制對資源的訪問，因此團隊有時只有一個成員是很有用的。 例如，訓練中的使用者可以建立與其個人的連線 [!DNL Google] 帳戶。 任何團隊成員也能連線至個人 [!DNL Google] 帳戶，因此在此情況下，最好讓使用者成為訓練團隊的唯一成員。

組織可能擁有所需的團隊數，而使用者可能屬於一或多個團隊。

使用者可從左側導覽面板的下拉式清單中選取其團隊。 使用者只看到自己所屬的團隊。 選取團隊可讓使用者存取該團隊的資源。

* [團隊角色](#team-roles)
* [團隊管理](#team-management)

### 團隊角色

使用者在其每個團隊中都具有下列其中一個角色：

* **[!UICONTROL 團隊管理員]**:除了其他團隊角色的功能之外，管理員角色還允許用戶添加、刪除或更改團隊成員的角色。
* **[!UICONTROL 團隊成員]**:團隊成員角色允許用戶建立和執行方案。
* **[!UICONTROL 團隊監控]**:此 [!UICONTROL 監控] 角色允許用戶訪問方案的執行資訊，但無法設計方案或更改其「活動」狀態。
* **[!UICONTROL 團隊運算元]**:此 [!UICONTROL 運算子] 角色可讓使用者查看執行資料，並變更藍本的「作用中」狀態。
* **[!UICONTROL 團隊受限成員]**:此角色的功能目前無法使用，並將於近期提供使用。 目前不建議將使用者指派給此角色。

### 團隊管理

* [建立團隊](#create-a-team)
* [設定團隊通知選項](#set-team-notification-options)

#### 建立團隊

組織擁有者和管理員可建立團隊。

要建立團隊，請執行以下操作：

1. 在左側導覽面板中，按一下 **[!UICONTROL 組織]**
1. 選取 **[!UICONTROL 團隊]** 標籤。
1. 按一下 **[!UICONTROL 新增團隊]** 在團隊清單下。
1. 輸入新團隊的名稱，然後按一下 **新增**.

#### 設定團隊通知選項

電子郵件通知選項是在團隊層級設定。

1. 在左側導覽面板中，按一下 **[!UICONTROL 團隊]**
1. 選取 **[!UICONTROL 通知選項]** 標籤。
1. 啟用您希望團隊接收的通知。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">「[!UICONTROL在方案運行中警告]」</td> 
      <td> <p>當情境執行中出現警告時，收到電子郵件</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL方案運行中的錯誤]</td> 
      <td>執行案例時發生錯誤時，會收到電子郵件。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL方案停用]</p> </td> 
      <td><p>當情境停用時，會收到電子郵件。</p><p><b>注意：</b> 只有當由於錯誤而自動停用藍本時，才會通知您停用藍本。 您不會收到手動停用案例的相關通知。</p><p>在某些情況下，藍本可能會由 [!DNL Workfront Fusion] 工程團隊，因為情況導致效能或其他問題。 在這些情況下，您不會收到 [!DNL Workfront Fusion]. </p></td>

</tr>
</tbody>
</table>

自動儲存通知選項的變更

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/organization-add-team-350x181.png" style="width: 350;height: 181;"> </p>
-->