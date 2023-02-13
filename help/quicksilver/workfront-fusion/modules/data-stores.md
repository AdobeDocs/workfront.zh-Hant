---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: 資料儲存於 [!DNL Adobe Workfront Fusion]
description: 資料儲存類似於資料庫或簡單表，可以儲存來自方案的資料，從而可以在個別方案或方案運行之間傳輸資料。 您可以在同步期間使用資料儲存來儲存來自各種系統的新資料。
author: Becky
feature: Workfront Fusion
exl-id: 2a665a71-b819-4861-b119-f5c28b87e9c5
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1176'
ht-degree: 1%

---

# 資料儲存於 [!DNL Adobe Workfront Fusion]

資料儲存類似於資料庫或簡單表，可以儲存來自方案的資料，從而可以在個別方案或方案運行之間傳輸資料。 您可以在同步期間使用資料儲存來儲存來自各種系統的新資料。

資料儲存模組可讓您對您 [!DNL Adobe Workfront Fusion] 資料存放區：

* 新增
* 取代
* 更新
* 擷取
* 刪除
* 搜尋
* 計數

如需使用資料存放區模組的資訊，請參閱 [[!UICONTROL 資料儲存] 模組](../../workfront-fusion/apps-and-their-modules/data-store-modules.md).

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] （工作自動化和整合） </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>貴組織必須購買 [!DNL Adobe Workfront Fusion] 和 [!DNL Adobe Workfront] 以使用本文所述的功能。</td> 
  </tr> 
 </tbody> 
</table>

若要了解您擁有的計畫、授權類型或存取權，請聯絡您的 [!DNL Workfront] 管理員。

如需 [!DNL Adobe Workfront Fusion] 許可證，請參閱 [[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 在中建立資料儲存 [!DNL Workfront Fusion]

* [設定資料儲存](#set-up-the-data-store)
* [設定資料結構](#set-up-the-data-structure)

### 設定資料儲存

您必須先在中建立資料存放區，才能在中使用資料存放區 [!DNL Workfront Fusion].

>[!NOTE]
>
>貴組織的可用資料存放區數量有限。 如果您嘗試建立的資料儲存空間多於可用資料， [!DNL Workfront] 傳回a [!UICONTROL 已達到最大儲存] 錯誤。
>
>如需詳細資訊，請參閱 [達到的最大儲存錯誤](#maximum-stores-reached-error) 這篇文章。

1. 登入 [!DNL Workfront Fusion] 帳戶。
1. 按一下 **[!UICONTROL 資料儲存]** ，即可取得Advertising Cloud的說明。
1. 按一下 **[!UICONTROL 新增資料存放區]** 在螢幕的右上角。
1. 輸入新資料儲存的設定。

   中欄位的粗體標題 [!DNL Workfront Fusion] 模組指示所需的設定。

   <table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td>[!UICONTROL資料儲存名] </td> 
      <td> <p>輸入資料儲存的名稱。 </p> </td> 
     </tr> 
     <tr> 
      <td> <p>[!UICONTROL資料結構]</p> </td> 
      <td> <p>資料結構是表的列清單。 此清單指示列名和資料類型。</p> <p>執行下列任一項作業：</p> 
       <ul> 
        <li style="font-weight: bold;">選擇已建立的資料結構</li> 
        <li> <p style="font-weight: bold;">新增資料結構</p> <p>按一下 <strong>[!UICONTROL添加]</strong> 來建立新資料結構。</p> <p>如需詳細資訊，請參閱 <a href="#set-up-the-data-structure" class="MCXref xref">設定資料結構</a> 一節。</p> </li> 
        <li style="font-weight: bold;"> <p>將欄位留空</p> <p style="font-weight: normal;">如果您未選擇或添加資料結構，則資料庫將僅包含主鍵。 如果只想保存密鑰，並且只想知道資料庫中是否存在特定密鑰，則這種資料庫類型非常有用。</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td> <p>[!UICONTROL資料儲存大小(MB)]</p> </td> 
      <td> <p>從內部資料儲存總量中分配資料儲存的大小。</p> <p>注意：可隨時更改保留金額。</p>  </td> 
     </tr> 
    </tbody> 
   </table>

### 設定資料結構

1. 建立或編輯資料存放區時，按一下 **[!UICONTROL 新增]**.
1. 在 **[!UICONTROL 新增資料結構]** 框中，配置以下欄位：

   <table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td>[!UICONTROL資料結構名稱]</td> 
      <td> <p> 輸入新資料結構的名稱。</p> </td> 
     </tr> 
     <tr> 
      <td> <p>[!UICONTROL規範]</p> </td> 
      <td> <p>執行下列任一操作來設定資料儲存的欄。</p> 
       <ul> 
        <li> <p>按一下 <strong>[!UICONTROL添加項]</strong> 手動指定一列的屬性。</p> <p>輸入 <strong>[!UICONTROL名稱]</strong> 和 <strong>[!UICONTROL類型]</strong> 對於資料儲存欄，並定義對應的屬性。</p> </li> 
        <li> <p>按一下 <strong>[!UICONTROL生成器]</strong> 以決定您提供之範例資料的欄。</p> 
         <div class="example" data-mc-autonum="<b>Example: </b>">
          <span class="autonumber"><span><b>範例: </b></span></span> 
          <p>例如，下列JSON範例資料會建立三欄：姓名、年齡和電話號碼。 電話號碼是行動電話和固定電話號碼的集合。</p> 
          <p><code>&lbrace;</code> </p> 
          <p><code>"name":"John",</code> </p> 
          <p><code>"age":30,</code> </p> 
          <p><code>"phone number": &lbrace;</code> </p> 
          <p><code>"mobile":"987654321",</code> </p> 
          <p><code>"landline":"123456789"</code> </p> 
          <p><code>&rbrace;</code> </p> 
          <p><code>&rbrace;</code> </p> 
          <p>資料儲存檢視中的空白欄：</p> 
          <p> <img src="assets/empty-columns-350x132.png" style="width: 350;height: 132;"> </p> 
          <p>然後，您可以手動或使用 [!DNL Workfront Fusion] 資料儲存模組。</p> 
         </div> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL嚴格] </td> 
      <td> <p>啟用此選項可確保裝載符合資料結構。 包含未在資料結構中指定之額外項目的裝載會被拒絕。</p> </td> 
     </tr> 
    </tbody> 
   </table>

## 編輯現有資料儲存區

您可以在 [!UICONTROL 資料儲存] 區域 [!DNL Workfront Fusion].

* [編輯資料儲存的屬性](#edit-the-properties-of-a-data-store)
* [編輯資料儲存的內容](#edit-the-contents-of-a-data-store)

### 編輯資料儲存的屬性

資料儲存的屬性包括資料儲存所使用的資料結構以及資料儲存的大小。

1. 按一下 **[!UICONTROL 資料儲存]** ![](assets/data-store-icon.png) ，開啟 [!UICONTROL 資料儲存] 的上界。
1. 按一下 **[!UICONTROL 編輯]** ![](assets/data-store-edit.png) 旁邊。
1. （可選）如果要將此資料儲存所使用的資料結構更改為其他現有資料結構，請從 **[!UICONTROL 資料結構]** 下拉式清單。

   或

   （可選）如果要將此資料儲存區使用的資料結構更改為全新的資料結構，請參閱 [設定資料結構](#set-up-the-data-structure) 這篇文章。

1. （選用）將新大小輸入 **[!UICONTROL 資料儲存大小(MB)]** 欄位。
1. 按一下&#x200B;**[!UICONTROL 儲存]**。

### 編輯資料儲存的內容

1. 按一下 **[!UICONTROL 資料儲存]** 圖示 ![](assets/data-store-icon.png) ，開啟 [!UICONTROL 資料儲存] 的上界。
1. 按一下 **[!UICONTROL 瀏覽]** ![](assets/browse-data-store.png) 旁邊。
1. （選用）將欄拖曳至所需位置以重新排序欄。
1. （可選） [!UICONTROL 編輯] 按一下 **[!UICONTROL 編輯]** 圖示 ![](assets/data-store-edit.png)，然後輸入所需值。
1. （選用）按一下「 」，將新項目新增至資料存放區 **[!UICONTROL 新增]**，然後輸入新項的資訊。
1. 按一下&#x200B;**[!UICONTROL 儲存]**。

## 疑難排解

* [從資料儲存中恢復丟失的資料](#restoring-lost-data-from-a-data-store)
* [空間不足錯誤](#out-of-space-error)
* [達到的最大儲存錯誤](#maximum-stores-reached-error)

### 從資料儲存中恢復丟失的資料

目前沒有可以自動還原丟失資料的工具。

#### 因應措施

1. 檢查項目插入資料存放區的所有執行記錄。

   有關檢查執行日誌的詳細資訊，請參閱 [在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-scenario-execution-history.md).

1. 複製資料。
1. 再次將資料插入您的資料存放區。

   有關將資料插入資料儲存區的資訊，請參見 [編輯資料儲存的內容](#edit-the-contents-of-a-data-store) 這篇文章。

### [!UICONTROL 空間不足] 錯誤

安 [!UICONTROL 空間不足] 發生錯誤，因為先前建立的資料儲存區已指派給您已分配的資料儲存區儲存區。

#### 因應措施

1. 編輯任何現有資料存放區，以使用較少的空間。 這樣可騰出空間存放新資料。

   如需詳細資訊，請參閱 [編輯資料儲存的屬性](#edit-the-properties-of-a-data-store) 這篇文章。

>[!NOTE]
>
>建議您不要將所有空間指派給單一資料存放區，除非您確定不需要更多資料存放區。

### [!UICONTROL 已達到最大儲存] 錯誤

A [!UICONTROL 已達到最大儲存] 發生錯誤是因為您的組織已使用其所有可用資料儲存。 組織的可用資料儲存數量等於可用方案數量的兩倍。 因此，可用資料存放區的總數取決於您購買的計畫。

例如，如果您的組織已購買含15個藍本的計畫，則組織最多可以有30個資料儲存區。

#### 因應措施

若要減少現有資料存放區的數量，請考慮執行下列其中一項操作：

* 結合現有資料存放區
* 刪除未使用的資料儲存
