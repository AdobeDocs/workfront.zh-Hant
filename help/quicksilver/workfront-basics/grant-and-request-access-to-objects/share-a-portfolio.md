---
title: 共用投資組合
description: 如果您有存取投資組合的許可權，可以與其他使用者共用投資組合。
author: Alina
draft: Probably
feature: Get Started with Workfront
exl-id: 79643202-2d91-4028-b673-c3443b50d898
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '381'
ht-degree: 0%

---

# 共用投資組合

指派存取層級時，您的Adobe Workfront管理員可授予您檢視或編輯投資組合的存取權。 您必須擁有計畫授權才能編輯投資組合。 如需詳細資訊，請參閱 [授予投資組合的存取權](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-portfolios.md).

除了授予您的存取層級之外，您還可以從可與您共用專案組合的使用者那裡獲得檢視或管理特定專案組合的許可權。 如需存取層級和許可權的詳細資訊，請參閱 [存取層級和許可權如何搭配運作](../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md).

許可權專屬於Workfront中的一個專案，可定義使用者可對該專案執行的動作。

## 關於共用投資組合的考量事項

除了下列考量事項外，另請參閱 [物件許可權共用概觀](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

>[!NOTE]
>
>Workfront管理員可以新增或移除系統中所有使用者的任何專案許可權，而無需擁有這些專案。

* 依預設，投資組合的建立者擁有投資組合的管理許可權。
* 您可以單獨共用一個投資組合，也可以同時共用多個投資組合。 共用投資組合等同於在Workfront中共用其他物件。 如需詳細資訊，請參閱 [共用物件](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).

* 您只能授予Portfolio的「檢視」或「管理」許可權。

  ![](assets/screen-shot-2014-01-23-at-12.45.15-pm.png)    ![](assets/screen-shot-2014-01-22-at-10.03.43-am-190x167.png)

* 共用專案組合時，使用者預設會繼承與專案組合相關聯之所有子物件的相同許可權。

  如需Workfront中物件階層的詳細資訊，請參閱 [瞭解Adobe Workfront中的物件](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

* 您可以從Portfolio中移除繼承的許可權。 如需有關從物件移除許可權的詳細資訊，請參閱 [移除物件的許可權](../../workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md).

## Portfolio許可權

下表顯示當允許使用者檢視或管理Portfolio時，您可以授予他們哪些許可權：

| **動作** | **管理** | **檢視** |
|---|---|---|
| 編輯Portfolio詳細資訊 | ✓ (A) |   |
| 檢視Portfolio | ✓ (A) | ✓ (A) |
| 刪除Portfolio | ✓ (A) |   |
| 附加自訂表格 | ✓ (A) |   |
| 編輯自訂欄位 | ✓ (A) |   |
| 新增或移除程式&#42; | ✓ (A) |   |
| 新增或移除專案&#42; | ✓ (A) |   |
| 核准專案 | ✓ (A) |   |
| Portfolio最佳化&#42; | ✓ (A) |   |
| 新增檔案資料夾&#42; | ✓ (A) | ✓ (A) |
| 新增檔案 | ✓ (A) | ✓ (A) |
| 更新/評論 | ✓ (A) | ✓ (A) |
| 共用 | ✓ (A) | ✓ (A) |
| 共用系統範圍 |   | ✓ (A) |

*這些許可權是由其他物件（如專案、方案、檔案）的存取層級和許可權所控制。
