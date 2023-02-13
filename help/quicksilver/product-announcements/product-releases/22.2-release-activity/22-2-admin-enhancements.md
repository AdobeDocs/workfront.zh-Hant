---
title: 22.2管理員增強功能
description: 22.2管理員增強功能
author: Luke
draft: Probably
feature: Product Announcements, System Setup and Administration
exl-id: 55fb0b85-937d-4903-8a64-6f627dd4291f
source-git-commit: be4904f0b37870c1bfc8ec345e468d5fc283aa36
workflow-type: tm+mt
source-wordcount: '1009'
ht-degree: 0%

---

# 22.2管理員增強功能

本頁面說明在「預覽」環境的22.2版中進行的所有管理員增強功能。 這些增強功能將可在生產環境中使用

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

2022年4月4日當周。 如需22.2版所有可用變更的清單，請參閱 [22.2版本概觀](../../../product-announcements/product-releases/22.2-release-activity/22-2-release-overview.md).

## 設定自訂表單以搭配多個物件類型使用

現在，您可以設定新的或現有的自訂表單以搭配多個物件類型使用，讓表單更實用。 用戶將能夠在您為其配置的所有類型的對象上附加並填寫表單。

之前，您可以設定自訂表單以只搭配一個物件類型使用。

此功能適用於先前在您的Workfront系統中建立的所有自訂表單。 例如，如果已為Task對象類型建立了自定義表單，則您現在可以配置該表單以與其他對象類型（如Project和Issue）一起使用。

如需詳細資訊，請參閱 [開始建立自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#start) 在文章中 [建立或編輯自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

>[!NOTE]
>
>* 此功能初次預覽發行時，我們暫時停用了複製多物件自訂表單的功能。 這項能力於3月24日啟用。 如需複製自訂表單的相關資訊，請參閱 [複製自訂表單以建立新表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/copy-custom-form-to-create-a-new-one.md).
>* 在計算的自訂欄位中，您參考的某些欄位可能與為表單設定的物件類型不相容。 我們的解決方案是萬用字元，可讓計算根據表單所附加的物件輸出不同的值。 3月24日，我們加了萬用字元。 如需如何使用的資訊，請參閱 [多物件自訂表單中的計算自訂欄位](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md#calculat) 在文章中 [將計算資料新增至自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).
>* 針對自訂表單中的分區，我們已建立一組通用的檢視和編輯權限，這些權限適用於您可以為表單設定的所有物件類型。 在一種情況下，我們發現其中一個權限（有限編輯）可能會在表單上造成錯誤。 此問題已於3月24日修正。 如需分段的詳細資訊，請參閱 [為自訂表單新增區段分頁](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-section-break-to-a-custom-form.md).
>


## Blueprint目錄可供所有用戶使用，並且管理員可允許請求

所有Adobe Workfront用戶現在都可以瀏覽可用藍圖目錄。 如需詳細資訊，請參閱 [瀏覽藍圖目錄並請求安裝藍圖](../../../administration-and-setup/blueprints/browse-catalog.md).

此外，系統管理員可以讓用戶訪問請求安裝藍圖。 分配請求隊列以儲存請求允許用戶從Blueprint目錄中發出請求。 如需詳細資訊，請參閱 [配置對Blueprint的訪問](../../../administration-and-setup/blueprints/configure-access-to-blueprints.md).

## 將影像新增至自訂表單

在您建立或編輯的自訂表單中，您現在可以新增影像，並加入提供資訊或說明的工具提示，供使用者暫留在影像上時閱讀。

例如，這可能有助於顯示新產品的品牌，或提供使用者在填寫表單時所需的視覺資訊。

過去，自訂表單完全以文字為基礎。

>[!NOTE]
>
>在尚未現代化的新Adobe Workfront體驗區域中，例如批量編輯項目時顯示的方塊，自訂表單影像無法顯示。 我們會繼續更新這些區域，以便顯示這些區段。

如需詳細資訊，請參閱 [在自訂表單中新增或編輯資產介面工具集](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

## 新預設訪問級別配置

為了更好地滿足建立新訪問級別的大多數管理員的需求，我們更改了下面列出的「微調您的設定」選項的預設配置。 當您按一下齒輪圖示時，就會顯示這些 ![](assets/gear-icon-in-access-levels.png) 在「編輯」按鈕上。

所有這些變更都會停用先前預設已啟用的選項。 如果這不符合貴組織的需求，您可以在設定新的存取層級時或稍後隨時啟用這些功能。

>[!IMPORTANT]
>
>此預設配置更改僅影響您從現在開始建立的訪問級別，而不影響您以前建立的任何訪問級別。

* 在具有計畫許可證類型的新訪問級別中：

   * 專案、工作、問題、產品組合、方案、報表、篩選器、檔案和範本現已停用全系統共用功能。
   * 檢視內建報表和公開共用報表也在報表中停用。
   * 對於文檔，「公開共用文檔」也被禁用。

* 在具有工作許可證類型的新訪問級別中：

   * 篩選器和檔案現已停用「全系統共用」功能。
   * 對於文檔，「公開共用文檔」也被禁用。

* 在具有「請求」或「查看」許可證類型的新訪問級別中：

   * 現在已針對篩選器停用「全系統共用」。

## 停用群組

隨著內部組織變更，您可能需要停止在Workfront中使用特定群組並建立新群組。 為了提供這些協助，我們新增了在不遺失群組歷史資料的情況下停用群組的能力。 對於不需要查看的一般使用者，非作用中群組會從「群組預先類型」欄位中清除。

您仍可以找到並設定您管理之非活動群組的選項、偏好設定和物件關聯。 停用群組並不會變更該群組所附加之物件的任何內容。

以前無法停用群組。

如需詳細資訊，請參閱 [停用或重新啟用群組](../../../administration-and-setup/manage-groups/create-and-manage-groups/deactivate-or-reactivate-a-group.md).

## Blueprint安裝歷史記錄增強功能

安裝Blueprint時，現在會顯示訊息，指出已成功與Blueprint一併安裝的特定物件（例如角色、團隊或群組），以及任何無法安裝的物件。 您也可以按一下安裝歷史記錄表中特定安裝旁邊的「查看詳細資訊」(View Details)，查看「Blueprint詳細資訊」(Blueprint Details)頁面上已安裝對象的清單。

如需詳細資訊，請參閱 [安裝Blueprint](../../../administration-and-setup/blueprints/blueprints-install.md).

![](assets/blueprints-installation-history-350x95.png)

## 現在在生產環境中安裝僅限預覽的Blueprint時，系統會顯示警告

某些藍圖僅可用於在預覽環境中安裝，以用於測試。

如果您在生產環境、沙箱1或沙箱2中存取僅限預覽的內容，安裝按鈕不會作用中，您可能會看到警告訊息。

如需詳細資訊，請參閱 [安裝Blueprint](../../../administration-and-setup/blueprints/blueprints-install.md).
