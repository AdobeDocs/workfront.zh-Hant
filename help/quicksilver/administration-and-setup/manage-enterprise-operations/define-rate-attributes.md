---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-locations
title: 定義費率屬性
description: 費率屬性可讓您新增其他維度至工作角色以外的費率，藉以擴充Adobe Workfront的費率卡和費率功能。 接著Workfront可以自動選取指派的正確比率，確保財務正確性及跨專案的一致性。
author: Lisa
feature: System Setup and Administration
role: Admin
source-git-commit: 8e948d1c90a9d528c7ffd4963e14630ae7577e70
workflow-type: tm+mt
source-wordcount: '1378'
ht-degree: 1%

---


# 定義費率屬性

{{highlighted-preview-article-level}}

費率屬性可讓您新增其他維度至工作角色以外的費率，藉以擴充Adobe Workfront的費率卡和費率功能。 這對於機構與企業而言至關重要，因為費率不僅會因工作角色而有所不同，也會因機構、地點、品牌、成本中心或其他因素而有所不同。
結合這些屬性，Workfront可以自動選取指派的正確費率，確保財務正確性及跨專案的一致性。

>[!IMPORTANT]
>
>費率屬性是單次的基本設定。

一旦啟用屬性並套用至費率卡和費率後，稍後變更它們可能會危害您整個財務設定的資料完整性。

## 費率屬性概要

費率屬性會被視為一次性設定，因為：

* 屬性一旦啟用，就會成為財務資料模型的一部分。
* 費率、指派、計畫值及實際值都取決於所選的屬性值。
* 稍後變更屬性（重新命名、移除或重新排序）可能會導致：

   * 費率與屬性之間失去連結
   * 無效或「孤立」費率
   * 帳單和報告中的不一致

基於這些原因，屬性在初始Workfront實作期間應仔細設計，之後則保持不變。

### 用作比率屬性的物件

Workfront目前支援三個可作為比率屬性的系統物件：

* **群組**：經常重新命名為&#x200B;_機構_&#x200B;或&#x200B;_業務單位_。
* **公司**：可以代表&#x200B;_品牌_、_使用者端_&#x200B;或&#x200B;_客戶_。
* **位置**：通常用作&#x200B;_市場_、_地區_&#x200B;或&#x200B;_辦公室_。

  位置以階層方式定義，最多可定義3個層次。 （範例：如果您將「地點」定義為「洛杉磯」，則加州和美國也會用於費率比對。）

當您設定屬性時，可重新命名每個物件以符合貴組織的術語。
例如：

* &quot;Agency&quot;標籤=群組物件參考
* 「成本中心」標籤=子群組物件參考
* &quot;Location&quot;標籤=位置物件參考

這可讓設定反映您的業務結構，同時維護Workfront的資料模型完整性。

### Workfront中費率屬性的相關附註

* Workfront支援最多5個屬性層級。 系統一律遵循屬性階層，選取最具體的可用相符專案。

   * 0 =一般基本匯率
   * 1 - 5 =逐步提高特定費率

* 您可以重新命名屬性來反映您的業務（代理商、品牌、市場、成本中心等）。
* 僅設定一次：稍後變更屬性可能會破壞財務資料的完整性。
* 系統任何位置都未參考的屬性，可以安全地刪除。

  但是，如果屬性已在使用中（在比率卡、使用者設定檔、資源或指派中參照），則會封鎖刪除以保護資料完整性。 在這些情況下，嘗試移除屬性（尤其是透過API呼叫）將會導致錯誤。

* 上線前測試：建立試行費率卡，並驗證指派中解析的費率是否正確。
* 記錄您的設定：與團隊共用您的費率屬性設定，讓他們瞭解費率如何運作。

### 可套用費率屬性的位置

在Workfront中存在匯率的所有區域都支援匯率屬性：

* 費率卡：依職務角色加屬性來定義費率。
* 專案層次覆寫：在專案層次覆寫費率時套用屬性。
* 職務角色（在設定中）：使用屬性設定預設職務角色費率。
* 使用者（使用者設定檔）：將原生屬性指派給個別使用者，以便其指派會自動解析為正確的費率。
<!--
* Staffing plan resources
* Non-labor resources: Attributes can also be defined on resources such as equipment or services.-->

<!--Non-labor resource categories and -->職務角色不直接在物件層級支援費率屬性。 它們會透過其上定義的費率連線至費率屬性。

當您能夠建立與正確屬性值繫結的預留位置指派時，您的費率將會相應地填入。

* 對於工作角色，當您稍後以實際使用者取代預留位置時，系統會自動將指派的屬性重設為該使用者設定檔上定義的屬性。 此時，無法在指定層次編輯屬性。 它們繼承自使用者，以保留一致性，並防止使用者屬性和套用率之間出現不相符的情況。
  <!--* For non-labor resource categories, placeholder assignments can be used similarly: You assign the category through a placeholder that carries the required attributes. Once the actual non-labor resource is substituted, the attributes are automatically pulled from the resource's profile. Just like with users, these attributes cannot be overridden manually at the assignment level, ensuring financial data integrity and preventing accidental mismatches between resources and their designated attributes.-->

## 存取權要求

+++ 展開以檢視這篇文章中所述功能的存取權要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] 封裝</td> 
   <td>Workflow Ultimate</td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] 授權</td> 
   <td><p>[!UICONTROL 標準]</p></td>
  </tr> 
  <tr> 
   <td>存取層級設定</td> 
   <td>[!UICONTROL 系統管理員]</td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 設定費率屬性

每個屬性都有一組可設定的選項，包括一般屬性和篩選器。
篩選器可控制定義費率時，如何建議和驗證屬性值。 它們對於保持屬性選擇一致、引導使用者使用有效選項以及防止無效組合至關重要。

{{step-1-to-setup}}

1. 在左側面板中，按一下&#x200B;**評等屬性**。
1. 按一下圖表中的加號圖示以新增屬性。

   >[!NOTE]
   >
   >在圖表中最多可以有五個屬性。 由上到下的順序會定義套用屬性的階層。 按一下&#x200B;**旋轉**&#x200B;圖示![旋轉圖示](assets/rotate-attribute-view-icon.png)，從左到右顯示圖表。 您也可以放大或縮小，並將圖表調整至熒幕大小。

1. 選取屬性以開啟畫面右側的設定面板。

   ![設定費率屬性](assets/configure-rate-attributes.png)

1. 將物件（「群組」、「公司」、「位置」）重新命名為您的企業所需的術語（例如「代理商」、「位置」、「成本中心」）。
1. 按一下每個屬性上的&#x200B;**儲存**&#x200B;以儲存您的命名慣例。

   這些屬性的名稱將顯示在系統中的所有費率卡和費率上。

1. 在設定面板中設定每個屬性的屬性：

   * **必要**：選取屬性是否為費率的必要欄位。
   * **用於收入計算**：將此屬性包含在收費率計算中。
   * **用於成本計算**：在成本費率計算中包含此屬性。

     >[!NOTE]
     >
     >必須選取至少一個計算選項，屬性才能在財務計算中運作。

   * （選擇性） **階層式**：允許屬性遵循父子關係，例如「城市>州/省>國家/地區」。

     此屬性僅適用於Location物件。

### 定義屬性的篩選器

屬性可使用兩種型別的篩選器：

* 建議篩選器會根據系統邏輯或先前的屬性選擇，縮小可用選項清單。 它們讓下拉式清單具有內容感知且易於使用。

  範例：機構>地點>成本中心

  在此設定中，「成本中心」屬性應具有同時參照「機構」與「地點」的「建議篩選」。

  新增費率時，如果您先選取機構= &quot;Star&quot;，則「位置」下拉式清單只會建議屬於&quot;Star&quot;的位置。

  如果您接著在費率上選取「地點=芝加哥」，「成本中心」下拉式清單只會建議與「星星」和芝加哥相連結的「成本中心」。

* 關係篩選器會建立屬性之間的相依性鏈。 它們可確保系統瞭解屬性如何相互關聯並強制執行有效的相依性。

  範例：機構>地點>成本中心

  在此設定中，「代理機構」屬性應具有「關係篩選」，以將其繫結至有效的「地點」與「成本中心」。

篩選器必須一律雙向設定。 如果屬性A有屬性B的關係篩選，則屬性B應該有建議篩選返回屬性A。這可確保資料完整性和乾淨的使用者體驗。

1. 選取選項，以定義設定面板中屬性的「建議篩選」和「關係篩選」：

   * **篩選器型別**：

      * **標準**&#x200B;篩選器會將通用條件套用至屬性物件。 例如，「位置>作用中= True」（只會顯示作用中的位置）。

        無論是否選取其他屬性，一律會套用「標準」篩選。

      * **Attribute**&#x200B;篩選器會將鏈結中的一個屬性連結到另一個屬性。 例如，地點>參考=機構（只會顯示與所選機構相連結的地點）。

        只有在參照的屬性具有值時，才會套用「屬性」篩選。 例如，如果選取「機構」，則僅建議有效的「地點」。 如果「機構」空白，則會顯示所有地點（但仍受套用至地點的標準篩選條件的限制）。

   * **欄位**：屬性物件的直接欄位，例如「位置ID」或「作用中旗標」。
   * **運運算元**：這些選項取決於選取的欄位型別。 例如Equals、Not Equals、Is Blank、True/False。
   * （僅限標準篩選型別） **值**：例如，Is Active = True。
   * （僅限屬性篩選型別） **Reference**：此篩選所依賴的屬性，例如Agency。
   * （僅限屬性篩選型別） **參考欄位**：參考屬性上必須符合的欄位，例如機構識別碼。

1. 按一下每個屬性上的&#x200B;**儲存**&#x200B;以儲存屬性和篩選器。


