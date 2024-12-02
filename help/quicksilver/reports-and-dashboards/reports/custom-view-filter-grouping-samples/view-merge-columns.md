---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 檢視：合併一個共用欄中多個欄的資訊
description: 您可以合併顯示在多個獨立欄中的資訊，並將其顯示在一個共用欄中。
author: Nolan
feature: Reports and Dashboards
exl-id: d4f9db12-59ce-4cfc-90dd-e611b49fafdf
source-git-commit: 8c51f8acbe4cefc2404709d9b52c2fe5ec3c7fca
workflow-type: tm+mt
source-wordcount: '1076'
ht-degree: 0%

---

# 檢視：合併一個共用欄中多個欄的資訊

<!-- Audited: 11/2024 -->

您可以合併顯示在多個獨立欄中的資訊，並將其顯示在一個共用欄中。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td> <p> 目前： 
   <ul>
   <li>請求修改檢視</li> 
   <li>計畫修改報表</li>
   </ul>
     </p>
     <p> 新增： 
   <ul>
   <li>修改檢視的貢獻者</li> 
   <li>用於修改報告的標準</li>
   </ul>
     </p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>編輯報告、儀表板、行事曆的存取權以修改報告</p> <p>編輯對篩選器、檢視、群組的存取權以修改檢視</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理報表的許可權</p> </td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 共用或合併欄時的注意事項

* 您可以合併兩個相鄰欄並顯示每個欄的資訊（以分行符號分隔），也可以合併兩個相鄰欄的資訊（每個欄的資訊之間沒有分隔符號）。
* 您可以將本文中所述的相同語法套用至已共用欄和相鄰欄，以合併來自兩個以上欄的資訊。
* `valueformat=HTML`行在共用資料行中是必要的。 否則，從Adobe Workfront匯出報表時，欄不會包含任何資訊（將以空白顯示）。
* 合併的欄可能不支援條件式格式。

  存在下列例外：

   * 在Workfront中檢視資訊時，如果構成合併欄的欄彼此格式不同，則會保留第一欄的格式，並忽略所有其他欄的格式。
   * 將檢視匯出至PDF檔案時，條件式格式會套用至合併欄中的第一欄。
   * 將檢視匯出至Excel檔案時，合併的欄會顯示為單獨的欄。 個別欄也會顯示各自的條件式格式規則。

* 具有&#x200B;**viewalias**&#x200B;屬性的資料行可以限制您可以合併的資料行數量。 若要避免這些限制，請避免使用&#x200B;**viewalias**&#x200B;屬性。 如果您必須在欄中加入&#x200B;**viewalias**&#x200B;屬性，請確定它是列在欄中的最後一個專案。

* 如果將具有共用欄的清單匯出為Excel或Tab分隔格式，這些欄會在匯出的檔案中分隔出來。

* 當一個或兩個欄顯示`tile`型別欄位時，合併的欄會自動引入強制分行符號。 例如，含格式的文字欄位是`tile`型別欄位。 在此情況下，以文字模式檢視欄時有`type=tile`的行碼。

## 合併兩欄資料，不含分行符號

您可以合併多個不同欄的資料，將其顯示在一欄中，每欄的值之間沒有分隔符號或空格。

>[!TIP]
>
>合併兩欄時，如果不能同時顯示同一筆記錄的值，建議使用此方法。 例如，在「工作專案」報表中，「問題名稱」和「任務名稱」欄可以合併，而不在它們之間加上分行符號，因為「工作專案」絕不能同時有「問題名稱」和「任務名稱」。 工作專案可以是Workfront中的問題或任務。

若要合併兩欄資料而不使用分行符號，請執行下列動作：

1. 移至物件清單。
1. 從&#x200B;**檢視**&#x200B;下拉式清單中選取檢視，然後按一下&#x200B;**編輯**&#x200B;圖示![](assets/edit-icon.png)以編輯檢視。
1. 移至您要合併的第一個欄，然後按一下&#x200B;**切換到文字模式** > **編輯文字模式**。
1. 將下列文字新增至您要合併的第一欄：

   `sharecol=true`

   合併清單或報表的前兩欄時，Workfront會在包含第一欄物件相關資訊的每一行文字前加上`column.0.`，並在包含第二欄相關資訊的每一行文字前加上`column.1.` 。

   您必須在第一欄的欄號前面加上該欄的編號。 欄計數一律以清單或報告最左邊標籤為`column.0.`的欄開始。

   如果共用多欄，請確保在包含每欄共用資訊的程式碼行中新增欄編號。


   **範例：**&#x200B;以下是合併資料行的文字模式程式碼，該資料行包含三個不同的資料行，從清單的第二個資料行開始。 合併的值包括專案名稱、計劃開始日期和專案所有者的名稱，這三個值之間沒有間隙：

   ```
   column.1.valuefield=name
   column.1.valueformat=HTML
   column.1.sharecol=true
   column.2.valuefield=plannedStartDate
   column.2.valueformat=atDate
   column.2.sharecol=true
   column.3.valuefield=owner:name
   column.3.valueformat=HTML
   ```

   ![](assets/shared-column-no-line-breaks-350x142.png)


1. 按一下&#x200B;**完成**，然後按一下&#x200B;**儲存檢視**。

## 使用分行符號合併兩欄的資料

執行下列操作以合併多個欄的資料，將其顯示在一個通用欄中，並在每個欄的值之間加上分行符號：

1. 移至物件清單。
1. 從&#x200B;**檢視**&#x200B;下拉式清單中選取檢視，然後按一下&#x200B;**編輯**&#x200B;圖示![](assets/edit-icon.png)以編輯檢視。
1. 在您要合併的兩個欄之間新增第三個欄。

   >[!TIP]
   >
   >* 您要合併的欄必須彼此相鄰。
   >* 您必須按一下要合併的第一欄。

1. 按一下&#x200B;**切換到文字模式** > **編輯文字模式**，然後在步驟1中新增的中間欄中加入下列程式碼：

   ```
   value=<br>
   valueformat=HTML
   width=1
   sharecol=true
   ```

1. 按一下第一欄，然後按一下&#x200B;**切換到文字模式** > **編輯文字模式**，然後將下列文字新增至欄：

   `sharecol=true`

   當您合併清單或報告的前兩欄時，Workfront會在包含第一欄中物件相關資訊的每一行文字前面`column.0.`、包含與`column.1.`共用資訊的欄，以及包含第二欄相關資訊的文字行前面`column.2.`。

   如果組合欄位於檢視的中間，則會根據欄在檢視中的位置對其進行編號。 欄計數一律以清單或報告最左邊標籤為`column.0.`的欄開始。

   如果共用多個欄，請確保在包含共用資訊的程式碼行中新增欄編號。

   **範例：**&#x200B;下列是共用欄的文字模式代碼，其中包含專案名稱、規劃開始日期及具有分行符號的專案所有者名稱。 共用欄是專案檢視的第二欄。

   ```
   column.1.displayname=Project_StartDate_Owner
   column.1.sharecol=true
   column.1.textmode=true
   column.1.valuefield=name
   column.1.valueformat=HTML
   column.2.value=<br>
   column.2.width=1
   column.2.valueformat=HTML
   column.2.sharecol=true
   column.3.valuefield=plannedStartDate
   column.3.valueformat=atDate
   column.3.sharecol=true
   column.4.value=<br>
   column.4.width=1
   column.4.valueformat=HTML
   column.4.sharecol=true
   column.5.textmode=true
   column.5.valuefield=owner:name
   column.5.valueformat=HTML 
   ```

   ![](assets/shared-column-with-line-breaks-350x199.png)

1. 按一下&#x200B;**完成**，然後按一下&#x200B;**儲存檢視**。
