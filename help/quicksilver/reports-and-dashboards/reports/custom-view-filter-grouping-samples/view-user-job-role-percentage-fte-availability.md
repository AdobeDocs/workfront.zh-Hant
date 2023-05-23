---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: '''查看：用戶作業角色佔FTE可用性的百分比'
description: 您可以向用戶清單的視圖中添加一列，以顯示用戶關聯的作業角色清單以及每個作業角色的FTE可用性百分比（如用戶配置檔案中所定義）。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: d479b0b1-8ad5-47d6-8ef8-80261b46ecea
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '358'
ht-degree: 0%

---

# 視圖：用戶作業角色佔FTE可用性的百分比

您可以向用戶清單的視圖中添加一列，以顯示用戶關聯的作業角色清單以及每個作業角色的FTE可用性百分比（如用戶配置檔案中所定義）。

有關定義用戶FTE可用性百分比的資訊，請參閱 [編輯用戶的配置檔案](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)。

![user_with_percent_avialability_per_role_png](assets/user-with-percent-avialbility-per-role-350x138.png)

## 訪問要求

您必須具有以下訪問權限才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront許可證*</td> 
   <td> <p>請求修改視圖 </p>
   <p>計畫修改報表</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯對報表、儀表板、日曆的訪問以修改報表</p> <p>編輯對篩選器、視圖、分組的訪問以修改視圖</p> <p><b>附註</b>

如果您仍然沒有訪問權限，請詢問您的Workfront管理員是否在您的訪問級別設定了其他限制。 有關Workfront管理員如何修改您的訪問級別的資訊，請參見 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自定義訪問級別</a>。</p> </td>
</tr>   
  <tr> 
   <td role="rowheader">對象權限</td> 
   <td> <p>管理對報表的權限</p> <p>有關請求附加訪問的資訊，請參見 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求訪問對象 </a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要瞭解您擁有的計畫、許可證類型或訪問權限，請與您的Workfront管理員聯繫。

## 查看用戶職務角色佔FTE可用性的百分比

1. 轉到用戶清單。
1. 從 **視圖** 下拉菜單，選擇 **新建視圖**。

1. 在&#x200B;**列預覽** 的 **添加列**。

1. 按一下新列的標題，然後按一下 **切換到文本模式**。
1. 將滑鼠移到文本模式區域上，然後按一下 **按一下可編輯文本**。
1. 刪除在中查找的文本 **文本模式** 框，並用以下代碼替換它：

   <pre>displayname=角色時間百分比<br>清單分隔符=<p><br>listmethod=nested(userRoles)。lists<br>textmode=true<br>類型=迭代<br>valueexpression=CONCAT({role},'-',{timePercentage},'%')<br>valueformat=HTML</pre>

1. 按一下 **保存**，則 **保存視圖**。

1. （可選）指定視圖的名稱，然後按一下 **保存視圖**。
