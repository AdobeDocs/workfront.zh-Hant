---
title: 2026年第三季度管理員增強功能
description: 2026年第三季度管理員增強功能
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: a9688886f32cd41dd7d53dbf0a918f25fdd04a0b
workflow-type: tm+mt
source-wordcount: '1328'
ht-degree: 4%

---

# 2026年第三季度管理員增強功能

本頁說明管理員在2026年第三季度版本中針對預覽環境所做的增強功能。 如上所述，這些增強功能將於生產環境中提供。

如需2026年第三季度發行週期中目前可用的所有變更清單，請參閱[2026年第三季度發行概觀](/help/quicksilver/product-announcements/product-releases/26-q3-release-activity/26-q3-release-overview.md)。

<!--

## Change tracking for unified review and approval

>[!NOTE]
>
>Preview: July 7, 2026
>Production fast release: July 15, 2026
>Production for everyone: July 16, 2026

The Change History page in Workfront now captures activity across unified review and approval workflows, giving administrators a complete governance trail for review and document lifecycle events.

Approval, stage, and participant actions are now tracked. These actions may include:

* Making an approval decision in the Frame.io viewer
* Creating or deleting an approval
* Updating a document such as renaming, moving, or deleting it

Each entry includes the standard tracked fields: date and time, operation, user name (or "system generated"), and object name. Frame.io viewer comments are not included.

This phase of change tracking does not include MCP events. Those will be part of a future release.

For more information, see [View and manage change history](/help/quicksilver/administration-and-setup/manage-enterprise-operations/view-and-manage-change-history.md).

-->

## 內部查詢欄位取代Typeahead欄位型別

>[!NOTE]
>
>預覽： 2026年7月7日生產快速發行： 2026年7月15日適用於所有人的生產： 2026年7月16日

自訂表單中的新&#x200B;**內部查詢**&#x200B;欄位型別提供動態篩選。 它類似於「預先輸入」欄位型別，可讓使用者透過輸入部分名稱來搜尋及選取現有的Workfront物件。 內部查詢上的篩選器可以參考表單上另一個欄位的值，但Typeaheads無法這麼做。

內部查詢支援多選，而且此欄位型別還可以改善大型資料集的效能。 內部查詢支援下列原生Workfront物件：專案、公司、群組、工作角色、Portfolio、方案、團隊、範本、使用者、任務、問題、檔案和位置。

內部查詢欄位型別正在取代Typeahead欄位型別。 您可以按一下右側欄位選項中的按鈕，快速地將現有的預先輸入欄位轉換為內部查詢。 轉換時，歷史資料會保留在欄位上，在報表中的使用方式也相同。

>[!IMPORTANT]
>
>Workfront Fusion案例或API型自動化等外部整合可能會參考舊版欄位結構，並需要在轉換後進行更新。 在將預先輸入欄位轉換為內部查詢欄位之前，您應該驗證任何整合。

如需詳細資訊，請參閱[建立自訂表格](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)。

## 原生參考欄位支援的預設值邏輯

>[!NOTE]
>
>預覽： 2026年7月7日生產快速發行： 2026年7月15日適用於所有人的生產： 2026年7月16日
>
>此功能僅適用於Workflow Prime或Ultimate套件上的組織。

在自訂表單中，原生參考欄位現在可讓您新增預設值邏輯。

原生參考欄位上的此邏輯型別僅在使用者介面中可用，在Workfront API中則不可用。

如需詳細資訊，請參閱[新增邏輯規則至自訂表單和欄位](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/display-skip-logic-form-designer.md)中的文章[新增預設值邏輯至自訂表單](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/display-skip-logic-form-designer.md#add-default-value-logic-to-a-custom-form)。

## 自訂表單中原生欄位篩選的更新

>[!NOTE]
>
>預覽： 2026年7月7日生產快速發行： 2026年7月15日適用於所有人的生產： 2026年7月16日

原生欄位上存在的系統篩選器現在套用至自訂表單中的欄位，並且管理員可以看到。

當您新增已套用系統篩選器的原生參考欄位時，您可以將相同的篩選器套用至自訂表單中的欄位，並視需要在「文字模式」方塊中修改篩選器。

將您自己的自訂篩選器新增到欄位會覆寫欄位的系統篩選器。 如果您未輸入自訂篩選器，則預設會套用系統篩選器。

此外，原生參考欄位現在提供動態篩選。 動態篩選器可讓您根據其他欄位的值來縮小專案清單的範圍。

例如，當您在專案欄位篩選中使用`?portfolioID={portfolio}.{ID}`，並且自訂表單上有Portfolio原生欄位時，專案欄位僅顯示所選投資組合中的專案。 如果Portfolio欄位留空，則所有專案都可在「專案」欄位中使用。

如需詳細資訊，請參閱[建立自訂表格](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)。

## 保護欄位名稱，避免意外重新命名

>[!NOTE]
>
>預覽： 2026年7月7日生產快速發行： 2026年7月15日適用於所有人的生產： 2026年7月16日

為了保護整合和資料完整性，我們已更新如何在自訂表單的欄位設定面板中編輯欄位名稱。

欄位設定面板中的欄位名稱現在預設為唯讀。 您仍然可以編輯欄位名稱，但重新命名需要明確的確認步驟。 先前稱為&#x200B;**名稱**&#x200B;的欄位也已更新為&#x200B;**API名稱**，以便更佳地反映其技術重要性。 **標籤**&#x200B;欄位仍可編輯。

如需詳細資訊，請參閱[建立自訂表格](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#notes-on-field-names-and-labels)。

## 檢視Workfront物件的變更記錄

>[!NOTE]
>
>預覽： 2026年6月11日生產環境快速發行： 2026年6月11日適用於所有人的生產： 2026年7月16日

為了讓您更輕鬆地檢視在一個中央清單中發生的變更，我們已建立「變更記錄清單」。 此清單會顯示物件、作業和變更來源（例如使用者或Workfront系統）等資訊。

以前，稽核記錄可供使用，但不涵蓋物件。

如需詳細資訊，請參閱[檢視及管理變更記錄](/help/quicksilver/administration-and-setup/manage-enterprise-operations/view-and-manage-change-history.md)。

## 將舊版儲存產品組合轉換為Adobe雲端儲存空間的新系統偏好設定

>[!NOTE]
>
>預覽： 2026年6月11日每個人都要生產： 2026年6月11日

Workfront管理員現在可以直接從「系統偏好設定」將舊版儲存產品組合轉換為Adobe雲端儲存空間。 若要轉換產品組合，請在新的選取產品組合中選取它們，以轉換為企業儲存欄位並儲存頁面。

當產品組合轉換為Adobe雲端儲存空間時：

* 您無法再將使用舊版 Workfront 儲存空間的專案移至此專案組合
* 此專案組合中建立的所有新專案均使用 Adobe 雲端儲存空間
* Frame.io是使用Adobe雲端儲存空間的檔案檢視器
* 使用舊版Workfront儲存空間的子物件會保留在舊版儲存空間

先前，將Adobe雲端儲存空間專案新增至舊版儲存空間產品組合，會自動將該產品組合轉換為Adobe雲端儲存空間。

如需詳細資訊，請參閱[設定系統偏好設定](/help/quicksilver/administration-and-setup/manage-workfront/security/configure-security-preferences.md)。

## RTF 文字欄位取代格式化文字的欄位類型

>[!NOTE]
>
>預覽： 2026年5月28日生產環境快速發行： 2026年6月11日適用於所有人的生產： 2026年7月16日

自訂表單中的新&#x200B;**RTF**&#x200B;欄位型別是強大的文字編輯器，除了粗體、斜體、底線、專案符號、編號、超連結和區塊引號等傳統選項外，還有上標和下標、標題和表格等格式選項。 字元限制仍為15,000。

RTF文字欄位型別正在將文字取代為格式欄位型別。 您可以按一下右側欄位選項中的按鈕，快速地將具有格式欄位的現有文字轉換為RTF文字。 轉換時，歷史資料會保留在欄位上，在報表中的使用方式也相同。

>[!IMPORTANT]
>
>Workfront Fusion案例或API型自動化等外部整合可能會參考舊版欄位結構，並需要在轉換後進行更新。 在將欄位轉換為RTF文字之前，您應該驗證任何整合。

如需詳細資訊，請參閱[建立自訂表格](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)。

## 自訂表單中支援的原生財務欄位

>[!NOTE]
>
>預覽： 2026年5月28日生產環境快速發行： 2026年6月11日適用於所有人的生產： 2026年7月16日

您現在可以在自訂表單中加入Workfront原生財務欄位。 以前不支援財務欄位。

您可以參考的可用財務欄位取決於表單型別。

如需詳細資訊，請參閱[建立自訂表格](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-workfront-native-fields)。

## 自訂表單可以全系統共用，並提供附加權限

>[!NOTE]
>
>預覽： 2026年5月28日生產環境快速發行： 2026年6月11日適用於所有人的生產： 2026年7月16日

已在自訂表單中新增共用選項「系統中的每個人都可以檢視和附加」。 當您選取此選項時，系統範圍內的所有使用者都可以將表單附加到其他物件。

在整個系統內共用可免除在新增群組時手動共用表單及跨群組或代理程式更新許可權的需求。

如需詳細資訊，請參閱[共用自訂表格](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md)。

## 新系統偏好設定可以在大量編輯時強制填寫必要欄位

>[!NOTE]
>
>預覽： 2026年5月28日生產環境快速發行： 2026年6月11日適用於所有人的生產： 2026年7月16日

目前，當大量編輯物件時，只有當使用者修改欄位時才會強制執行必要欄位。 如果欄位未修改，則會視為選用且未驗證。

新的系統偏好設定現在可讓您強制大量編輯中的必填欄位。 若要不允許儲存大量編輯的物件，除非所有必要欄位都有值，請在[設定] > [系統] > [偏好設定]頁面上選取[一律強制大量編輯必要欄位]選項&#x200B;****。

如需詳細資訊，請參閱[設定系統偏好設定](/help/quicksilver/administration-and-setup/manage-workfront/security/configure-security-preferences.md)。
