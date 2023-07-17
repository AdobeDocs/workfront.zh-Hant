---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 「檢視：合併一個共用欄中多個欄的資訊」
description: 您可以合併顯示在多個獨立欄中的資訊，並將其顯示在共用欄中。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: d4f9db12-59ce-4cfc-90dd-e611b49fafdf
source-git-commit: 976e8c7fe0362392928ac9cd6be1a9ba7c653dda
workflow-type: tm+mt
source-wordcount: '1023'
ht-degree: 0%

---

# 檢視：合併一個共用欄中多個欄的資訊

您可以合併顯示在多個獨立欄中的資訊，並將其顯示在共用欄中。

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>請求修改檢視 </p>
   <p>計畫修改報告</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>編輯報告、儀表板、行事曆的存取權以修改報告</p> <p>編輯對篩選器、檢視、群組的存取權以修改檢視</p> <p><b>附註</b>

如果您仍然沒有存取權，請詢問您的Workfront管理員是否對您的存取層級設定了其他限制。 如需有關Workfront管理員如何修改您的存取層級的資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理報表的許可權</p> <p>如需請求其他存取許可權的詳細資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">要求物件的存取權 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的Workfront管理員。

## 共用或合併欄時的注意事項

* 您可以合併兩個相鄰欄並顯示每個欄的資訊，每個欄的資訊之間以分行符號分隔，也可以合併兩個相鄰欄的資訊，每個欄的資訊之間沒有分隔符號。
* 您可以將本文中所述的相同語法套用至已共用欄和相鄰欄，以合併來自兩個以上欄的資訊。
* 此 `valueformat=HTML` 行在共用欄中是必要的。 否則，從Adobe Workfront匯出報表時，欄不會包含任何資訊（將為空白）。
* 合併的欄可能不支援條件式格式設定。

  存在下列例外：

   * 在Workfront中檢視資訊時，如果構成合併欄的欄彼此格式不同，則會保留第一欄的格式，並忽略所有其他欄的格式。
   * 將檢視匯出至PDF檔案時，條件式格式會套用至合併欄中的第一欄。
   * 將檢視匯出至Excel檔案時，合併的欄會顯示為單獨的欄。 個別欄也會顯示各自的條件式格式規則。

* 具有的欄 **viewalias** attribute可限制可合併的欄數。 若要避免這些限制，請避免使用 **viewalias** 屬性。 如果您必須包含 **viewalias** 屬性，請確定它是欄中列出的最後一個專案。

* 如果將含有共用欄的清單匯出為Excel或Tab分隔格式，這些欄會在匯出的檔案中分隔出來。

* 當一個或兩個欄顯示 `tile` 型別欄位，在合併的欄中會自動引入強制分行符號。 例如，含有格式的文字欄位是 `tile` 輸入欄位。 在此案例中，有一行代碼為 `type=tile` 在文字模式下檢視欄時。

## 合併兩欄資料而不使用分行符號

您可以合併多個不同欄的資料，將其顯示在一欄中，每欄的值之間沒有分隔符號或空格。

>[!TIP]
>
>合併無法同時顯示同一筆記錄的值的兩欄時，建議使用此方法。 例如，在「工作專案」報表中，「問題名稱」和「任務名稱」欄可以合併，而不需要它們之間的分行符號，因為「工作專案」不能同時有「問題名稱」和「任務名稱」。 工作專案可以是Workfront中的問題或任務。

若要這麼做：

1. 使用文字模式進行檢視，將下列文字新增至您要合併的第一欄：

   `sharecol=true`

   合併清單或報表的前兩欄時，Workfront會在包含第一欄中物件相關資訊的每一行文字的前面加上 `column.0.` 以及包含第二欄相關資訊的文字行 `column.1.` .

   您必須在第一欄的欄號前面加上該欄的編號。 欄計數一律以清單或報表最左邊標籤為「 」的欄開始 `column.0.`.

   如果您共用多個欄，請確保在包含每個欄的共用資訊的程式碼行中新增欄編號。

   **範例：** 以下是合併欄的文字模式程式碼，該合併欄包含三個不同的欄，從清單的第二欄開始。 合併的值包括專案名稱、計劃開始日期和專案所有者的名稱，且三個值之間沒有間隙：

   `column.1.valuefield=name`

   `column.1.valueformat=HTML`

   `column.1.sharecol=true`

   `column.2.valuefield=plannedStartDate`

   `column.2.valueformat=atDate`

   `column.2.sharecol=true`

   `column.3.valuefield=owner:name`

   `column.3.valueformat=HTML`

![](assets/shared-column-no-line-breaks-350x142.png)

1. 按一下 **儲存**，則 **儲存檢視**.

## 使用分行符號合併兩欄的資料

執行下列操作來合併多欄的資料，以在一個通用欄中顯示資料，並在每欄的值之間加上分行符號：

1. 在您要合併的兩個欄之間新增第三個欄。

   >[!TIP]
   >
   >* 您要合併的欄必須彼此相鄰。
   >* 您必須按一下要合併的第一欄。

1. 按一下 **切換至文字模式** 和將下列程式碼新增至您在步驟1中新增的中間欄：

   `value=<br>`

   `valueformat=HTML`

   `width=1`

   `sharecol=true`


1. 將下列文字新增至第一欄：

   `sharecol=true`

   合併清單或報表的前兩欄時，Workfront會在包含第一欄中物件相關資訊的每一行文字的前面加上 `column.0.`，與共用資訊的欄 `column.1.`，以及包含第二欄相關資訊的文字行 `column.2.`.

   如果組合欄位於檢視的中間，則欄會根據它們在檢視中的位置編號。 欄計數一律以清單或報表最左邊標籤為「 」的欄開始 `column.0.`.

   如果您共用多個欄，請確定在包含共用資訊的程式碼行中新增欄編號。

   **範例：** 以下是共用欄的文字模式代碼，該共用欄包含專案名稱、計劃開始日期以及具有分行符號的專案所有者名稱。 共用欄是專案檢視的第二欄。


   `column.1.displayname=Project_StartDate_Owner`

   `column.1.sharecol=true`

   `column.1.textmode=true`

   `column.1.valuefield=name`

   `column.1.valueformat=HTML`

   `column.2.value=<br>`

   `column.2.width=1`

   `column.2.valueformat=HTML`

   `column.2.sharecol=true`

   `column.3.valuefield=plannedStartDate`

   `column.3.valueformat=atDate`

   `column.3.sharecol=true`

   `column.4.value=<br>`

   `column.4.width=1`

   `column.4.valueformat=HTML`

   `column.4.sharecol=true`

   `column.5.textmode=true`

   `column.5.valuefield=owner:name`

   `column.5.valueformat=HTML`


   ![](assets/shared-column-with-line-breaks-350x199.png)


1. 按一下 **儲存**，則 **儲存檢視**.
