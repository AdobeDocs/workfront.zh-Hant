---
filename: delegate-work-overview
content-type: overview
navigation-topic: delegate-work
title: 委派工作概覽
description: 當您計畫短期不在辦公室時，您可以暫時將您的工作委派給其他使用者，以確保您的缺席不會成為完成工作的障礙。
author: Lisa
feature: Work Management
exl-id: aec2ce78-278f-48d2-af8c-e4e5b31ac856
source-git-commit: 2def8297fe606adaeaef6cc079b718531377919d
workflow-type: tm+mt
source-wordcount: '902'
ht-degree: 1%

---

# 委派工作概覽

當您計畫短期不在辦公室時，您可以暫時將您的工作委派給其他使用者，以確保您的缺席不會成為完成工作的障礙。

例如，如果您回訪前某些任務已到期，但您沒有時間在離開前完成它們，您可以將任務委派給另一個使用者，這樣他們就可以按時完成任務，並且不會將專案的完成延遲到您回訪後。

您可以在[!DNL Adobe Workfront]中委派下列物件：

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>Projects where you are designated as the Project Owner (not yet, not for the MVP)</p> </li>
  -->

* 指派給您的任務
* 指派給您的問題
* 指派給您的專案、任務或問題核准。

  >[!TIP]
  >
  >   您無法委派時程表、檔案或校訂核准。


本文包含有關委派指派給您的任務和問題的一般資訊。

如需有關委派專案、任務和問題核准的資訊，請參閱[委派核准要求](../../review-and-approve-work/manage-approvals/delegate-approval-requests.md)。

有關如何委派任務和問題的資訊，請參閱[委派任務和問題](../../manage-work/delegate-work/how-to-delegate-work.md)。

## 委派任務和問題總覽

委派任務和問題時請考慮以下事項：

* 您的[!DNL Workfront]或群組管理員必須在[!UICONTROL 設定]區域中啟用「委派」偏好設定，然後才能將您的工作委派給其他人。

  如需詳細資訊，請參閱[設定全系統的任務和問題偏好設定](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md)。

* 您只能從[!UICONTROL 首頁]區域委派任務和問題。
* 委派工作時，下列授權型別會有例外：

   * 您可以將工作委派給檢閱者或要求者，但[!DNL Workfront]不建議這麼做。
   * 檢閱者可以將工作委派給其他人。 他們無法在其[!UICONTROL 首頁]區域中檢視工作專案。 他們只能檢視核准。
   * 請求者無法將工作委派給其他人。 他們無法在其[!UICONTROL 首頁]區域中檢視工作專案
* 您只能委派指派給您的任務和問題。 您無法委派指派給其他使用者、團隊或工作角色的任務和問題。
* 您只能委派在委派開始日期之前未完成的任務和問題。
* 如果工作專案在委派時間範圍內完成，該專案會保留在委派者的「首頁」區域以及被指派者的「首頁」區域中2週，然後[!DNL Workfront]會自動移除它。
* 您選取為委派的使用者會獲得與您委派給他們的任務和問題之許可權相同的許可權。 這些許可權必須在其存取層級內運作，有時其存取層級可能低於您的存取層級。

>[!NOTE]
>
>  對於在委派開始後指派的專案，在指派專案給[!DNL Workfront]後，最多可能需要一小時才能與委派共用新指派的專案。

* 如果在您選擇將您的工作委派給其他使用者的期間內指派給您其他任務和問題，如果任務或問題日期在該時間範圍內，則新指派的工作會自動委派給您所選時間範圍內的相同人員。
* 多位使用者可選取同一位使用者作為委派。
* 委派的任務和問題未顯示在資源管理工具中，例如委派使用者的[!UICONTROL 工作負載平衡器]或[!UICONTROL 資源規劃工具]。
* 您可以在[!DNL Workfront]的多個區域中檢視委派的工作和委派名稱。 如需詳細資訊，請參閱文章[委派任務和問題](../delegate-work/how-to-delegate-work.md)中的「尋找委派的工作和委派資訊」一節。


  >[!IMPORTANT]
  >
  >  如果使用者對其存取層級中的任務只有「檢視」存取權，而您對您委派給他們的任務具有「管理」許可權，則他們可獲得您委派給他們的任務的「管理」許可權。 但是，他們將無法對委派的任務執行與您相同的動作。 他們必須向系統管理員請求任務的編輯存取權，才能在您不在時更新任務。

* 停止委派不會移除委派給使用者的許可權，這些許可權涵蓋委派給他們的任務和問題。
* 如果系統或停用[!UICONTROL 設定]區域中的[!UICONTROL 允許使用者委派其任務和問題]設定，則目前委派的使用者會從他們先前已委派給的任務和問題中移除。 不會移除其對任務或問題的許可權。

## 任務指派和委派之間的差異和相似性

| 動作 | 指派 | 委派 |
|--------------------------------------------------------------------------------------------------------------------------------|---------------------------------------|-----------------------------------------------------|
| 獲指派或委派的使用者可以編輯或刪除其獲指派或委派的工作專案 | 根據許可權和存取層級 | 根據許可權和存取層級 |
| 指派或委派的使用者顯示在工作專案的標頭中 | 是 | 是 |
| 指派或委派的任務或問題會顯示在受指派人或委派者的首頁區域 | 是，直到專案完成 | 是，僅適用於委派的時間範圍 |
| 您可以從首頁區域指派或委派工作給使用者 | 是 | 是 |
| 您可以使用指派或委派工作給使用者 | 是 | 否 |
| 您可以指派或委派工作給清單中的使用者，或是從工作專案的標頭指派或委派工作 | 是 | 否 |
| 任何使用者都可以指派或委派未與其關聯的工作專案給其他使用者 | 根據許可權和存取層級 | 否。只有受指派人可以委派自己的專案。 |
| 針對已指派或委派給使用者的工作，其計畫、實際或預算時數會在資源管理工具中為該使用者顯示 | 是 | 否 |
