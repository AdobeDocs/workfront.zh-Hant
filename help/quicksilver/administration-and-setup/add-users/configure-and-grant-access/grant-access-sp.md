---
title: 授予方案計畫員的訪問權限
description: 作為Adobe Workfront管理員，您可以使用訪問級別來定義用戶對方案規劃器的訪問。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 4343f0ff-2f78-4556-801f-db9d94f80c95
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '688'
ht-degree: 0%

---

# 授予方案計畫員的訪問權限

作為Adobe Workfront管理員，您可以使用存取層級來定義使用者對方案規劃程式的存取，如 [存取層級概觀](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

除了訪問方案規劃器之外，具有非系統管理員訪問級別的用戶還必須具有財務資料的訪問權限，以便查看計畫中包含的任何財務資訊，如預算、成本和職務職責費率。 如需詳細資訊，請參閱 [授予金融資料的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

## 存取需求

您必須具備下列條件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront計畫*</p> </td> 
   <td>業務或更高版本</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>查看或更高版本。 如需詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref" data-mc-variable-override="">Adobe Workfront授權概觀</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td> <p>您必須為Adobe Workfront方案規劃器購買額外的許可證，才能訪問本文所述的功能。</p> <p>有關獲取Workfront方案計畫程式的資訊，請參閱 <a href="../../../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref" data-mc-variable-override="">使用方案計畫員所需的訪問權限</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級*</td> 
   <td> <p>查看方案計畫員的訪問權限或更高</p> <p><b>注意</b>:如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何變更您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>物件權限</p> </td> 
   <td> <p>查看計畫的權限或更高</p> <p>有關請求對計畫進行額外訪問的資訊，請參閱 <a href="../../../scenario-planner/request-access-to-plan.md" class="MCXref xref" data-mc-variable-override="">請求方案計畫員中計畫的訪問權</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 使用自定義訪問級別配置對方案規劃器的用戶訪問

1. 開始建立或編輯存取層級，如 [建立或修改自訂存取層級](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. 按一下右側的選項 **方案計畫員** 用於此訪問級別。

   >[!NOTE]
   >
   >請求或外部許可證類型不允許查看或編輯方案計畫員的訪問權限。

1. （可選）要配置您正在處理的訪問級別中其他對象和區域的訪問設定，請繼續以下文章之一列出： [設定Adobe Workfront的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md)，例如 [授予任務的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) 和 [授予金融資料的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. 完成後，按一下 **儲存**.

## 按許可證類型訪問方案計畫器

有關每個訪問級別中的用戶可以使用方案計畫器執行的操作的資訊，請參閱本節 [方案計畫員區域](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#scenario) 在文章中 [每種物件類型皆可使用的功能](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## 方案計畫員按訪問級別設定訪問

以下資訊可幫助您了解如何使用訪問級別設定來控制用戶對Workfront方案規劃器中資訊的訪問。

* [無權存取](#no-access)
* [檢視存取](#view-access)
* [編輯存取](#edit-access)

### 無權存取 {#no-access}

無法訪問方案規劃器的用戶在將方案表徵圖添加到其佈局模板時，無法在主菜單中看到方案表徵圖，也無法查看與他們共用的計畫和方案。 如果與無權訪問方案計畫員的用戶共用指向計畫的連結，則用戶無法查看或編輯計畫。

### 檢視存取 {#view-access}

具有方案計畫員查看訪問權限的用戶可以執行以下操作：

* 查看主菜單中的方案表徵圖 ![](assets/esp-icon-in-main-menu.png)，但「計畫」區域為空，除非用戶按一下另一個用戶共用的計畫連結。
* 當其他使用者共用連結時檢視計畫。

   這包括計畫中的任何職務角色資訊。

   如果接收方用戶還有權訪問財務資料，則還包括有關計畫的職務費率和成本資訊。 如需詳細資訊，請參閱 [授予金融資料的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

### 編輯存取 {#edit-access}

具有對方案規劃器的編輯訪問權限的用戶可以執行以下操作：

* 查看主菜單中的方案表徵圖 ![](assets/esp-icon-in-main-menu.png) 並使用它存取計畫資料。
* 建立計畫。
* 查看、編輯和刪除他們建立的計畫。
* 查看、編輯和刪除其他用戶使用共用連結訪問的計畫。

   這包括計畫中的任何職務角色資訊。

   如果接收方用戶有權訪問財務資料，則還包括有關計畫的工作角色費率和成本資訊。 如需詳細資訊，請參閱 [授予金融資料的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
