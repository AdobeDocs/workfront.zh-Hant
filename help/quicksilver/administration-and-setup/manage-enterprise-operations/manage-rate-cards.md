---
user-type: administrator
product-area: system-administration;setup
navigation-topic: manage-rate-cards
title: 管理費率卡
description: 費率卡代表與客戶訂立的合約協定，合約中針對將完成工作的工作角色定義了每小時的費率。 在費率卡中，您可以根據屬性為每個工作角色定義多個收費率。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 3972f498-c461-4535-82c6-ad1b60d3ed86
source-git-commit: e5ac8fde409b960aacd3cf7daa0532e9bc3e8121
workflow-type: tm+mt
source-wordcount: '1337'
ht-degree: 1%

---

# 管理費率卡

{{highlighted-preview-article-level}}

費率卡代表與客戶訂立的合約協定，合約中針對將完成工作的工作角色定義了每小時的費率。 在費率卡中，您可以根據機構、地點或成本中心等屬性，為每個工作角色定義多個收費率。 您的唯一費率屬性是在「設定」區域中設定。 如需詳細資訊，請參閱[定義費率屬性](/help/quicksilver/administration-and-setup/manage-enterprise-operations/define-rate-attributes.md)。

例如，代理商A的工作角色為位於巴黎的Designer，代理商B的工作角色為另一個位於巴黎的Designer，而位於紐約的第三個Designer未指派給代理商，每個代理商的計費率不同。 不過，費率卡上的工作角色不需要屬性。 屬性可作為工具，用來建立更精細的速率。 費率卡上的收費率也可以是生效日期，因此費率在指定日期開始和結束。

您也可以鎖定費率卡上的費率，以防止在專案或任務層級覆寫費率。 鎖定費率是收費率階層中最高的費率，專案的保留費率除外。 如需詳細資訊，請參閱[收入與成本階層概覽](/help/quicksilver/manage-work/projects/project-finances/overview-revenue-cost-hierarchy.md)。

## 存取權要求

+++ 展開以檢視這篇文章中所述功能的存取權要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] 封裝</td> 
   <td>Workflow Ultimate</td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] 授權</td> 
   <td>[!UICONTROL 標準]</td>
  </tr> 
  <tr> 
   <td>存取層級設定</td> 
   <td>編輯[!UICONTROL 費率卡]的存取權</td> 
  </tr> 
  <tr> 
   <td>物件許可權</td> 
   <td>若要編輯與您共用的費率卡，您必須擁有費率卡的管理許可權。</td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 新增費率卡

{{step-1-to-setup}}

1. 在左側面板中，按一下&#x200B;[!UICONTROL **分級卡**]。
1. 按一下&#x200B;[!UICONTROL **新費率卡**]，然後按一下&#x200B;[!UICONTROL **建立新費率卡**]。
1. 在&#x200B;[!UICONTROL **新費率卡**]&#x200B;方塊中輸入費率卡的名稱和描述。

   名稱必須是唯一的。

   ![新費率卡對話方塊](assets/new-rate-card-dialog.png)

1. （選擇性）選取費率卡的&#x200B;[!UICONTROL **群組**]。 這是定義費率卡的機構。
1. （選擇性）選取費率卡的&#x200B;[!UICONTROL **公司**]。 這是合約費率適用的使用者端。

   >[!NOTE]
   >
   >「群組」和「公司」不僅用於費率卡詳細資訊，也用於附加費率卡至專案時的篩選。

1. 按一下「**建立**」。

   比率卡片>工作角色和比率畫面隨即顯示。

1. 按一下&#x200B;[!UICONTROL **新增工作角色**]。
1. 在&#x200B;[!UICONTROL **新收費率**]&#x200B;方塊中，選取&#x200B;[!UICONTROL **工作角色**]&#x200B;以定義收費率。

   ![新收費率對話方塊](assets/new-job-role-rate-on-rate-card.png)

1. （選擇性）選取帳單費率屬性，例如「代理機構」、「地點」或「成本中心」。

   >[!NOTE]
   >
   >這些屬性會個別定義，可能會影響收入和成本的計算。 如需詳細資訊，請參閱[定義費率屬性](/help/quicksilver/administration-and-setup/manage-enterprise-operations/define-rate-attributes.md)。

1. 選取收費率的&#x200B;[!UICONTROL **貨幣**]。
1. （選擇性）輸入工作角色的&#x200B;[!UICONTROL **工作角色別名**]。

   如果您輸入的別名名稱尚不存在，您可以將其新增。

   將費率卡附加至專案時，別名會出現在預留位置指派、費用和報表等資訊中，而不是內部工作角色名稱。

   >[!NOTE]
   >
   >* 在單一比率卡中，每個工作角色和屬性組合只能有一個別名。
   >* 必須在費率卡上更新別名，並且無法在專案上編輯別名。

1. 在&#x200B;[!UICONTROL **收費率**]&#x200B;欄位中，輸入此工作角色及其屬性的收費率。
1. （選擇性）選取&#x200B;[!UICONTROL **鎖定率**]&#x200B;以鎖定此率，不允許在專案或任務層級變更此率。 如有需要，您可稍後將其解鎖。
1. （選擇性）按一下&#x200B;[!UICONTROL **新增日期有效費率**]，將有效日期套用至收費率。
1. （選擇性）再按一下&#x200B;[!UICONTROL **新增日期有效費率**]，為此工作角色及其屬性新增更多具有有效日期的計費費率。
1. （視條件而定）如果您要為此職務角色新增一個以上的收費率，請輸入下列資訊：

   * [!UICONTROL **收費率**]：時間期間的收費率值。
   * [!UICONTROL **開始日期**]：費率開始的日期。
   * [!UICONTROL **結束日期**]：費率結束的日期。

     第一個收費率不需要有開始日期，而最後一個收費率不需要有結束日期。 費率日期之間允許間隙，但不允許重疊日期。 在間隔期間，帳單費率階層的其他區域會根據任務的收入型別來決定帳單費率。 如需詳細資訊，請參閱[收入與成本階層概覽](/help/quicksilver/manage-work/projects/project-finances/overview-revenue-cost-hierarchy.md)。

1. 按一下「[!UICONTROL **儲存**]」。
1. （選擇性）若要針對具有不同屬性的相同工作角色或不同工作角色新增其他收費率，請按一下[新增]工作角色&#x200B;[!UICONTROL **&#x200B;**]。

   當您建立費率卡時，會將每個角色的費率新增到費率卡中。 以日期為基礎的目前有效費率會以圖示![目前費率圖示](assets/current-rate-icon.png)表示。

   ![顯示費率的費率卡](assets/rates-on-rate-card.png)

## 編輯費率卡詳細資料和費率

{{step-1-to-setup}}

1. 在左側面板中，按一下&#x200B;[!UICONTROL **分級卡**]。
1. 若要編輯現有的費率卡，請按一下「費率卡」清單中的費率卡名稱。
1. 若要更新費率卡詳細資料，請按一下左側面板中的&#x200B;[!UICONTROL **詳細資料**]。
1. （選擇性）若要將自訂表單附加至費率卡，請按一下[詳細資料]頁面右上角的&#x200B;[!UICONTROL **新增自訂表單**]&#x200B;欄位，然後從顯示的清單中選取自訂表單。

   如需附加自訂表單的詳細資訊，請參閱[新增自訂表單至物件](/help/quicksilver/workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md)。

1. 編輯費率卡詳細資料後，按一下&#x200B;[!UICONTROL **儲存變更**]。
1. 按一下左側面板中的&#x200B;[!UICONTROL **工作角色和費率**]&#x200B;以編輯收費率。
1. 若要編輯速率，請選取速率旁邊的核取方塊，然後按一下畫面底部動作列中的&#x200B;[!UICONTROL **編輯**]。

   如需動作列的詳細資訊，請參閱[使用增強型清單](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md)。

   >[!NOTE]
   >
   >因為每個費率都與角色和屬性的組合相關聯以建立唯一費率，所以當您編輯費率時，無法變更角色和屬性。

1. 若要從費率卡刪除收費率，請選取費率旁的核取方塊，然後按一下動作列上的&#x200B;[!UICONTROL **刪除**]。
1. 若要鎖定速率，請選取速率旁邊的核取方塊，然後按一下動作列上的&#x200B;[!UICONTROL **鎖定**]。

   無法在專案或任務層級變更鎖定費率。 鎖定圖示會顯示在清單中的鎖定速率旁。

   您也可以從動作列解除鎖定鎖定率。

1. 若要依百分比調整費率，請遵循下列步驟：

   1. 在「費率卡>職務角色與費率」畫面上，選取您要調整的所有費率。

      您可以選擇一種或多種費率。 全部會依相同的百分比調整。

   1. 按一下動作列上的&#x200B;[!UICONTROL **調整費率**]。
   1. 在&#x200B;[!UICONTROL **調整職務角色費率**]&#x200B;方塊中，選擇您要在選取的時段（現有有效日期）期間進行費率調整，還是要定義自訂日期範圍。

      ![調整工作角色費率方塊](assets/adjust-job-role-rates-dialog.png)

   1. 輸入費率的調整值。

      此值以百分比套用。 例如，如果您輸入10，則選取的費率會增加10%。

   1. 按一下&#x200B;[!UICONTROL **更新費率**]。
   1. 按一下確認訊息上的&#x200B;[!UICONTROL **更新**]。

      選取的比率會以百分比增加。

## 匯入費率卡

請參閱文章[從範本](/help/quicksilver/administration-and-setup/manage-enterprise-operations/import-rate-cards.md)匯入費率卡。

## 複製費率卡

{{step-1-to-setup}}

1. 在左側面板中，按一下&#x200B;[!UICONTROL **分級卡**]。
1. 選取清單中費率卡旁的核取方塊，然後按一下&#x200B;**複製**&#x200B;圖示![復製圖示](assets/copy-icon.png)。
1. 在&#x200B;[!UICONTROL **複製費率卡**]&#x200B;方塊中輸入新費率卡的名稱。 然後，按一下&#x200B;[!UICONTROL **建立**]。

   新的費率卡已儲存。 視需要編輯費率卡詳細資料、工作角色和費率。

## 刪除整個費率卡

{{step-1-to-setup}}

1. 在左側面板中，按一下&#x200B;[!UICONTROL **分級卡**]。
1. 選取清單中費率卡旁的核取方塊，然後按一下&#x200B;**刪除**&#x200B;圖示![刪除圖示](assets/delete.png)。

   >[!NOTE]
   >
   >附加至專案的評等卡將從專案中刪除。

