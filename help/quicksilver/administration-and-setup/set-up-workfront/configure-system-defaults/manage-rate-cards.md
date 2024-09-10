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
source-git-commit: caaba90f4cdd835e1a1fddf16bcefa30995cca0d
workflow-type: tm+mt
source-wordcount: '667'
ht-degree: 0%

---

# 管理費率卡

{{highlighted-preview-article-level}}

費率卡可讓您根據位置，為每個角色定義多個收費率。 您可能擁有位於巴黎的Designer以及位於紐約的第二個Designer的工作角色，每個工作角色具有不同的收費率。 但是，費率卡上的工作角色不需要位置。 費率卡上工作角色（可能還有地點）的計費費率也可包含有效日期。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

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
   <td><p>新增：[！UICONTROL Standard]</p>
   或
   <p>目前： [！UICONTROL計畫]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td>編輯對[！UICONTROL財務資料]的存取權</td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td>若要編輯與您共用的費率卡，您必須擁有費率卡的管理許可權。</td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 新增費率卡

{{step-1-to-setup}}

1. 在左側面板中，按一下&#x200B;[!UICONTROL **分級卡**]。
1. 按一下&#x200B;[!UICONTROL **新增費率卡**]，然後在[!UICONTROL 新增費率卡]方塊中輸入費率卡的名稱，以取代「未命名的費率卡」。
1. （選擇性）在費率卡詳細資訊畫面上，新增&#x200B;[!UICONTROL **描述**]。
1. （選擇性）若要將自訂表單附加至費率卡，請按一下右上角的&#x200B;[!UICONTROL **新增自訂表單**]&#x200B;欄位，然後從顯示的清單中選取自訂表單。

   如需附加自訂表單的詳細資訊，請參閱[新增自訂表單至物件](/help/quicksilver/workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md)。

1. 按一下左側導覽面板中的&#x200B;[!UICONTROL **工作角色和費率**]。
1. 在「費率卡工作角色與費率」畫面上，按一下&#x200B;[!UICONTROL **新增工作角色**]。
1. 在對話方塊中，選取&#x200B;[!UICONTROL **工作角色**]&#x200B;以定義收費率。

   「預設收費率」會顯示此職務角色的系統層次費率（若已定義）。

   ![新收費率對話方塊](assets/location-rate-for-rate-card.png)

1. 選取工作角色的&#x200B;[!UICONTROL **貨幣**]。
1. （選擇性）選取工作角色的&#x200B;[!UICONTROL **位置**]。
1. 在&#x200B;[!UICONTROL **收費率1**]&#x200B;欄位中，輸入此地點的收費率。 然後，按一下[儲存][!UICONTROL **一次覆寫收費率。**]

   或

   按一下&#x200B;[!UICONTROL **新增費率**]，以新增更多具有有效日期的特定於地點的收費率。

1. （視條件而定）如果您要為此地點新增一個以上的收費率，請輸入下列資訊：

   * **[!UICONTROL 收費率1]、2等：**&#x200B;時段的收費率值。
   * **[!UICONTROL 開始日期]：**&#x200B;費率覆寫開始日期。
   * **[!UICONTROL 結束日期]：**&#x200B;費率覆寫結束的日期。

     帳單費率1不會有開始日期，而最後的帳單費率不會有結束日期。 部分日期會自動新增。 例如，如果「帳單費率1」沒有結束日期，而您新增了開始日期為2023年5月1日的「帳單費率2」，則會在「帳單費率1」中新增結束日期為2023年4月30日的「帳單費率2」，因此不會有間隙。

1. 按一下「[!UICONTROL **儲存**]」。
1. （選擇性）若要針對其他位置的相同工作角色或個別工作角色新增其他收費率，請按一下&#x200B;[!UICONTROL **新增工作角色**]。
1. （可選）若要編輯費率卡，請在「設定」的「費率卡」清單中按一下費率卡名稱。 若要編輯收費率，請按一下費率卡左側導覽面板中的&#x200B;[!UICONTROL **工作角色與費率**]。 然後，選取費率並按一下&#x200B;**編輯**&#x200B;圖示![編輯圖示](assets/edit-icon.png)。

## 複製費率卡

{{step-1-to-setup}}

1. 在左側面板中，按一下&#x200B;[!UICONTROL **分級卡**]。
1. 選取清單中費率卡旁的核取方塊，然後按一下&#x200B;**複製**&#x200B;圖示![復製圖示](assets/copy-icon.png)。
1. 在[!UICONTROL 複製費率卡]方塊中輸入費率卡的名稱，以取代「未命名的費率卡」。 然後，按一下&#x200B;**儲存**。

   新的費率卡已儲存。 視需要編輯費率卡詳細資料、工作角色和費率。

## 刪除整個費率卡

{{step-1-to-setup}}

1. 在左側面板中，按一下&#x200B;[!UICONTROL **分級卡**]。
1. 選取清單中費率卡旁的核取方塊，然後按一下&#x200B;**刪除**&#x200B;圖示![刪除圖示](assets/delete.png)。

   >[!NOTE]
   >
   >附加至專案的評等卡將從專案中刪除。
