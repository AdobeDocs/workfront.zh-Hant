---
title: 階層與階層連結概觀
description: 您可以在工作區中的記錄型別之間建立多個工作區階層。
hide: true
hidefromtoc: true
source-git-commit: 6aba4316228a320cf33e419249a64b3cf56e8f39
workflow-type: tm+mt
source-wordcount: '752'
ht-degree: 0%

---

<!--update the metadata with real information when making this available in TOC and in the left nav:

---
title: Hierarchy and Breadcrumb Overview
description: You can create multiple workspace hierarchies between the record types in a workspace. 
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
hide: yes 
hidefromtoc: yes 
---
-->

# 階層與階層連結概觀

身為工作區管理員，您可以在Adobe Workfront Planning的記錄型別與其他物件型別之間，定義彈性但結構化的階層。

階層是記錄型別之間的連線，或記錄型別與Workfront專案之間的連線。

如需建立階層的相關資訊，請參閱[建立工作區階層](/help/quicksilver/planning/architecture/create-workspace-hierarchies.md)。

下列是在工作區中使用階層的好處：

* 組織工作，以反映您的團隊實際規劃、運作及交付的方式。
* 讓使用者透過參考一組階層連結來瞭解他們在系統中的位置，如何連結記錄型別，以及策略如何進入執行。
* 提供更佳的導覽功能，並為所有工作流程建立清楚度和持續性。
* 定義符合組織運作方式的流程，支援所有工作階段的彈性與一致性。

## 使用階層時的注意事項

* 您可以為一個工作區建立多個階層。
* 您最多可以在一個階層中連線4個記錄和物件型別。
* 您只能在工作區階層中連線下列物件型別：
   * 記錄屬於您建立階層之工作區的型別。
   * Workfront專案。 Workfront專案無法新增為其他記錄型別的父項。 它們永遠是階層中的最後一個子系。
* 您無法在階層中新增下列物件型別：
   * 來自其他工作區的記錄型別，即使這些記錄型別設為可連線或全域記錄型別亦然。 只有在全域記錄型別已新增至您建立階層的工作區時，您才可以將全域記錄型別新增至階層。
   * 所有其他Workfront物件。
   * AEM Assets
* 階層可同時包含Planning記錄型別和Workfront專案。

      例如，您可以將具有規劃策略和Workfront專案的行銷活動記錄型別當做相同工作區階層中的子項。
  * 如果選取的記錄型別之間已經存在連線，系統會重複使用現有的連線。
* 如果沒有任何連線，Workfront會在階層設定中建立一個連線。
* 對於要包含在階層中的記錄和物件，必須為連線的欄位開啟&#x200B;**在連結的記錄型別上建立對應的欄位**&#x200B;設定。
* 以下是階層設定的規則：
   * 在指定的工作區中，記錄型別只能有一個父記錄型別。

     例如，策略記錄型別不能同時具有行銷活動和目標籤錄型別作為相同工作區中的父級。
   * 記錄型別可以是多個階層中的父項。

     例如，一個工作區中可以有三個不同的階層，而且每個階層都可以將「行銷活動」當作其父記錄型別。
   * 當您將一個記錄連線到多個或多個或多個記錄型別時，可以將一個記錄連線到多個相同型別的父記錄。
例如，策略A可同時屬於促銷活動X和促銷活動Y。
   * 記錄型別可以連線到多個子記錄型別。

     例如，Campaign記錄型別可以是多個其他記錄型別（例如戰術、測試和其他記錄型別）的父級。
   * 將全域記錄型別新增至多個工作區後，它們可能會出現在多個階層內的多個工作區中。

     例如，如果促銷活動是全域記錄型別，且屬於Workspace 1的階層，則可將其新增為Workspace 2的現有記錄型別，並成為該階層的一部分。 但是只有當在Workspace 1中指定為全域記錄型別，但未新增到Workspace 2時，它才能成為Workspace 2中階層的一部分。


## 檢視階層連結時的注意事項

當您在記錄型別之間建立階層時，它們會對屬於這些記錄型別的記錄產生階層連結。

例如，如果您建立階層並連結「行銷活動」與「戰術」、「活動」，然後連結「專案」，當您導覽至階層中連線之任何型別的記錄時，您可以檢視記錄在該階層中的放置位置。

請考量下列事項：

* 如果記錄型別是多個階層的一部分，您可以從記錄頁面上的記錄階層連結切換階層。
* 階層連結可跨Workfront和Planning運作。

  例如，檢視連結至Planning行銷活動和戰術以及Workfront產品組合和方案的專案時，您可以從階層連結在Planning和Workfront物件型別之間切換。

  如需詳細資訊，請參閱[建立工作區階層](/help/quicksilver/planning/architecture/create-workspace-hierarchies.md)。


