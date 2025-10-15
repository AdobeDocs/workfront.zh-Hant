---
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: best-practices-catalog
title: 設定對藍圖的存取權
description: 作為系統管理員，您可以透過設定請求佇列來儲存請求，從而為使用者啟用請求安裝藍圖的存取權。 在那裡，您只有一個位置可追蹤和更新請求。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: d85f363f-2ab4-45cb-b851-a7f33e1ca905
source-git-commit: 5fd855bec596926a4361fd07a1a763c7956e5e61
workflow-type: tm+mt
source-wordcount: '512'
ht-degree: 0%

---

# 設定對藍圖的存取權

所有[!DNL Adobe Workfront]使用者都可以瀏覽藍圖目錄。

作為系統管理員，您可以：

* 新增[!UICONTROL 藍圖]至版面配置範本中的主功能表，並將版面配置範本指派給使用者或群組。 如需詳細資訊，請參閱[使用配置範本自訂[!UICONTROL 主功能表]](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md)和[將使用者指派給配置範本](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md)。

  >[!NOTE]
  >
  >* 未指派版面配置範本的使用者將在[!UICONTROL 主功能表]中看到[!UICONTROL 藍圖]圖示。
  >* 當您建立新的版面配置範本時，[!UICONTROL 藍圖]圖示預設會包含在[!UICONTROL 主要功能表]的[!UICONTROL 作用中專案]清單中。


* 透過設定要求佇列以儲存要求，來啟用使用者要求安裝藍圖的存取權。 在那裡，您只有一個位置可追蹤和更新請求。 如需詳細資訊，請遵循下列程式。
* 安裝Blueprint。 如需詳細資訊，請參閱[安裝Blueprint](../../administration-and-setup/blueprints/blueprints-install.md)。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront套件</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td>
   <p>標準</p>
   <p>規劃</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td>Workfront管理員 </td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先決條件 {#prerequisites}

* 您必須使用現有請求佇列來儲存Blueprint請求。 專案必須儲存為請求佇列，而且必須處於[!UICONTROL 目前]狀態。
* 要求佇列必須為公用。 在請求佇列詳細資料中，&quot;[!UICONTROL 誰可以新增請求至此佇列？「]」必須設定為&#x200B;**[!UICONTROL 任何人]**。

>[!TIP]
>
>如果您想要為Blueprint請求建立新的請求佇列，應該在設定Blueprint存取權之前先建置它。 如需建立要求佇列的詳細資訊，請參閱[建立要求佇列](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)。

## 選取要儲存Blueprint請求的請求佇列

您必須先為這些請求選取請求佇列，使用者才能要求您為其安裝Blueprint。 在定義請求佇列之前，使用者只能瀏覽Blueprint目錄。

{{step1-to-blueprints}}

1. 按一下目錄畫面右上角的&#x200B;**[!UICONTROL 設定Blueprint要求]**。

   <!--
   <li value="3" data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>In the <strong>Configure blueprints</strong> dialog, ensure that the <strong>Configure request queues</strong> tab is selected.</p> </li>
   -->

1. 在&#x200B;**[!UICONTROL 設定Blueprint]**&#x200B;對話方塊上，開始輸入使用中要求佇列的名稱，並在其出現在搜尋結果中時選取它。

   >[!IMPORTANT]
   >
   >此清單中只會顯示公開請求佇列。 若要將您的要求佇列公開，請參閱上面的[必要條件](#prerequisites)一節。

   已設定請求佇列偏好設定，使用者現在可以請求藍圖安裝。

   ![設定要求佇列](assets/Blueprints_access_setup_request_queue.png)

1. （選擇性）若要變更實際要求佇列，請按一下&#x200B;**[!UICONTROL 編輯此要求佇列]**。

   請求佇列專案會在新的瀏覽器標籤中開啟，您可以視需要更新。

1. （選擇性）如果請求佇列包含主題群組或佇列主題，您可以從清單中選取它們。
1. 若要返回Blueprint目錄，請按一下&#x200B;**[!UICONTROL 關閉]**。

>[!NOTE]
>
>當您安裝請求的Blueprint時，您應該將請求佇列中的問題狀態變更為&#x200B;**[!UICONTROL 已關閉]**&#x200B;或&#x200B;**[!UICONTROL 已解決]**，以便通知請求者。 如需有關安裝Blueprint的資訊，請參閱[安裝Blueprint](../../administration-and-setup/blueprints/blueprints-install.md)。
