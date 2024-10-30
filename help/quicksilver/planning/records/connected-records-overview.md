---
title: 連線記錄概觀
description: 在記錄型別之間建立連線後，可以將個別記錄彼此連線。 本文說明在Adobe Workfront Planning中連線記錄時，您必須考慮的事項。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: be51023c-8e11-42e7-aa4f-34484c30eb03
source-git-commit: 22a1525658f4ba60d638d5080f8c178fcf500441
workflow-type: tm+mt
source-wordcount: '558'
ht-degree: 0%

---

# 連線記錄概觀

<span class="preview">本頁醒目提示的資訊指出尚未普遍可用的功能。 它僅在預覽環境中可供所有客戶使用。 每月發行至生產環境後，生產環境中為啟用快速發行的客戶也提供相同的功能。</span>

<span class="preview">如需快速發行資訊，請參閱[為您的組織啟用或停用快速發行](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>

{{planning-important-intro}}

您可以將Adobe Workfront Planning記錄彼此連線，或從其他應用程式連線至物件。

本文說明在Adobe Workfront Planning中連線記錄時，您必須考慮的事項。

如需如何將記錄連結至彼此或另一個物件的詳細資訊，請參閱[連結記錄](/help/quicksilver/planning/records/connect-records.md)。


## 有關連線記錄的考量事項

* 在您連線記錄型別之後，連線的記錄型別會在它們所連結的記錄型別表格中，以及在記錄的頁面上，顯示為連結的記錄欄位。
* 您可以從連結記錄欄位中瀏覽並新增連結記錄的記錄和物件以及物件型別。
* 您可以在連結的記錄型別表格中，新增連結的記錄型別的欄位（查詢欄位）。

  此外，您也可以在您連結的記錄型別表格中，新增您正在連結的記錄型別的欄位（查詢欄位）。

  例如，如果您從促銷活動的記錄型別連結產品的記錄型別，則可以顯示促銷活動的產品欄位，以及產品的促銷活動欄位。
* 您無法手動更新您連結之記錄中的查閱欄位值。

  查詢欄位的值會在原始記錄或物件上更新後，自動填入您正在連結的Workfront Planning記錄。

* 有權存取Workfront Planning和「檢視」或擁有工作區較高許可權的所有人，都可以看見您在記錄之間或記錄與其他應用程式物件之間建立的連線。 無論連線至應用程式的許可權為何，使用者都可以檢視連線的記錄和物件。
* 如果您對連線記錄所在的工作區具有管理許可權，則可以檢視及編輯其他人的連線。
* 您可以將一個記錄連線到另一個應用程式的一或多個物件。視您在連線記錄型別時選取的連線型別而定。 如需詳細資訊，請參閱文章[連線記錄型別概觀](/help/quicksilver/planning/architecture/connect-record-types-overview.md)中的「連線型別」一節。

## 您可以連線記錄的區域

您可以在下列區域將記錄連線到其他記錄，或從其他應用程式連線到物件：

* 您可以在Workfront Planning記錄的下列區域中，將記錄連線至Workfront物件或Experience Manager Assets物件：

   * Planning中記錄型別的表格檢視中的已連線記錄欄位。
   * 記錄的預覽或頁面在詳細資訊索引標籤的已連線記錄欄位中。
   * 記錄在「連線」標籤上的預覽或頁面。

* 您可以在下列區域將Workfront物件連線至Workfront Planning記錄：

   * 從Workfront物件的Planning區段。
   * <span class="preview">從Workfront物件的自訂表單上的Planning連線欄位。</span>

  如需詳細資訊，請參閱[管理來自Workfront物件的記錄連線](/help/quicksilver/planning/records/manage-records-in-planning-section.md)