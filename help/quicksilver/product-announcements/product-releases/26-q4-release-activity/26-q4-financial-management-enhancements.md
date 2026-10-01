---
title: 2026年第四季度Financial Management增強功能
description: 2026年第四季度Financial Management增強功能
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
subfeature_v2:
  - id: a29813d3-f0cc-4b60-9396-13b558370803
    internal-label: Product announcements
source-git-commit: 0c08d79733bc6da0ecfd41f765ce2c624e71ad0e
workflow-type: tm+mt
source-wordcount: '373'
ht-degree: 0%
---
# 2026年第四季度Financial Management增強功能

本頁說明2026年第四季度發行的「預覽」環境中的Financial Management增強功能。 如上所述，這些增強功能將於生產環境中提供。

如需2026年第四季版本週期目前可用的所有變更清單，請參閱[2026年第四季版本概觀](/help/quicksilver/product-announcements/product-releases/26-q4-release-activity/26-q4-release-overview.md)。

<!--

## Enhancements to billing rates on templates

>[!NOTE]
>
>Preview: October 1, 2026
>Production fast release: October 15, 2026
>Production for everyone: October 15, 2026

Multiple updates have been made to the billing rates functionality on a project template.

### For customers on all Workfront and Workflow packages

The Rates area on templates has been updated to an enhanced list.

For more information, see [Use enhanced lists](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).

### For customers on the Workflow Ultimate package only

Rate attributes are now available to apply to job role billing rates on the template.

For more information, see [Edit project templates](/help/quicksilver/manage-work/projects/create-and-manage-templates/edit-templates.md#add-more-items-to-a-template) and [Override Job Role Billing Rates at the project level](/help/quicksilver/manage-work/projects/project-finances/override-job-role-billing-rates-at-the-project-level.md).

-->

## 公司收費率的增強功能

>[!NOTE]
>
>預覽： 2026年9月3日
>生產快速發行： 2026年9月17日
>適用於所有人的生產： 2026年10月15日

已對公司收費率功能進行多項更新。

### 適用於所有Workfront和工作流程套件的客戶

* 我們已更新對話方塊，以更現代的設計新增及編輯公司收費率，並與Workfront的其他區域一致。
* 「允許公司層級的計費費率覆寫專案層級的計費費率」設定會在將公司新增至專案時正確新增費率覆寫，而計畫的收入計算會使用公司層級的計費費率。
* 無權在專案層級編輯一般財務和編輯收費率的使用者無法再將公司新增到該專案。

### 僅適用於工作流程Ultimate封裝的客戶

費率屬性現在可套用至公司層級的收費率。 有效日期也可套用至公司費率。

備註：尚未將公司層次的費率新增至費率階層。

如需詳細資訊，請參閱[覆寫公司層級的工作角色收費率](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/override-job-role-billing-rates-company-level.md)和[以公司層級收費率覆寫專案層級收費率](/help/quicksilver/manage-work/projects/project-finances/override-project-level-with-company-level-billing-rates.md)。

## 屬性階層現在會自動維持連線

>[!NOTE]
>
>預覽： 2026年9月3日
>生產快速發行： 2026年9月17日
>適用於所有人的生產： 2026年10月15日
>此功能僅適用於Workflow Ultimate套件上的組織。

在Workfront的各種區域（例如進階指派）中使用比率屬性作為篩選器時，現在會將其他驗證套用至父子篩選。

以前，如果您將一個屬性連結至父項，而該父項連結至祖父項，則系統不會自動將原始屬性識別為也屬於該祖父項。 現在，當您選擇最低層級屬性時，系統會自動指定其上方的每個層級。

如需屬性的相關資訊，請參閱[定義費率屬性](/help/quicksilver/administration-and-setup/manage-enterprise-operations/define-rate-attributes.md)。
