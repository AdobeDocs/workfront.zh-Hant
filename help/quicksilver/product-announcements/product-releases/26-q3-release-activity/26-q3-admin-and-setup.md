---
title: 2026年第三季度管理員增強功能
description: 2026年第三季度管理員增強功能
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: a88a468901cc7a28139315ab820fc612f1c31736
workflow-type: tm+mt
source-wordcount: '438'
ht-degree: 0%

---

# 2026年第三季度管理員增強功能

本頁說明管理員在2026年第三季度版本中針對預覽環境所做的增強功能。 如上所述，這些增強功能將於生產環境中提供。

如需2026年第三季度發行週期中目前可用的所有變更清單，請參閱[2026年第三季度發行概觀](/help/quicksilver/product-announcements/product-releases/26-q3-release-activity/26-q3-release-overview.md)。

## RTF文字會以格式欄位型別取代文字

>[!NOTE]
>
>預覽： 2026年5月28日>生產快速版本： 2026年6月11日>每個人的生產： 2026年7月16日

自訂表單中的新&#x200B;**RTF**&#x200B;欄位型別是強大的文字編輯器，除了粗體、斜體、底線、專案符號、編號、超連結和區塊引號等傳統選項外，還有上標和下標、標題和表格等格式選項。 字元限制仍為15,000。

RTF文字欄位型別正在將文字取代為格式欄位型別。 您可以按一下右側欄位選項中的按鈕，快速地將具有格式欄位的現有文字轉換為RTF文字。 轉換時，歷史資料會保留在欄位上，在報表中的使用方式也相同。

>[!IMPORTANT]
>
>Workfront Fusion案例或API型自動化等外部整合可能會參考舊版欄位結構，並需要在轉換後進行更新。 在將欄位轉換為RTF文字之前，您應該驗證任何整合。

如需詳細資訊，請參閱[建立自訂表格](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)。

## 自訂表單中支援的原生財務欄位

>[!NOTE]
>
>預覽： 2026年5月28日>生產快速版本： 2026年6月11日>每個人的生產： 2026年7月16日

您現在可以在自訂表單中加入Workfront原生財務欄位。 以前不支援財務欄位。

您可以參考的可用財務欄位取決於表單型別。

如需詳細資訊，請參閱[建立自訂表格](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-workfront-native-fields)。

## 自訂表單可在系統範圍內共用，並可存取以附加

>[!NOTE]
>
>預覽： 2026年5月28日>生產快速版本： 2026年6月11日>每個人的生產： 2026年7月16日

已在自訂表單中新增共用選項「系統中的每個人都可以檢視和附加」。 當您選取此選項時，系統範圍內的所有使用者都可以將表單附加到其他物件。

在整個系統內共用可免除在新增群組時手動共用表單及跨群組或代理程式更新許可權的需求。

如需詳細資訊，請參閱[共用自訂表格](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md)。

## 新系統偏好設定可強制大量編輯的必要欄位

>[!NOTE]
>
>預覽： 2026年5月28日>生產快速版本： 2026年6月11日>每個人的生產： 2026年7月16日

目前，當大量編輯物件時，只有當使用者修改欄位時才會強制執行必要欄位。 如果欄位未修改，則會視為選用且未驗證。

新的系統偏好設定現在可讓您強制大量編輯中的必填欄位。 若要不允許儲存大量編輯的物件，除非所有必要欄位都有值，請在[設定] > [系統] > [偏好設定]頁面上選取[一律強制大量編輯必要欄位]選項&#x200B;**&#x200B;**。

