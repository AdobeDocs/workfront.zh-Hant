---
product-area: enterprise-scenario-planner-product-area
keywords: 計畫、許可權、共用、方案、案例、案例
navigation-topic: enterprise-scenario-planner-navigation-topic
title: 在「情境規劃工具」中共用計畫
description: 您可以將您在Adobe Workfront情境規劃工具中建立的計畫與其他使用者共用。
author: Alina
feature: Workfront Scenario Planner
exl-id: b8bbb533-4384-414c-8574-4e137962b8ca
source-git-commit: aa2e9a012a60ab10e2d027dedae520b5e06686c7
workflow-type: tm+mt
source-wordcount: '880'
ht-degree: 0%

---

# 在[!DNL Scenario Planner]中共用計畫

<!--Audited: 07/2024-->

您可以與其他使用者共用[!DNL Adobe Workfront Scenario Planner]中的計畫，讓他們可以在您執行的工作上共同作業。

>[!TIP]
>
>如果您將計畫的連結傳送給其他人，您也必須與他們共用計畫，他們才能檢視它。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] 封裝</p> </td> 
   <td> 
   <p>Workfront Ultimate</p>
<p><b>附註</b></p>
<p>如果您有不同的Workfront套件，請洽詢您的Workfront代表。</p>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] 授權</p> </td> 
   <td> <p>[！UICONTROL Light]或更高</p> 
   <p>[！UICONTROL Review]或更高版本</p> </td> 
  </tr> 
    <tr> 
   <td>存取層級設定</td> 
   <td> <p>[！UICONTROL Edit]對的存取權 [!DNL Scenario Planner]</p> </td> 
  </tr> 
  <tr> 
   <td> <p>物件許可權 </p> </td> 
   <td> <p>[！UICONTROL Manage]計畫的許可權</p> </td> 
  </tr> 
 </tbody> 
</table>

如需有關存取Scenario Planner的詳細資訊，請參閱[使用 [!DNL Scenario Planner]](../scenario-planner/access-needed-to-use-sp.md)所需的存取。

如需Workfront存取需求的相關資訊，請參閱[Workfront檔案的存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

<!--Old:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] plan*</p> </td> 
   <td> <ul></li>
   <li><p>New: Ultimate </p></li>
   <p>The Scenario Planner is not available for the new Workfront Select or Workfront Prime plans. </p>
   <li><p>Current: [!UICONTROL Business] or higher</p></ul>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] license*</p> </td> 
   <td> <p>New: Light or higher</p> 
   <p>Current: [!UICONTROL Review] or higher</p> </td> 
  </tr> 
  <tr> 
   <td>Product* </td> 
   <td> <ul><li><p>For the new Workfront plans:</p><p> Adobe Workfront</li></p>
   <li><p>For the current Workfront plans: </p>
   <p>Adobe Workfront</p> <p>Adobe Workfront Scenario Planner</p></li></ul>
   
   <p>For more information, see <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Access needed to use the [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Access level </td> 
   <td> <p>[!UICONTROL Edit] access to the [!DNL Scenario Planner]</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Object permissions </p> </td> 
   <td> <p>[!UICONTROL Manage] permissions to a plan</p> <p>For information on requesting additional access to a plan, see <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Request access to a plan in the [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## 先決條件

* 授予計畫許可權的使用者必須擁有存取層級（由您的[!DNL Scenario Planner]管理員授予）中[!DNL Workfront]區域的存取權，才能獲得計畫的許可權。

  例如，[!UICONTROL 要求者]無法檢視、建立或編輯計畫。 您與擁有請求者授權的使用者共用計畫時，請記住這一點。

<!--
  NOTE: ensure this stays this way and they don't restrict Workers from SP as well?? OR ensure you can even SEE Requestors as an option or they are not grayed out??)
  -->

如需有關各種授權型別對[!DNL Scenario Planner]的存取權的詳細資訊，請參閱[授與 [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md)的存取權。

## 關於計畫共用的考量事項

* 所有使用者（包括系統管理員）都只能存取他們建立的計畫。
* 您可以大量共用單一計畫或共用多個計畫。
* 您無法檢視未建立或未與您共用的計畫。
* 您只能與其他使用者共用計畫。 您無法與群組、團隊或公司共用計畫。
* 您必須先儲存計畫，然後才能進行共用。
* 您可以與其他使用者共用計畫的URL。 如果使用者沒有許可權至少檢視計畫，當他們收到URL時，可以向另一個使用者請求計畫的存取權。 如需有關請求計畫存取權的資訊，請參閱[在 [!DNL Scenario Planner]](../scenario-planner/request-access-to-plan.md)中請求計畫存取權。
* 共用已與其他人共用的多個計畫時，您共用的使用者不會取代，但會新增至您選取之每個計畫的現有使用者。

## 計畫許可權選項

下表列出您在共用計畫時可授與的許可權。 如需使用者根據其授權所取得存取權的詳細資訊，請參閱[授與 [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md)的存取權。

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>動作</strong> </p> </th> 
   <th> <p><strong>[！UICONTROL管理]</strong> </p> </th> 
   <th> <p><strong>[！UICONTROL檢視]</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>檢視計畫 </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>檢視方案 </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td>檢視案例</td> 
   <td>✓</td> 
   <td><span style="font-weight: normal;">✓</span> </td> 
  </tr> 
  <tr> 
   <td>檢視職位角色</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>檢視成本和預算資訊*</td> 
   <td>✓</td> 
   <td>✓ </td> 
  </tr> 
  <tr> 
   <td>管理成本與預算資訊*</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>建立方案</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>建立案例</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>刪除行動方案或情境</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td>複製案例</td> 
   <td>✓ </td> 
   <td> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>發佈情境**</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

*您必須擁有財務資料的存取權，才能檢視或管理計畫的財務資訊，即使您擁有計畫的管理許可權。 如需有關存取財務資料的資訊，請參閱[授予財務資料的存取權](../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)。

**您必須擁有建立和管理專案的許可權，才能發佈情境。

如需有關專案存取層級的資訊，請參閱[授與專案的存取權](../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md)。

如需有關專案許可權的資訊，請參閱[在 [!DNL Adobe Workfront]](../workfront-basics/grant-and-request-access-to-objects/share-a-project.md)中共用專案。

## 共用計畫

{{step1-to-scenario-planner}}

1. 按一下計畫名稱以開啟

   或

   選取數個計畫以大量共用它們。

   >[!TIP]
   >
   >您可以按一下計畫標題右上角與計畫共用的使用者頭像，以共用計畫。

1. （視條件而定）如果您開啟計畫，請按一下&#x200B;**[!UICONTROL 計畫]**&#x200B;名稱右側的![更多](assets/more-icon.png)圖示[!UICONTROL 更多圖示]，然後按一下&#x200B;**[!UICONTROL 共用]**

   或

   如果您選取多個計畫來大量共用它們，請按一下計劃清單頂端的&#x200B;**[!UICONTROL 共用]**&#x200B;圖示![](assets/share-icon-26x26.png)以開啟[!UICONTROL 計畫]存取方塊。

   >[!TIP]
   >
   >* 擁有您選取之所有計畫許可權的使用者會顯示在[!UICONTROL 計畫]存取方塊中。
   >* 任何其他使用者都會新增至，不會取代所有所選計畫上的現有使用者。

1. 在&#x200B;**[!UICONTROL 將計畫存取權授予]**&#x200B;欄位中，開始輸入您要共用計畫的使用者名稱，然後在他們出現在清單中時選取他們。
1. 從使用者名稱右側的許可權下拉式功能表中，選取您要授予計畫計畫的許可權層級。
1. 從下列選項中選取：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[！UICONTROL檢視]</td> 
      <td>您共用計畫的使用者將擁有檢視計畫的許可權。 他們無法編輯計畫、新增方案、案例或發佈案例的相關資訊。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL管理]</td> 
      <td> <p>您共用計畫的使用者具有管理計畫的許可權，包括編輯資訊、新增方案、情境和發佈計畫。 </p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >您只能在建立計畫時刪除計畫。 您無法刪除與您共用的計畫。

1. 按一下「**[!UICONTROL 儲存]**」。

   計畫現在會與您指定的使用者共用。

   您可以在計劃清單的「與我共用」欄中或計畫標題右上角，檢視擁有計畫許可權的使用者。

   >[!TIP]
   >
   >您可以在計劃清單中套用[!UICONTROL 與我共用]篩選器，以檢視與您共用的計畫。


