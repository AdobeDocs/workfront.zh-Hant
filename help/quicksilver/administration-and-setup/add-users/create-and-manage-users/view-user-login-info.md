---
title: 檢視使用者登入資訊
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: 您可以藉由指定您要在使用者清單的檢視或使用者的報表中納入此資訊，來檢視使用者登入Workfront的頻率以及上次登入的時間。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 7b37c34a-d628-4d9b-9688-e4b9f89c666b
source-git-commit: 20cb940de1d42057ed11e4e7d59f1875cdba38bb
workflow-type: tm+mt
source-wordcount: '582'
ht-degree: 1%

---

# 檢視使用者登入資訊

您可以藉由指定您要在使用者清單的檢視或使用者的報表中納入此資訊，來檢視使用者登入Adobe Workfront的頻率以及上次登入的時間。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具備下列專案才能執行本文所述的步驟：

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
   <td role="rowheader">存取層級設定</td> 
   <td> <p>您必須具備下列其中一項：</p> 
    <ul> 
     <li> <p>系統管理員存取層級。 如需詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予使用者完整管理存取權</a>。 </p> </li> 
     <li> <p>您的存取層級中的<b>使用者</b>設定已設定為<b>編輯</b>存取權，其中<b>建立</b>以及在<b>微調您的設定</b> <img src="assets/gear-icon-in-access-levels.png">下啟用的兩個<b>使用者管理員</b>選項中的至少一個。 </p> <p>在這兩個選項中，如果已啟用使用者<b>管理員（群組使用者）</b>，您必須是該使用者所屬群組的群組管理員。</p> <p>如需存取層級中<b>使用者</b>設定的詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">授予使用者存取權</a>。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Workfront如何記錄登入資訊

Workfront會記錄下列有關登入系統之使用者的資訊：

* **登入計數**： Workfront會將每24小時登入一次應用程式的使用者計數。 若一位使用者使用不同瀏覽器、電腦或行動裝置登入多次，Workfront會將一天內發生的所有登入計為單次登入。 「登入計數」包含從建立使用者時開始的資訊。
* **上次登入日期**：使用者上次登入的日期。 每次從任何瀏覽器、行動裝置或其他應用程式登入的日期，都會記錄在此欄位中。

以下列任一方式登入Workfront即會計為Workfront的登入：

* Workfront網頁應用程式
* Workfront行動應用程式(iOS或Android裝置)
* 任何受支援的Workfront與其他第三方應用程式(Slack、Jira)的整合
* Workfront與其他第三方應用程式之間的任何自訂整合。
* WORKFRONT API

  >[!NOTE]
  >
  >透過Workfront API登入Workfront，僅適用於尚未加入Adobe Business Platform的組織。

## 在使用者清單或報告中顯示使用資訊

您可以在使用者清單的檢視或使用者的報告中顯示「登入計數」和「上次登入日期」欄位。\
如需建立報告的詳細資訊，請參閱[建立自訂報告](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)。

若要在使用者清單檢視中顯示使用資訊：

1. 前往Workfront中的使用者清單。
1. 從&#x200B;**檢視**&#x200B;下拉式功能表中，選取&#x200B;**新增檢視**。

1. 按一下熒幕右下角附近的&#x200B;**新增欄**。
1. 在&#x200B;**顯示在此欄**&#x200B;欄位中，開始輸入&#x200B;**登入計數**，然後當它出現在&#x200B;**使用者**&#x200B;下的清單中時選取它。

1. 再按一下「**新增欄**」。
1. 在&#x200B;**顯示於欄**&#x200B;欄位中，開始輸入&#x200B;**上次登入日期**，然後當它出現在&#x200B;**使用者**&#x200B;下的清單中時選取它。

1. （選擇性）按一下&#x200B;**進階選項**，然後從下拉式選單中選取&#x200B;**欄位格式**，以將上次登入的時間或一週中的某天包含在欄中。

1. 按一下「**儲存視圖**」。\
   檢視包含使用者已登入次數和上次登入時間的相關資訊。
