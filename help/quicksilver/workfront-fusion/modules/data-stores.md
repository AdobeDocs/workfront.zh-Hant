---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: ' [!DNL Adobe Workfront Fusion]中的資料存放區'
description: 資料存放區（類似於資料庫或簡單表格）可以儲存情境中的資料，以便在個別情境或情境執行之間傳輸資料。 您可以在同步期間使用資料存放區來儲存來自不同系統的新資料。
author: Becky
feature: Workfront Fusion
exl-id: 2a665a71-b819-4861-b119-f5c28b87e9c5
source-git-commit: 00a969175626d27b70d516921097725fdf818799
workflow-type: tm+mt
source-wordcount: '1336'
ht-degree: 1%

---

# [!DNL Adobe Workfront Fusion]中的資料存放區

資料存放區（類似於資料庫或簡單表格）可以儲存情境中的資料，以便在個別情境或情境執行之間傳輸資料。 您可以在同步期間使用資料存放區來儲存來自不同系統的新資料。

資料存放區模組可讓您對[!DNL Adobe Workfront Fusion]資料存放區中的記錄執行下列動作：

* 新增
* 取代
* 更新
* 擷取
* 刪除
* 搜尋
* 計數

如需有關使用資料存放區模組的資訊，請參閱[[!UICONTROL 資料存放區]模組](../../workfront-fusion/apps-and-their-modules/data-store-modules.md)。

如需有關Workfront Fusion中資料存放區的影片簡介，請參閱：

* [資料存放區](https://video.tv.adobe.com/v/3427029/){target=_blank}

## 存取需求

您必須具有下列存取權才能使用本文中的功能：

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計劃</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權</td> 
   <td> <p>新增：[！UICONTROL Standard]</p><p>或</p><p>目前： [！UICONTROL Work]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] 授權**</td> 
   <td>
   <p>目前：無[!DNL Workfront Fusion]授權需求。</p>
   <p>或</p>
   <p>舊版：任何 </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>
   <p>新增：</p> <ul><li>[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Workfront]計畫：您的組織必須購買[!DNL Adobe Workfront Fusion]。</li><li>已包含[！UICONTROL Ultimate] [!DNL Workfront]計畫： [!DNL Workfront Fusion]。</li></ul>
   <p>或</p>
   <p>目前：您的組織必須購買[!DNL Adobe Workfront Fusion]。</p>
   </td> 
  </tr>
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

如需[!DNL Adobe Workfront Fusion]授權的相關資訊，請參閱[[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md)。

## 可用的資料空間

<!--If your organization is on the new Workfront plan model (Select, Prime, and Ultimate packages), your total data store size is:-->

如果您的組織使用新的Workfront計畫模型（Select、Prime和Ultimate套件），則組織的計畫會影響您的Fusion執行個體可用的資料儲存大小和數量。

### Ultimate計畫

Ultimate套件上的Fusion執行個體會收到：

* 100 MB的空間
* 50個資料存放區

### 選取和主要計畫

Select或Prime套件上的Fusion執行個體會收到：—>

* 第一個500K作業為100 MB。

* 每個額外的100,000作業為10 MB。

  例如，擁有600K作業的組織會收到110 MB。

您的組織最多可以擁有50個資料存放區。 這些資料存放區的合併大小不得超過您組織的資料存放區總大小。

## 在[!DNL Workfront Fusion]中建立資料存放區

* [設定資料存放區](#set-up-the-data-store)
* [設定資料結構](#set-up-the-data-structure)

### 設定資料存放區

您必須先在[!DNL Workfront Fusion]中建立資料存放區，才能在模組中使用資料存放區。

>[!NOTE]
>
>您的組織可用的資料存放區數量有限。 如果您嘗試建立的資料存放區超過可用的數目，[!DNL Workfront]會傳回[!UICONTROL 已達最大存放區數]個錯誤。
>
>如需詳細資訊，請參閱本文中的[最大存放區數量已達錯誤](#maximum-stores-reached-error)。

1. 登入您的[!DNL Workfront Fusion]帳戶。
1. 按一下左側導覽面板中的&#x200B;**[!UICONTROL 資料存放區]**。
1. 按一下熒幕右上角的&#x200B;**[!UICONTROL 新增資料存放區]**。
1. 輸入新資料存放區的設定。

   [!DNL Workfront Fusion]模組中欄位上的粗體標題表示必要設定。

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
      <td> <p>資料結構是表格的欄清單。 此清單指示欄名稱和資料型別。</p> <p>執行下列其中一項：</p> 
       <ul> 
        <li style="font-weight: bold;">選取已建立的資料結構</li> 
        <li> <p style="font-weight: bold;">新增資料結構</p> <p>按一下<strong>[！UICONTROL新增]</strong>以建立新的資料結構。</p> <p>如需詳細資訊，請參閱本文中的<a href="#set-up-the-data-structure" class="MCXref xref">設定資料結構</a>一節。</p> </li> 
        <li style="font-weight: bold;"> <p>將此欄位留空</p> <p style="font-weight: normal;">如果您未選取或新增資料結構，資料庫將僅包含主索引鍵。 如果您只想儲存金鑰，而且只想知道資料庫中是否存在特定金鑰，這種資料庫型別就相當實用。</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td> <p>[！UICONTROL資料儲存大小(MB)</p> </td> 
      <td> <p>從您的內部資料儲存總量中配置資料儲存的大小。</p> <p> 預設值為10 MB。 如果您的95 MB配置中有10 MB以下的未配置資料存放區空間，預設大小為未配置存放區的數量。  <p>備註：預留金額可隨時變更。</p>  </td> 
     </tr> 
    </tbody> 
   </table>

### 設定資料結構

1. 建立或編輯資料存放區時，請按一下[新增]。****
1. 在顯示的&#x200B;**[!UICONTROL 新增資料結構]**&#x200B;方塊中，設定下列欄位：

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
      <td> <p>執行下列任一項作業來設定資料存放區的欄。</p> 
       <ul> 
        <li> <p>按一下<strong>[！UICONTROL新增專案]</strong>以手動指定一欄的屬性。</p> <p>輸入資料儲存欄位的<strong>[！UICONTROL名稱]</strong>和<strong>[！UICONTROL型別]</strong>，並定義對應的屬性。</p> </li> 
        <li> <p>按一下<strong>[！UICONTROL Generator]</strong>，從您提供的範例資料中決定資料行。</p> 
         <div class="example" data-mc-autonum="<b>Example: </b>">
          <span class="autonumber"><span><b>範例： </b></span></span> 
          <p>例如，以下JSON範例資料會建立三欄：名稱、年齡和電話號碼。 電話號碼是行動電話和有線電話的集合。</p> 
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
          <p>然後，您可以手動或使用[!DNL Workfront Fusion]資料存放區模組，將值新增至資料存放區。</p> 
         </div> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td>[！UICONTROL嚴格] </td> 
      <td> <p>啟用此選項以確保承載符合資料結構。 包含資料結構中未指定之額外專案的裝載會被拒絕。</p> </td> 
     </tr> 
    </tbody> 
   </table>

## 編輯現有的資料存放區

您可以在[!DNL Workfront Fusion]的[!UICONTROL 資料存放區]區域中編輯現有資料存放區的屬性和內容。

* [編輯資料存放區的屬性](#edit-the-properties-of-a-data-store)
* [編輯資料存放區的內容](#edit-the-contents-of-a-data-store)

### 編輯資料存放區的屬性

資料存放區的屬性包含資料存放區使用的資料結構，以及資料存放區的大小。

1. 按一下左側導覽面板中的&#x200B;**[!UICONTROL 資料存放區]** ![](assets/data-store-icon.png)以開啟[!UICONTROL 資料存放區]區域。
1. 按一下您要編輯的資料存放區旁的&#x200B;**[!UICONTROL 編輯]** ![](assets/data-store-edit.png)。
1. （選擇性）如果要將此資料存放區使用的資料結構變更為其他現有的資料結構，請從&#x200B;**[!UICONTROL 資料結構]**&#x200B;下拉式清單中選取它。

   或

   （選擇性）如果您想要將此資料存放區使用的資料結構變更為全新的資料結構，請參閱本文中的[設定資料結構](#set-up-the-data-structure)。

1. （選擇性）在&#x200B;**[!UICONTROL 資料儲存大小（以MB]**&#x200B;為單位）欄位中輸入新大小，以變更資料儲存的大小。
1. 按一下「**[!UICONTROL 儲存]**」。

### 編輯資料存放區的內容

1. 按一下左側導覽面板中的&#x200B;**[!UICONTROL 資料存放區]**&#x200B;圖示![](assets/data-store-icon.png)，以開啟[!UICONTROL 資料存放區]區域。
1. 按一下您要編輯的資料存放區旁的&#x200B;**[!UICONTROL 瀏覽]**。
1. （選用）將欄拖曳至所需位置以重新排序。
1. （選擇性）按一下單一儲存格中的&#x200B;**[!UICONTROL 編輯]**&#x200B;圖示，然後輸入所要的值，以編輯[!UICONTROL 該儲存格。]
1. （選擇性）按一下&#x200B;**[!UICONTROL 新增]**，然後輸入新專案的資訊，以新增專案至資料存放區。
1. 按一下「**[!UICONTROL 儲存]**」。

## 疑難排解

* [從資料存放區還原遺失的資料](#restoring-lost-data-from-a-data-store)
* [空間不足錯誤](#out-of-space-error)
* [已達到最大存放區數錯誤](#maximum-stores-reached-error)

### 從資料存放區還原遺失的資料

目前沒有工具可自動還原遺失的資料。

#### 因應措施

1. 檢查將專案插入資料存放區之案例的所有執行記錄。

   如需檢查執行記錄的詳細資訊，請參閱[在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-scenario-execution-history.md)中檢視案例的執行記錄。

1. 複製資料。
1. 再次將資料插入您的資料存放區。

   如需有關將資料插入資料存放區的資訊，請參閱本文中的[編輯資料存放區的內容](#edit-the-contents-of-a-data-store)。

### [!UICONTROL 空間不足]錯誤

發生[!UICONTROL 空間不足]錯誤，因為先前建立的資料存放區已指派給您配置的資料存放區存放區。

#### 因應措施

1. 編輯任何現有資料存放區，以使用較少空間。 這可釋放空間給新資料存放區。

   如需詳細資訊，請參閱本文中的[編輯資料存放區的屬性](#edit-the-properties-of-a-data-store)。

>[!NOTE]
>
>建議您不要將所有空間指派給單一資料存放區，除非您確定不需要更多資料存放區。

### [!UICONTROL 最大存放區數達到]個錯誤

發生[!UICONTROL 最大存放區數量達到]個錯誤，因為您的組織已使用其所有可用的資料存放區。 組織有許多可用資料存放區，其數量等於可用案例數量的兩倍。 因此，可用資料儲存的總數取決於您購買的計畫。

例如，如果您的組織已購買包含15種情境的計畫，則組織最多可以有30個資料存放區。

#### 因應措施

若要減少現有資料存放區的數量，請考慮執行下列任一項作業：

* 合併現有資料存放區
* 刪除未使用的資料存放區
