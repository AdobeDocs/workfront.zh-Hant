---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: '錯誤訊息：無效引數：轉換值'
description: 「嘗試變更現有自訂表單上自訂欄位格式時，出現下列錯誤訊息：『無效引數：轉換值'&amp； lt；..&amp；gt；"
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 4f7aac95-4afb-422d-877b-0fa49ef43883
source-git-commit: 62d1b9563d83bd82b569e143f69e379e2f4ffbc2
workflow-type: tm+mt
source-wordcount: '330'
ht-degree: 0%

---

# 錯誤訊息：無效引數：轉換值

## 問題

嘗試變更現有自訂表單上自訂欄位格式時，您收到下列錯誤訊息：「無效引數：轉換值&quot;&lt;...>&quot;\
![custom_field_format_invalid_parameter_error.png](assets/custom-field-format-invalid-parameter-error-350x148.png)

## 原因

此訊息會發生在以下情況中：

例如，您有一個格式為文字的自訂欄位。  現在，您想要將自訂欄位的格式變更為貨幣。 在您的Adobe Workfront執行個體的某個位置，此欄位已附加至物件，而且其中已指定資訊。 至少有一個此類欄位中的現有資訊已經格式化為文字。 因此，欄位格式無法變更為貨幣。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p><a href="https://www.workfront.com/plans" target="_blank">Workfront計畫</a>*</p> </td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">授權總覽</a>*</p> </td> 
   <td>計劃</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"><strong>存取層級*</strong> </td> 
   <td> <p>編輯下列專案的存取權：</p> 
    <ul> 
     <li> <p>建立報告、儀表板和行事曆</p> </li> 
     <li> <p>建立篩選器、檢視和群組</p> </li> 
    </ul> <p><b>注意</b>：如果您還是沒有存取權，請詢問您的Workfront管理員是否對您的存取層級設定了其他限制。 如需Workfront管理員如何變更存取層級的詳細資訊，請參閱<a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 解決方案

執行下列動作：

1. 為可能擁有此欄位與其自訂Forms相關聯的所有物件建立報告。\
   如需建立報表的相關資訊，請參閱[建立自訂報表](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)。

1. 在報表檢視中加入您嘗試編輯的自訂欄位，以便檢視哪個物件有此欄位填入文字值。
1. 修正以文字格式顯示之物件的「自訂欄位」值，並為它們提供「貨幣」格式的值，然後再次嘗試變更「自訂表單」上的「格式」欄位。\
   或\
   如果您有太多欄位值已填入文字格式資訊，請考慮新增自訂欄位至您的自訂表單，並將其格式化為貨幣。
