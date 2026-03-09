---
product-area: requests
navigation-topic: create-and-manage-request-queues
title: 建立專案輸入Forms
description: 您可以使用專案錄取表單來簡化在Workfront中建立專案的流程
author: Alina
feature: Work Management, Requests
role: User, Admin
hide: true
hidefromtoc: true
source-git-commit: e4d57d0b5042dc4889d5b676396b56c05ab1515d
workflow-type: tm+mt
source-wordcount: '1329'
ht-degree: 2%

---

# 建立專案錄取表單

<span class="preview">此頁面上的資訊是指尚未普遍提供的功能。 它僅在預覽環境中可供所有客戶使用。 每月發行至生產環境後，生產環境中為啟用快速發行的客戶也提供相同的功能。</span>

<span class="preview">如需快速發行資訊，請參閱[為您的組織啟用或停用快速發行](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>

專案輸入表單是一種請求表單，可讓使用者請求專案。 專案是從表單建立的，不需要從提交的問題建立專案。

## 存取權要求

+++ 展開以檢視這篇文章中所述功能的存取權要求。

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td> <p>任何 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td> 
   <p>新授權： Standard </p>
   或
   <p>目前授權：計畫 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>您必須是Workfront管理員才能建立專案錄取表單。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">其他產品</td> 
   <td> <p>貴組織必須已購買Workfront Planning才能使用自動化等Planning功能。</p> </td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 專案輸入Forms的功能和限制

### 功能

專案錄取表單包含下列功能：

#### Workfront規劃自動化

Workfront專案輸入表單支援Workfront規劃自動化，可設定已建立之專案特定的屬性。

如需Planning自動化的詳細資訊，請參閱[設定Adobe Workfront Planning自動化](/help/quicksilver/planning/records/configure-automations-to-create-records.md)。

### 核准設定

專案錄取表單包括設定已提交請求的核准者的功能。

### 限制

#### 支援的欄位型別

專案輸入Forms可以包含任何具有專案物件型別的自訂表單中的欄位。

專案輸入Forms目前不支援下列欄位型別：

* 區域
* 公式
* 統計
* 單行統計
* 規劃連線
* 參考專案原生欄位（唯讀）的原生欄位參考（例如，`workRequiredExpression`）

#### 要求體驗

專案錄取表單只能用於新的請求體驗。

如需有關新請求體驗的資訊，請參閱[建立及提交請求](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md)。

#### 共用

專案接收表單不支援公開共用。 共用選項包括：

* **任何人**：系統中的任何人都可以使用表單來提交專案請求。
* **指定的使用者**：您可以選取哪些特定使用者可以存取專案申請表單。

## 建立專案錄取表單

{{step1-to-requests}}

1. 啟用熒幕右上角的&#x200B;**切換至新的體驗**&#x200B;設定。
1. 按一下畫面右上角的&#x200B;**要求表單**。

   >[!NOTE]
   >
   >由於只有Workfront管理員可以建立錄取表單，因此請求表單按鈕僅對管理員可見。

   目前可用的請求表單清單隨即顯示。 這包括Workfront Planning的請求表單。

1. 按一下畫面右上角的&#x200B;**新要求表單**。
1. 輸入申請表單的名稱。 依預設，表單的名稱是&#x200B;**未命名的表單**。
1. 選取下拉式清單頂端附近的物件型別&#x200B;**專案**。 這是目前唯一可用的Workfront專案型別。 清單中的其他專案屬於Workfront Planning。
1. （選用）為要求表單新增&#x200B;**描述**。
1. 按一下 **建立**。所選記錄型別的請求表單會在「表單」標籤中開啟。

   專案錄取表單產生器會開啟至表單索引標籤。

   依預設，輸入表單包含下列資訊：

   * **預設的分節**：這是Workfront套用至要求表單的預設分割槽符號。 所有記錄欄位都顯示在&#x200B;**預設區段**&#x200B;區域。
   * **主旨**&#x200B;欄位：將在Workfront中識別要求的欄位。 主旨欄位的設定和值無法編輯。
   * 與專案關聯的所有欄位。

     提交專案請求的每個人均可看見請求表單中包含的欄位。

1. 若要新增欄位至表單，請按一下左側導覽中的欄位型別，然後選取欄位。
1. （選擇性）若要移除欄位，請將游標移至您要移除之表單上的欄位上，然後按一下&#x200B;**x**&#x200B;圖示以移除該欄位。
1. （選擇性）若要從表單中移除&#x200B;**預設區段**，請執行下列動作：

   1. 從預設區段中移除所有欄位。
   1. 按一下&#x200B;**Content elements**&#x200B;索引標籤並新增區段，然後新增區段的名稱。
   1. 新增欄位至新區段。
   1. 按一下&#x200B;**x**&#x200B;圖示以移除&#x200B;**預設區段**。
1. 按一下任何欄位，然後使用表單右側面板中的控制項來定義其大小或下列任何資訊：

   * **標籤**：這是欄位在要求表單上顯示的名稱。 這不會變更記錄欄位的名稱。
   * **指示**：新增欄位的詳細資訊。
   * **建立必要欄位**：選取時，該欄位必須具有值。 否則，無法提交表單。
   * **新增邏輯**：定義必須符合哪些條件才能顯示或隱藏欄位。

   >[!TIP]
   >
   >   在表單上選取欄位後，每個欄位的欄位型別都會顯示在右側面板的頂端。
   >     

1. （選擇性）按一下表單左側的&#x200B;**Content elements**&#x200B;標籤，然後新增下列任一元素：

   * **描述文字**
   * **分割槽符號**

   如需建立自訂表單的詳細資訊，請參閱[建立自訂表單](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)。

1. 按一下表單左側的&#x200B;**自動化**&#x200B;標籤，然後執行下列任一動作：

   * 選取專案範本
   * 附加任何自訂表格
   * 設定專案所有者
   * 將專案新增至投資組合或方案

   您在此處所做的任何選取都將套用至從此輸入表單建立的專案。

1. （選擇性）按一下&#x200B;**預覽**&#x200B;以檢視其他使用者使用表單提交新記錄時表單的顯示方式。

1. （選擇性）按一下&#x200B;**組態**&#x200B;標籤，然後新增至少一位使用者或團隊&lt;&lt;至&#x200B;**核准者**&#x200B;欄位，以核准此錄取表單的新要求。

   * 將輸入表單與核准者建立關聯時，任何新請求都必須先由所有核准者核准，才能產生專案。
   * 您可以將一個或多個核准者新增至輸入表單。
   * 如果至少有一位核准者拒絕該請求，則請求會遭到拒絕，且不會建立專案。
   * 在核准或拒絕專案之前，所有核准者都必須做出決定。
   * 如果團隊被設定為核准者，則只需從團隊中做出一個決定。

     如需新增核准至請求表單的詳細資訊，請參閱[新增核准至請求表單](/help/quicksilver/planning/requests/add-approval-to-request-form.md)。

1. （選擇性）按一下標題中表單名稱右側的&#x200B;**更多**&#x200B;功能表![更多功能表](assets/more-menu.png)，然後按一下&#x200B;**編輯**&#x200B;以更新表單名稱。

1. 按一下&#x200B;**發佈**&#x200B;以發佈表單並取得其唯一連結。

   會發生下列情況：

   * **發佈**&#x200B;按鈕已移除。
   * **取消發佈**&#x200B;按鈕已新增至表單。 按一下此按鈕，表單將無法存取。
   * **共用**&#x200B;按鈕已新增至表單。
   * 此表單將在Workfront主要功能表的請求區域中變得可用。

1. 按一下&#x200B;**共用**&#x200B;以與其他人共用表單。
1. 按一下頁首中表單名稱左側的向左箭頭以關閉表單。

   **請求表單**&#x200B;表格檢視會開啟，並將表單新增至其中。

1. （選擇性）暫留在表格檢視中的要求表單名稱上，然後按一下表單名稱右側的&#x200B;**更多**&#x200B;功能表![更多](assets/more-menu.png)，然後按一下下列其中一項：

   * **編輯表單**：按一下以進一步編輯表單上的資訊。
   * **取消發佈**：按一下以取消發佈表單，該表單會從Workfront的要求區域移除它。
   * **共用**：按一下此以修改誰可以存取表單。
   * **複製連結**：按一下此以快速複製要求表單的連結，而不開啟表單。
   * **刪除**：按一下以刪除表單。 使用表單新增的所有請求和記錄都不會刪除。 無法復原表單。

   >[!NOTE]
   >
   >您可以在表格檢視中識別專案輸入表單，因為它們會在「物件型別」欄中顯示「專案」。

1. 按一下標題中&#x200B;**要求表單**&#x200B;左側的向左箭頭，關閉要求表單表格。

