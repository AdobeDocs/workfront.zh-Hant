---
product-area: documents;workfront-integrations
navigation-topic: workfront-for-experience-manager-enhanced-connector
title: 使用增強型聯結器傳送檔案
description: 您可以從Workfront傳送檔案至Experience Manager Assets。 從Workfront上傳並傳送至Experience Manager Assets的檔案仍會計入您的整體檔案儲存。 從Experience Manager Assets連結的Assets不計入整體儲存空間。
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: d687d2db-28e0-45e8-9d60-8419921f02e9
source-git-commit: 3f9a824780f2ded914d461a473aef3b6ecfa8701
workflow-type: tm+mt
source-wordcount: '409'
ht-degree: 1%

---

# 使用增強型聯結器傳送檔案

您可以從Workfront傳送檔案至Experience Manager Assets。 從Workfront上傳並傳送至Experience Manager Assets的檔案仍會計入您的整體檔案儲存。 從Experience Manager Assets連結的Assets不計入整體儲存空間。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront套件</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td> 
   <p>投稿人或以上</p>
   <p>要求或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">其他產品</td> 
   <td>Experience Manager Assets </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>編輯檔案的存取權</p> s="MCXref xref"&gt;建立或修改自訂存取層級</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>檢視檔案的存取許可權或以上許可權</p></td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。
+++

## 先決條件

開始之前，您必須

* 安裝適用於Experience Manager的Workfront增強型聯結器。

## 傳送檔案至Experience Manager Assets

當使用者將檔案從Workfront傳送到Experience Manager Assets時，對應的中繼資料會沿著檔案傳輸。 如果已設定，則每次進行變更時，中繼資料都會持續同步。

若要傳送檔案：

1. 前往Workfront中的&#x200B;**檔案**&#x200B;區域，並選取您要傳送的檔案。
1. 按一下「**傳送至**」，然後選擇您的管理員設定的Experience Manager Assets整合。

   >[!NOTE]
   >
   >您可以為此整合選擇任何名稱，因此可能沒有特別提及Experience Manager Assets。

   ![傳送至](assets/copy-of-send-to-in-toolbar-350x149.png)

1. 選擇要將資產移至何處，然後按一下&#x200B;**選取資料夾**。
1. 當您找到想要的目的地，請按一下[儲存]。**&#x200B;**

## 傳送新版本至Experience Manager Assets

您可以將新版本新增至先前已上傳至Workfront的檔案。 如需詳細資訊，請參閱[上傳檔案的新版本](../../../documents/managing-documents/upload-new-document-version.md)。 上傳最新版本後，您可以將其傳送至Experience Manager Assets。 如果Workfront中的對應欄位已變更，新版本會在傳送時更新Experience Manager Assets中的中繼資料。

若要傳送最新版本：

1. 前往Workfront中的&#x200B;**檔案**&#x200B;區域，然後找到檔案。
1. 按一下「**傳送至**」，然後選擇您的管理員設定的Experience Manager Assets整合。

   >[!NOTE]
   >
   >您可以為此整合選擇任何名稱，因此可能沒有特別提及Experience Manager Assets。

   ![傳送至](assets/copy-of-send-to-in-toolbar-350x149.png)

1. 按一下「**儲存**」。新版本會儲存在與舊版本相同的位置。
