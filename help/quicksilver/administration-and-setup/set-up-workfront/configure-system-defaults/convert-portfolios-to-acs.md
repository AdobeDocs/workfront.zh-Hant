---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: 將舊版產品組合轉換為Adobe雲端儲存空間
description: 從「系統偏好設定」的「儲存偏好設定」區域，將現有的舊版Workfront儲存產品組合轉換為Adobe雲端儲存空間。
author: Courtney
feature: System Setup and Administration
role: Admin
source-git-commit: 9d28f52ace4d443bdffc475baf79d482152d4157
workflow-type: tm+mt
source-wordcount: '358'
ht-degree: 5%

---

# 將舊版產品組合轉換為Adobe雲端儲存空間

身為Workfront管理員，您可以從系統偏好設定中的儲存偏好設定區域，將現有的舊版Workfront儲存產品組合轉換為Adobe雲端儲存空間。 產品組合轉換後，其行為會與任何其他Adobe雲端儲存產品組合相似。

如需轉換後產品組合的行為方式及其子物件受到影響的詳細資訊，請參閱[在Adobe雲端儲存空間](/help/quicksilver/review-and-approve-work/workfront-storage.md)上移至Workfront中的[物件可攜性](/help/quicksilver/review-and-approve-work/workfront-storage.md#object-portability)。

## 存取權要求

+++ 展開以檢視這篇文章中所述功能的存取權要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 封裝</td> 
   <td><p>任何Workflow封裝</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td><p>標準</p> <p>規劃</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td>您必須是Workfront管理員。 </td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 轉換投資組合之前

在轉換舊版Workfront儲存產品組合之前，請考量下列事項：

* 轉換只會影響投資組合本身。 使用舊版Workfront儲存空間的子專案和計畫會保留在舊版儲存空間。
  >[!NOTE]
  >
  >只有有人手動將Adobe雲端儲存空間專案新增至子舊版計畫時，才會自動轉換成Adobe雲端儲存空間。
* 產品組合上的檔案和檔案資料夾在轉換後會保留在舊版Workfront儲存空間中。
* 轉換後，您無法將舊版Workfront儲存專案新增到產品組合中。

## 將舊版產品組合轉換為Adobe雲端儲存空間

若要將一個或多個舊版Workfront儲存產品組合轉換為Adobe雲端儲存空間：

{{step-1-to-setup}}

1. 在左側導覽中選取&#x200B;**系統**，然後選取&#x200B;**偏好設定**。

1. 向下捲動至&#x200B;**儲存偏好設定**&#x200B;區段。

1. 在&#x200B;**選取要轉換成Adobe雲端儲存空間的產品組合**&#x200B;欄位中，選取一或多個舊版Workfront儲存產品組合。

1. 按一下「**儲存**」。

   系統會顯示確認訊息，說明轉換投資組合時所發生的情況：

   * 您無法再將舊版Workfront儲存專案移至產品組合。
   * 產品組合中建立的所有新專案都會使用Adobe雲端儲存空間。
   * Frame.io是產品組合Adobe雲端儲存空間專案中檔案的檢視器。
   * 使用舊版Workfront儲存空間的子專案會保留在舊版儲存空間。
   * 子程式會保留在舊版儲存空間。

1. 按一下&#x200B;**轉換**&#x200B;以確認。

   所選的產品組合會轉換為Adobe雲端儲存空間。
