---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: 停用或重新啟用公司
description: 您可以停用您不再使用的公司，同時保留其所有相關的歷史資料。 如果您停用已在系統某個位置使用的公司，它會繼續如常運作。 不會移除或封鎖。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 479dfb9d-0e47-4790-a33a-336b415fbf6e
source-git-commit: b6f6964bb80f172849434c669df2b0ecd735a590
workflow-type: tm+mt
source-wordcount: '410'
ht-degree: 0%

---

# 停用或重新啟用公司

您可以停用您不再使用的公司，同時保留其所有相關的歷史資料。 如果您停用已在系統某個位置使用的公司，它會繼續如常運作。 不會移除或封鎖。

## 存取需求

您必須具備下列條件，才能在 [!DNL Workfront]:

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Workfront] 計劃*</p> </td> 
   <td>[!UICONTROL團隊]或更高版本</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Adobe Workfront] 授權*</p> </td> 
   <td>[!UICONTROL計畫]</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"><strong>訪問級別配置*</strong> </td> 
   <td> <p>下列其中一項：</p> 
    <ul> 
     <li> <p>[!UICONTROL系統管理員]存取級別，允許您編輯系統中的任何公司。 如需詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予使用者完整的管理存取權</a>. </p> </li> 
     <li> <p>對管理公司的管理存取，允許您編輯系統中的任何公司。 如需詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">授予用戶對特定區域的管理訪問權限</a>.</p> </li> 
    </ul> <p><b>附註</b>:  
     <ul> 
      <li> <p>您也可以管理與任何群組相關聯的公司，而您在這些群組中被指派為群組管理員。</p> </li> 
      <li> <p>若要新增至，並從 [!DNL Workfront] 系統，您必須具備下列其中一項：</p> 
       <ul> 
        <li> <p>[!UICONTROL系統管理員]訪問級別。 如需詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予使用者完整的管理存取權</a>. </p> </li> 
        <li> <p>在訪問級別中，必須為[!UICONTROL用戶]設定選擇[!UICONTROL編輯]。 此外，對於[!UICONTROL用戶]設定，在[!UICONTROL微調您的設定]下 <img src="assets/gear-icon-in-access-levels.png"> ，必須啟用[!UICONTROL建立]選項和兩個[!UICONTROL用戶管理]選項中的至少一個。 </p> <p> <img src="assets/access-req-users.png" style="width: 350;height: 101;"> </p> <p>如果您使用「[!UICONTROL用戶管理員（組用戶）]」選項，則必須是用戶所屬組的組管理員。</p> </li> 
       </ul> <p>如需存取層級中「使用者」設定的相關資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">授予使用者存取權</a>.</p> </li> 
     </ul> </p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您擁有的計畫、許可類型或訪問級別配置，請與 [!DNL Workfront] 管理員。

## 停用或重新啟用公司

1. 按一下 **[!UICONTROL 主菜單]** 圖示 ![](assets/main-menu-icon.png) 在 [!DNL Adobe] Workfront，然後按一下 **[!UICONTROL 設定]** ![](assets/gear-icon-settings.png).

1. 在左側面板中，按一下 **[!UICONTROL 公司]** ![](assets/companies-icon-left-panel.png).

1. 選取一或多個公司以停用或重新啟用。
1. 按一下 **[!UICONTROL 編輯]**.
1. 若為單一公司，請停用 **[!UICONTROL 活動]** 選項停用，或啟用選項以啟用它。

   或

   若是多家公司，請選取 **[!UICONTROL 否]** 從 **[!UICONTROL 活動]** 下拉式功能表來停用，或 **[!UICONTROL 是]** 來啟用。

1. 按一下 **[!UICONTROL 儲存變更]**.
