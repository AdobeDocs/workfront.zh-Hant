---
title: 22.2管理員增強功能
description: 22.2管理員增強功能
author: Luke
draft: Probably
feature: Product Announcements, System Setup and Administration
recommendations: noDisplay, noCatalog
exl-id: 55fb0b85-937d-4903-8a64-6f627dd4291f
source-git-commit: ccba3a3d7c0cac50dbd29cae677b076811904a91
workflow-type: tm+mt
source-wordcount: '1020'
ht-degree: 0%

---

# 22.2管理員增強功能

本頁說明22.2版對預覽環境所做的所有管理員增強功能。 這些增強功能將在生產環境中提供

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

2022年4月4日當週。 如需22.2版所有可用變更的清單，請參閱 [22.2版本總覽](../../../product-announcements/product-releases/22.2-release-activity/22-2-release-overview.md).

## 設定自訂表單以搭配多種物件型別使用

現在您可以設定新的或現有的自訂表單以搭配多種物件型別，讓表單的用途更加廣泛。 使用者將可以在您為其設定表單的所有型別物件上附加和填寫表單。

以前您可以設定自訂表單以僅使用一個物件型別。

此功能適用於先前在Workfront系統中建立的所有自訂表單。 例如，如果您已經有為Task物件型別建立的自訂表單，您現在可以設定表單以搭配其他物件型別使用，例如「專案」和「問題」。

如需詳細資訊，請參閱區段 [開始建立自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#start) 在文章中 [建立或編輯自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

>[!NOTE]
>
>* 我們初次發行預覽功能時，已暫時停用複製多物件自訂表單的功能。 此功能已於3月24日啟用。 如需複製自訂表單的相關資訊，請參閱 [複製自訂表單以建立新表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/copy-custom-form-to-create-a-new-one.md).
>* 在計算自訂欄位中，您參考的某些欄位可能與為表單設定的物件型別不相容。 我們的解決方案是萬用字元，允許計算根據表單附加到的物件輸出不同的值。 我們在3月24日新增了萬用字元。 如需使用方法的詳細資訊，請參閱區段 [多物件自訂表單中的已計算自訂欄位](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md#calculat) 在文章中 [新增計算資料至自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).
>* 針對自訂表單中的分割槽符號，我們已建立一組通用檢視和編輯許可權，這些許可權適用於您可以為表單設定的所有物件型別。 在其中一個案例中，我們發現其中一個「有限編輯」許可權可能會造成表單錯誤。 此問題已在3月24日修正。 如需分節符號的詳細資訊，請參閱 [新增分割槽符號至自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-section-break-to-a-custom-form.md).
>

## 藍圖目錄可供所有使用者使用，管理員可以允許請求

所有Adobe Workfront使用者現在可以瀏覽可用藍圖的目錄。 如需詳細資訊，請參閱 [瀏覽藍圖目錄並請求安裝藍圖](../../../administration-and-setup/blueprints/browse-catalog.md).

此外，系統管理員可以啟用使用者的存取權，以請求安裝藍圖。 指派要求佇列以儲存要求，可讓使用者從藍圖目錄提出要求。 如需詳細資訊，請參閱 [設定對藍圖的存取權](../../../administration-and-setup/blueprints/configure-access-to-blueprints.md).

## 新增影像至自訂表單

在您建立或編輯的自訂表單中，您現在可以新增影像，並包含使用者將滑鼠懸停在影像上時可閱讀的資訊性或說明性工具提示。

例如，此功能有助於顯示新產品的品牌，或提供使用者填寫表單時所需的視覺資訊。

以前，自訂表單完全以文字為基礎。

>[!NOTE]
>
>在新的Adobe Workfront體驗區域（尚未現代化，例如當您大量編輯專案時顯示的方塊）中，不顯示自訂表單影像。 這些區域會在我們持續更新時顯示。

如需詳細資訊，請參閱 [在自訂表單中新增或編輯資產Widget](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

## 新的預設存取層級設定

為了更符合建立新存取層級的大多數管理員的需求，我們已變更下列之「微調您的設定」選項的預設設定。 當您按一下齒輪圖示時，這些畫面就會顯示 ![](assets/gear-icon-in-access-levels.png) 在「編輯」按鈕上。

所有這些變更都會停用先前預設啟用的選項。 如果這不符合貴組織的需求，您可以在設定新存取層級時或稍後隨時啟用它們。

>[!IMPORTANT]
>
>此預設組態變更只會影響您從現在開始建立的存取層級，不會影響您先前建立的任何存取層級。

* 在具有「計畫」授權型別的新存取層級中：

   * 專案、任務、問題、投資組合、方案、報告、篩選器、檔案和範本的全系統共用現已停用。
   * 檢視內建報告和公開共用報告也會對報告停用。
   * 檔案也會停用公開共用檔案。

* 在具有「工作」授權型別的新存取層級中：

   * 篩選器和檔案的共用系統範圍現已停用。
   * 檔案也會停用公開共用檔案。

* 在具有「要求」或「檢閱」授權型別的新存取層級：

   * 已針對篩選器停用全系統共用。

## 停用群組

隨著內部組織變更，您可能需要停止使用Workfront中的特定群組，並建立新群組。 為協助解決此問題，我們新增了停用群組的功能，同時不會遺失其歷史資料。 對於不需要檢視的一般使用者，非作用中群組會從群組預先輸入欄位中清除。

您仍然可以尋找並設定您管理之非使用中群組的選項、偏好設定及物件關聯。 而停用群組並不會變更群組所附加物件的任何相關內容。

過去，您無法停用群組。

如需詳細資訊，請參閱 [停用或重新啟用群組](../../../administration-and-setup/manage-groups/create-and-manage-groups/deactivate-or-reactivate-a-group.md).

## Blueprint安裝歷史記錄增強功能

安裝Blueprint時，現在會顯示已成功與Blueprint一起安裝的特定物件（例如角色、團隊或群組）以及任何無法安裝的物件。 您也可以按一下安裝歷史記錄表格中特定安裝旁的檢視詳細資訊，來檢視「Blueprint詳細資訊」頁面上的已安裝物件清單。

如需詳細資訊，請參閱 [安裝Blueprint](../../../administration-and-setup/blueprints/blueprints-install.md).

![](assets/blueprints-installation-history-350x95.png)

## 現在，在生產環境中安裝僅限預覽的Blueprint時會顯示警告

某些Blueprint只能安裝在預覽環境中以進行測試。

如果您在生產環境、沙箱1或沙箱2中存取僅預覽內容，則安裝按鈕不會啟用，並且您可能會看到警告訊息。

如需詳細資訊，請參閱 [安裝Blueprint](../../../administration-and-setup/blueprints/blueprints-install.md).
