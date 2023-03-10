---
product-previous: workfront-proof
product-area: documents
navigation-topic: automated-workflow-workfront-proof
title: 在 [!DNL Workfront Proof]
description: 這會重複在Workfront中設定校樣中找到的資訊。 在這裡或那裡整合。 也許這裡更好。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 605569df-8e63-476d-a0cd-e73802042011
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '1637'
ht-degree: 0%

---

# 在 [!DNL Workfront Proof]

>[!IMPORTANT]
>
>本文說明獨立產品中的功能 [!DNL Workfront Proof]. 有關內部校對的資訊 [!DNL Adobe Workfront]，請參閱 [校對](../../../review-and-approve-work/proofing/proofing.md).

當您有複雜的審核流程，或者您定期將要審核的內容發送給相同的人員組時，自動化工作流可讓您更輕鬆地管理內容審核和批准。

您會建立校樣，然後它會從舞台移至舞台，直到最終核准。 需要批准時，會通知相關用戶。

![phates_diagram.png](assets/stages-diagram-350x81.png)

您可以在上傳檔案或上傳檔案後，將自動化工作流程新增至校樣。

## 使用自動化工作流程建立校樣

1. 開始建立校樣。
1. 在 **[!UICONTROL 共用]** ，按一下 **[!UICONTROL 使用自動化工作流]**.

   您可以取消選取此選項，以切換回標準工作流程。

1. （可選）如果您想使用自動化工作流程範本， [!DNL Workfront] 管理員已配置並與您共用，請在 **[!UICONTROL 選擇工作流模板]** 下拉式功能表。

   >[!NOTE]
   >
   >修改範本的能力取決於 [!DNL Workfront] 管理員。 如果禁用了修改模板的功能，則只有模板的所有者才能修改它。

1. 指定下列資訊以設定自動化工作流程的第一階段：

   * **[!UICONTROL 名稱]:** 階段名稱會顯示在工作流圖表上，並包含在發送給審核者的電子郵件通知中。
   * **[!UICONTROL 截止時間]:** 此欄位的功能會因您在 **[!UICONTROL 根據]** 下拉式清單。

   * **[!UICONTROL 從校樣建立]:** 選擇校樣的截止日期。
   * **[!UICONTROL 從啟動階段]:** 選取要新增至階段啟動日期的工作天數，以自動設定校樣的截止日期。
   * **[!UICONTROL 啟動階段]:** 對於工作流程的每個階段，您可以決定其應啟動的時間。 對於您的第一個階段，可使用下列選項。

      * 論校樣建立
      * 在特定時間和日期
      * 手動\

         後續階段可使用其他選項。 這些選項需要父級階段。 它們是：
      * 在達到之前的截止日期之後
      * 所有決策均為「已核准」或「已核准」，且有所變更
      * 所有決定均獲批准
      * 所有決定都是
   * **[!UICONTROL 根據]:** 您在此下拉式清單中選取的選項會影響 **[!UICONTROL 截止時間]** 欄位。

   * **[!UICONTROL 校樣建立]:** 在 **[!UICONTROL 截止時間]** 欄位，選擇校樣的截止日期。

   * **[!UICONTROL 階段啟動]:** 在 **[!UICONTROL 截止時間]** 欄位中，選取要新增至階段啟動日期的工作天數，以自動設定校樣的截止日期。

   * **[!UICONTROL 鎖台]:** 選擇何時可以鎖定舞台。
   * **[!UICONTROL 主要決策者]:** 在舞台上選擇主決策者。 只有在將審核者添加到舞台後，決策者才可在下拉清單中使用。
   * **[!UICONTROL 只需一個決定]:** 選擇此選項，以便在某個決策者做出決策後完成審核。\

      如果您在 **[!UICONTROL 主要決策者]** 下拉式功能表。

   * **[!UICONTROL 私人舞台]:** 選取此選項時，未添加到此階段或帳戶中不是主管、管理員或帳單管理員的人員將看不到評論和決策


1. （可選）將審核者添加到舞台。
1. 添加審核者時，請考慮以下事項：

   * 審核者只能添加到校樣一次。 （您無法將同一個人新增至校樣的多個階段。）
   * 被添加到私人舞台的審核者只能看到在該舞台上添加的校樣和評論。
   * 依預設，將使用者新增至階段會授予使用者從建立校樣開始即可檢視校樣的存取權。\

      系統管理員可以配置校對系統，以限制用戶訪問校樣，直到工作流進入添加用戶的階段。 如需詳細資訊，請參閱

1. （選用）按一下 **[!UICONTROL 新階段]**，然後重複步驟4和步驟5，將多個階段新增至自動化工作流程。
1. 在 [!UICONTROL 組織] 和 [!UICONTROL 更多設定] 區段 [!UICONTROL 新校樣] 頁面，如

## 自動化工作流圖表

設定校樣的工作流程時，您會注意到已建立圖表。 添加到校樣的每個階段都會顯示在圖中，清楚地指示各個階段之間的依賴關係。 私人階段會以鍵圖示標示。

圖表會浮動，這表示即使您向下捲動頁面，圖表仍會顯示。

如果您不需要查看圖表，可以隱藏它(1)。

![圖表.png](assets/diagram-350x93.png)

## 添加階段

您可以將其他階段新增至您要建立或修改的工作流程。

1. 如果要將階段新增至現有校樣，請前往「校樣詳細資訊」頁面，如 [在中管理校樣詳細資料 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).
1. 在 **[!UICONTROL 工作流程]** ，按一下 **[!UICONTROL 新階段]**.

1. 指定階段的資訊，如 [!UICONTROL 使用自動化工作流程建立校樣] 一節。
1. 按一下 **[!UICONTROL 添加階段]**，然後按一下 **[!UICONTROL 完成]**.

## 刪除階段

1. 按一下舞台(1)右上角可用的垃圾桶圖示。\
   將游標暫留在舞台上時，圖示就會出現。\
   ![deleting_a_stage.png](assets/deleting-a-stage-350x250.png)

## 舞台設定

* **[!UICONTROL 階段名稱]**:顯示在工作流程圖表上，並包含在傳送給審核者的電子郵件通知中。
* **[!UICONTROL 啟動階段]**:對於工作流程的每個階段，您可以決定其應啟動的時間。 對於您的第一個階段，將提供下列選項：

   * 論校樣建立
   * 在特定時間和日期
   * 手動
   * 只有這三個選項可用於第一階段。 當您新增第二個階段時，其他選項將可供使用；它們要求您選擇父級階段。
   * 在達到前一個截止日期之後（需要挑選父級階段）
   * 所有決定均獲批准或 [!UICONTROL 已核准並變更] （需要挑選父級階段）
   * 所有決策均已批准（需要挑選父級階段）
   * 所有決策都會做出（需要挑選父級階段）

* **[!UICONTROL 截止時間]:** 您可以決定如何在工作流程的每個階段計算截止日期。 選項為：

   * 從校樣建立：在 [!UICONTROL 截止日期] 欄位(9)您可以選取校樣的截止日期。
   * 從啟動階段：在 [!UICONTROL 截止日期] 下拉式清單中，您會選取要新增至階段啟動日期的工作天數，以自動設定校樣的截止日期。

* **[!UICONTROL 鎖定]:** 有許多選項決定何時可以鎖定舞台。 選項包括：

   * 手動鎖
   * 絕不
   * 下一階段開始時
   * 做出所有決定時

**[!UICONTROL 主要決策者]**:在舞台上設定主決策者。 只有在將審閱者添加到舞台後，可用的決策者才會出現在清單中。

>[!NOTE]
>
>如果選擇主決策者，則此階段將不再提供一個所需的決策選項。

* **[!UICONTROL 只需一個決定]**:您可以在舞台上啟用此選項。 這意味著，一旦某個決策者作出決定，就將完成審查。
* **[!UICONTROL 隱私權]:** 每個階段都可設為私人。 如果階段為私人階段，未加入此階段或帳戶中非主管、管理員或帳單管理員的人員將看不到評論和決策。 如需詳細資訊，請參閱 [自動化工作流程概觀](../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md) .

## 將審核者添加到舞台

1. 在每個階段底部的欄位中輸入聯繫人姓名或電子郵件地址。
1. 按一下綠色加號圖示以新增。
1. 設定校樣上的角色。
1. 設定電子郵件警報。
1. 設定第一階段時，您也可以選擇變更校樣的擁有者。

   >[!NOTE]
   >
   >* 審核者只能添加到校樣一次。 您無法將同一個人新增至校樣的多個階段。
   >* 未添加到私人舞台的審閱者無法看到該舞台上的校樣或評論。



## 將校樣轉換為自動化工作流程

您可以將基本校樣轉換為自動化工作流程。

1. 按一下 **[!UICONTROL 轉換為自動化工作流程]** 在 [!UICONTROL 校樣詳細資料] 頁面。
將校樣重新處理至「自動化工作流程」後，所有階段都為使用中、公開及其 [!UICONTROL 鎖台] 選項預設為「手動」。 使用者及其設定會保留所有階段。

   * 在每個階段中，「啟動階段」都設為「在校樣建立時」。
   * 在每個階段中，從選項計算的截止日期都設定為「校樣」建立。
   * 如果在基本校樣上僅選擇了一個決策選項，則所有階段都選擇了它。
   * 如果是基本校樣 [!UICONTROL 主要決策者] 已選取，則會將具有該收件者的階段設為，而其他所有收件者則將其設為「無」。
   * 階段名稱保持不變。

## 將其他範本新增至現有的自動化工作流程

將基本校樣轉換為「自動化工作流程」後，您可以新增其他範本至該工作流程。

1. 在「校樣詳細資訊」頁面的「工作流程」區段中，按一下 **[!UICONTROL 新增範本].**

   * 範本設定會決定可對新增此範本的校樣執行什麼動作。 例如，如果範本具有 [!UICONTROL 新增階段並新增人員至階段] 選項禁用，按鈕 [!UICONTROL 新增階段] 和 [!UICONTROL 共用證明] 將不會顯示。
   * 若 [!UICONTROL 添加階段選項] 在指定範本中將其新增至 [!UICONTROL 新增範本] 按鈕無法顯示。
   * 如果將人員添加到「自動化工作流」模板中的階段，但校樣上也已出現，則如果應用了此模板，系統將自動從階段中刪除此人員。 如果沒有其他人添加到此特定階段，則將顯示以下錯誤，因為系統將不允許向工作流添加空階段。

      ![error_when_adding_template.png](assets/error-when-adding-template-350x66.png)
