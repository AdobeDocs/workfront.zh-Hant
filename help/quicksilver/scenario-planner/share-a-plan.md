---
product-area: enterprise-scenario-planner-product-area
keywords: 計畫，權限，共用，方案，方案，方案
navigation-topic: enterprise-scenario-planner-navigation-topic
title: 在方案計畫器中共用計畫
description: 您可以與其他用戶共用在Adobe Workfront方案規劃器中建立的計畫。
author: Alina
feature: Workfront Scenario Planner
exl-id: b8bbb533-4384-414c-8574-4e137962b8ca
source-git-commit: 82a5102d28700368a094502dcd6026462c149eb1
workflow-type: tm+mt
source-wordcount: '916'
ht-degree: 0%

---

# 在 [!DNL Scenario Planner]

您可以在 [!DNL Adobe Workfront Scenario Planner] 與其他使用者共同作業，讓他們能夠與您共同作業。

>[!TIP]
>
>如果您將計畫連結傳送給其他人，您也必須與他們共用計畫，方便他們檢視。

## 存取需求

您必須具備下列條件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b> 計劃*</b> </p> </td> 
   <td>[!UICONTROL Business]或更高版本</td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b> 授權*</b> </p> </td> 
   <td> <p>[!UICONTROL Review]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td><b>產品</b> </td> 
   <td> <p>您必須為 [!DNL Adobe Workfront Scenario Planner] 存取本文所述功能。</p> <p>如需有關取得 [!DNL Workfront Scenario Planner]，請參閱 <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">使用 [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>訪問級別配置*</strong> </td> 
   <td> <p>[!UICONTROL編輯]對 [!DNL Scenario Planner]</p> <p>如果您仍無法存取，請詢問您的 [!DNL Workfront] 管理員。 若要了解 [!DNL Workfront] 管理員可以更改您的訪問級別，請參閱 <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>物件權限</strong> </p> </td> 
   <td> <p> 計畫的[!UICONTROL管理]權限
     <p>有關請求對計畫進行額外訪問的資訊，請參閱 <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">[!UICONTROL要求]存取 [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 必要條件

* 授予計畫權限的使用者必須具有 [!DNL Scenario Planner] 區域，如 [!DNL Workfront] 管理員，以便接收計畫的權限。

   例如， [!UICONTROL 請求者] 無法查看、建立或編輯計畫。 與擁有申請者授權的使用者共用計畫時，請謹記這一點。

<!--
  NOTE: ensure this stays this way and they don't restrict Workers from SP as well?? OR ensure you can even SEE Requestors as an option or they are not grayed out??)
  -->

如需存取 [!DNL Scenario Planner] 有關各種許可證類型，請參見 [授予的存取權 [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md).

## 計畫共用的考量事項

* 您可以共用單一計畫，也可以大量共用多個計畫。
* 您無法查看未建立或未與您共用的計畫。
* 您只能與其他使用者共用計畫。 您無法與群組、團隊或公司共用計畫。
* 您必須先儲存計畫，才能共用它。
* 您可以與其他使用者共用計畫的URL。 如果使用者沒有至少可檢視計畫的權限，則在收到URL時，他們可向其他使用者要求存取計畫。 有關請求訪問計畫的資訊，請參閱 [在 [!DNL Scenario Planner]](../scenario-planner/request-access-to-plan.md).
* 共用已與他人共用的多個計畫時，您共用的使用者不會取代，而是會新增至您所選每個計畫的現有使用者。

## 共用計畫

1. 按一下 **[!UICONTROL 主菜單]** 圖示 ![](assets/main-menu-icon.png) 在Workfront的右上角，然後按一下 **[!UICONTROL 藍本]**.
1. 按一下計畫的名稱以開啟它

   或

   選取數個要大量共用的計畫。

   >[!TIP]
   >
   >您可以按一下與其共用計畫的用戶的變數，在計畫題頭的右上角共用計畫。

1. （條件性）如果您開啟計畫，請按一下 **[!UICONTROL 更多]** 圖示 ![](assets/more-icon.png) 至 [!UICONTROL 計畫] 名稱，然後按一下 **[!UICONTROL 共用]**

   或

   如果您選取了數個要大量共用的計畫，請按一下 **[!UICONTROL 共用]** 圖示 ![](assets/share-icon-26x26.png) 開啟 [!UICONTROL 計畫] 存取方塊。

   >[!TIP]
   >
   >* 對您選取的所有計畫擁有權限的使用者會顯示在 [!UICONTROL 計畫] 存取方塊。
   >* 任何其他用戶都將添加到，並且不會替換所有選定計畫上的現有用戶。


1. 在 **[!UICONTROL 授予計畫存取權]** 欄位中，開始鍵入要與共用計畫的用戶的名稱，然後在清單中顯示時選擇這些用戶。
1. 從用戶名右側的權限下拉菜單中，選擇要授予計畫的權限級別。
1. 從以下項目中選取：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL視圖]</td> 
      <td>您與共用計畫的使用者將擁有檢視計畫的權限。 他們無法編輯計畫、添加方案、方案或發佈方案的資訊。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL管理]</td> 
      <td> <p>您共用計畫的用戶具有管理計畫的權限，包括編輯資訊、添加方案、方案和發佈計畫。 </p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >只有在建立計畫時，才可以刪除計畫。 您無法刪除與您共用的計畫。

1. 按一下&#x200B;**[!UICONTROL 儲存]**。

   此計畫現在已與您指定的用戶共用。

   您可以在計劃清單或計畫標題右上角的「與我共用」列中查看具有計畫權限的用戶。

   >[!TIP]
   >
   >您可以透過套用 [!UICONTROL 與我共用] 篩選計劃清單。

## 計畫權限選項

下表列出了共用計畫時可授予的權限。 如需使用者根據其授權所取得存取權限的詳細資訊，請參閱 [授予的存取權 [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md).

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>動作</strong> </p> </th> 
   <th> <p><strong>[!UICONTROL管理]</strong> </p> </th> 
   <th> <p><strong>[!UICONTROL視圖]</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>查看計畫 </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>查看方案 </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td>查看方案</td> 
   <td>✓</td> 
   <td><span style="font-weight: normal;">✓</span> </td> 
  </tr> 
  <tr> 
   <td>查看作業角色</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>查看成本和預算資訊*</td> 
   <td>✓</td> 
   <td>✓ </td> 
  </tr> 
  <tr> 
   <td>管理成本和預算資訊*</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>建立方案</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>建立藍本</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>刪除方案或方案</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td>複製方案</td> 
   <td>✓ </td> 
   <td> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>發佈案例**</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

*您必須擁有財務資料的訪問權限，才能查看或管理計畫的財務資訊，即使您擁有計畫的管理權限。 如需存取金融資料的相關資訊，請參閱 [授予金融資料的存取權](../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

**您必須有建立的存取權和管理專案的權限，才能發佈案例。

如需專案存取層級的相關資訊，請參閱 [授予專案的存取權](../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md).

如需專案權限的相關資訊，請參閱 [在中共用專案 [!DNL Adobe Workfront]](../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).
