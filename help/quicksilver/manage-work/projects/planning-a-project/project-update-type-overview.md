---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: 專案更新型別總覽
description: 專案的更新型別會指示Adobe Workfront計算專案時間表的方式。 專案計畫的變更可能會觸發專案時間表變更。 專案的時間表必須自動或手動重新計算，以確保符合這些變更的最新狀態。
author: Alina
feature: Work Management
exl-id: a6394961-2ac8-4b95-aa1b-dba8108c612f
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '515'
ht-degree: 0%

---

# 專案更新型別總覽

專案的更新型別會指示Adobe Workfront計算專案時間表的方式。 專案計畫的變更可能會觸發專案時間表變更。 專案的時間表必須自動或手動重新計算，以確保符合這些變更的最新狀態。

如需重新計算專案時間表的相關資訊，請參閱[重新計算專案時間表](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md)。

## 專案更新型別

視您希望Workfront重新計算專案時間表的時間而定，專案共有四種更新型別。 從下列清單中選擇更新型別。

如需有關如何更新專案更新型別的資訊，請參閱[選取專案更新型別](../../../manage-work/projects/manage-projects/select-project-update-type.md)。

>[!IMPORTANT]
>
>如果專案的時間表超過15年，Workfront不會自動計算或於變更時計算時間表。 超過15年的專案更新型別一律為手動。

* **自動與變更時：**&#x200B;這是預設設定。 每次在專案中或時間表所依存的其他專案中發生變更時，專案時間表都會更新。 專案時間表也會每晚更新。 \
  這是建議的設定，可確保專案時間表隨時保持最新。

  當您更新任務或專案並觸發時間表重新計算時，所有可用日期會立即顯示，允許您繼續工作。 在擁有超過100個任務的專案中，需要更長計算的日期會變暗。

  ![](assets/dates-dimmed-when-insline-editing-350x146.png)

  這表示重新計算尚未完成，日期可能會變更。

* **僅變更：**&#x200B;每次專案或時間表所依賴的其他專案發生變更時，專案時間表都會更新；不會發生排程更新。\
  如果您擔心系統效能，而且專案或時間表所依賴的其他專案中很少發生變更，您可能會想要選取此選項。

* **僅限自動：**&#x200B;專案時間表每晚都會更新；變更後不會立即更新。\
  如果您擔心系統效能，以及專案或時間表所依賴的其他專案中每天都發生許多變更，您可能會想要選取此選項。

  >[!NOTE]
  >
  >如果專案處於Planning狀態，則不會每晚自動重新計算。 它只會在變更時重新計算。

* **僅限手動：**&#x200B;專案時間表只有在您選取&#x200B;**重新計算時間表**&#x200B;的選項時才會更新，如[重新計算專案時間表](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md)一節中的「手動重新計算」一節所述。\
  如果您一次對專案進行許多變更，且希望在所有變更完成後（而不是在每次個別變更後）重新計算時間表，則可能需要選取此選項。
