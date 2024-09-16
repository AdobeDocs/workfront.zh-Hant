---
product-area: enterprise-scenario-planner-product-area
keywords: 計畫、許可權、共用、方案、案例、案例
navigation-topic: enterprise-scenario-planner-navigation-topic
title: 在「情境規劃工具」中請求計畫的存取權
description: 當計畫的連結與您共用時，您可以在「Adobe Workfront情境規劃工具」中請求計畫的存取權。
author: Alina
feature: Workfront Scenario Planner
exl-id: fa47cb8c-a3ca-4748-b67d-2d8ed34b9b4a
source-git-commit: bbc3ac852dae3d9a503b4585dfc229d43c9aed28
workflow-type: tm+mt
source-wordcount: '500'
ht-degree: 1%

---

# 要求[!DNL Scenario Planner]中計畫的存取權

當計畫的連結共用給您時，您可以在[!DNL Adobe Workfront Scenario Planner]中要求計畫的存取權。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] 計畫*</p> </td> 
   <td> <ul></li>
   <li><p>新增：Ultimate </p></li>
   <p>新的Workfront Select或Workfront Prime計畫無法使用「情境規劃工具」。 </p>
   <li><p>目前： [！UICONTROL Business]或更高版本</p></ul>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] 授權*</p> </td> 
   <td> <p>新增：淺色或更高</p> 
   <p>目前： [！UICONTROL Review]或以上</p> </td> 
  </tr> 
  <tr> 
   <td>產品* </td> 
   <td> <ul><li><p>針對新的Workfront計畫：</p><p> Adobe Workfront</li></p>
   <li><p>針對目前的Workfront計畫： </p>
   <p>Adobe Workfront</p> <p>Adobe Workfront情境規劃工具</p></li></ul>

<p>如需詳細資訊，請參閱<a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">使用[!DNL Scenario Planner]</a>所需的存取權。 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>存取層級 </td> 
   <td>  <p>[！UICONTROL檢視]或更高存取權以存取 [!DNL Scenario Planner]</p>  </td> 
  </tr>
 </tbody> 
</table>

*如需詳細資訊，請參閱[Workfront檔案的存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先決條件

您必須具備下列專案，才能在[!DNL Scenario Planner]中要求計畫的存取權：

* 計畫的連結。

>[!NOTE]
>
>如果您沒有[!DNL Scenario Planner]的存取層級許可權，而您嘗試從連結存取計畫，則無法要求此計畫的存取權。 相反地，畫面會顯示通知您聯絡[!DNL Workfront]管理員。

## 要求[!DNL Workfront Scenario Planner]中計畫的存取權

如果您尚沒有計畫的許可權，而您從與您共用的連結瀏覽至該計畫，畫面會顯示並通知您沒有許可權檢視計畫。 系統會提示您向計畫建立者請求許可權。

>[!TIP]
>
>您只能向計畫的擁有者或建立者要求許可權。 您無法向也有權存取計畫的其他使用者要求許可權。

若要要求許可權：

1. 按一下計畫的連結。

   ![](assets/request-access-to-plan-350x277.png)

1. 在「**[!UICONTROL 要求存取]**」下拉式功能表中，指出您要授與的許可權等級。 從下列選項中選取：

   * [!UICONTROL 檢視]
   * [!UICONTROL 管理]

   您無法要求高於您[!DNL Scenario Planner]存取層級的許可權。 例如，如果您有[!DNL Scenario Planner]的檢視存取權，則無法要求[!UICONTROL 管理]許可權。

   如需不同許可權層級的詳細資訊，請參閱[在 [!DNL Scenario Planner]](../scenario-planner/share-a-plan.md)中共用計畫。

   如需Workfront管理員可以管理[!DNL Scenario Planner]存取權的相關資訊，請參閱[授與 [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md)存取權。

1. （選擇性）在&#x200B;**[!UICONTROL 留下註解方塊]**&#x200B;中輸入註解或要求，然後按一下&#x200B;**[!UICONTROL 要求存取]**。

   會發生下列情況：

   * [!DNL Workfront]傳送電子郵件通知給計畫擁有者，讓他們授予要求的許可權。\
     ![](assets/request-access-to-plan-email-350x156.png)

   * 在計畫擁有者授予要求的許可權後，如果您的[!DNL Workfront]管理員在您的系統中啟用了使用者通知的物件共用，並且您在您的設定檔中啟用了[!UICONTROL 某人與我共用物件]電子郵件通知，您會收到一封電子郵件，告知您已授予許可權。

     ![](assets/access-granted-to-plan-email-350x172.png)

   * 您也可以從[!UICONTROL 首頁]區域和[!DNL Workfront]行動應用程式將許可權授與計畫。

   如需有關啟用系統通知的資訊，請參閱[為系統中的每個人設定事件通知](../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md)。

   如需有關在您的設定檔中啟用通知的資訊，請參閱[通知：其他資訊](../workfront-basics/using-notifications/notifications-misc-information.md)。
