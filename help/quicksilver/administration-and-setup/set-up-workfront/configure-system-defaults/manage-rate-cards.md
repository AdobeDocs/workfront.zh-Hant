---
user-type: administrator
product-area: system-administration;setup
navigation-topic: manage-rate-cards
title: 管理費率卡
description: 費率卡可讓您根據位置，為每個角色定義多個收費率。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 3972f498-c461-4535-82c6-ad1b60d3ed86
source-git-commit: a61635022da9eed7c2fc61bad1cbca0f7f23d7ec
workflow-type: tm+mt
source-wordcount: '680'
ht-degree: 0%

---

# 管理費率卡

{{highlighted-preview-article-level}}

費率卡可讓您根據位置，為每個角色定義多個收費率。 您可以讓位於巴黎的設計師擔任工作角色，讓位於紐約的第二位設計師擔任工作角色，每個角色具有不同的收費率。 但是，費率卡上的工作角色不需要位置。 費率卡上工作角色（可能還有地點）的計費費率也可包含有效日期。

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計劃</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權</td> 
   <td><p>新計畫： [！UICONTROL Standard] </p>
       <p>或</p> 
       <p>目前計畫： [！UICONTROL計畫] </p>
   </td>    
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>編輯對[！UICONTROL財務資料]的存取權</p> <p><b>注意</b>：如果您還是沒有存取權，請詢問您的 [!DNL Workfront] 管理員是否對您的存取層級設定其他限制。 如需瞭解如何 [!DNL Workfront] 管理員可以修改您的存取層級，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td>若要編輯與您共用的費率卡，您必須擁有費率卡的管理許可權。</td> 
  </tr> 
 </tbody> 
</table>

## 新增費率卡

{{step-1-to-setup}}

1. 在左側面板中，按一下 [!UICONTROL **評等卡**].
1. 按一下 [!UICONTROL **新費率卡**]，然後在中輸入費率卡的名稱 [!UICONTROL 新費率卡] 方塊，以取代「未命名的費率卡」。
1. （選用）在費率卡詳細資訊畫面上，新增 [!UICONTROL **說明**].
1. （可選）若要將自訂表單附加至費率卡，請按一下 [!UICONTROL **新增自訂表格**] 欄位，並從顯示的清單中選取自訂表單。

   如需附加自訂表單的詳細資訊，請參閱 [新增自訂表單至物件](/help/quicksilver/workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

1. 按一下 [!UICONTROL **職務角色與費率**] ，位於左側導覽面板中。
1. 在費率卡職位角色和費率畫面上，按一下 [!UICONTROL **新增工作角色**].
1. 在對話方塊中，選取 [!UICONTROL **工作角色**] 以定義開立帳單費率。

   「預設收費率」會顯示此職務角色的系統層次費率（若已定義）。

   ![新收費率對話方塊](assets/location-rate-for-rate-card.png)

1. 選取 [!UICONTROL **貨幣**] 工作角色的。
1. （選用）選取 [!UICONTROL **位置**] 工作角色的。
1. 在 [!UICONTROL **收費率1**] 欄位，輸入此地點的收費率。 然後，按一下 [!UICONTROL **儲存**] 以一次覆寫收費率。

   或

   按一下 [!UICONTROL **新增費率**] 以新增更多具有有效日期的特定地點收費率。

1. （視條件而定）如果您要為此地點新增一個以上的收費率，請輸入下列資訊：

   * **[!UICONTROL 收費率1]、2等：** 時間期間的收費率值。
   * **[!UICONTROL 開始日期]：** 費率覆寫開始的日期。
   * **[!UICONTROL 結束日期]：** 費率覆寫結束的日期。

     帳單費率1不會有開始日期，而最後的帳單費率不會有結束日期。 部分日期會自動新增。 例如，如果「帳單費率1」沒有結束日期，而您新增了開始日期為2023年5月1日的「帳單費率2」，則會在「帳單費率1」中新增結束日期為2023年4月30日的「帳單費率2」，因此不會有間隙。

1. 按一下「[!UICONTROL **儲存**]」。
1. （選擇性）若要針對其他位置的相同工作角色或個別工作角色新增其他收費率，請按一下 [!UICONTROL **新增工作角色**].
1. （可選）若要編輯費率卡，請在「設定」的「費率卡」清單中按一下費率卡名稱。 若要編輯收費率，請按一下 [!UICONTROL **職務角色與費率**] 在費率卡的左側導覽面板中。 然後，選取費率並按一下 **編輯** 圖示 ![編輯圖示](assets/edit-icon.png).

## 複製費率卡

{{step-1-to-setup}}

1. 在左側面板中，按一下 [!UICONTROL **評等卡**].
1. 選取清單中費率卡旁的核取方塊，然後按一下 **複製** 圖示 ![復製圖示](assets/copy-icon.png).
1. 在「 」中輸入費率卡的名稱 [!UICONTROL 複製率卡片] 方塊，以取代「未命名的費率卡」。 然後，按一下 **儲存**.

   新的費率卡已儲存。 視需要編輯費率卡詳細資料、工作角色和費率。

## 刪除整個費率卡

{{step-1-to-setup}}

1. 在左側面板中，按一下 [!UICONTROL **評等卡**].
1. 選取清單中費率卡旁的核取方塊，然後按一下 **刪除** 圖示 ![「刪除」圖示](assets/delete.png).

   >[!NOTE]
   >
   >附加至專案的評等卡將從專案中刪除。
