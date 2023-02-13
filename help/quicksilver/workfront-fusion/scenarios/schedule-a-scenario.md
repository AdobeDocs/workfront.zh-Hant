---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: 排程Adobe Workfront Fusion中的案例
description: 依預設，藍本每15分鐘執行一次。 您可以定義啟動的案例執行的時間和頻率，以變更此設定。
author: Becky
feature: Workfront Fusion
exl-id: bce89abe-ec37-4705-a88f-de62c8b27f49
source-git-commit: 59941ea1ce523a0d1036138a83f771b058049b34
workflow-type: tm+mt
source-wordcount: '516'
ht-degree: 1%

---

# 在中排程藍本 [!DNL Adobe Workfront Fusion]

依預設，藍本每15分鐘執行一次。 您可以定義啟動的案例執行的時間和頻率，以變更此設定。

## 存取需求

您必須具備下列存取權才能使用本文中的功能：

<table style="table-layout:auto">   
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] 計劃*</td> 
   <td> <p>[!DNL Pro] 或更高</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權*</td> 
   <td> <p>[!UICONTROL計畫]、[!UICONTROL工作]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion]授權**</td> 
  <td> <p>[!UICONTROL [!DNL Workfront Fusion] （工作自動化和整合） </p><p>[!UICONTROL [!DNL Workfront Fusion] （工作自動化） </p>  </td>    </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>貴組織必須購買 [!DNL Adobe Workfront Fusion] 和 [!DNL Adobe Workfront] 以使用本文所述的功能。</td> 
  </tr> 
 </tbody> 
</table>

若要了解您擁有的計畫、授權類型或存取權，請聯絡您的 [!DNL Workfront] 管理員。

如需 [!DNL Adobe Workfront Fusion] 許可證，請參閱 [[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 排程藍本

1. 在「藍本」詳細資訊頁面的右上角，按一下 **[!UICONTROL 選項]** > **[!UICONTROL 排程]**

   或

   按一下 **[!UICONTROL 排程]** 圖示（時鐘）。

1. 在以下欄位中輸入資訊：

   <table style="table-layout:auto">   
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL運行方案]</td> 
      <td> <p>選取要執行藍本的頻率，然後選取間隔。</p> 
       <ul> 
        <li> <p><strong>[!UICONTROL以規則間隔]</strong> </p> <p>輸入執行之間的分鐘數。 預設值為15分鐘。</p> </li> 
        <li> <p><strong>[!UICONTROL一次]</strong> </p> <p>輸入要運行方案的日期和時間。 使用格式 <code>MM/DD/YYYY h:mm A</code>. 範例: <code>06/25/2019 11:00 PM</code>.</p> </li> 
        <li> <p><strong>[!UICONTROL每天]</strong> </p> <p>輸入方案要執行的時間。 使用格式 <code>h:mm A</code>. 範例: <code>11:00 PM</code>.</p> </li> 
        <li> <p><strong>[!UICONTROL一週天數]</strong> </p> <p>天數：選取要執行方案的一週天數。 您可以選取一或多天。</p> <p>時間：輸入希望方案在所選天運行的時間。 使用格式 <code>h:mm A</code>. 範例: <code>11:00 PM</code></p> </li> 
        <li> <p><strong>[!UICONTROL當月天數]</strong> </p> <p>天數：選取要執行方案的月份天數。 您可以選取一或多天。</p> <p>時間：輸入希望方案在所選天運行的時間。 使用格式 <code>h:mm A</code>. 範例: <code>11:00 PM</code></p> </li> 
        <li> <p><strong>[!UICONTROL指定日期]</strong> </p> <p>月：選擇要運行方案的月份。 您可以選取一或多個月。</p> <p>天數：選取要執行方案的月份天數。 您可以選取一或多天。</p> <p>時間：輸入希望方案在所選天運行的時間。 使用格式 <code>h:mm A</code>. 範例: <code>11:00 PM</code></p> </li> 
       </ul> <p>注意：方案必須存在日期才能在該日期執行。 例如，僅排程當月31日的情境不會在2月、4月、6月、9月或11月執行，因為這些月沒有31日。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL高級計畫]</td> 
      <td>您可以定義執行藍本的特定時間間隔。 您可以指定每日時間間隔、周或月。 對於每個間隔，按一下 <strong>[!UICONTROL添加]</strong> 並依照[!UICONTROL執行案例]欄位中的說明填入欄位。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL開始]</td> 
      <td>輸入要在其後運行方案的日期和時間。 使用格式 <code>MM/DD/YYYY h:mm A</code>. 範例: <code>06/25/2019 11:00 PM</code>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL結束]</td> 
      <td>輸入方案要運行的日期和時間。 使用格式 <code>MM/DD/YYYY h:mm A</code>. 範例: <code>06/25/2019 11:00 PM</code>.</td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下 **[!UICONTROL 確定]** 儲存排程設定並返回藍本。
