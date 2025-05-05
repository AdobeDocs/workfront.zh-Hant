---
product-previous: workfront-proof
product-area: documents
navigation-topic: manage-your-work-workfront-proof
title: 在 [!DNL Workfront Proof]中建立和管理自訂檢視
description: 您可以建立檔案和校樣的自訂檢視，以您想要的方式列出專案。 您也可以將「自訂」檢視中的資訊匯出為報表（CSV、逗號分隔值、檔案格式）。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 7c6f3fdd-f767-4e8d-937a-1c7645aba55b
source-git-commit: ddaee5b339982c826c14b67775d81f3a2bd7bc37
workflow-type: tm+mt
source-wordcount: '2472'
ht-degree: 0%

---

# 在[!DNL Workfront Proof]中建立和管理自訂檢視

>[!IMPORTANT]
>
>本文提及獨立產品[!DNL Workfront Proof]中的功能。 有關[!DNL Adobe Workfront]內部校訂的資訊，請參閱[校訂](../../../review-and-approve-work/proofing/proofing.md)。

您可以建立檔案和校樣的自訂檢視，以您想要的方式列出專案。 您也可以將「自訂」檢視中的資訊匯出為報表（CSV、逗號分隔值、檔案格式）。

>[!NOTE]
>
>自訂檢視僅適用於Select和Premium計畫。 請聯絡我們的銷售團隊以取得報價。

## 建立自訂檢視

建立自訂檢視時，您可以選擇：

* 是要包含校樣、檔案，還是同時包含兩者
* 顯示哪些欄
* 排序依據的欄
* 欄的排序順序（升序或降序）
* 使用哪些型別的篩選器來判斷檢視中包含哪些資訊

建立自訂檢視後，即可立即使用。 新檢視的名稱也會包含在「我的自訂檢視」標題下方的下拉式功能表中（在「標準檢視」下方）。

若要建立自訂檢視：

1. 移至&#x200B;**[!UICONTROL 檢視]**&#x200B;頁面。
1. 如需檢視的詳細資訊，請參閱 [!DNL Workfront Proof][&#128279;](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md)中的管理檢視頁面上的專案。
1. 根據您是要從頭開始建立新的自訂檢視，還是要根據現有的標準檢視建立新的自訂檢視，執行下列任一項作業：

   * 若要根據現有標準檢視建立新的自訂檢視：從下拉式功能表中，選取要作為新自訂檢視基礎的現有標準檢視。 按一下「**[!UICONTROL 檢視設定]**」圖示，然後按一下「**[!UICONTROL 複製]**」以新增自訂檢視。

   * ![自訂檢檢視示](assets/proof-custom-view-icon.png)

   * 若要從頭開始建立新的自訂檢視：按一下&#x200B;**[!UICONTROL 新增檢視]**&#x200B;圖示。
   * ![新檢視](assets/proof-newview.png)

1. 在&#x200B;**[!UICONTROL 詳細資料]**&#x200B;區段中，指定下列資訊：

   * **[!UICONTROL 名稱]** （必要）：新檢視的名稱。 使用唯一名稱，讓使用者在檢視的下拉式選單中輕鬆找到自訂檢視。
   * **[!UICONTROL 專案]**：選取您要同時包含校訂和檔案、僅校訂，還是僅包含檢視中的檔案。 依預設，校樣和檔案都包括在內。

1. 在&#x200B;**[!UICONTROL 欄]**&#x200B;區段中，決定要納入自訂檢視中的欄。

   1. 按一下向右箭頭圖示。
   1. ![向右箭號](assets/proof-view-rightarrow.png)

   1. 連按兩下所選資料行的名稱。
   1. 您必須至少選取一欄，而一欄只能新增一次。
   1. 從您要納入新檢視中的&#x200B;**[!UICONTROL 可用資料行]**&#x200B;區域選取資料行。
   1. 資料行從&#x200B;**[!UICONTROL 可用的資料行]**&#x200B;清單移至&#x200B;**[!UICONTROL 選取的資料行]**&#x200B;清單。

   1. 您可以從標準欄中選取，或選擇自訂欄位和決定原因作為自訂檢視中的欄。 （如果您已在帳戶中設定這些欄位，則它們會顯示在可用欄的標準清單區域下。）
   1. 您可以包含的標準欄

      <table style="table-layout:auto">
      <thead>

      </thead>
      <tbody>  
      <tr>   
      <td><strong>作用中階段名稱</strong></td>   
      <td>自動化工作流程中作用中階段的名稱。</td>  
      </tr>  
      <tr>   
      <td><strong>評論</strong></td>   
      <td>已接收的評論數。</td>
      </tr>  
      <tr>   
      <td><strong>計數器</strong></td>
      <td>顯示已上傳至您帳戶的一些校訂（您必須在「帳戶設定」中啟用校訂計數器選項）。</td>
      </tr>
      <tr>
      <td><strong>已建立</strong></td>
      <td>建立專案的日期和時間。</td>
      </tr>
      <tr>
      <td><strong>建立者</strong></td>
      <td>建立專案的使用者。</td>
      </tr>
      <tr>
      <td><strong>[!UICONTROL 日期已新增到校訂]</strong></td>
      <td>新增到校訂的日期。 </td>
      </tr>
      <tr>
      <td><strong>截止日期</strong></td>
      <td>整個校訂的截止日期。</td>
      </tr>
      <tr>
      <td><strong>決策</strong></td>
      <td>從預期數量中給出的決策數量（例如0 / 1、1 / 1等）</td>
      </tr>
      <tr>
      <td><strong>[!UICONTROL 下載]</strong></td>
      <td>原始檔案的下載次數。</td>
      </tr>
      <tr>
      <td><strong>檔案名稱</strong></td>
      <td>檔案或校訂的名稱。</td>
      </tr>
      <tr>
      <td><strong>資料夾</strong></td>
      <td>包含專案的資料夾。</td>
      </tr>
      <tr>
      <td><strong>上次活動</strong></td>
      <td>專案上最後一個活動的日期和時間。</td>
      </tr>
      <tr>
      <td><strong>最新決定於</strong></td>
      <td>最後做出決定的日期和時間。</td>
      </tr>
      <tr>
      <td><strong>我的期限</strong></td>
      <td>您自己明確新增為檢閱者/核准者（如果適用）之校訂的截止日期。</td>
      </tr>
      <tr>
      <td><strong>所有者</strong></td>
      <td>專案的擁有者。</td>
      </tr>
      <tr>
      <td><strong>所有者國家/地區</strong></td>
      <td>在系統中為證明所有者註冊的國家/地區。 </td>
      </tr>
      <tr>
      <td><strong>上層校訂</strong></td>
      <td>上層校訂的名稱。</td>
      </tr>
      <tr>
      <td><strong>進度</strong></td>
      <td><p>進度列。 顯示尚未開始、開啟、註解或決定的校訂。</p><p>此資訊未排序。</p></td>
      </tr>
      <tr>
      <td><strong>校樣名稱</strong></td>
      <td>證明的名稱。</td>
      </tr>
      <tr>
      <td><strong>校訂型別</strong></td>
      <td><p>校訂型別：靜態檔案、靜態網頁、互動式網頁（.zip上傳）、互動式網頁(https)、影片、音訊和其他。 </p><p>合併的校訂會識別為「合併的校訂型別」。 校訂的檔案型別。</p></td>
      </tr>
      <tr>
      <td><strong>檔案大小(MB)</strong></td>
      <td><p>與磁碟使用配額相關的證明檔案大小。</p><p>為目前版本的校訂提供的此資訊。 如果沒有最新版本，則為最新版本。</p></td>
      </tr>
      <tr>
      <td><p> </p><p><strong>作用中階段期限</strong></p></td>
      <td>自動化工作流程中階段的截止日期。</td>
      </tr>
      <tr>
      <td><strong>階段名稱</strong></td>
      <td>自動化工作流程中每個階段的名稱。 這包括過去的階段、作用中的階段和未來的階段。</td>
      </tr>
      <tr>
      <td><strong>狀態</strong></td>
      <td>「使用中」、「已鎖定」、「草稿」或「已提交」。</td>
      </tr>
      <tr>
      <td><strong>狀態</strong></td>
      <td>「擱置中」、「需要變更」、「已核准變更」、「已核准」或「不相關」。</td>
      </tr>
      <tr>
      <td><strong>標記</strong></td>
      <td>附加到專案的所有標籤。</td>
      </tr>
      <tr>
      <td><strong>即將到來的階段名稱</strong></td>
      <td> 自動化工作流程中尚未啟動的每個階段名稱。 </td>
      </tr>
      <tr>
      <td><strong>版本計數器</strong></td>
      <td> 專案的版本數。 </td>
      </tr>
      <tr>
      <td><strong>校訂版本號碼</strong></td>
      <td><i>校訂的版本號碼。</i></td>
      </tr> 
      </tbody>
      </table>

   1. （選擇性）執行下列任一項作業，將資料行移至&#x200B;**[!UICONTROL 選取的資料行]**&#x200B;區域，使其包含在新檢視中：

      * 重新排序&#x200B;**[!UICONTROL 選取的欄]**&#x200B;清單中的任何欄。
      * 在&#x200B;**[!UICONTROL 選取的資料行]**&#x200B;清單中顯示資料行的順序決定資料行在自訂檢視中的顯示順序。
      * 這些資料行會依照您從&#x200B;**[!UICONTROL 可用的資料行]**&#x200B;清單新增的順序，顯示在&#x200B;**[!UICONTROL 選取的資料行]**&#x200B;清單中。

      * 若要在&#x200B;**[!UICONTROL 選取的資料行]**&#x200B;清單中重新排序資料行，請選取資料行的名稱，然後將其在清單中向上或向下拖曳。

      * 按一下選取資料行的名稱，然後按一下&#x200B;**[!UICONTROL 向左]**&#x200B;箭頭，從&#x200B;**[!UICONTROL 選取的資料行]**&#x200B;清單移除資料行。 或者，您可以連按兩下所選資料行的名稱（該資料行會移回&#x200B;**[!UICONTROL 可用的資料行]**&#x200B;清單）。

      * 欄只能新增一次。 例如，如果您將[註解]欄從[!UICONTROL 可用]移至[!UICONTROL 選取的欄]清單，此欄的名稱將會從[!UICONTROL 可用欄]清單中消失。

1. 在&#x200B;**[!UICONTROL 排序]**&#x200B;區段中，指定下列資訊：

   * **排序依據：**&#x200B;如果您要設定專案在自訂檢視中列出的特定順序，請使用[!UICONTROL 排序]標籤。 如果您未選取要排序的欄，預設值為無欄，即無特殊排序欄或順序。
   * 只有您在[!UICONTROL 資料行]索引標籤上選取的資料行才會包含在[!UICONTROL 依資料行排序]下拉式清單中。
   * **遞增或遞減：**&#x200B;選取您要依預設以遞增或遞減方式排序欄。

1. 使用&#x200B;**[!UICONTROL 篩選器]**&#x200B;區段來定義一或多個條件，以選取要包含在自訂檢視中的專案。 如果您想要將自訂檢視作為報表，篩選器特別實用。
1. 若要在自訂檢視中加入所有專案，請略過&#x200B;**[!UICONTROL 篩選器]**&#x200B;區段。
1. 可用的篩選器：

   * **欄位：**&#x200B;選取此篩選的欄位（預設欄位為註解）。 欄位清單包含所有標準欄位（如[!UICONTROL 欄]索引標籤中所示）。 此清單不限於您選取要顯示的欄。
   * **運運算元：**&#x200B;篩選器可用的運運算元取決於您選取的欄位型別。 選取顯示[欄位]與[值]欄位之間關係的運運算元。 您稍後會填入此資訊。
   * **值：**&#x200B;根據您選取的欄位和運運算元，在此欄位中選取或輸入您選取的值。 根據您選擇的運運算元，可能會有一個「值」欄位，或兩個或無。 請參閱下列範例。
   * **使用下列邏輯套用篩選器：**&#x200B;不同欄位之間的篩選條件將使用AND運運算元。 使用相同欄位的多個篩選條件將針對相同欄位使用OR運運算元。

     如果您只想檢視沒有註解的校樣，請選取下列值：

      * 欄位：註解
      * 運運算元：等於
      * 值欄位：0

     如果您只想檢視含有兩個或多個註解的校樣，請選取下列值：

      * 欄位：註解
      * 運運算元：大於或等於
      * 值欄位：2

     如果您只想檢視介於1到4個註解的校樣，請選取下列值：

      * 欄位：註解
      * 運運算元：介於
      * 值欄位（第一個欄位）：1
      * 值欄位（第二個欄位）：4

        您可以變更已新增至「自訂」檢視的篩選器，而不會發生任何問題，或是視需要按一下[!UICONTROL 設定]篩選器旁的十字圖示來移除篩選器。

        因為[欄位]清單不限於您在[!UICONTROL 欄]索引標籤上選取的欄，所以當您建立篩選器時，請注意該篩選器是否包含您未選取要在自訂檢視中顯示的欄。 例如，檢視的下列篩選器將選取版本計數器值為2或以上的所有校樣：

         * 欄位=版本計數器
         * 運運算元=大於或等於
         * 值欄位= 2

           >[!NOTE]
           >
           >您可以變更已新增至「自訂」檢視的篩選器，而不會發生任何問題，或是視需要按一下[!UICONTROL 設定]篩選器旁的十字圖示來移除篩選器。



1. 在&#x200B;**[!UICONTROL 共用]**&#x200B;區段中，選取您帳戶中的哪些使用者將能夠看到您的自訂檢視。
1. 自訂檢視是建立者專屬的檢視。 依照預設，新的「自訂」檢視僅對建立者可見；不過，您可以選擇下列其中一個選項來共用您的自訂檢視：

   * **只有您才能看到此自訂檢視** （預設）：如果您希望自訂檢視僅供您使用，請選取此選項。
   * **所有使用者都可以看到此自訂檢視**：選取此選項可讓您的帳戶中的所有使用者都可以使用自訂檢視。
   * **選取可以看見此自訂檢視的使用者**：選取此選項可讓自訂檢視僅供特定使用者使用。
   * 開始輸入您想要存取自訂檢視的使用者名稱或電子郵件地址，然後按一下下拉式清單中出現的名稱。
   * 如果您目前選擇不與其他使用者共用您的檢視，您稍後可以編輯自訂檢視來執行此操作。

1. 按一下「**[!UICONTROL 建立]**」。
1. 此自訂檢視已顯示並可在[!DNL Views]頁面上使用。 如需檢視的詳細資訊，請參閱 [!DNL Workfront Proof][&#128279;](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md)中 [!DNL Views] 頁面上的管理專案。

## 編輯自訂檢視

您可以輕鬆編輯自訂檢視。 若要編輯自訂檢視：

1. 移至&#x200B;**[!UICONTROL 檢視]**&#x200B;頁面。\
   如需檢視的詳細資訊，請參閱 [!DNL Workfront Proof][&#128279;](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md)中的管理檢視頁面上的專案。

1. 按一下[!UICONTROL 檢視]按鈕(1)
1. 從下拉式選單中選取您要編輯的檢視。\
   ![編輯檢視](assets/proof-view-edit.png)

1. 按一下&#x200B;**[!UICONTROL 檢視選項]**&#x200B;按鈕，然後按一下&#x200B;**[!UICONTROL 編輯檢視]**。\
   ![檢視選項](assets/proof-view-options.png)\
   便會顯示「編輯自訂檢視」頁面。

1. 按一下[!UICONTROL 動作]功能表。 (3)\
   只有在檢視中包含「校樣名稱」欄時，此按鈕才可用。
1. 從功能表選取[!UICONTROL 編輯檢視]。 (4) \
   ![editing_custom_view_2.png](assets/editing-custom-view-2-350x258.png)

1. 此時會顯示「編輯自訂檢視」頁面。

![Edit_custom_view_page.png](assets/edit-custom-view-page-350x543.png)

>[!NOTE]
>
>如果您編輯「自訂」檢視，「選取的欄」清單中的欄將自動按字母順序排列。 在更新檢視之前，您必須視需要重新排列它們。


## 複製自訂檢視

「複製檢視」功能可讓您輕鬆複製現有的自訂檢視。 例如，如果您想要為所有設計人員設定個別的檢視，則除了校訂所有者（設計人員）之外，每個檢視都相同，這真的很有用。

若要複製自訂檢視：

1. 移至&#x200B;**[!UICONTROL 檢視]**&#x200B;頁面。\
   如需檢視的詳細資訊，請參閱 [!DNL Workfront Proof][&#128279;](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md)中的管理檢視頁面上的專案。

1. 按一下&#x200B;**[!UICONTROL 檢視]**&#x200B;按鈕。 (1)
1. 從清單中選取您的「自訂」檢視。 (2)
1. 按一下&#x200B;**[!UICONTROL 動作]**&#x200B;功能表。 (3)\
   只有在檢視中包含「校樣名稱」欄時，此按鈕才可用。

1. 從功能表中選取[!UICONTROL 複製]。 (4)\
   ![copying_custom_view.png](assets/copying-custom-view-350x258.png)

1. 在「複製自訂檢視」頁面中，會填入所有原始設定。 根據您的選擇修改自訂檢視，然後按一下&#x200B;**[!UICONTROL 複製檢視]**&#x200B;按鈕。 您會立即進入新檢視。\
   ![複製自訂檢視](assets/copy-custom-view-page-350x542.png)

## 共用自訂檢視

如果您尚未在檢視的「共用」區段中選取其他使用者，「共用檢視」功能可讓您與他們共用檢視。 當您與其他使用者共用自訂檢視時，該檢視會出現在「檢視」下拉式功能表的[!UICONTROL 我的自訂檢視]區段中。

若要與其他使用者共用自訂檢視：

1. 移至&#x200B;**[!UICONTROL 檢視]**&#x200B;頁面。\
   如需檢視的詳細資訊，請參閱 [!DNL Workfront Proof][&#128279;](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md)中的管理檢視頁面上的專案。

1. 按一下&#x200B;**[!UICONTROL 檢視]**&#x200B;按鈕(1)
1. 從清單中選取您的自訂檢視(2)
1. 按一下&#x200B;**[!UICONTROL 動作]**&#x200B;功能表。 (3)\
   只有在檢視中包含「校樣名稱」欄時，此按鈕才可用。

1. 從功能表選取[!UICONTROL 共用檢視] (4)
1. 接著會顯示「編輯自訂檢視」頁面。
1. 在[!UICONTROL 共用]區段中，選取您要共用檢視的使用者，然後按一下&#x200B;**[!UICONTROL 更新檢視]**。

   ![Edit_custom_view_page__1_.png](assets/edit-custom-view-page--1--350x543.png)

## 將自訂檢視匯出為CSV檔案

若要將資料從自訂檢視匯出至CSV檔案：

1. 移至&#x200B;**[!UICONTROL 檢視]**&#x200B;頁面。\
   如需檢視的詳細資訊，請參閱 [!DNL Workfront Proof][&#128279;](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md)中的管理檢視頁面上的專案。

1. 按一下&#x200B;**[!UICONTROL 檢視]**&#x200B;按鈕。 (1)
1. 從清單中選取您的「自訂檢視」 。 (2)
1. 按一下&#x200B;**[!UICONTROL 動作]**&#x200B;功能表。 (3)\
   只有在檢視中包含「校樣名稱」欄時，此按鈕才可用。

1. 從功能表選取[!UICONTROL 匯出至CSV]。 (4)\
   ![exporting_custom_view.png](assets/exporting-custom-view-350x258.png)\
   在單獨的瀏覽器視窗中，「正在產生報表：100%」會出現，外加記錄數量（您的自訂檢視包含在報表中的專案數量）

1. （視條件而定）如果出現安全性訊息，指出報表下載目前遭到封鎖，請按一下「 」允許繼續下載。
1. 當「檔案下載」視窗出現並詢問您是否要開啟或儲存檔案時，請按一下&#x200B;**[!UICONTROL 儲存]**。
1. 選取電腦上的位置並儲存檔案。

## 刪除自訂檢視

您可以輕鬆刪除自訂檢視。 若要這麼做：

1. 移至&#x200B;**[!UICONTROL 檢視]**&#x200B;頁面。\
   如需檢視的詳細資訊，請參閱 [!DNL Workfront Proof][&#128279;](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md)中的管理檢視頁面上的專案。

1. 按一下&#x200B;**[!UICONTROL 檢視]**&#x200B;按鈕。
1. 從清單中選取您的自訂檢視
1. 按一下&#x200B;**[!UICONTROL 動作]**&#x200B;功能表。 (3)\
   只有在檢視中包含「校樣名稱」欄時，此按鈕才可用。

1. 從功能表中選取[!UICONTROL 刪除]。 (4)\
   ![deleting_custom_view.png](assets/deleting-custom-view-350x258.png)

1. 按一下「**[!UICONTROL 刪除]**」(5)以確認您要刪除目前的自訂檢視\
   ![delete__1_.png](assets/delete--1--350x187.png)

1. 預設的「所有專案」檢視會顯示，而您已刪除的自訂檢視不再出現在&#x200B;**[!UICONTROL 檢視]**&#x200B;下拉式功能表中。
