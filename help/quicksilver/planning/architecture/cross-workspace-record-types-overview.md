---
title: 跨工作區記錄型別概觀
description: 您可以將記錄型別啟用為全域或可連線。 全域記錄型別可以從Adobe Workfront Planning的中央或主要工作區新增至多個工作區，而可連線的記錄型別則可從其本身以外的工作區連線至。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: aeedd871-dcd3-4fb3-bfc5-99db3e7c9296
source-git-commit: f88b6ec019963ff6256e35b9c94eb4d1b7e99730
workflow-type: tm+mt
source-wordcount: '1539'
ht-degree: 0%

---


# 跨工作區記錄型別總覽

<span class="preview">本頁醒目提示的資訊指出尚未普遍可用的功能。 它僅在預覽環境中可供所有客戶使用。 每月發行至生產環境後，生產環境中為啟用快速發行的客戶也提供相同的功能。</span>

<span class="preview">如需快速發行資訊，請參閱[為您的組織啟用或停用快速發行](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>

{{planning-important-intro}}

您可以在Adobe Workfront Planning中為記錄型別啟用跨工作區功能。 可以從多個工作區參考或存取跨工作區記錄型別。

>[!IMPORTANT]
>
>有增強的Workfront套件需求，以便能夠為系統中的記錄型別啟用跨工作區功能。 如需詳細資訊，請參閱[Adobe Workfront Planning存取總覽](/help/quicksilver/planning/access/access-overview.md)。


以下是記錄型別的跨工作區功能：

* <span class="preview">**全域記錄型別**：使用者可以將全域記錄型別新增至他們管理的其他工作區。</span>

* **可連線的記錄型別**：使用者可以從其他工作區連線到此記錄型別。

本文提供跨工作區記錄型別的概觀。 如需有關定義記錄型別的跨工作區功能的資訊，請參閱[設定記錄型別的跨工作區功能](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md)。

<div class="preview">

## 全域記錄型別概觀

全域記錄型別可以從Workfront Planning的中央或主要工作區新增到多個工作區。

針對具有通用工作流程的多團隊組織實作Workfront Planning時，您可能需要為關鍵記錄型別（例如行銷活動或交付專案）定義一致結構和中繼資料，這些記錄型別可以新增到每個團隊的工作區，以擷取和管理其工作。

此外，您可能需要每個團隊的工作彙總到中央層級。

在此類工作流程中，您可以確保團隊在解鎖跨團隊可見度的同時一致地擷取其工作，而不需要將所有內容新增至一個工作區，或組織中的每個人都新增至每個工作區。 您可以使用全域記錄型別來達成此目的。

若要使用全域記錄型別，請執行下列動作：

1. 在您管理的工作區中，將記錄型別設定為全域。

   工作區管理員可以將許可權授予具有Standard授權的使用者或團隊、群組、角色和公司，以將選擇的記錄型別新增到他們管理的工作區。

   原始記錄型別將存在於其原始工作區中，但將顯示在其他工作區中。

   如需詳細資訊，請參閱[設定記錄型別的跨工作區功能](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md)。
1. 從已設定為全域記錄型別的現有工作區中，將記錄型別新增至次要工作區。

   記錄型別將存在於以下工作區中：

   * 它的原始工作區，在工作區中它被指定為全域記錄型別。
   * 次要工作區。

   如需詳細資訊，請參閱[從其他工作區新增現有記錄型別](/help/quicksilver/planning/architecture/add-existing-record-types-from-another-workspace.md)。

   以下各節將說明全域記錄型別的相關考量事項，以及這些記錄在其原始或次要工作區中的運作方式。

### 有關其原始工作區中全域記錄型別的考量事項

設定為全域的記錄型別具有以下屬性：

* 其所有資訊（外觀、原始欄位）只能在原始工作區中編輯。

* 您可以從原始工作區對全域記錄型別執行下列動作：

   * 編輯它

     編輯全域記錄型別包括編輯其外觀、跨工作區功能以及在原始工作區中建立的所有欄位。
   * 建立及管理申請表單
   * 建立及管理自動化

* 只有在全域記錄型別尚未新增至次要工作區時，您才可以將其刪除。 您必須先從次要工作區移除它（透過刪除它），才能從原始工作區刪除它。

  如需詳細資訊，請參閱[刪除記錄型別](/help/quicksilver/planning/architecture/delete-record-types.md)。
* 您新增至全域記錄型別的記錄只會顯示給對其新增所在工作區具有檢視許可權的使用者。
* 您從次要工作區新增的記錄會累計，並顯示在原始工作區中。 原始工作區的所有成員都會獲得其檢視許可權。
* 將原始全域記錄型別新增至多個次要工作區時，會出現下列情況：

   * 原始工作區的成員會自動取得從任何工作區新增之所有記錄的「檢視」許可權，即使他們不是這些工作區的成員。
   * 次要工作區成員只能檢視其所屬工作區的記錄。
* 全域記錄型別的已連線記錄型別將可用於從新增此記錄型別的工作區進行連線。

  例如，如果您的Campaign全域記錄型別與Regions記錄型別有連線，而您將Campaign記錄型別新增至次要工作區，則Regions將變為可從次要工作區連線至跨工作區。 次要工作區成員現在可以建立行銷活動，並將其連結至區域。

* 從原始工作區為全域記錄型別建立的欄位，會從新增記錄型別的所有工作區中顯示。 您只能從原始工作區編輯欄位設定。 在原始工作區中建立的欄位設定在所有成員的次要工作區中是唯讀的，無論其在次要工作區上的許可權為何。 次要工作區管理員無法修改原始工作區中設定的欄位設定。 只有原始工作區的工作區管理員才能修改原始工作區中的欄位設定。

### 關於次要工作區中全域記錄型別的考量事項

* 次要工作區貢獻者可在團隊的工作區中取得全域記錄型別的貢獻許可權。 他們可以從次要工作區新增及管理其中的記錄。

* 次要工作區檢視器可在其團隊的工作區中取得全域記錄型別的檢視許可權。 他們無法新增及管理其中的記錄。

* 次要工作區管理員可以對從次要工作區中的全域記錄型別新增的記錄型別執行下列其他動作：

   * 刪除它。

     從次要工作區中刪除記錄型別只會將其從次要工作區中移除， 也會刪除從次要工作區新增至此的記錄和欄位。 這不會從其原始工作區或已新增記錄型別的任何其他次要工作區中刪除記錄型別。

     如需詳細資訊，請參閱[刪除記錄型別](/help/quicksilver/planning/architecture/delete-record-types.md)。
   * 共用記錄型別的檢視。

     <!-- when they will be able to add fields to the secondary space, this bullet will need this extra information: 
         After adding fields to the global record type in the secondary workspace, shared views might not open for other users in workspaces. The fields exist only in the secondary workspace and they would not be visible in any other workspace. Only fields created in the primary workspace are visible in all secondary workspaces where there the record type is added. -->

  <!--These two capabilities will come later - and edit some of the bullets below after these capabilities are released:
    * Add new fields
        Fields added to a global record from a secondary workspace are visible only from the secondary workspace. 
    * Share it
    * Add request forms to it
    * Add automations to it-->

* 任何使用者都無法在次要工作區中對全域記錄型別執行下列動作：

   * 編輯它

     您無法編輯其外觀、跨工作區功能或從原始工作區新增的欄位。
   * 共用
   * 建立及管理申請表單
   * 建立及管理自動化

* 只有在您擁有下列工作區的「檢視」或更高許可權時，才可從這些工作區看見新增至次要工作區的記錄：

   * 要新增工作區的次要工作區。
   * 全域記錄型別的原始工作區。
   * 新增全域工作區的所有其他工作區。

* 在次要工作區中建立的記錄存在下列情況：

   * 如果您對原始工作區具有「管理」許可權，而對次要工作區沒有許可權，則可以從原始工作區中的次要工作區檢視新增的記錄，但無法從原始工作區管理這些記錄。
   * 如果您對次要工作區具有管理許可權，則可以從全域記錄型別的原始工作區以及新增記錄的次要工作區來管理記錄。
   * 只有在您擁有其他次要工作區的「檢視」許可權時，才能檢視這些工作區中的記錄，在這些工作區中新增了全域記錄型別。

### 存取全域記錄型別的連線

在原始工作區中連線至全域記錄型別的記錄型別，會從已新增全域記錄型別的其他工作區中顯示，並且可用於從已新增全域記錄型別的次要工作區連線。

### 全域記錄型別的API存取

使用Workfront Planning API從次要工作區將記錄新增至全域記錄型別時，系統會檢查使用者是否有權在全域記錄型別的原始工作區中建立記錄。

以下是一些案例：

* 如果使用者具有存取權，則會在全域記錄型別的原始工作區中建立記錄。

* 如果使用者沒有存取權，使用者會收到錯誤，表明他們無權存取全域記錄型別的原始工作區，他們需要提供他們有權建立記錄的工作區ID。

</div>

## 可連線記錄型別的概觀

您可以從您管理的任何工作區連線到已定義為可連線的記錄型別。

您的團隊可能需要將其記錄連結至其他工作區的記錄型別，或檢視屬於其他工作區中記錄之記錄所擷取的資訊。 您可以將記錄型別指定為可連線，以達成此組態。

若要使用可連線的記錄型別，請執行下列動作：

1. 將記錄型別設定為在特定工作區中可連線。

   工作區管理員可以選取指定的記錄型別可以連線到哪些工作區。

   原始記錄型別將存在於其原始工作區中，並且可從另一個工作區存取該原始記錄型別。

   如需詳細資訊，請參閱[設定記錄型別的跨工作區功能](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md)。
1. 從您管理的另一個工作區連線到指定為可連線的記錄型別。

   如需詳細資訊，請參閱[連線記錄型別](/help/quicksilver/planning/architecture/connect-record-types.md)。
