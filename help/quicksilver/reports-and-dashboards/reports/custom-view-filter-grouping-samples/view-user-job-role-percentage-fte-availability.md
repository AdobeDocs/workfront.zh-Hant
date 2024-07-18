---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: “檢視：用戶工作角色佔 FTE 可用性的百分比”
description: 您可以將列添加到用戶 清單的視圖，以显示與用戶關聯的工作角色的清單，以及用戶 設定檔中定義的每個作業角色的 FTE 可用性百分比。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: d479b0b1-8ad5-47d6-8ef8-80261b46ecea
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '353'
ht-degree: 0%

---

# 檢視：使用者工作角色的FTE可用性百分比

您可以在使用者清單的檢視中新增欄位，以顯示使用者相關聯的「工作角色」清單，以及每個工作角色的FTE可用性百分比（如使用者設定檔中所定義）。

如需定義使用者FTE可用性百分比的相關資訊，請參閱[編輯使用者的設定檔](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)。

![用戶_with_percent_avialbility_per_角色.png](assets/user-with-percent-avialbility-per-role-350x138.png)

## 存取需求

您必須具有以下存取權限才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Systems工作台計劃*</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Systems Workfront 許可證*</td> 
   <td> <p>請求修改視圖 </p>
   <p>計劃修改報表</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>編輯報告、儀表板、行事曆的存取權以修改報告</p> <p>編輯對篩選器、檢視、群組的存取權以修改檢視</p> <p><b>附註</b>

如果您仍然沒有訪問許可權，請詢問您的 Workfront 管理員是否在您的訪問許可權級別中設置了其他限制。 有關 Workfront 管理員如何修改存取權限等級的資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自定義訪問級別</a>。</p> </td>
</tr>   
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理報表的許可權</p> <p>有關請求其他存取權限的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對物件 </a>的存取權限 。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要瞭解您擁有的計劃、許可證類型或訪問許可權，請聯繫您的 Workfront 管理員。

## 檢視 用戶工作角色 FTE 可用性的百分比

1. 轉到使用者清單。
1. 從&#x200B;**檢視**&#x200B;下拉式功能表中，選取&#x200B;**新增檢視**。

1. 在&#x200B;**欄預覽**&#x200B;區域中，按一下&#x200B;**新增欄**。

1. 按兩下新欄的標題，然後按下 **切換到文字模式**。
1. 將滑鼠移到文字模式區域，然後按下按兩下&#x200B;**以編輯文字**。
1. 移除在「文字模式&#x200B;**」**&#x200B;框中找到的文字，並將其替換為以下代碼：
   <pre>顯示名稱=角色 時間百分比<br>listdelimiter=<p><br>listmethod=nested（userRoles）.lists<br>textmode=true<br>type=iterate<br>valueexpression=CONCAT（{role}，'-'，{timePercentage}，'%'）<br>valueformat=HTML</pre>

1. 單擊儲存&#x200B;**，然後按兩下****儲存 檢視**。

1. （選擇）指定視圖的名稱，然後按下 **儲存 檢視**。
