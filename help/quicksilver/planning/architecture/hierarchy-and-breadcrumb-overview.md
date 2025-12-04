---
title: 階層與階層連結概觀
description: 您可以在工作區中的記錄型別之間建立多個工作區階層。
hide: true
hidefromtoc: true
source-git-commit: f345cc0d41dc1bd62e7361fa0755cb7ba72465a0
workflow-type: tm+mt
source-wordcount: '405'
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

下列是在工作區中使用階層的好處：

* 組織工作，以反映您的團隊實際規劃、運作及交付的方式。
* 使用者透過參考指出他們在系統中的位置的一組階層連結，瞭解他們所在的位置、記錄型別如何連結，以及策略如何進入執行。
* 提供更佳的導覽功能，並為所有工作流程建立清晰度和連續性。
* 階層不會強制使用剛性、系統定義的結構，而是允許您定義符合組織運作方式的流程，同時支援所有工作階段的彈性與一致性。

## 使用階層時的注意事項

* 身為工作區管理員，您可以為一個工作區建立多個階層。
* 如果選取的記錄型別之間已經存在連線，系統會重複使用現有的連線。
* 如果沒有任何連線，Workfront會自動建立一個連線，作為階層設定的一部分。
* 以下是階層設定的規則：
   * 在指定的工作區中，記錄型別只能有一個父記錄型別。

     例如，策略記錄型別不能同時具有行銷活動和目標籤錄型別作為相同工作區中的父級。
   * 當您將一個記錄連線到多個或多個或多個記錄型別時，可以將一個記錄連線到多個相同型別的父記錄。
例如，策略A可同時屬於促銷活動X和促銷活動Y。
   * 記錄型別可以連線到多個子記錄型別。

     例如，Campaign記錄型別可以是多個其他記錄型別（例如戰術、測試和其他記錄型別）的父級。
   * 階層可包含Planning記錄型別和Workfront物件型別。

     例如，您可以將「行銷活動」記錄型別與「規劃策略」和「Workfront專案」作為子項。
   * 全域記錄型別可能會出現在多個階層內的多個工作區中。
   * Workfront物件型別也可以出現在多個階層以及不同的工作區中。
     <!--Not sure what this means: * Shared record can't be part of hierarchies.-->
   * 具有未在其連結的記錄型別上建立對應欄位的連線的記錄型別也可以是階層的一部分。 依預設，在階層設定期間建立的新連線一律會在連結的記錄型別上建立對應的欄位。

## 檢視階層連結時的注意事項


