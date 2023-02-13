---
product-area: documents;workfront-integrations
navigation-topic: workfront-for-experience-manager-enhanced-connector
title: 使用增強連接器傳送檔案
description: 您可以將檔案從Workfront傳送至Experience Manager Assets。 從Workfront上傳並傳送至Experience Manager Assets的檔案，仍會計入您整體的檔案儲存空間。 從Experience Manager Assets連結的資產不會計入整體儲存。
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: d687d2db-28e0-45e8-9d60-8419921f02e9
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '453'
ht-degree: 1%

---

# 使用增強連接器傳送檔案

您可以將檔案從Workfront傳送至Experience Manager Assets。 從Workfront上傳並傳送至Experience Manager Assets的檔案，仍會計入您整體的檔案儲存空間。 從Experience Manager Assets連結的資產不會計入整體儲存。

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>Pro或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>要求或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>Experience Manager Assets </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯對文檔的訪問</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>查看文檔上的訪問權限或更高版本</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 必要條件

開始之前，您必須

* 安裝Workfront for Experience Manager增強連接器。

## 傳送檔案至Experience Manager Assets

當使用者將檔案從Workfront傳送至Experience Manager Assets時，對應的中繼資料會隨檔案傳輸。 如果已設定，則每次進行變更時，中繼資料都會持續同步。

要發送文檔，請執行以下操作：

1. 前往 **檔案** 區域，然後選取要傳送的檔案。
1. 按一下 **傳送至**，然後選擇管理員設定的Experience Manager Assets整合。

   >[!NOTE]
   >
   >您可以為此整合選擇任何名稱，因此不得具體提及Experience Manager Assets。

   ![](assets/copy-of-send-to-in-toolbar-350x149.png)

1. 選取您要資產前往的位置，然後按一下 **選擇資料夾**.
1. 找到所需目的地後，按一下 **儲存**.

## 傳送新版本至Experience Manager Assets

您可以將新版本新增至先前已上傳至Workfront的檔案。 如需詳細資訊，請參閱 [上傳新版本的檔案](../../../documents/managing-documents/upload-new-document-version.md). 上傳最新版本後，您就可以將其傳送至Experience Manager Assets。 如果Workfront中的對應欄位已變更，新版本會在傳送時更新Experience Manager Assets中的中繼資料。

若要傳送最新版本：

1. 前往 **檔案** 區域，並找到檔案。
1. 按一下 **傳送至**，然後選擇管理員設定的Experience Manager Assets整合。

   >[!NOTE]
   >
   >您可以為此整合選擇任何名稱，因此不得具體提及Experience Manager Assets。

   ![](assets/copy-of-send-to-in-toolbar-350x149.png)

1. 按一下&#x200B;**儲存**。新版本會儲存在與舊版相同的位置。
