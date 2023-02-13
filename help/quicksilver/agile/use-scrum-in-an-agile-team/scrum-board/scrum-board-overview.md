---
content-type: overview
product-area: agile-and-teams
navigation-topic: scrum-board
title: 畫板概觀
description: Scrum敏捷故事板會顯示完成狀態和燃耗圖。
author: Lisa
feature: Agile
exl-id: 584288bb-2d98-4b69-8deb-d3b8e54d328c
source-git-commit: 6f817ca39c7489b85673ff601faf440fe51ab72c
workflow-type: tm+mt
source-wordcount: '867'
ht-degree: 0%

---

# [!UICONTROL Scrum] 展示板概觀

此 [!UICONTROL Scrum] 敏捷故事板與完成狀態和燃耗圖一起顯示。 這些敏捷元件適用於下列情況： [!UICONTROL Adobe Workfront]:

* 在敏捷的迭代中。 有關在純靈活環境（具有積壓和迭代）中使用敏捷故事板、燃耗圖和完成狀態的詳細資訊，請參閱 [在敏捷的環境中工作](../../../agile/work-in-an-agile-environment/work-in-an-agile-environment.md).
* 以敏捷檢視檢視專案時。 如需如何在現有專案內善用敏捷故事板、燃耗圖和完成狀態的詳細資訊，請參閱 [在敏捷檢視中管理專案](../../../manage-work/projects/manage-projects/manage-projects-in-agile-view.md).

![敏捷迭代](assets/agile-iteration-with-callouts.png)

## 文章板佈局和功能

![敏捷故事板](assets/agile-storyboard-callouts.png)

文章展示板包含下列元素：

* **[!UICONTROL 父項動態] 欄：** 與故事板上的其他專欄不同，  [!UICONTROL 父項動態]  列不是任務狀態，而是存在於包含小版本或項目中包含子任務的任何動態。 只有文章展示板上至少有一個子任務的父文章才能駐留在此列中。 父動態本身不會在動態展示板上從狀態移至狀態。

   在小版本中，只有當文章板上的一個或多個文章包含至少一個滿足以下要求的子任務時，此列才會顯示在文章板上：

   * 分配給與父任務相同的敏捷團隊
   * 屬於小版本

      在項目中，每當任務至少具有一個子任務時，此列就會顯示。

      ![上層動態列](assets/agile-parentstory-swimlane.png)

* **任務狀態：** 根據文章所在的狀態列指示文章在小版本或項目中的進展情況。

   您可以修改敏捷視圖，為專案自訂任務狀態，如 [建立或自訂敏捷檢視](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md#customizing-an-agile-view) in [檢視概觀，於 [!UICONTROL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

* **游巷：** 當父故事及其子任務出現在故事板上時，會為故事及其子任務建立一條泳道。 這提供視覺上的區別，以便更清楚地了解一個故事的子任務在整個故事片的進度。

   在迭代中，只有當故事板上的故事包含至少一個滿足以下要求的子任務時，泳道才會出現在故事板上：

   * 分配給與父任務相同的敏捷團隊
   * 屬於小版本

   在項目中，每當任務至少有一個子任務或一個父任務時，就會出現泳道。

* **個別動態：** 故事和問題會顯示在故事板上的任何游泳道下面。 這與游泳道中的故事有視覺上的區別。

## 子任務與動態之間的關係

如果文章包含子任務，則無法更新父文章本身的任何資訊（如點/小時或完成百分比）。 此外，您無法將動態移到動態展示板上以更新其狀態。 相反，你對故事子任務所做的任何改變都反映在故事上。 所有子任務的合併動態點或小時決定父動態的點或小時。

例如，如果一個故事只有一個子任務值為4點，那麼故事本身也有4點。 如果將子任務點值更改為3，則父小節的點值將更改為3。 如果在同一篇文章上建立另一個子任務，並將該子任務的點值設定為4，則文章的點值將更改為7，以反映這兩個子任務的合併點值。

同樣的邏輯適用於第二層子任務（子任務的子任務）。 如果子任務具有一個或多個第二級子任務，則根據第二級子任務計算子任務。

## 故事板與積壓的關係

>[!NOTE]
>
>本節中的資訊僅適用於迭代的敏捷視圖；專案的敏捷檢視不使用積壓工作。 (如需有關小版本上敏捷檢視與專案之間差異的詳細資訊，請參閱使用 [!UICONTROL 敏捷] 查看項目中的迭代節」 [在敏捷檢視中管理專案](../../../manage-work/projects/manage-projects/manage-projects-in-agile-view.md).)

小版本積壓僅顯示可設定估計的動態或子任務。 如果父項動態顯示的子任務顯示在動態板上（因為這些子任務被分配給同一個敏捷團隊，並且屬於小版本），則父項任務不會顯示在積壓上。 在此情況下，只有子任務顯示在積壓工作上，而子任務和父項動態顯示在動態板上。

例如，假設A故事包含子任務1和子任務2（兩個子任務均分配給同一個敏捷團隊）。 在這種情況下，故事A在故事板上顯示在具有子任務1和子任務2的游泳道中。 但是，在積壓工作中只顯示子任務1和子任務2。

同樣的邏輯適用於第二層子任務（子任務的子任務）。 如果子任務具有分配給同一敏捷團隊的一個或多個第二級子任務，並且屬於小版本，則在積壓工作中只顯示第二級子任務。

有關積壓的詳細資訊，請參閱 [管理敏捷積壓](../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md).
