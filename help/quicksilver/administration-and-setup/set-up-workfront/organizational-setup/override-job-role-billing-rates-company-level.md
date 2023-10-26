---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: 覆寫公司層級的工作角色收費率
description: 建立職務角色時，您可以選擇選取該角色的每小時收費率。 您可以建立公司特定的每小時收費率。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: ee60987e-78b5-4853-9a4f-e44aa7a81c05
source-git-commit: f66a6c340d8789db447c860d995d9836a30eeeb0
workflow-type: tm+mt
source-wordcount: '480'
ht-degree: 1%

---

# 覆寫公司層級的工作角色收費率

建立職務角色時，您可以選擇選取該角色的每小時收費率。 您可以建立公司特定的多個每小時收費率。 每個收費率在特定日期範圍內有效。

在專案層次，您可以啟用允許公司層次收費率覆寫專案層次費率的選項。 如需詳細資訊，請參閱 [以公司層級的收費率覆寫專案層級的收費率](../../../manage-work/projects/project-finances/override-project-level-with-company-level-billing-rates.md).

## 存取需求

您必須具備下列條件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計劃*</td> 
   <td> <p>任何 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權*</td> 
   <td>計劃</td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>如果您不是系統管理員，可以管理對公司的存取權</p> <p>[！UICONTROL Edit]財務資料的存取權</p> <p><b>注意</b>：如果您還是沒有存取權，請詢問您的 [!DNL Workfront] 管理員是否對您的存取層級設定其他限制。 如需瞭解如何 [!DNL Workfront] 管理員可以修改您的存取層級，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的 [!DNL Workfront] 管理員。

## 覆寫或變更用於特定工作角色的已建立收費率

1. 按一下 **[!UICONTROL 主要功能表]** 圖示 ![](assets/main-menu-icon.png) 位於的右上角 [!DNL Adobe] Workfront，然後按一下 **[!UICONTROL 設定]** ![](assets/gear-icon-settings.png).

1. 按一下 **[!UICONTROL 公司]**.
1. 找出指派工作角色的公司。
1. 按一下清單中的公司名稱。
1. 按一下 **[!UICONTROL 收費率]** 在左側面板中。
1. 按一下 **[!UICONTROL 新增收費率] > [!UICONTROL 新收費率]**，或選擇要編輯的現有費率。
1. 在 [!UICONTROL 新收費率] 對話方塊，選取 [!UICONTROL **工作角色**] 以定義帳單費率。

   此 [!UICONTROL **預設收費率**] 顯示此職務角色的系統層級費率。

   ![新收費率對話方塊](assets/date-effective-billing-rates-for-company.png)

1. 在 [!DNL **收費率1**] 欄位，輸入收費率。 然後，按一下 [!UICONTROL **儲存**] 以一次覆寫收費率。

   或

   按一下 [!UICONTROL **新增費率**] 以新增具有有效日期的更多計費費率。

1. （視條件而定）如果您要新增多個收費率，請輸入下列資訊：

   * **[!UICONTROL 收費率1]、2等**：時間期間的收費率值。
   * **[!UICONTROL 開始日期]**：費率生效的日期。
   * **[!UICONTROL 結束日期]**：費率結束的日期。

     帳單費率1不會有開始日期，而最後的帳單費率不會有結束日期。 部分日期會自動新增。 例如，如果「帳單費率1」沒有結束日期，而您新增了開始日期為2023年5月1日的「帳單費率2」，則會在「帳單費率1」中新增結束日期為2023年4月30日的「帳單費率2」，因此不會有間隙。

1. 按一下&#x200B;[!UICONTROL **儲存**]。

   >[!NOTE]
   >
   >專案上工作角色費率變更只會影響該專案。 公司層級變更的費率將影響所有專案。 如需詳細資訊，請參閱 [覆寫工作角色帳單費率與計算專案收入的概要](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).
