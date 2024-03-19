---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: 刪除自訂表單上的物件型別
description: 您可以在現有的自訂表單上刪除與表單相關聯的物件型別。 完成此操作後，使用者無法再將表單附加到該型別的物件。
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: ca6565c4-3d9e-4a11-a7b6-fce701923bf2
source-git-commit: ccb2b6bb9fa63d29523ff396490f9580ad130bdd
workflow-type: tm+mt
source-wordcount: '367'
ht-degree: 0%

---

# 刪除自訂表單上的物件型別

<span class="preview">本頁醒目提示的資訊指出尚未普遍可用的功能。 它僅適用於所有客戶的預覽環境，或適用於啟用快速發行的客戶的生產環境。</span>

<span class="preview">如需快速發行版本的相關資訊，請參閱 [啟用或停用組織的快速發行](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">如需目前版本的相關資訊，請參閱 [2024年第二季版本總覽](/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-release-overview.md).</span>

您可以在現有的自訂表單上刪除與表單相關聯的物件型別。 完成此操作後，使用者無法再將表單附加到該型別的物件。

## 存取需求

您必須具備下列專案才能執行本文所述的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront計畫</p> </td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td>
   <p>新增：標準</p>
   <p>或</p>
   <p>目前：計畫</p></td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>管理自訂表單的存取權</p> </td> 
  </tr>  
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱 [Workfront檔案中的存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## 刪除自訂表單上的物件型別

您可以從現有的自訂表單中刪除物件型別。

自訂表單必須至少有一個物件型別。

>[!CAUTION]
>
>如果人員已將自訂表單附加到您要刪除的物件型別並新增資料，當您刪除表單上的該物件型別時，該資料將會永久刪除。 其中可能包含使用者稍後所需的歷史資訊。
>
>一般而言，建議您儘可能減少編輯已使用中的自訂表單的次數。 沒有通知系統可提醒使用自訂表單的人員您的變更。

{{step-1-to-setup}}

1. 按一下 **自訂Forms** 在左側面板中。
1. 選取您要編輯的自訂表單，然後按一下 **編輯** <span class="preview">或 ![編輯圖示](assets/edit-icon.png).</span>
1. 按一下任何頁面上的X **物件型別** ，然後按一下「 」 **刪除** 在顯示的警告訊息上。

   ![](assets/click-x-object-types.jpg)

1. （可選）針對您要從表單中移除的任何其他物件型別，重複上一步驟。
1. 按一下 **完成**，然後按一下 **儲存並關閉**.
