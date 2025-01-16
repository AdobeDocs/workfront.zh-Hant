---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: 在Adobe Workfront Fusion中排程情境
description: Adobe Workfront Fusion檔案已移至新位置。 本文已棄用，但包含新文章的連結，內容涵蓋此功能。
author: Becky
feature: Workfront Fusion
exl-id: bce89abe-ec37-4705-a88f-de62c8b27f49
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '632'
ht-degree: 0%

---

# 在[!DNL Adobe Workfront Fusion]中排程情境

>[!IMPORTANT]
>
>Adobe Workfront Fusion檔案已移至新位置。
>
>本文資訊可在以下文章中找到：
>
>* [排程情境](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/configure-scenario-settings/schedule-a-scenario.html)
>
>請更新任何書籤。
>
>本文已不再更新，將於不久將來移除。

依預設，一個案例每15分鐘執行一次。 您可以定義已啟動案例執行的時間和頻率，以變更此專案。 融合情境可以排程為每5分鐘執行一次。

## 存取需求

您必須具有下列存取權才能使用本文中的功能：

<table style="table-layout:auto">   
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] 計畫*</td> 
   <td> <p>[!DNL Pro] 或更高</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權*</td> 
   <td> <p>[！UICONTROL計畫]，[！UICONTROL工作]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Adobe Workfront Fusion]授權**</td> 
  <td>
   <p>目前授權需求：無[!DNL Workfront Fusion]授權需求。</p>
   <p>或</p>
   <p>舊版授權需求： [！UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration]，[！UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
   </td>    </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>
   <p>目前產品需求：如果您有[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Adobe Workfront]計畫，您的組織必須購買[!DNL Adobe Workfront Fusion]及[!DNL Adobe Workfront]，才能使用本文所述的功能。 [!DNL Workfront Fusion]包含在[！UICONTROL Ultimate] [!DNL Workfront]計畫中。</p>
   <p>或</p>
   <p>舊版產品需求：您的組織必須購買[!DNL Adobe Workfront Fusion]及[!DNL Adobe Workfront]，才能使用本文所述的功能。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的[!DNL Workfront]管理員。

如需[!DNL Adobe Workfront Fusion]授權的相關資訊，請參閱[[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md)。

## 排程情境

1. 在「情境詳細資料」頁面的右上角，按一下&#x200B;**[!UICONTROL 選項]** > **[!UICONTROL 排程]**

   或

   按一下情境觸發程式模組上的&#x200B;**[!UICONTROL 排程]**&#x200B;圖示（時鐘）。

1. 在下列欄位中輸入資訊：

   <table style="table-layout:auto">   
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[！UICONTROL執行案例]</td> 
      <td> <p>選取您要執行情境的頻率，然後選取間隔。</p> 
       <ul> 
        <li> <p><strong>[！UICONTROL為固定間隔]</strong> </p> <p>輸入執行之間的分鐘數。 預設值為15分鐘。</p> </li> 
        <li> <p><strong>[！UICONTROL一次]</strong> </p> <p>輸入您希望案例執行的日期和時間。 使用格式<code>MM/DD/YYYY h:mm A</code>。 範例： <code>06/25/2019 11:00 PM</code>。</p> </li> 
        <li> <p><strong>[！UICONTROL每天]</strong> </p> <p>輸入您希望案例執行的時間。 使用格式<code>h:mm A</code>。 範例： <code>11:00 PM</code>。</p> </li> 
        <li> <p><strong>[！UICONTROL一週天數]</strong> </p> <p>天數：選取您希望案例在一週中執行的天數。 您可以選取一或多天。</p> <p>時間：輸入您希望案例在所選日期執行的時間。 使用格式<code>h:mm A</code>。 範例： <code>11:00 PM</code></p> </li> 
        <li> <p><strong>[！UICONTROL當月天數]</strong> </p> <p>天數：選取您希望案例執行的月份天數。 您可以選取一或多天。</p> <p>時間：輸入您希望案例在所選日期執行的時間。 使用格式<code>h:mm A</code>。 範例： <code>11:00 PM</code></p> </li> 
        <li> <p><strong>[！UICONTROL指定的日期]</strong> </p> <p>月份：選取您要執行案例的月份。 您可以選取一或多個月份。</p> <p>天數：選取您希望案例執行的月份天數。 您可以選取一或多天。</p> <p>時間：輸入您希望案例在所選日期執行的時間。 使用格式<code>h:mm A</code>。 範例： <code>11:00 PM</code></p> </li> 
       </ul> <p>備註：案例必須有日期才能在該日期執行。 例如，僅排定在該月第31天的情境將不會在2月、4月、6月、9月或11月執行，因為這些月份沒有第31天。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL進階排程]</td> 
      <td>您可以定義執行情境的特定時間間隔。 您可以指定一天中的時間間隔、工作日或月。 對於每個間隔，按一下<strong>[！UICONTROL新增]</strong>，並按照[！UICONTROL執行案例]欄位中的說明填寫欄位。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL開始]</td> 
      <td>輸入您希望案例執行的日期和時間。 使用格式<code>MM/DD/YYYY h:mm A</code>。 範例： <code>06/25/2019 11:00 PM</code>。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL結尾]</td> 
      <td>輸入您希望案例執行的日期和時間。 使用格式<code>MM/DD/YYYY h:mm A</code>。 範例： <code>06/25/2019 11:00 PM</code>。</td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下&#x200B;**[!UICONTROL 確定]**&#x200B;以儲存排程設定並返回案例。
