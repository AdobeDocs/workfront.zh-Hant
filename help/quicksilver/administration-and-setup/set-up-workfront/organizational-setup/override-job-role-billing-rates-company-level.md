---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: 覆寫公司層級的工作角色收費率
description: 建立職務角色時，您可以選擇選取該角色的每小時收費率。 您可以建立公司特定的每小時收費率。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: ee60987e-78b5-4853-9a4f-e44aa7a81c05
source-git-commit: 15063d937a5ba9b5285c66a0987e8deea6cc6d74
workflow-type: tm+mt
source-wordcount: '438'
ht-degree: 0%

---

# 覆寫公司層級的工作角色收費率

建立職務角色時，您可以選擇選取該角色的每小時收費率。 您可以建立公司特定的多個每小時收費率。 每個收費率在特定日期範圍內有效。

在專案層次，您可以啟用允許公司層次收費率覆寫專案層次費率的選項。 如需詳細資訊，請參閱[以公司層級的收費率覆寫專案層級的收費率](../../../manage-work/projects/project-finances/override-project-level-with-company-level-billing-rates.md)。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] 封裝</td> 
   <td><p>任何</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] 授權</td> 
   <td><p>[!UICONTROL 標準]</p>
       <p>[!UICONTROL 計畫]</p></td>
  </tr> 
  <tr> 
   <td>存取層級設定</td> 
   <td> <p>如果您不是系統管理員，可以管理對公司的存取權</p>
   <p>編輯財務資料的存取權</p> </td>
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 覆寫或變更用於特定工作角色的已建立收費率

{{step-1-to-setup}}

1. 按一下&#x200B;**[!UICONTROL 公司]**。
1. 找出指派工作角色的公司。
1. 按一下清單中的公司名稱。
1. 按一下左側面板中的&#x200B;**[!UICONTROL 收費率]**。
1. 按一下&#x200B;**[!UICONTROL 新增收費率] > [!UICONTROL 新增收費率]**，或選擇要編輯的現有收費率。
1. 在[!UICONTROL 新收費率]對話方塊中，選取&#x200B;[!UICONTROL **工作角色**]&#x200B;以定義收費率。

   [!UICONTROL **預設收費率**]&#x200B;會顯示此工作角色的系統層級費率。

   ![新收費率對話方塊](assets/date-effective-billing-rates-for-company.png)

1. 在&#x200B;[!DNL **收費率1**]&#x200B;欄位中，輸入收費率。 然後，按一下[儲存][!UICONTROL **一次覆寫收費率。**]

   或

   按一下&#x200B;[!UICONTROL **新增費率**]&#x200B;以新增更多具有有效日期的計費費率。

1. （視條件而定）如果您要新增多個收費率，請輸入下列資訊：

   * **[!UICONTROL 記帳費率1]、2等**：時間期間的收費率值。
   * **[!UICONTROL 開始日期]**：費率生效的日期。
   * **[!UICONTROL 結束日期]**：費率結束的日期。

     帳單費率1不會有開始日期，而最後的帳單費率不會有結束日期。 部分日期會自動新增。 例如，如果「帳單費率1」沒有結束日期，而您新增了開始日期為2023年5月1日的「帳單費率2」，則會在「帳單費率1」中新增結束日期為2023年4月30日的「帳單費率2」，因此不會有間隙。

1. 按一下「[!UICONTROL **儲存**]」。

   >[!NOTE]
   >
   >專案上工作角色費率變更只會影響該專案。 公司層級變更的費率將影響所有專案。 如需詳細資訊，請參閱[覆寫工作角色收費率以及計算專案收入的總覽](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md)。
