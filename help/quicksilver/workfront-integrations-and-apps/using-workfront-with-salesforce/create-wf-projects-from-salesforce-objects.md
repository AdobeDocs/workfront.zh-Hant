---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-salesforce
title: 從 [!DNL Salesforce] 物件建立 [!DNL Adobe Workfront] 專案
description: 安裝Salesforce的 [!DNL Adobe Workfront] 之後，您可以定義在 [!DNL Salesforce] 商機與帳戶上符合某些條件時建立 [!DNL Workfront] 專案的觸發程式。
author: Becky
feature: Workfront Integrations and Apps
exl-id: b38c91ae-342b-4002-a947-7a0ab1aaca93
source-git-commit: ad2fc27db2a19ea231e925d5991dbef27ea48030
workflow-type: tm+mt
source-wordcount: '1496'
ht-degree: 3%

---

# 從[!DNL Salesforce]物件建立[!DNL Adobe Workfront]個專案

安裝Salesforce的[!DNL Adobe Workfront]之後，您可以定義在[!DNL Salesforce] [!UICONTROL 機會]和[!UICONTROL 帳戶]上符合某些條件時，建立[!DNL Workfront]專案的觸發器。

## 存取需求

您必須具有下列存取權才能使用本文所述的功能：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計畫*</td> 
   <td> <p>[！UICONTROL Pro]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權*</td> 
   <td> <p>[！UICONTROL計畫]</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的[!DNL Workfront]管理員。

## 先決條件

若要提交來自[!DNL Salesforce] [!UICONTROL 機會]或帳戶的[!DNL Workfront]要求
確保您的環境中有以下專案：

* 您的[!DNL Workfront]系統管理員已安裝[!DNL Workfront for Salesforce]。\
   如需有關安裝[!DNL Workfront for Salesforce]的詳細資訊，請參閱[安裝 [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md)

* 您的[!DNL Workfront]管理員已將[!DNL Workfront]區段新增至您的[!UICONTROL 機會]和帳戶
頁面配置。\
   如需有關將[!DNL Workfront]區段新增至版面配置的詳細資訊，請參閱[為 [!DNL Salesforce] 使用者設定 [!DNL Adobe Workfront] 區段](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md)。

* 您有[!DNL Workfront]帳戶，可以從[!UICONTROL 機會]或帳戶內的[!DNL Workfront]區段登入該帳戶
.

## 正在設定從[!DNL Salesforce]建立[!DNL Workfront]個專案

* [瞭解專案的自動建立](#understanding-the-automatic-creation-of-projects-understanding-the-automatic-creation-of-projects)
* [設定觸發程式](#configuring-triggers-configuring-triggers)
* [瞭解專案名稱](#understanding-project-names-understanding-project-names)

### 瞭解專案的自動建立 {#understanding-the-automatic-creation-of-projects}

作為[!DNL Salesforce]系統管理員，您可以定義在[!DNL Salesforce]中發生下列情況時，可在[!DNL Workfront]中自動建立專案的觸發器：

* [!UICONTROL 商機]的[!UICONTROL 階段]已更新。
* 帳戶的[!UICONTROL 型別]
已更新。

只有在您已安裝[!DNL Workfront for Salesforce]之後，才能設定觸發程式。  \
如需有關安裝[!DNL Workfront for Salesforce]的資訊，請參閱[安裝 [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md)。

在建立或更新[!DNL Salesforce]專案時，在設定觸發程式以自動建立[!DNL Workfront]專案時，請考慮下列事項：

* 您必須是[!DNL Salesforce]和[!DNL Workfront]系統管理員才能設定觸發器。
* 在您設定觸發程式後，任何更新[!UICONTROL 機會]的[!UICONTROL 階段]或帳戶的[!UICONTROL 型別]的人
可觸發建立[!DNL Workfront]專案。 這包含沒有[!DNL Workfront]帳戶的[!DNL Salesforce]位使用者。
* 您可以使用的觸發器數量沒有限制。
* 您無法根據相同條件建立多個觸發器。 依預設，觸發器是唯一的。
* 專案建立後，就會自動連結至機會或產生專案的帳戶。 建立後，此連結便無法中斷。
* 當在機會或帳戶的生命週期中多次符合觸發的條件時，一個機會或帳戶可以連結到[!DNL Workfront]中的多個專案。

  例如，如果您為[!UICONTROL 商機]定義一個以上的[!UICONTROL 階段]以觸發專案，則會針對該商機所達到的每個已定義階段，在該商機的生命週期內建立專案。 此外，如果您將[!UICONTROL 商機]的[!UICONTROL 階段]從一個已定義的階段更新至另一個階段，然後更新回已定義的階段，則會在您第二次將[!UICONTROL 階段]欄位更新至相同的已定義階段時，建立第二個專案。

* [!DNL Workfront]中的一個專案在任何指定時間只能連結到[!DNL Salesforce]中的一個機會或一個帳戶，但不能同時連結到兩者。

### 設定觸發程式 {#configuring-triggers}

一旦設定觸發程式，[!UICONTROL Salesforce Classic]或[!DNL Lightning Experience]架構就會啟用建立[!DNL Workfront]專案的程式。

若要在[!UICONTROL Salesforce]中設定觸發程式：

1. 以系統管理員身分登入[!DNL Salesforce]。
1. （條件式）在[!DNL Salesforce Classic]中，按一下&#x200B;**[!UICONTROL 設定]**，然後在&#x200B;**[!UICONTROL 建置]**&#x200B;區段下，展開&#x200B;**[!UICONTROL 閃電]**。

   或

   在[!DNL Salesforce] Lightning Experience中，按一下&#x200B;**[!UICONTROL 設定]圖示**，然後按一下&#x200B;**[!UICONTROL 設定]**，並在&#x200B;**[!UICONTROL 平台工具]**&#x200B;下方展開&#x200B;**[!UICONTROL 應用程式]**。

1. 按一下&#x200B;**[!UICONTROL 已安裝的封裝]**。

   請注意，**[!DNL Workfront]**&#x200B;套件已經安裝。

1. 按一下&#x200B;**[!DNL Workfront]**&#x200B;旁的&#x200B;**[!UICONTROL 設定]**。

1. 以系統管理員身分登入[!DNL Workfront]。

   顯示&#x200B;**[!UICONTROL Triggers]**&#x200B;頁面。

   ![salesforce_triggers_page_empty.png](assets/salesforce-triggers-page-empty-350x134.png)

1. 按一下&#x200B;**[!UICONTROL 新增觸發器]**。
1. 從&#x200B;**[!UICONTROL [!DNL Salesforce]物件]**&#x200B;下拉式功能表中，選取&#x200B;**[!UICONTROL 機會]**。

   這是必填欄位。

1. （視條件而定）指定下列專案：

   1. 從&#x200B;**[!UICONTROL 階段]**&#x200B;下拉式功能表中，選取&#x200B;**[!UICONTROL 階段]**。\

      當機會到達此處指定的[!UICONTROL 階段]時，會在[!DNL Workfront]中建立專案。 這是必填欄位。

   1. 在&#x200B;**[!UICONTROL Portfolio或方案]**&#x200B;欄位中，開始輸入您要將專案放置在[!DNL Workfront]中的Portfolio或方案名稱，然後在其出現在清單中時選取它。\

      如果您未指定Portfolio或計畫，則會建立新專案，並在設定觸發程式時將其新增至登入[!DNL Workfront]之使用者的[!UICONTROL 我擁有的專案]清單。 該使用者也是新專案的專案所有者。

   1. 開始輸入您要與新[!DNL Workfront]專案關聯的範本名稱，然後在其出現在清單中時選取它。\

      這是必填欄位。


      >[!NOTE]
      >
      >如果您已在您計畫用於此整合的範本上指定範本所有者，則該範本所有者會成為新專案的專案所有者。 根據範本，新專案會顯示在新專案擁有者的使用者[!UICONTROL 我擁有的專案]清單下。

   1. （選擇性）如果您想要為任何一個銷售機會下銷售的每種產品型別建立新專案，請選取&#x200B;**[!UICONTROL 為每個銷售的產品型別建立新專案]欄位**。
   1. （視條件而定）在&#x200B;**[!UICONTROL 產品]**&#x200B;下拉式功能表中選取&#x200B;**[!UICONTROL 產品]**。

      這是必填欄位。

   1. （視條件而定）如果指定的產品位於[!UICONTROL 機會]上，請開始輸入您要與新[!DNL Workfront]專案關聯的&#x200B;**[!UICONTROL 範本]**&#x200B;名稱。 當它出現在清單中時選取它。

      這是必填欄位。

      將新產品新增至[!DNL Salesforce]機會時所建立的專案放在為機會選取的相同Portfolio或方案中。

      >[!IMPORTANT]
      >
      >專案只有在[!UICONTROL 機會]上更新階段時才會建立。 為更新「階段」欄位時指定的每個產品建立唯一的專案，而不是因為產品已新增到[!UICONTROL 機會]。

1. （選擇性）按一下&#x200B;**[!UICONTROL 新增觸發器]**。
1. （選擇性）從&#x200B;**[!UICONTROL [!DNL Salesforce]物件]**下拉式功能表中，選取**帳戶
**。

   這是必填欄位。
1. （視條件而定）指定下列專案：

   1. 從&#x200B;**[!UICONTROL 型別]**&#x200B;下拉式功能表中選取&#x200B;**[!UICONTROL 型別]**。

      任何**Account時
**被指定為[!DNL Salesforce]中在此指定的&#x200B;**[!UICONTROL 型別]**，在[!DNL Workfront]中建立了一個&#x200B;**[!UICONTROL 專案]**。

      這是必填欄位。

   1. （選擇性）開始輸入&#x200B;**[!UICONTROL Portfolio]**&#x200B;或&#x200B;**[!UICONTROL 方案]**&#x200B;的名稱，您要將專案放置在&#x200B;**[!UICONTROL Portfolio或方案]**&#x200B;欄位的[!DNL Workfront]中，然後當它出現在清單中時選取它。

      若您未指定Portfolio或方案，則會建立新專案並將其新增至從[!DNL Salesforce]登入[!DNL Workfront]之使用者的&#x200B;**[!UICONTROL 我擁有的專案]**&#x200B;清單中。 使用者也是新專案的專案所有者。

   1. 開始輸入您想要與新[!DNL Workfront]專案關聯的&#x200B;**[!UICONTROL 範本]**&#x200B;名稱，然後在其出現在清單中時選取它。

      這是必填欄位。

      >[!NOTE]
      >
      >如果您已在您計畫用於此整合的範本上指定範本所有者，則該範本所有者會成為新專案的專案所有者。 根據範本，新專案會顯示在新專案擁有者的使用者&#x200B;**[!UICONTROL 我擁有的專案]**&#x200B;清單下。

   ![salesforce_triggers_page_with_cleaned_up_template_names.png](assets/salesforce-triggers-page-with-cleaned-up-template-names-350x157.png)

1. 按一下「**[!UICONTROL 儲存]**」。

   現在會在每次符合觸發程式時產生[!DNL Workfront]個專案。

### 瞭解專案名稱 {#understanding-project-names}

根據產生專案的觸發器，[!DNL Workfront]中的專案名稱可能會遵循下列其中一種模式：

* 如果專案是根據商機或帳戶觸發程式所建立，則專案名稱為： *`<Salesforce object name>`： `<Project template name>` （透過[!DNL Salesforce]）*。
* 如果專案是根據同時包含新增「產品」的機會觸發程式所建立，則專案名稱為： *`<Salesforce object name>`： `<Salesforce product name>` （透過[!DNL Salesforce]）*。

## 檢視[!DNL Workfront]個專案

若您的[!DNL Workfront]管理員已將[!DNL Workfront]區段新增至您的[!UICONTROL 商機]或帳戶
頁面配置，您可以看到在此區段的[!UICONTROL 專案]索引標籤中自動建立的專案。\
如需將[!DNL Workfront]區段新增至[!UICONTROL 機會]或帳戶的頁面配置的詳細資訊
，請參閱[設定 [!DNL Salesforce] 使用者的 [!DNL Adobe Workfront] 區段](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md)。

您必須擁有[!DNL Workfront]帳戶並登入[!DNL Workfront]，才能檢視[!UICONTROL 專案]索引標籤。

若要檢視從[!UICONTROL 商機]或帳戶建立的專案
：

1. 移至[!UICONTROL 商機]或帳戶
.
1. 移至&#x200B;**[!DNL Workfront]**&#x200B;區段。

   >[!NOTE]
   >
   >根據您的[!DNL Workfront]管理員設定此區段的方式，它可能有不同的名稱。

1. 選取&#x200B;**[!UICONTROL 專案]**&#x200B;索引標籤。

   此標籤會列出所有由已定義觸發器建立的專案。 任何在[!DNL Salesforce]中同時擁有[!DNL Workfront]帳戶且可能有權在[!DNL Workfront]中檢視這些專案的使用者，也可以在[!UICONTROL 機會]或帳戶的[!DNL Salesforce]中檢視它們
產生這些事件的人。

   您可以檢視下列整合所建立專案的相關資訊：

   * 專案名稱
   * 參考號碼
   * 輸入日期
   * 擁有者的名稱
   * 狀態
   * 狀況
   * 規劃完成日期
   * 完成百分比

     在[!DNL Workfront]中更新此資訊時，您可以看到此清單中已更新的欄位。

1. （選用）按一下專案名稱，以在Workfront中開啟。
1. （選擇性）按一下[!UICONTROL 專案詳細資料]區域或專案標題中的[!UICONTROL **[!UICONTROL 移至Salesforce]**]以存取[!UICONTROL 機會]或帳戶
專案的來源。 您的系統或群組管理員必須新增[!UICONTROL 整合]欄位至您的版面配置範本，才能在專案標題中找到。

   >[!NOTE]
   >
   >所有[!DNL Workfront]個可以檢視專案的使用者皆可看到[!UICONTROL 移至Salesforce]連結。 您必須有[!DNL Salesforce]帳戶才能前往產生專案的[!DNL Salesforce]商機或帳戶。
