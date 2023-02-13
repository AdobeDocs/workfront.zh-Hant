---
title: 查看用戶登錄資訊
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: 您可以指出您要將這項資訊納入使用者清單的檢視中，或列在使用者的報表中，借此查看使用者登入Workfront的頻率以及上次登入的時間。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 7b37c34a-d628-4d9b-9688-e4b9f89c666b
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '570'
ht-degree: 0%

---

# 查看用戶登錄資訊

您可以指出您要將這項資訊納入使用者清單的檢視中，或列在使用者的報表中，借此查看使用者登入Adobe Workfront的頻率以及上次登入的時間。

## 存取需求

您必須具備下列條件才能執行本文所述步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td> <p>計劃 </p>   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置</td> 
   <td> <p>您必須具備下列其中一項：</p> 
    <ul> 
     <li> <p>系統管理員訪問級別。 如需詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予使用者完整的管理存取權</a>. </p> </li> 
     <li> <p><b>使用者</b> 在您的存取層級中設定 <b>編輯</b> 存取，使用 <b>建立</b> 和兩者中的至少一個 <b>使用者管理</b> 選項 <b>微調您的設定</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>在這兩個選項中，如果用戶 <b>管理員（群組使用者）</b> 啟用時，您必須是使用者所屬群組的群組管理員。</p> <p>如需 <b>使用者</b> 在存取層級中設定，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">授予使用者存取權</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Workfront記錄登入資訊的方式

Workfront會記錄下列使用者登入系統的相關資訊：

* **登入計數**:Workfront會計算每24小時登入應用程式一次的使用者。 如果一個使用者使用不同的瀏覽器、電腦或行動裝置多次登入，Workfront會將一天中發生的所有登入都計為一次登入。 「登入計數」包含的資訊從建立使用者時開始。
* **上次登入日期**:使用者上次登入的日期。 來自任何瀏覽器、行動裝置或其他應用程式的每次登入日期都會記錄在此欄位中。

以下列任一方式登入Workfront，即計為Workfront登入：

* Workfront Web應用程式
* Workfront行動應用程式(iOS或Android裝置)
* 任何支援的Workfront與其他協力廠商應用程式整合(Slack、Jira)
* Workfront與其他協力廠商應用程式之間的任何自訂整合。
* Workfront API

   >[!NOTE]
   >
   >透過Workfront API登入Workfront的功能，僅供尚未上線至Adobe商業平台的組織使用。

## 在使用者清單或報表中顯示使用資訊

您可以在使用者清單的檢視或使用者的報表中顯示「登入計數」和「上次登入日期」欄位。\
如需建立報表的詳細資訊，請參閱 [建立自訂報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

要在用戶清單視圖中顯示使用資訊，請執行以下操作：

1. 前往Workfront中的使用者清單。
1. 從 **檢視** 下拉式功能表，選取 **新建視圖**.

1. 按一下 **添加列** 靠近螢幕的右下角。
1. 在 **顯示在此列中** 欄位，開始鍵入 **登入計數**，然後選取顯示於下方清單中的 **使用者**.

1. 按一下 **添加列** 。
1. 在 **顯示在欄中** 欄位，開始鍵入 **上次登入日期**，然後選取顯示於下方清單中的 **使用者**.

1. （選用）按一下 **進階選項**，然後選取 **欄位格式** 從下拉式功能表，將上次登入的時間或星期幾納入欄中。

1. 按一下 **保存視圖**.\
   檢視包含使用者登入次數及上次登入時間的相關資訊。
