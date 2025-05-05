---
content-type: overview
product-area: agile-and-teams
navigation-topic: scrum-board
title: Scrum板概述
description: Scrum敏捷故事板會與完成狀態和待執行工作圖表一起顯示。
author: Lisa
feature: Agile
exl-id: 584288bb-2d98-4b69-8deb-d3b8e54d328c
source-git-commit: d660707dd69fab78095eed1414092a7c909ba174
workflow-type: tm+mt
source-wordcount: '878'
ht-degree: 0%

---

# [!UICONTROL Scrum]主機板概述

[!UICONTROL Scrum]敏捷故事板會與完成狀態和待執行工作圖表一起顯示。 在[!UICONTROL Adobe Workfront]的下列情況下可以使用這些敏捷元件：

* 在敏捷反複專案上。 如需有關在純敏捷環境（包含積壓和反複專案）中使用敏捷故事板、待執行工作表和完成狀態的詳細資訊，請參閱[在敏捷環境中工作](../../../agile/work-in-an-agile-environment/work-in-an-agile-environment.md)。
* 在敏捷檢視中檢視專案時。 如需如何在現有專案中善用敏捷故事板、待執行工作表和完成狀態的資訊，請參閱[在敏捷檢視中管理專案](../../../manage-work/projects/manage-projects/manage-projects-in-agile-view.md)。

![敏捷反複專案](assets/agile-iteration-with-callouts.png)

## 內文板版面配置與功能

![敏捷故事板](assets/agile-storyboard-callouts.png)

本文板由下列元素組成：

* **[!UICONTROL 父級劇本]欄：**&#x200B;與劇本面板上的其他欄不同，[!UICONTROL 父級劇本]欄不是工作狀態，而是用來存放任何包含疊代或專案中子工作的劇本。 此欄中只能存在劇本面板上至少有一個子任務的父劇本。 父級內文本身不會跨內文展示板從狀態移至狀態。

  在反複專案中，只有當故事板上的一或多個故事包含至少一個符合以下要求的子任務時，此欄才會出現在故事板上：

   * 指派給與上層任務相同的敏捷團隊
   * 屬於反複專案

     在專案中，每當任務至少有一個子任務時，就會出現此欄。

     ![父級劇本欄](assets/agile-parentstory-swimlane.png)

* **任務狀態：**&#x200B;根據內文所在的狀態列，指出內文在反複專案或專案中的進度。

  修改敏捷檢視即可自訂專案的任務狀態，如[!UICONTROL Adobe Workfront][&#128279;](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)中檢視總覽的[建立或自訂敏捷檢視](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md#customizing-an-agile-view)中所述。

* **泳道：**&#x200B;當父劇本及其子任務出現在劇本面板上時，會為劇本及其子任務特別建立泳道。 這提供了視覺上的區別，以便更好地檢視劇本的子任務在整個劇本板中的進度。

  在反複專案中，只有當故事板上的故事包含至少一個符合以下要求的子任務時，泳道才會出現在故事板上：

   * 指派給與上層任務相同的敏捷團隊
   * 屬於反複專案

  在專案中，只要任務至少有一個子任務或一個父任務，泳道就會出現。

* **個別劇本：**&#x200B;個別劇本和問題會顯示在劇本面板上任何泳道的下方。 這提供了與泳道中故事的視覺區別。

## 子任務和劇本之間的關係

如果內文包含子任務，您就無法更新上層內文本身的任何資訊（例如點/小時或完成百分比）。 此外，您無法將內文跨內文板移動以更新其狀態。 反之，您對內文子工作所做的任何變更都會反映在內文上。 所有子工作的合併內文點或時數會決定父內文的點或時數。

例如，如果內文只有一個子作業被指定為4點，則內文本身也有4點。 如果將子任務點值變更為3，父內文的點值就會變更為3。 如果您在相同內文上建立另一個子任務，並將該子任務的點值設為4，則內文的點值會變更為7，以反映兩個子任務的組合點值。

此邏輯同樣適用於第二層子任務（子任務的子任務）。 如果子任務有一或多個第二層子任務，則會根據第二層子任務計運算元任務。

## 劇本面板與待處理專案之間的關係

>[!NOTE]
>
>本節中的資訊僅適用於疊代的敏捷檢視；專案的敏捷檢視不使用待處理專案。 （如需疊代與專案敏捷檢視之間差異的詳細資訊，請參閱[在敏捷檢視中管理專案](../../../manage-work/projects/manage-projects/manage-projects-in-agile-view.md)中的「在疊代上使用[!UICONTROL 敏捷]檢視時的差異」。）

反複專案待處理專案只會顯示您可以設定預估的內文或子任務。 如果父級劇本具有顯示在劇本面板上的子任務（因為它們被指派給相同的敏捷團隊並屬於疊代），父級任務不會顯示在待辦專案中。 在此情況下，待處理專案中只會顯示子任務，而子任務和父級劇本則會顯示在劇本面板上。

例如，假設「內文A」包含「子任務1」和「子任務2」（且這兩個子任務都指派給相同的敏捷團隊）。 在此情況下，內文A會顯示在內文板上的泳道中，內含子任務1和子任務2。 不過，待處理專案中只會顯示子任務1和子任務2。

此邏輯同樣適用於第二層子任務（子任務的子任務）。 如果子任務有一或多個第二層子任務指派給相同的敏捷團隊並屬於疊代，則待處理專案中只會顯示第二層子任務。

如需待處理專案的詳細資訊，請參閱[管理敏捷待處理專案](../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md)。
