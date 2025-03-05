---
title: 連線記錄型別概觀
description: 指示個別記錄型別如何彼此關聯的一種方法是連線它們。 此外，您可以將Adobe Workfront Planning記錄型別與其他應用程式的物件型別連線起來，以增強您的使用者體驗，並將他們的焦點放在一個應用程式中。
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 1c04c68b-7a7f-46ae-b750-2b1f79855de4
source-git-commit: bddd0dcd2263bd65420a17e4b9cc74336877719f
workflow-type: tm+mt
source-wordcount: '1518'
ht-degree: 1%

---

# 連線記錄型別概觀

<span class="preview">本頁醒目提示的資訊指出尚未普遍可用的功能。 它僅在預覽環境中可供所有客戶使用。 每月發行至生產環境後，生產環境中為啟用快速發行的客戶也提供相同的功能。</span>

<span class="preview">如需快速發行資訊，請參閱[為您的組織啟用或停用快速發行](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>

您可以透過連線個別記錄型別來指示它們彼此相關，或與來自其他應用程式的物件相關。

本文概述記錄型別連線，並說明您可以在記錄與物件型別之間建立的連線型別。

如需有關您連線記錄型別的資訊，請參閱[連線記錄型別](/help/quicksilver/planning/architecture/connect-record-types.md)。

## 有關連線記錄型別的考量事項

在Workfront Planning中連線有兩個步驟：

1. 首先，您必須建立兩個記錄型別之間的連線，或記錄型別與來自另一個應用程式的物件型別。 如需如何連線記錄型別的詳細資訊，請參閱[連線記錄型別](/help/quicksilver/planning/architecture/connect-record-types.md)。
1. 其次，您可以在連線兩種記錄型別之後，將一種型別的個別記錄與另一種型別的記錄連線。 如需有關連線記錄的資訊，請參閱[連線記錄](/help/quicksilver/planning/records/connect-records.md)。

關於連線記錄型別，請考量下列事項：

* 您可以在Adobe Workfront Planning中連線下列實體：

   * 兩種記錄型別。

     依預設，您可以從相同的工作區連線兩種記錄型別。 您也可以設定記錄型別，以便從其他工作區連線記錄型別。 如需詳細資訊，請參閱[編輯記錄型別](/help/quicksilver/planning/architecture/edit-record-types.md)。
   * 來自另一個應用程式的記錄型別和物件型別。

* 您可以從下列應用程式將Workfront Planning記錄型別與下列物件型別連線：

   * Adobe Workfront：

      * 專案
      * 專案組合
      * 計劃
      * 公司
      * 群組

   * Adobe Experience Manager Assets：

      * 影像
      * 資料夾

     >[!IMPORTANT]
     >
     >您必須擁有Adobe Experience Manager Assets授權，且貴組織的Workfront執行個體必須上線至Adobe商業平台或Adobe Admin Console，才能將Workfront Planning記錄連線至Adobe Experience Manager Assets。
     >
     >如果您對加入Adobe Admin Console有任何疑問，請參閱[Adobe統一體驗常見問題集](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/unified-experience-faq.md)。

* 為連線的記錄型別建立記錄後，您可以透過連線的記錄欄位將它們相互連結。  如需詳細資訊，請參閱[連線記錄](/help/quicksilver/planning/records/connect-records.md)。

* 將記錄型別與另一個記錄型別或另一個應用程式的物件型別連線後，就會出現下列情況：

   * **當您連線兩個Planning記錄型別時**：連結的記錄欄位會在您連線的記錄型別上建立。 類似的連結記錄欄位會在您連線的記錄型別上建立。

     例如，如果您將「Campaign」記錄型別與「Product」記錄型別連結，您命名為「Linked Product」的連結記錄欄位（連線欄位）會在Campaign記錄型別上建立。 系統會在產品記錄型別上建立自動命名為「Campaign」的連結記錄型別。

   * **當您從另一個應用程式連線具有物件型別的記錄型別時**：

      * 連結的記錄欄位會在您連線的記錄型別上建立。 不會在其他應用程式的物件型別上自動建立任何連結的記錄欄位。
      * 無法從Workfront物件存取規劃記錄欄位。
      * Planning記錄會顯示於Workfront物件的Planning標籤中。 如需詳細資訊，請參閱[管理來自Workfront物件的記錄連線](/help/quicksilver/planning/records/manage-records-in-planning-section.md)。
      * <span class="preview">您可以建立Planning連線自訂欄位，並將其附加至Workfront物件的自訂表單。 如需詳細資訊，請參閱[建立自訂表格](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)。</span>
      * 當您的Experience Manager管理員透過Workfront與Adobe Experience Manager Assets之間的整合設定中繼資料對應時，可從Workfront資產存取規劃記錄欄位。 如需詳細資訊，請參閱[設定Adobe Workfront與Experience Manager Assets之間的資產中繼資料對應](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping.html?lang=en)。


   * **當您從您連線的記錄或物件加入查閱欄位時**：除了建立連結的記錄欄位之外，您還可以從連線的記錄或物件型別連線到稱為查閱欄位的欄位。 連結（或查詢欄位）的資訊，來自於您所連線的記錄，顯示在您所連線的記錄上。

     您可以將其他記錄型別或其他應用程式物件的欄位連線到Workfront Planning記錄型別。

     連結欄位是唯讀的，會自動顯示連線記錄的資訊。

     您可以在公式、篩選器或群組中參照其他記錄或物件型別的查閱欄位。

     例如，如果您將「行銷活動」記錄型別與Workfront專案連線，並且選擇將專案的「計畫完成日期」欄位帶入Workfront計畫記錄，則系統會自動為行銷活動建立名為「計畫完成日期」（來自「專案」）的連結欄位。 您無法手動編輯此連結的欄位。 計畫完成日期（來自專案）欄位會顯示連結專案的計畫完成日期。

     >[!IMPORTANT]
     >
     >擁有工作區檢視或較高許可權的每個人皆可檢視查閱欄位中的資訊，無論其在連結物件型別應用程式中的許可權或存取層級，或其在其他工作區的許可權為何。

     連結的記錄欄位前面有關聯圖示![](assets/relationship-field-icon.png)。

     連結的欄位前面有識別欄位型別的圖示。 例如，連結（或查詢）欄位前面有圖示，表示欄位是數字、段落或日期。

## 連線型別

在兩個記錄型別之間或記錄與來自另一個應用程式的物件型別之間建立連線後，您可以在連線的記錄欄位中新增記錄。

根據您可將多少筆記錄新增至已連線的記錄欄位，在連線記錄型別時，您可以選擇下列連線型別：

* [多對多](#many-to-many-connection-type)
* [一對多](#one-to-many-connection-type)
* [多對一](#many-to-one-connection-type)
* [一對一](#many-to-one-connection-type)

>[!WARNING]
>
>連線下列專案時，無法使用這些選項：
>
>* 來自不同工作區的兩個記錄
>
>* 記錄型別和Experience Manager資產

### 多對多連線型別

![](assets/many-to-many-connection-picker.png)

當您在記錄型別之間建立多對多連線時，您可以從兩種記錄型別中選取連線欄位中的多個記錄。

例如，如果您在行銷活動和專案之間建立多對多連線，您可以為每個行銷活動選取多個專案，並為每個專案選取多個行銷活動。

電影和演員之間的關係是現實生活中多對多關係型別的一個例子。 每部電影可以有多位演員，每位演員都可以在多部電影中播放。

當您選取此連線型別時，您無法在儲存後變更連線型別。

### 一對多連線型別

![](assets/one-to-many-connection-picker.png)


當您在記錄型別之間建立一對多連線時，您接著可以在目前記錄型別的連線欄位中選取多個記錄，但您連線的記錄型別中對應的連線欄位將只允許選取一個記錄。 在第二個記錄型別上自動建立的已連線記錄欄位會自動設定為多對一關係型別。

例如，如果您在行銷活動和專案之間建立一對多連線，您可以為每個行銷活動選取多個專案，但每個專案只能連線至一個行銷活動。

現實中一對多關係型態的一個範例是圖書館與書籍之間的關係：圖書館的詳細目錄中有許多書籍；但在特定時間點，一個特定書籍只能位於一個圖書館中。

當您選取此連線型別時，您稍後可以將其變更為多對多連線型別。

### 多對一連線型別

![](assets/many-to-one-connection-picker.png)


當您在記錄型別之間建立多對一連線時，您就可以只用所連線記錄型別中的一個記錄來連線目前記錄型別中的每個記錄。 在第二個記錄型別上自動建立的已連線記錄欄位會自動設定為一對多關係型別。

例如，如果您將行銷活動與專案連線，並選擇這種連線型別，您只能將一個專案新增至行銷活動。 但您可以將多個行銷活動新增至一個專案。

現實生活中，許多電影與一個演員之間的關係就是多對一關係的例子：一個演員可以出現在許多電影中，但每部電影的演員中只能有一個特定的演員。

當您選取此連線型別時，您稍後可以將其變更為多對多連線型別。

### 一對一連線型別

![](assets/one-to-one-connection-picker.png)

當您在記錄型別之間建立一對一連線時，在這兩種記錄型別中，您只能將每筆記錄與另一記錄型別中的一個記錄連線。

例如，如果您將行銷活動與專案連線，並選擇這種連線型別，您就可以將一個行銷活動與一個專案連線。 一個專案只能連線至一個行銷活動。

一對一關係的實際例子，是個人與其國家/地區的唯一識別碼（例如社會保險號碼、護照ID、當地識別碼ID）之間存在的關係：每個人/地區只有一個唯一識別碼，每個唯一識別碼只能連結至一個人。

當您選取此連線型別時，您稍後可以將其變更為任何其他連線型別。
