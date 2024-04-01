---
title: 2024年第二季度管理員增強功能
description: 2024年第二季度管理員增強功能
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: a297ee8d-d949-45ab-a219-437316fa8fa3
source-git-commit: 2faa01024a1a174bacb42e9c6e24f528252f49f4
workflow-type: tm+mt
source-wordcount: '802'
ht-degree: 0%

---

# 2024年第二季度管理員增強功能

此頁面說明2024年第二季度版本對「預覽」環境所做的所有管理員增強功能。 如上所述，這些增強功能將於生產環境中提供。

如需2024年第二季發行週期目前可用的所有變更清單，請參閱 [2024年第二季版本總覽](/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-release-overview.md).

## 顯示邏輯和略過邏輯現在可在表單設計工具預覽模式中使用

>[!NOTE]
>
>預覽版本：2024年Mach 28；所有客戶生產：24.4 （2024年4月）

Beta版自訂表單設計工具現在可讓您在預覽模式下測試顯示邏輯及略過邏輯。 以前，即使套用了邏輯，預覽中仍會顯示所有欄位。

如需在表單設計工具中預覽自訂表單的詳細資訊，請參閱 [使用表單設計工具來組織和預覽表單](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/organize-a-form.md).

## 公司和使用者現在支援進階自訂表單欄位

>[!NOTE]
>
>預覽版本： 2024年3月14日；適用於所有客戶的生產： 24.4 （2024年4月）

當您將自訂表單附加至公司或使用者時，現在可以使用進階自訂表單功能，例如外部查詢欄位和Workfront原生欄位。 進階功能可在「公司詳細資訊」和「使用者詳細資訊」頁面上使用，而非「編輯公司」和「編輯使用者」對話方塊。 必須在新的表單設計工具中建立自訂表單，才能利用這些欄位型別。

如需自訂表單欄位的詳細資訊，請參閱 [使用表單設計工具設計表單](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## JumpSeat整合現在可用於新封裝型別

>[!NOTE]
>
>預覽版本： 2024年2月26日；快速版本的生產版：24.3版（2024年3月14日）；所有客戶的生產版：24.4 （2024年4月）

使用其中一個新套件型別（即Select、Prime或Ultimate）的帳戶現在可以使用現有的JumpSeat整合。 您必須擁有使用中的JumpSeat訂閱才能啟用整合。

如需JumpSeat整合的詳細資訊，請參閱 [設定JumpSeat整合](/help/quicksilver/administration-and-setup/configure-integrations/configure-jumpseat.md).

## 表單設計工具Beta版提供Workfront原生欄位

>[!NOTE]
>
>預覽版本： 2024年2月29日；快速版本的生產版：24.3版（2024年3月14日）；所有客戶的生產版：24.4 （2024年4月）

Workfront原生欄位現在可讓您新增至自訂表單。 此新欄位型別可讓您以邏輯方式組織資料並將其呈現給使用者，而無需在自訂欄位中重新建立現有資料。

在自訂表單欄位清單中選取原生欄位以將該欄位新增至表單設計工具後，您可以為表單物件選取任何原生欄位。 例如，如果表單設計器頂端的「物件型別」清單顯示「專案」，您將能夠選取專案的原生欄位，但不能選取任務特定的欄位。

當自訂表單附加到物件時，會從物件資料填入欄位。 例如，附加到專案的自訂表單上的說明欄位將提取專案說明。 （如果沒有可用資料，欄位可能會顯示「N/A」。）

自訂表單中使用的原生欄位在設計工具的欄位資料庫中變為可供重複使用。也可從設定>自訂Forms >欄位區域看到，讓您檢視這些欄位在哪些表單中使用。

此功能僅在表單設計工具（測試版）中可用，不在舊版表單產生器中可用。

如需詳細資訊，請參閱 [使用表單設計工具設計表單](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

[觀看此功能的示範影片。](https://video.tv.adobe.com/v/3427702/){target=_blank}

## 屬性對應現在可供已移轉至Adobe IMS的組織使用

>[!NOTE]
>
>預覽版本： 2024年2月22日；適用於所有客戶的生產： 2024年2月22日

Workfront系統管理員現在可以為已移轉至Adobe IMS的組織設定使用者屬性對應。 這可讓使用者資訊從組織的SSO （單一登入）提供者傳遞到Workfront，因此使用者的資料不必同時輸入到Workfront和SSO提供者。

以前，此功能僅適用於尚未上線Adobe IMS的組織。

如需設定屬性對應的說明，請參閱 [在Adobe統一體驗中對應使用者屬性](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/map-user-attributes.md#map-user-attributes-in-the-adobe-unified-experience) 在文章中 **對應使用者屬性並自動布建新使用者**.

## 表單設計工具Beta版現在提供略過邏輯和顯示邏輯

>[!NOTE]
>
>預覽版本： 2024年2月8日；快速版本的生產版：24.2版（2024年2月15日）；所有客戶的生產版：待定

您現在可以編輯現有的顯示和略過邏輯，並在表單設計工具Beta版中新增邏輯至自訂表單。 易於使用的邏輯產生器可協助您根據表單中的選取專案定義要顯示或略過的欄位。

表單設計器畫布中欄位上的圖示表示已在該欄位上設定邏輯，或該欄位用於其他欄位上設定的邏輯規則。

如需詳細資訊，請參閱 [使用表單設計工具新增顯示邏輯和略過邏輯](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/display-skip-logic-form-designer.md).
