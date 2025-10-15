---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
title: 對應使用者屬性
description: 使用單一登入(SSO)，您可以將身分提供者的Active Directory中的屬性傳遞給Adobe Workfront使用者。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 3d523584-dcb8-4aa6-8217-611f22dc1450
source-git-commit: 9e7d20fe165e08997c14e207406fb8bed7597a56
workflow-type: tm+mt
source-wordcount: '956'
ht-degree: 1%

---

# 對應使用者屬性

<!--Audited 2/2024-->

使用單一登入(SSO)，您可以將身分提供者的Active Directory中的屬性傳遞給Adobe Workfront使用者。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront套件</td> 
   <td><p>任何</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td><p>標準</p><p>規劃</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td><p>您必須是Workfront管理員</p></td>
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案[中的](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)存取需求。

+++

## 對應屬性的提示

對應屬性時，請牢記下列事項：

* 一律在預覽沙箱或客戶重新整理(CR)沙箱中測試。
* 使用管理員與非管理員帳戶進行測試，以確認您正確對應屬性。
* 每次使用者透過單一登入登入時，都會套用對應的屬性。

  範例：如果您在Workfront中對映「姓氏」並更新其名稱，而未更新其身分提供者中的值，則會在使用者下次登入時，覆寫姓氏以符合身分提供者中任何專案的值。

## 對應組織的使用者屬性

根據您的組織是否使用Adobe統一體驗，對應屬性的程式會有所不同。

若要判斷您的組織是否位在Adobe統一體驗上，請檢查您用來存取Workfront的URL。

| URL | Adobe體驗 |
|---|---|
| （公司名稱）.my.workfront.com | 傳統體驗 |
| experience.adobe.com | Adobe統一體驗 |

* [在傳統體驗中對應使用者屬性](#map-user-attributes-in-the-classic-experience)
* [在Adobe統一體驗中對應使用者屬性](#map-user-attributes-in-the-adobe-unified-experience)

### 在傳統體驗中對應使用者屬性

1. 按一下Adobe Workfront右上角的&#x200B;**主功能表**&#x200B;圖示![主功能表圖示](assets/main-menu-icon.png)，然後按一下&#x200B;**設定** ![齒輪設定圖示](assets/gear-icon-settings.png)。

1. 按一下&#x200B;**系統** > **單一登入(SSO)**。

1. 在&#x200B;**Type**&#x200B;下拉式清單中，按一下&#x200B;**SAML 2.0**。

1. 按一下&#x200B;**對應使用者屬性**。

   ![對應使用者屬性](assets/map-user-attributes.png)

1. 在出現的選項列中，對應您Workfront使用者所需的屬性。

   您可以對應如地址、經理、工作角色、主群組等屬性。

   屬性對應在1:1比例上運作。 例如，您不能設定使用者屬於的每個群組；您只能為每個使用者設定一個。

   >[!IMPORTANT]
   >
   >我們不建議在屬性對應中對應存取層級。 如果這樣做，設定預設值時請務必小心，以免不慎移除管理員存取權。

   下表說明可用來對應屬性的欄位：

   <table style="table-layout:auto"> 
    <col data-mc-conditions=""> 
    <col data-mc-conditions=""> 
    <tbody> 
     <tr> 
      <td role="rowheader">Workfront 使用者屬性</td> 
      <td>選擇您要對應的屬性名稱</td> 
     </tr> 
     <tr> 
      <td role="rowheader">目錄屬性</td> 
      <td>輸入您要使用的SSO屬性標籤。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">預設值</td> 
      <td> <p>選擇Workfront使用者屬性後，如果連線期間的值為NULL，則此欄位會填入系統中對應的預設值。 只有在您打算套用屬性對應規則時（請參閱步驟7），才能在此處輸入值。 預設值會作為這些規則的例外。</td> 
     </tr> 
    </tbody> 
   </table>

1. （選擇性）按一下&#x200B;**規則**&#x200B;將規則新增至屬性。

   1. 在下拉式清單中，選取您要使用的屬性修飾元。
   1. 在右側的2個欄位中，輸入目錄屬性值以及要取代它的值。

      ![規則欄位](assets/rule-fields.png)

   您可以按一下&#x200B;**新增規則**&#x200B;來新增更多規則至屬性。

1. （選擇性）若要對應更多使用者屬性，請按一下[新增對應] **並重複步驟6-7。**
1. 按一下「**儲存**」。

### 在Adobe統一體驗中對應使用者屬性

1. 按一下Adobe Workfront左上角的&#x200B;**主功能表**&#x200B;圖示![主功能表圖示](assets/main-menu-left.png)，然後按一下&#x200B;**設定** ![齒輪設定圖示](assets/gear-icon-settings.png)。

1. 按一下&#x200B;**系統** > **單一登入(SSO)**。

1. 選取&#x200B;**Adobe**&#x200B;索引標籤。

1. （選擇性和條件性）如果您的組織在傳統體驗中設定了屬性對應，而您想要將該屬性對應複製到Adobe統一體驗，請按一下&#x200B;**移轉對應**。 然後，您可以捨棄、刪除或編輯這些對應。

   >[!NOTE]
   >
   >建議您第一次在Adobe統一體驗中設定對應時移轉對應。 稍後再移轉這些檔案並沒有壞處，但不需要多次移轉。

1. 若要建立新的屬性對應，請按一下[新增對應]。****

1. 按一下Workfront欄位名稱旁的箭頭，然後選取您要對應到的[!DNL Workfront]欄位。

1. （選擇性）如果要為指定欄位建立多個規則，請按一下&#x200B;**一律**&#x200B;旁的箭頭，並選取要規則使用的運運算元。

1. （視條件而定）如果您在「一律」之外選取運運算元，請選取運運算元套用的Workfront欄位和值。

   >[!NOTE]
   >
   >運運算元`Is Truthy`和`Is Falsy`不需要值。

1. 選取您要將Identity Manager中的屬性值套用至Workfront欄位，或是要套用特定的常數值。

1. 輸入要套用的Identity Manager欄位名稱，或輸入要套用的常數值文字。

1. （選擇性）若要為相同的Workfront欄位新增更多規則，請按一下[新增規則] ****，然後依照步驟4-9執行。

   >[!IMPORTANT]
   >
   > * 一律規則下的任何規則都會被忽略。 如果您有「一律」規則，則必須將其移至規則清單底部。 您可以按一下規則右側的三個點功能表，將規則上移或下移，以移動清單中的規則。
   > * 若要在清單中間建立規則，請按一下要位於新規則上方或下方的規則旁邊的三個點功能表，然後選取「**新增規則上方」**&#x200B;或「**新增規則下方」**。

1. 若要刪除規則，請按一下要刪除的規則旁邊的三個點功能表，然後選取&#x200B;**刪除**。
1. 若要刪除對應，請按一下對應卡片上的&#x200B;**刪除**&#x200B;圖示。

1. 若要儲存，請捲動至頁面頂端，然後按一下[儲存]。****


