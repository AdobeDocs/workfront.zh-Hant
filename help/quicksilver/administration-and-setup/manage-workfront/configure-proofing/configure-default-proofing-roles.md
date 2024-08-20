---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-proofing-functionality
title: 設定預設校訂角色
description: 身為Adobe Workfront管理員，您可以為存取在Workfront中建立校訂的使用者和訪客使用者設定預設校訂角色。 任何將使用者新增到校樣的人都可以為他們調整這些角色。
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: d64213bf-f270-404f-a45a-6f94c7b7cb91
source-git-commit: ab774e937a15aaa04704e872579df880a9b80aaf
workflow-type: tm+mt
source-wordcount: '550'
ht-degree: 2%

---

# 設定預設校訂角色

身為Adobe Workfront管理員，您可以為存取在Workfront中建立校訂的使用者和訪客使用者設定預設校訂角色。 任何將使用者新增到校樣的人都可以為他們調整這些角色。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

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
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>您必須是Workfront管理員。 如需Workfront管理員的相關資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予使用者完整管理存取權</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的Workfront管理員。

+++

## 設定預設校訂角色

{{step-1-to-setup}}

<!--
   <li In the left panel, click Proofs Proof roles.
   -->

1. 按一下左邊清單底部附近的&#x200B;**檢閱和核准**。
1. 在檔案校訂的&#x200B;**指定收件者的角色**&#x200B;區段中，為新增至校訂工作流程的使用者和訪客使用者選取預設角色。

   如需每個校訂角色及其相關許可權的清單，請參閱下方的[與校訂角色相關的許可權](#rights-associated-with-proofing-roles)。

   >[!NOTE]
   >
   >* 此設定僅適用於設定角色後在Workfront系統中建立的使用者，不適用於現有使用者。
   >* 將使用者新增至校訂的人員可以調整此角色，如[在Adobe Workfront中共用校訂](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md)中的[將使用者新增至校訂](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md#add)中所述。

1. 在開啟檔案校訂&#x200B;**區段的**&#x200B;非收件者角色中，為可存取校訂但未新增至校訂工作流程的使用者和訪客使用者選取預設角色。

   當使用者和訪客有權存取已建立校樣的檔案時，就會發生這種情況：即使他們尚未新增到校樣的工作流程中，也可以開啟校樣。

   **範例：**&#x200B;以下是您如何使用此設定的範例：

   * 您選取「**唯讀**」以限制所有校訂活動，例如新增評論和決定給被要求這樣做的人。
   * 您選取&#x200B;**檢閱者**，因為您希望團隊的任何成員都能在校訂上新增標示和註解。

1. 按一下「**儲存**」。

## 與校訂角色相關聯的許可權 {#rights-associated-with-proofing-roles}

下表顯示每個角色及其關聯的許可權：

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
   <th> <p><strong>檢視校訂</strong> </p> </th> 
   <th> <p><strong>新增標籤</strong> </p> </th> 
   <th> <p><strong>新增註解</strong> </p> </th> 
   <th> <p><strong>如果沒有回覆，請編輯自己的評論</strong> </p> </th> 
   <th> <p><strong>做出決定</strong> </p> </th> 
   <th> <p><strong>刪除其他人的評論</strong> </p> </th> 
   <th>解決評論</th> 
   <th>套用動作至註解</th> 
   <th> <p><strong>編輯校訂</strong> </p> </th> 
   <th>與他人共用校訂</th> 
   <th>建立新版本</th> 
   <th> <p><strong>在首頁區域檢視核准要求</strong> </p> </th> 
   <th>新增檢閱者</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p><strong>唯讀</strong> </p> </td> 
   <td> <p>✓ (A)</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> </td> 
   <td>✓ (A)</td> 
   <td> <p> </p> </td> 
   <td>✓ (A)</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>檢閱者</strong> </p> </td> 
   <td> <p>✓ (A)</p> </td> 
   <td> <p>✓ (A)</p> </td> 
   <td> <p>✓ (A)</p> </td> 
   <td> <p>✓ (A)</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> </td> 
   <td>✓ (A)</td> 
   <td> <p> </p> </td> 
   <td>✓ (A)</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>核准者</strong> </p> </td> 
   <td> <p>✓ (A)</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> <p>✓ (A)</p> </td> 
   <td> <p> </p> </td> 
   <td> </td> 
   <td>✓ (A)</td> 
   <td> <p> </p> </td> 
   <td>✓ (A)</td> 
   <td> </td> 
   <td> <p>✓ (A)</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>檢閱者和核准者</strong> </p> </td> 
   <td> <p>✓ (A)</p> </td> 
   <td> <p>✓ (A)</p> </td> 
   <td> <p>✓ (A)</p> </td> 
   <td> <p>✓ (A)</p> </td> 
   <td> <p>✓ (A)</p> </td> 
   <td> <p> </p> </td> 
   <td> </td> 
   <td>✓ (A)</td> 
   <td> <p> </p> </td> 
   <td>✓ (A)</td> 
   <td> </td> 
   <td> <p>✓ (A)</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>作者</strong> </p> </td> 
   <td> <p>✓ (A)</p> </td> 
   <td> <p>✓ (A)</p> </td> 
   <td> <p>✓ (A)</p> </td> 
   <td> <p>✓ (A)</p> </td> 
   <td> <p>✓ (A)</p> </td> 
   <td> <p> </p> </td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td> <p>✓ (A)</p> </td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td> </td> 
   <td>✓ (A)</td> 
  </tr> 
  <tr> 
   <td> <p><strong>仲裁者</strong> </p> </td> 
   <td> <p>✓ (A)</p> </td> 
   <td> <p>✓ (A)</p> </td> 
   <td> <p>✓ <strong></strong> </p> </td> 
   <td> <p>✓ (A)</p> </td> 
   <td> <p>✓ (A)</p> </td> 
   <td> <p>✓ (A)</p> <p> </p> </td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td> <p>✓ (A)</p> </td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>新Workfront計畫上的使用者可以將作者或版主角色授予系統中的任何使用者。 舊版計畫中的使用者可以將作者或版主角色授予系統中擁有校訂授權的任何使用者。
