---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: 中的資料存放區 [!DNL Adobe Workfront Fusion]
description: 資料存放區（類似於資料庫或簡單表格）可以儲存情境中的資料，以便在個別情境或情境執行之間傳輸資料。 您可以在同步期間使用資料存放區來儲存來自不同系統的新資料。
author: Becky
feature: Workfront Fusion
exl-id: 2a665a71-b819-4861-b119-f5c28b87e9c5
source-git-commit: 8b4182ae2b32488a02cacc16fcb6a246fcb571fd
workflow-type: tm+mt
source-wordcount: '1224'
ht-degree: 1%

---

# 中的資料存放區 [!DNL Adobe Workfront Fusion]

資料存放區（類似於資料庫或簡單表格）可以儲存情境中的資料，以便在個別情境或情境執行之間傳輸資料。 您可以在同步期間使用資料存放區來儲存來自不同系統的新資料。

資料存放區模組可讓您對中的記錄執行以下操作 [!DNL Adobe Workfront Fusion] 資料存放區：

* 新增
* 取代
* 更新
* 擷取
* 刪除
* 搜尋
* 計數

如需使用資料存放區模組的詳細資訊，請參閱 [[!UICONTROL 資料存放區] 模組](../../workfront-fusion/apps-and-their-modules/data-store-modules.md).

## 存取需求

您必須具有下列存取權才能使用本文中的功能：

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
   <td> <p>[！UICONTROL計畫]，[！UICONTROL工作]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Adobe Workfront Fusion]授權**</td> 
   <td>
   <p>目前授權需求：否 [!DNL Workfront Fusion] 授權需求。</p>
   <p>或</p>
   <p>舊版授權需求： [！UICONTROL [!DNL Workfront Fusion] 適用於工作自動化與整合] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>
   <p>目前產品需求：如果您有[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Adobe Workfront] 計畫，您的組織必須購買 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文所述功能。 [!DNL Workfront Fusion] 包含在[！UICONTROL Ultimate]中 [!DNL Workfront] 計畫。</p>
   <p>或</p>
   <p>舊版產品需求：貴組織必須購買 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文所述功能。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

若要瞭解您擁有哪些計畫、授權型別或存取權，請聯絡您的 [!DNL Workfront] 管理員。

有關以下專案的資訊： [!DNL Adobe Workfront Fusion] 授權，請參閱 [[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 在中建立資料存放區 [!DNL Workfront Fusion]

* [設定資料存放區](#set-up-the-data-store)
* [設定資料結構](#set-up-the-data-structure)

### 設定資料存放區

您必須先在中建立資料存放區，才能在模組中使用資料存放區 [!DNL Workfront Fusion].

>[!NOTE]
>
>您的組織可用的資料存放區數量有限。 如果您嘗試建立的資料存放區超過可用數量， [!DNL Workfront] 傳回 [!UICONTROL 已達到最大存放區] 錯誤。
>
>如需詳細資訊，請參閱 [已達到最大存放區數錯誤](#maximum-stores-reached-error) 本文章內容。

1. 登入您的 [!DNL Workfront Fusion] 帳戶。
1. 按一下 **[!UICONTROL 資料存放區]** ，位於左側導覽面板中。
1. 按一下 **[!UICONTROL 新增資料存放區]** 在熒幕的右上角。
1. 輸入新資料存放區的設定。

   中的欄位上的粗體標題 [!DNL Workfront Fusion] 模組會指出必要的設定。

   <table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td>[！UICONTROL資料存放區名稱] </td> 
      <td> <p>輸入資料存放區的名稱。 </p> </td> 
     </tr> 
     <tr> 
      <td> <p>[！UICONTROL資料結構]</p> </td> 
      <td> <p>資料結構是表格的欄清單。 此清單會指出欄名稱和資料型別。</p> <p>執行下列任一項作業：</p> 
       <ul> 
        <li style="font-weight: bold;">選取已建立的資料結構</li> 
        <li> <p style="font-weight: bold;">新增資料結構</p> <p>按一下 <strong>[！UICONTROL新增]</strong> 以建立新的資料結構。</p> <p>如需詳細資訊，請參閱 <a href="#set-up-the-data-structure" class="MCXref xref">設定資料結構</a> 章節。</p> </li> 
        <li style="font-weight: bold;"> <p>將欄位留空</p> <p style="font-weight: normal;">如果您未選取或新增資料結構，資料庫將僅包含主索引鍵。 如果您只想儲存金鑰，而且只想知道資料庫中是否存在特定金鑰，這種資料庫型別就很實用。</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td> <p>[！UICONTROL資料儲存大小(MB)</p> </td> 
      <td> <p>從您的內部資料儲存總量中配置資料儲存的大小。</p> <p>備註：預留金額可隨時變更。</p>  </td> 
     </tr> 
    </tbody> 
   </table>

### 設定資料結構

1. 建立或編輯資料存放區時，按一下 **[!UICONTROL 新增]**.
1. 在 **[!UICONTROL 新增資料結構]** 方塊中，設定下列欄位：

   <table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td>[！UICONTROL資料結構名稱]</td> 
      <td> <p> 輸入新資料結構的名稱。</p> </td> 
     </tr> 
     <tr> 
      <td> <p>[！UICONTROL規格]</p> </td> 
      <td> <p>執行下列任一項作業，設定資料存放區的欄。</p> 
       <ul> 
        <li> <p>按一下 <strong>[！UICONTROL新增專案]</strong> 以手動指定一欄的屬性。</p> <p>輸入 <strong>[！UICONTROL名稱]</strong> 和 <strong>[！UICONTROL型別]</strong> ，並定義對應的屬性。</p> </li> 
        <li> <p>按一下 <strong>[！UICONTROL Generator]</strong> 以從您提供的範例資料中決定欄。</p> 
         <div class="example" data-mc-autonum="<b>Example: </b>">
          <span class="autonumber"><span><b>範例: </b></span></span> 
          <p>例如，以下JSON範例資料會建立三欄：姓名、年齡和電話號碼。 電話號碼是行動電話和有線電話號碼的集合。</p> 
          <p><code>&lbrace;</code> </p> 
          <p><code>"name":"John",</code> </p> 
          <p><code>"age":30,</code> </p> 
          <p><code>"phone number": &lbrace;</code> </p> 
          <p><code>"mobile":"987654321",</code> </p> 
          <p><code>"landline":"123456789"</code> </p> 
          <p><code>&rbrace;</code> </p> 
          <p><code>&rbrace;</code> </p> 
          <p>資料存放區檢視中的空白欄：</p> 
          <p> <img src="assets/empty-columns-350x132.png" style="width: 350;height: 132;"> </p> 
          <p>然後，您可以手動或使用將值新增至資料存放區 [!DNL Workfront Fusion] 資料存放區模組。</p> 
         </div> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td>[！UICONTROL嚴格] </td> 
      <td> <p>啟用此選項以確保裝載符合資料結構。 包含未在資料結構中指定之額外專案的裝載會遭到拒絕。</p> </td> 
     </tr> 
    </tbody> 
   </table>

## 編輯現有的資料存放區

您可以在下列位置編輯現有資料存放區的屬性和內容： [!UICONTROL 資料存放區] 區域 [!DNL Workfront Fusion].

* [編輯資料存放區的屬性](#edit-the-properties-of-a-data-store)
* [編輯資料存放區的內容](#edit-the-contents-of-a-data-store)

### 編輯資料存放區的屬性

資料存放區的屬性包含資料存放區使用的資料結構，以及資料存放區的大小。

1. 按一下 **[!UICONTROL 資料存放區]** ![](assets/data-store-icon.png) 在左側導覽面板中開啟 [!UICONTROL 資料存放區] 區域。
1. 按一下 **[!UICONTROL 編輯]** ![](assets/data-store-edit.png) ，位於您要編輯的資料存放區旁。
1. （可選）如果要將此資料存放區使用的資料結構變更為其他現有資料結構，請從 **[!UICONTROL 資料結構]** 下拉式清單。

   或

   （選用）如果要將此資料存放區使用的資料結構變更為全新的資料結構，請參閱 [設定資料結構](#set-up-the-data-structure) 本文章內容。

1. （可選）將新大小輸入至以變更資料存放區的大小 **[!UICONTROL 資料儲存大小(MB)]** 欄位。
1. 按一下&#x200B;**[!UICONTROL 儲存]**。

### 編輯資料存放區的內容

1. 按一下 **[!UICONTROL 資料存放區]** 圖示 ![](assets/data-store-icon.png) 在左側導覽面板中開啟 [!UICONTROL 資料存放區] 區域。
1. 按一下 **[!UICONTROL 瀏覽]**  ，位於您要編輯的資料存放區旁。
1. （選用）將欄拖曳至所需位置以重新排序。
1. （可選） [!UICONTROL 編輯] 按一下 **[!UICONTROL 編輯]** 圖示填入，然後輸入所需的值。
1. （選用）按一下「 」，將新專案新增至資料存放區 **[!UICONTROL 新增]**，然後輸入新專案的資訊。
1. 按一下&#x200B;**[!UICONTROL 儲存]**。

## 疑難排解

* [從資料存放區還原遺失的資料](#restoring-lost-data-from-a-data-store)
* [空間不足錯誤](#out-of-space-error)
* [已達到最大存放區數錯誤](#maximum-stores-reached-error)

### 從資料存放區還原遺失的資料

目前沒有工具可自動還原遺失的資料。

#### 因應措施

1. 檢查將專案插入資料存放區之案例的所有執行記錄。

   如需檢查執行記錄的詳細資訊，請參閱 [在中檢視案例的執行歷史記錄 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-scenario-execution-history.md).

1. 複製資料。
1. 再次將資料插入您的資料存放區。

   如需將資料插入資料存放區的詳細資訊，請參閱 [編輯資料存放區的內容](#edit-the-contents-of-a-data-store) 本文章內容。

### [!UICONTROL 空間不足] 錯誤

一個 [!UICONTROL 空間不足] 發生錯誤，因為先前建立的資料存放區已指派給您配置的資料存放區存放區。

#### 因應措施

1. 編輯任何現有資料存放區，以使用較少空間。 這可釋放空間給您的新資料存放區。

   如需詳細資訊，請參閱 [編輯資料存放區的屬性](#edit-the-properties-of-a-data-store) 本文章內容。

>[!NOTE]
>
>建議您不要將所有空間指派給單一資料存放區，除非您確定不需要更多資料存放區。

### [!UICONTROL 已達到最大存放區] 錯誤

A [!UICONTROL 已達到最大存放區] 發生錯誤是因為您的組織已使用其所有可用的資料存放區。 組織有許多可用資料存放區，其數量等於可用案例數量的兩倍。 因此，可用資料存放區的總數取決於您購買的計畫。

例如，如果貴組織已購買包含15種情境的計畫，則組織最多可擁有30個資料存放區。

#### 因應措施

若要減少現有資料存放區的數量，請考慮執行下列任一項作業：

* 合併現有資料存放區
* 刪除未使用的資料存放區
