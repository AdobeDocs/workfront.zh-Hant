---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: 透過Adobe Admin Console刪除使用者
description: 您只能從Adobe Workfront Fusion中移除使用者，而保留任何其他Adobe產品設定檔的存取權，或者您可以從Adobe Admin Console中完全移除使用者。
author: Becky
feature: Workfront Fusion
exl-id: 0d989134-46c0-4637-b465-6fbe04258b8a
source-git-commit: 392eee3c7b1aacf92d7877f07a8154924f3926a0
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 0%

---

# 透過刪除使用者 [!DNL Adobe Admin Console]

>[!IMPORTANT]
>
>本文中的功能僅在貴組織的執行個體為 [!DNL Adobe Workfront Fusion] 已上線至 [!DNL Adobe Business Platform].
>
>針對因貴組織是否已上線至而不同的程式清單， [!DNL Adobe Business Platform]，請參閱 [平台式管理差異([!DNL Adobe Workfront Fusion]/[!DNL Adobe Business Platform])](../../workfront-fusion/fusion-in-admin-console/fusion-adobe-admin-console.md).

您可以移除以下專案的使用者： [!DNL Adobe Workfront Fusion] 僅限，將存取權保留給任何其他 [!DNL Adobe] 產品設定檔，或者您也可以將使用者從 [!DNL Adobe Admin Console] 完整。

## 刪除中的使用者 [!DNL Adobe Workfront Fusion]

若要刪除中的使用者 [!DNL Adobe Workfront Fusion]，您必須透過以下路徑停用使用者： [!DNL Adobe Admin Console].

使用者已從中停用 [!DNL Adobe Admin Console] 當適用下列其中一項時：

* 使用者會從產品或產品設定檔中移出，且不會指派給任何其他產品或產品設定檔。
* 使用者會從連結至產品設定檔的群組中移除，且不會包含在連結至產品設定檔的任何其他群組內。
* 使用者會從產品設定檔中移除，且不會指派給其他產品設定檔。
* 使用者在包含Workfront Fusion的組織中被刪除或停用。

  如需指示，請參閱以下的「移除使用者」一節： [個別管理使用者](https://helpx.adobe.com/enterprise/using/manage-users-individually.html).

在 [!DNL Workfront Fusion]時，停用會以下列其中一個方式影響使用者：

* 如果使用者只在一個組織中，則停用該使用者。
* 如果使用者在不止一個組織中，系統會將使用者從上修改該使用者的組織中移除 [!DNL Adobe Admin Console].
* 有關刪除使用者時的其他考量事項 [!DNL Workfront Fusion]，請參閱 [在中刪除使用者時的注意事項 [!DNL Workfront Fusion]](../../workfront-fusion/organizations/manage-fusion-users.md#consider)
