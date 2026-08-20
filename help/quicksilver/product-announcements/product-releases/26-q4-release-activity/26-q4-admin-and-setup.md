---
title: 2026年第四季管理員增強功能
description: 2026年第四季管理員增強功能
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: db296d9043cb793e1af74bca38197de682f54cb8
workflow-type: tm+mt
source-wordcount: '928'
ht-degree: 0%

---

# 2026年第四季管理員增強功能

本頁說明2026年第四季版本管理員對預覽環境所做的增強功能。 如上所述，這些增強功能將於生產環境中提供。

如需2026年第四季版本週期目前可用的所有變更清單，請參閱[2026年第四季版本概觀](/help/quicksilver/product-announcements/product-releases/26-q4-release-activity/26-q4-release-overview.md)。

<!--

## Interface improvements to the Actions list

>[!NOTE]
>
>Preview: August 20, 2026
>Production fast release: September 17, 2026
>Production for everyone: October 15, 2026

The Actions list in the Update Feeds section of the Setup area has an updated look and feel.

The following enhancements are included:

* We removed the Save and Cancel buttons.
* The Track column now appears in the last position.
* We removed the confirmation message that previously displayed when you saved changes in this area.

For information, see [Configure system updates](/help/quicksilver/administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md).

-->

## 群組管理員可以管理企業檔案

>[!NOTE]
>
>預覽： 2026年7月30日
>生產快速發行： 2026年8月13日
>適用於所有人的生產： 2026年10月15日

群組管理員現在可以建立、編輯和刪除他們管理的群組的企業設定檔，而不需要系統管理員存取權。 這可讓組織在群組層級委派業務設定檔管理時擁有更多彈性。

如需詳細資訊，請參閱[檢視和管理企業檔案](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/view-and-manage-business-profiles.md)。

## 版面配置範本支援增強型清單上的檢視

>[!NOTE]
>
>預覽： 2026年7月30日
>生產快速發行： 2026年8月13日
>適用於所有人的生產： 2026年10月15日

現在系統層級可透過版面配置範本支援增強型清單的檢視。 您可以隱藏現有的系統檢視、將特定檢視指派為預設檢視，以及將自訂檢視新增到系統檢視清單中。

配置範本中增強型清單的範例為&#x200B;**所有請求**&#x200B;和&#x200B;**進階指派**。 增強型清單的檢視旁會有「新體驗」標籤。

如需詳細資訊，請參閱[使用版面配置範本自訂篩選器、檢視和群組](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)。

## 大量編輯外部查閱欄位

>[!NOTE]
>
>預覽： 2026年7月30日
>生產快速發行： 2026年8月13日
>適用於所有人的生產： 2026年10月15日

大量編輯對話方塊現在允許編輯外部查閱欄位。 這在之前是不可能的。

在查閱欄位從屬於另一個查閱欄位的情況下，具有相依性的欄位無法大量編輯，除非正在編輯的所有物件的第一個欄位都相同。

例如，國家/地區清單取決於為區域所做的選擇。 如果一個專案的區域是亞洲，而另一個專案的區域是歐洲，當您大量編輯這兩個專案時，由於區域不相符，將無法使用「國家/地區」欄位。 如果您編輯兩個專案的地區相同，則也可以選取要用於兩個專案的國家/地區。

如需外部查閱欄位的詳細資訊，請參閱[建立自訂表單](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-external-lookup-fields)。

## 自訂表單設計工具預覽支援進階邏輯

>[!NOTE]
>
>預覽： 2026年7月30日
>生產快速發行： 2026年8月13日
>適用於所有人的生產： 2026年10月15日

自訂表單設計工具預覽模式現在支援進階邏輯選項，包括進階顯示邏輯、預設值邏輯、驗證邏輯、格式邏輯和可編輯性邏輯。 您可以在表單預覽中測試邏輯公式，並視需要在邏輯產生器中調整它們。 您也可以選取測試物件（專案、任務、問題等） 以預覽具有真實內容資料的表單。

先前，預覽模式僅支援基本顯示和略過邏輯選項。

請注意，這些邏輯型別僅適用於工作流程Prime或Ultimate套件上的組織：進階顯示、預設值、條件式格式化和可編輯性。

如需詳細資訊，請參閱[新增邏輯規則至自訂表單和欄位](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/display-skip-logic-form-designer.md)和[整理並預覽表單](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/organize-a-form.md)。

## 統一稽核和核准的變更追蹤

>[!NOTE]
>
>預覽： 2026年7月30日
>生產快速發行： 2026年8月13日
>適用於所有人的生產： 2026年10月15日

Workfront中的「變更歷史記錄」頁面現在會擷取統一檢閱和核准工作流程中的活動，為管理員提供檢閱和檔案生命週期事件的完整治理追蹤。

現在會追蹤核准、階段和參與者動作。 這些動作可能包括：

* 在Frame.io檢視器中做出核准決定
* 建立或刪除核准
* 更新檔案，例如重新命名、移動或刪除檔案

每個專案都包含標準追蹤欄位：日期和時間、作業、使用者名稱（或「系統產生」）和物件名稱。 會擷取MCP活動，包括進行更新的LLM （例如Claude）。 不包含Frame.io檢視器註解。

如需詳細資訊，請參閱[檢視及管理變更記錄](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/view-and-manage-change-history.md)。

## 在版面配置範本中將自訂應用程式定義為登入頁面

>[!NOTE]
>
>預覽： 2026年7月30日
>生產快速發行： 2026年8月13日
>適用於所有人的生產： 2026年10月15日

您現在可以將自訂應用程式設定為版面配置範本中的登入頁面。 已新增至主要功能表的自訂應用程式可用作登陸頁面。

自訂應用程式必須個別建立，才能作為主功能表或登入頁面選項使用。

如需詳細資訊，請參閱[使用版面配置範本自訂登入頁面](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-landing-page.md)和[使用Adobe App Builder建立Workfront的自訂應用程式](/help/quicksilver/app-builder/app-builder.md)。

## 設定變更記錄中的追蹤欄位

>[!NOTE]
>
>預覽： 2026年7月30日
>生產快速發行： 2026年8月13日
>適用於所有人的生產： 2026年10月15日

您可以在整個Workfront中新增要追蹤特定物件型別的欄位。 當使用者在該欄位中變更資訊時，系統會將有關變更的資訊記錄為變更歷史記錄中的專案。

以前，定義追蹤欄位的Configuration畫面是僅供檢視。

如需詳細資訊，請參閱[設定欄位以追蹤變更歷史記錄](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/configure-fields-in-change-history.md)。

## 變更歷史記錄的管理存取權已新增至存取層級

>[!NOTE]
>
>預覽： 2026年7月30日
>生產快速發行： 2026年8月13日
>適用於所有人的生產： 2026年10月15日

在「標準」存取層級上，您現在可以定義具有該層級的使用者是否應該擁有「變更記錄清單」的存取權。 **變更歷程記錄**&#x200B;選項可在存取層級的&#x200B;**允許**&#x200B;的管理存取區段中取得。

如需詳細資訊，請參閱[授予使用者對特定區域的管理存取權](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md)和[檢視及管理變更記錄](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/view-and-manage-change-history.md)。


