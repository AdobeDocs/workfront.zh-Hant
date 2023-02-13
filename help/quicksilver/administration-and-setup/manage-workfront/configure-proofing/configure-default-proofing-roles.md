---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-proofing-functionality
title: 配置預設校對角色
description: 身為Adobe Workfront管理員，您可以為存取Workfront中建立之校樣的使用者和訪客使用者設定預設校樣角色。 將使用者新增至校樣的任何人，都可以為他們調整這些角色。
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: d64213bf-f270-404f-a45a-6f94c7b7cb91
source-git-commit: 02191d80ea58f80de2e7be2ff55f43663e415e31
workflow-type: tm+mt
source-wordcount: '508'
ht-degree: 1%

---

# 配置預設校對角色

身為Adobe Workfront管理員，您可以為存取Workfront中建立之校樣的使用者和訪客使用者設定預設校樣角色。 將使用者新增至校樣的任何人，都可以為他們調整這些角色。

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td>計劃</td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>您必須是Workfront管理員。 如需Workfront管理員的相關資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予使用者完整的管理存取權</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 配置預設校對角色

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **設定** ![](assets/gear-icon-settings.png).

   <!--
   <li In the left panel, click Proofs Proof roles.
   -->

1. 按一下 **審核和批准** 靠近左側清單的底部。
1. 在 **文檔校樣的指定收件人的角色** 部分，為添加到校樣工作流的用戶和來賓用戶選擇預設角色。

   請參閱 [與校對角色相關聯的權限](#rights-associated-with-proofing-roles) 以取得每個校對角色的清單，以及與其相關聯的權利。

   >[!NOTE]
   >
   >* 此設定僅適用於角色設定後在Workfront系統中建立的使用者；對現有使用者而言則否。
   >* 將使用者新增至校樣的人員可以調整此角色，如 [新增使用者至校樣](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md#add) in [在Adobe Workfront內共用證明](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).


1. 在 **開啟檔案校樣的非收件者角色** 區段中，為可存取校樣但不新增至校樣工作流程的使用者和訪客使用者選取預設角色。

   當用戶和來賓有權訪問已建立校樣的文檔時，會發生這種情況：即使尚未將校樣新增至校樣的工作流程，他們也可以開啟校樣。

   **範例：** 以下範例說明如何使用此設定：

   * 您選取 **唯讀** 限制所有證明活動，例如新增留言及決策，讓被要求者執行。
   * 您選取 **審核者** 因為您希望團隊的任何成員都能在校樣上新增標籤和註解。

1. 按一下&#x200B;**儲存**。

## 與校對角色相關聯的權限 {#rights-associated-with-proofing-roles}

下表顯示每個角色及其相關的權限：

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p> </p> </th> 
   <th> <p><strong>檢視校樣</strong> </p> </th> 
   <th> <p><strong>新增行銷</strong> </p> </th> 
   <th> <p><strong>添加註釋</strong> </p> </th> 
   <th> <p><strong>如果沒有回覆，請編輯自己的留言</strong> </p> </th> 
   <th> <p><strong>做出決定</strong> </p> </th> 
   <th> <p><strong>刪除其他人的評論</strong> </p> </th> 
   <th>解決注釋</th> 
   <th>將動作套用至註解</th> 
   <th> <p><strong>編輯校樣</strong> </p> </th> 
   <th>與其他人共用證明</th> 
   <th>建立新版本</th> 
   <th> <p><strong>在「首頁」區域中查看批准請求</strong> </p> </th> 
   <th>新增審核者</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p><strong>唯讀</strong> </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> </td> 
   <td>✓</td> 
   <td> <p> </p> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>檢閱者</strong> </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> </td> 
   <td>✓</td> 
   <td> <p> </p> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>核准者</strong> </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> </td> 
   <td>✓</td> 
   <td> <p> </p> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> <p>✓</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>檢閱者和核准者</strong> </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> </td> 
   <td>✓</td> 
   <td> <p> </p> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> <p>✓</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>作者</strong> </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> <p>✓</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p><strong>仲裁者</strong> </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p><strong>✓</strong> </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> <p> </p> </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> <p>✓</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>新Workfront計畫的使用者可將作者或版主角色授與系統中的任何使用者。 舊版計畫的使用者可以將作者或版主角色授予系統中具有校樣授權的任何使用者。
