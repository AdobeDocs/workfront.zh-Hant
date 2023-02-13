---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: 專案更新類型概觀
description: 專案的「更新類型」會指出Adobe Workfront如何計算專案時間軸。 項目計畫中的更改可能觸發項目時間軸中的更改。 必須自動或手動重新計算專案的時間軸，以確保時間軸隨這些變更而最新。
author: Alina
feature: Work Management
exl-id: a6394961-2ac8-4b95-aa1b-dba8108c612f
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '512'
ht-degree: 0%

---

# 專案更新類型概觀

專案的「更新類型」會指出Adobe Workfront如何計算專案時間軸。 項目計畫中的更改可能觸發項目時間軸中的更改。 必須自動或手動重新計算專案的時間軸，以確保時間軸隨這些變更而最新。

有關重新計算項目時間軸的資訊，請參閱 [重新計算項目時間表](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

## 專案更新類型

項目有四種更新類型，具體取決於您希望Workfront重新計算項目時間軸的時間。 從下面的清單中選擇更新類型。

有關如何更新項目的更新類型的資訊，請參閱 [選擇項目更新類型](../../../manage-work/projects/manage-projects/select-project-update-type.md).

>[!IMPORTANT]
>
>如果專案的時間軸超過15年，Workfront不會自動或在變更時計算時間軸。 超過15年的專案更新類型一律為手動。

* **自動和更改：** 這是預設設定。 每次在項目中或時間軸所依賴的其他項目中發生更改時，都會更新項目時間軸。 每晚也會更新專案時間軸。 \
   這是建議的設定，因為它可確保項目時間軸始終保持最新。

   更新任務或項目並觸發時間軸重新計算時，將立即顯示所有可用日期，允許您繼續工作。 若專案的工作超過100個，需要較長計算時間的日期則會變灰。

   ![](assets/dates-dimmed-when-insline-editing-350x146.png)

   這表示重新計算尚未完成，日期可能會有所變更。

* **僅更改：** 每次在項目中或時間軸所依賴的其他項目中發生更改時，都會更新項目時間軸；未進行排程更新。\
   如果您擔心繫統效能，而且如果項目或時間軸所依賴的其他項目中很少發生更改，則可能需要選擇此選項。

* **僅自動：** 每晚更新項目時間表；進行變更後不會立即更新。\
   如果您擔心繫統效能，以及是否每天在項目中或時間軸所依賴的其他項目中發生許多更改，則可能需要選擇此選項。

   >[!NOTE]
   >
   >如果項目處於「計畫」狀態，則不會每晚自動重新計算該項目。 它只會在變更時重新計算。

* **僅手動：** 只有在您選取要 **重新計算時間表**，如文章的「手動重新計算」一節所述 [重新計算項目時間表](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).\
   如果您同時對專案進行許多變更，且希望時間軸重新計算在所有變更完成之後（而非每次個別變更後），您可以選取此選項。
