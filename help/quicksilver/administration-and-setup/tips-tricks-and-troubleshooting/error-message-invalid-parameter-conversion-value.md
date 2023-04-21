---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: '''錯誤訊息：參數無效：轉換值'
description: 「嘗試更改現有自定義表單上的自定義欄位格式時，您會收到以下錯誤消息：'無效參數：轉換值'&lt;...&gt;""
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 4f7aac95-4afb-422d-877b-0fa49ef43883
source-git-commit: 62d1b9563d83bd82b569e143f69e379e2f4ffbc2
workflow-type: tm+mt
source-wordcount: '336'
ht-degree: 1%

---

# 錯誤訊息：參數無效：轉換值

## 問題

嘗試更改現有自定義表單上的自定義欄位格式時，您會收到以下錯誤消息：&quot;無效參數：轉換值&quot;&lt;...>&quot;&quot;\
![custom_field_format_invalid_parameter_error.png](assets/custom-field-format-invalid-parameter-error-350x148.png)

## 原因

此訊息會發生在下列情境中：

例如，您有格式為「文字」的「自訂欄位」。  現在，您想要將「自訂欄位格式」變更為「貨幣」。 在Adobe Workfront例項的某處，此欄位已附加至物件，且其中已指定資訊。 至少一個此類欄位中的現有資訊已格式化為文本。 因此，欄位的格式無法變更為貨幣。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p><a href="https://www.workfront.com/plans" target="_blank">Workfront計畫</a>*</p> </td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">授權概觀</a>*</p> </td> 
   <td>計劃</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"><strong>存取層級*</strong> </td> 
   <td> <p>編輯對以下項目的訪問：</p> 
    <ul> 
     <li> <p>建立報表、控制面板和日曆</p> </li> 
     <li> <p>建立篩選、檢視和群組</p> </li> 
    </ul> <p><b>注意</b>:如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何變更您的存取層級的詳細資訊，請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 解決方案

執行下列動作：

1. 為所有可能將此欄位與其自訂Forms關聯的物件建立報表。\
   如需建立報表的相關資訊，請參閱 [建立自訂報表](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. 在報表檢視中加入您嘗試編輯的自訂欄位，以便查看哪個物件已將此欄位填入文字值。
1. 更正以文本格式顯示的對象的「自定義欄位」值，並為其指定格式為「貨幣」的值；然後嘗試再次更改「自定義表單」上的「格式」欄位。\
   或\
   如果已用文本格式化資訊填入太多欄位值，請考慮將新的「自定義欄位」添加到「自定義表單」中，並將其格式化為「貨幣」。
