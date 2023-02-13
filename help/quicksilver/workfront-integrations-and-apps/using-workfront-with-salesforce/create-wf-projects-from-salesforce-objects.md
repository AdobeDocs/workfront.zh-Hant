---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-salesforce
title: 建立 [!DNL Adobe Workfront] 項目來源 [!DNL Salesforce] 物件
description: 安裝後 [!DNL Adobe Workfront] 對於Salesforce，您可以定義建立 [!DNL Workfront] 符合特定條件的專案 [!DNL Salesforce] 機會和客戶。
author: Becky
feature: Workfront Integrations and Apps
exl-id: b38c91ae-342b-4002-a947-7a0ab1aaca93
source-git-commit: 5b889633a96d634a359181bfd53ec106b0f3705c
workflow-type: tm+mt
source-wordcount: '1507'
ht-degree: 3%

---

# 建立 [!DNL Adobe Workfront] 項目來源 [!DNL Salesforce] 物件

安裝後 [!DNL Adobe Workfront] 對於Salesforce，您可以定義建立 [!DNL Workfront] 符合特定條件的專案 [!DNL Salesforce] [!UICONTROL 機會] 和 [!UICONTROL 帳戶].

## 存取需求

您必須具備下列存取權，才能使用本文所述的功能：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計劃*</td> 
   <td> <p>[!UICONTROL Pro]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權*</td> 
   <td> <p>[!UICONTROL計畫]</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的 [!DNL Workfront] 管理員。

## 必要條件

提交 [!DNL Workfront] 來自 [!DNL Salesforce] [!UICONTROL 機會] 或帳戶確保您的環境中有下列項目：

* 您的 [!DNL Workfront] 已安裝管理員 [!DNL Workfront for Salesforce].\
   有關安裝的詳細資訊 [!DNL Workfront for Salesforce]，請參閱 [安裝 [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md)

* 您的 [!DNL Workfront] 管理員已新增 [!DNL Workfront] 區段 [!UICONTROL 機會] 和帳戶頁面配置。\
   如需新增 [!DNL Workfront] 區段至頁面配置，請參閱 [設定 [!DNL Adobe Workfront] 區段 [!DNL Salesforce] 使用者](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

* 您有 [!DNL Workfront] 帳戶，您可從 [!DNL Workfront] 區段 [!UICONTROL 機會] 或帳戶。

## 配置建立 [!DNL Workfront] 來自 [!DNL Salesforce]

* [了解自動建立專案](#understanding-the-automatic-creation-of-projects-understanding-the-automatic-creation-of-projects)
* [設定觸發器](#configuring-triggers-configuring-triggers)
* [了解專案名稱](#understanding-project-names-understanding-project-names)

### 了解自動建立專案 {#understanding-the-automatic-creation-of-projects}

作為 [!DNL Salesforce] 系統管理員，您可以定義觸發器，以自動在 [!DNL Workfront] 當 [!DNL Salesforce]:

* 此 [!UICONTROL 階段] a [!UICONTROL 機會] 已更新。
* 此 [!UICONTROL 類型] 帳戶的名稱。

只有在您安裝後，才可設定觸發器 [!DNL Workfront for Salesforce].  \
有關安裝的資訊 [!DNL Workfront for Salesforce]，請參閱 [安裝 [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md).

將觸發器設定為自動建立時，請考量下列事項 [!DNL Workfront] 專案時 [!DNL Salesforce] 項目已建立或更新：

* 您必須是 [!DNL Salesforce] 和 [!DNL Workfront] 系統管理員來設定觸發器。
* 設定觸發器後，任何更新 [!UICONTROL 階段] a [!UICONTROL 機會] 或 [!UICONTROL 類型] 帳戶可觸發建立 [!DNL Workfront] 專案。 包括 [!DNL Salesforce] 沒有 [!DNL Workfront] 帳戶。
* 您可以擁有的觸發器數量沒有限制。
* 您無法根據相同的條件建立多個觸發器。 預設情況下，觸發器是唯一的。
* 建立項目後，它將自動連結到生成該項目的機會或帳戶。 建立後，此連結就無法中斷。
* 一個機會或帳戶可以連結到 [!DNL Workfront] 在機會或帳戶的生命週期中多次滿足觸發條件時。

   例如，如果您定義多個 [!UICONTROL 階段] 對於 [!UICONTROL 機會] 要觸發項目，將為該機會到達的每個定義階段建立一個項目，以在該機會的生命週期中觸發。 此外，如果您更新 [!UICONTROL 階段] a [!UICONTROL 機會] 從一個定義的階段更新到另一個，然後將其更新回定義的階段，在您第二次更新時將建立第二個專案 [!UICONTROL 階段] 欄位至相同定義的階段。

* 一個專案 [!DNL Workfront] 只能連結到 [!DNL Salesforce] 在任何特定時間，但不能同時對兩者。

### 設定觸發器 {#configuring-triggers}

設定觸發器後，建立 [!DNL Workfront] 同時為兩者啟用專案 [!UICONTROL Salesforce Classic] 或 [!DNL Lightning Experience] 框架。

若要在中設定觸發器 [!UICONTROL Salesforce]:

1. 登入 [!DNL Salesforce] 作為系統管理員。
1. （有條件）輸入 [!DNL Salesforce Classic]，按一下 **[!UICONTROL 設定]**，在 **[!UICONTROL 建置]** 區段，展開 **[!UICONTROL 閃電]**.

   或

   在 [!DNL Salesforce] 閃電體驗，按一下 **[!UICONTROL 設定] 圖示**，然後 **[!UICONTROL 設定]**，在 **[!UICONTROL 平台工具]** 展開 **[!UICONTROL 應用程式]**.

1. 按一下 **[!UICONTROL 已安裝的軟體包]**.

   請注意， **[!DNL Workfront]** 已安裝軟體包。

1. 按一下 **[!UICONTROL 設定]** 下一頁 **[!DNL Workfront]**.

1. 登入 [!DNL Workfront] 作為系統管理員。

   此 **[!UICONTROL 觸發器]** 頁面。

   ![salesforce_triggers_page_empty.png](assets/salesforce-triggers-page-empty-350x134.png)

1. 按一下 **[!UICONTROL 新觸發程式]**.
1. 從 **[!UICONTROL [!DNL Salesforce]物件]** 下拉式功能表，選取 **[!UICONTROL 機會]**.

   這是必填欄位。

1. （條件性）指定下列項目：

   1. 從 **[!UICONTROL 階段]** 下拉式功能表，選取 **[!UICONTROL 階段]**.\

      當機會到達 [!UICONTROL 階段] 在此指定，將在 [!DNL Workfront]. 這是必填欄位。

   1. 在 **[!UICONTROL Portfolio或方案]** 欄位中，開始鍵入要放置項目的Portfolio或方案的名稱 [!DNL Workfront]，然後在清單中出現時選取它。\

      如果您未指定Portfolio或方案，則會建立新專案並新增至 [!UICONTROL 我擁有的專案] 登入的使用者清單 [!DNL Workfront] 設定觸發器時。 該用戶也是新項目的項目所有者。

   1. 開始鍵入要與新模板關聯的模板的名稱 [!DNL Workfront] 項目，然後在項目出現在清單中時選擇它。\

      這是必填欄位。


      >[!NOTE]
      >
      >如果您已在計畫用於此整合的模板上指定了「模板所有者」，則該模板將成為新項目的「項目所有者」。 新專案會顯示在 [!UICONTROL 我擁有的專案] 根據範本，屬於新專案擁有者的使用者清單。

   1. （選用）選取 **[!UICONTROL 為每個銷售的產品類型建立新項目] 欄位**，如果您想要為在任何一個銷售機會下銷售的每種產品類型建立新項目。
   1. （條件性）選取 **[!UICONTROL 產品]** 在 **[!UICONTROL 產品]** 下拉式功能表。

      這是必填欄位。

   1. （條件性）開始輸入 **[!UICONTROL 範本]** 與新 [!DNL Workfront] 項目(若指定的產品位於 [!UICONTROL 機會]. 在清單中出現時選取它。

      這是必填欄位。

      將新產品新增至 [!DNL Salesforce] 將opportunity放在為opportunity選擇的同一Portfolio或程式中。

      >[!IMPORTANT]
      >
      >只有在 [!UICONTROL 機會]. 在更新「階段」欄位時，會為每個指定的產品建立唯一的專案，而不是在產品新增至 [!UICONTROL 機會].

1. （選用）按一下 **[!UICONTROL 新觸發程式]**.
1. （選用）從 **[!UICONTROL [!DNL Salesforce]物件]** 下拉式功能表，選取**帳戶**。

   這是必填欄位。
1. （條件性）指定下列項目：

   1. 選取 **[!UICONTROL 類型]** 從 **[!UICONTROL 類型]** 下拉式功能表。

      任何**帳**指定為 **[!UICONTROL 類型]** 在此處指定 [!DNL Salesforce], **[!UICONTROL 專案]** 在中建立 [!DNL Workfront].

      這是必填欄位。

   1. （選用）開始輸入 **[!UICONTROL Portfolio]** 或 **[!UICONTROL 方案]** 您希望將專案放置於 [!DNL Workfront] 在 **[!UICONTROL Portfolio或方案]** 欄位，然後在清單中出現時選取它。

      如果您未指定Portfolio或方案，則會建立新專案並新增至 **[!UICONTROL 我擁有的專案]** 登入的使用者清單 [!DNL Workfront] 從 [!DNL Salesforce]. 使用者也是新專案的專案擁有者。

   1. 開始輸入 **[!UICONTROL 範本]** 與新 [!DNL Workfront] 項目，然後在項目出現在清單中時將其選中。

      這是必填欄位。

      >[!NOTE]
      >
      >如果您已在計畫用於此整合的模板上指定了「模板所有者」，則該模板將成為新項目的「項目所有者」。 新專案會顯示在 **[!UICONTROL 我擁有的專案]** 根據範本，屬於新專案擁有者的使用者清單。
   ![salesforce_triggers_page_with_cleaned_up_template_names.png](assets/salesforce-triggers-page-with-cleaned-up-template-names-350x157.png)

1. 按一下&#x200B;**[!UICONTROL 儲存]**。

   [!DNL Workfront] 現在，只要符合任何觸發器，就會產生專案。

### 了解專案名稱 {#understanding-project-names}

根據產生專案的觸發器，中的專案名稱 [!DNL Workfront] 可能會遵循以下任一模式：

* 如果根據業務機會或帳戶觸發器建立項目，則項目的名稱為： *`<Salesforce object name>`: `<Project template name>` (透過 [!DNL Salesforce])*.
* 如果根據包括添加新產品的機會觸發器建立項目，則項目的名稱為： *`<Salesforce object name>`: `<Salesforce product name>` (透過 [!DNL Salesforce])*.

## 檢視 [!DNL Workfront] 專案

若您的 [!DNL Workfront] 管理員已新增 [!DNL Workfront] 區段 [!UICONTROL 機會] 或帳戶頁面配置，您可以在 [!UICONTROL 專案] 頁簽。\
如需新增 [!DNL Workfront] 區段至 [!UICONTROL 機會] 或帳戶，請參閱 [設定 [!DNL Adobe Workfront] 區段 [!DNL Salesforce] 使用者](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

您必須有 [!DNL Workfront] 帳戶和登入 [!DNL Workfront] 若要檢視 [!UICONTROL 專案] 標籤。

檢視從 [!UICONTROL 機會] 或帳戶：

1. 前往 [!UICONTROL 機會] 或帳戶。
1. 前往 **[!DNL Workfront]** 區段。

   >[!NOTE]
   >
   >視您的 [!DNL Workfront] 管理員已配置此部分，其名稱可能不同。

1. 選取 **[!UICONTROL 專案]** 標籤。

   此索引標籤會列出由定義觸發器建立的所有專案。 中的任何使用者 [!DNL Salesforce] 也有 [!DNL Workfront] 帳戶，以及有權查看下列專案的使用者 [!DNL Workfront] 也可以在 [!DNL Salesforce] 針對 [!UICONTROL 機會] 或產生這些帳戶的帳戶。

   ![[!DNL salesforce_projects_tab_with_projects_listed].png](assets/salesforce-projects-tab-with-projects-listed-350x150.png)

   您可以檢視下列整合所建立專案的相關資訊：

   * 專案名稱
   * 參考號碼
   * 輸入日期
   * 所有者名稱
   * 狀態
   * 狀況
   * 計畫完成日期
   * 完成百分比

      此資訊在 [!DNL Workfront]，您就會看到此清單中更新的欄位。

1. （選用）按一下專案名稱，以在Workfront中開啟。
1. （選用）按一下 [!UICONTROL **[!UICONTROL 轉到Salesforce]**] 在 [!UICONTROL 專案詳細資料] 區域或專案標題來存取 [!UICONTROL 機會] 或專案發源地的帳戶。 您的系統或群組管理員必須將 [!UICONTROL 整合] 欄位中找到，以便在專案標題中找到。

   >[!NOTE]
   >
   >此 [!UICONTROL 轉到Salesforce] 連結可顯示給所有 [!DNL Workfront] 可檢視專案的使用者。 您必須有 [!DNL Salesforce] 帳戶，才能前往 [!DNL Salesforce] 生成項目的位置的機會或帳戶。
