---
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: best-practices-catalog
title: 設定Blueprint
description: 安裝Blueprint之前，您可以設定專案範本或組織結構的詳細資訊。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: df10bc8f-b980-4c61-ae6d-bcea03103738
source-git-commit: d46eb98c443a421f340b1021972ddb89eda1966b
workflow-type: tm+mt
source-wordcount: '1824'
ht-degree: 0%

---

# 設定Blueprint

您可以在安裝Blueprint之前設定其詳細資訊。 專案範本和組織結構藍圖類型通常需要設定一些偏好設定和映射某些屬性。 其他Blueprint類型可能不需要配置，您將按原樣安裝。 有關安裝的詳細資訊，請參見 [安裝Blueprint](/help/quicksilver/administration-and-setup/blueprints/blueprints-install.md).

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 計劃</strong></td>
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe [!DNL Workfront] 授權</strong></td>
   <td>[!UICONTROL計畫]</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>訪問級別配置</strong></td>
   <td> <p>[!UICONTROL系統管理員]</p> </td> 
  </tr> 
 </tbody> 
</table>

## 設定專案範本藍圖

1. 找到您要使用的藍圖。
1. 按一下 **[!UICONTROL 安裝]**，然後選擇環境：

   <table style="table-layout:auto">
        <tr>
        <td><strong>生產</strong></td>
        <td>生產是您的即時環境。</td>
    </tr>
    <tr>
        <td><strong>Sandbox 預覽</strong></td>
        <td>沙箱預覽是測試環境，可作為即時環境的復本，並由Workfront每週末重新整理。</td>
    </tr>
    <tr>
        <td><strong>沙箱1和2</strong></td>
        <td>「自訂重新整理沙箱」是個別的測試環境，由您手動重新整理。 取得自訂重新整理沙箱需額外付費。</td>
    </tr>
   </table>

1. 繼續下列小節：

   * [[!UICONTROL 範本偏好設定]](#template-preferences)
   * [[!UICONTROL 角色對應]](#role-mapping)
   * [[!UICONTROL 團隊對應]](#team-mapping)
   * [[!UICONTROL 公司對應]g](#company-mapping)
   * [[!UICONTROL 群組對應]](#group-mapping)

## [!UICONTROL 範本偏好設定] {#template-preferences}

選擇要如何安裝模板。

您也可以在安裝Blueprint之前指定範本所有權。 安裝範本後，您可以變更這些欄位。 如需詳細資訊，請參閱 [編輯專案範本](../../manage-work/projects/create-and-manage-templates/edit-templates.md).

![[!UICONTROL 範本偏好設定] 節](assets/Blueprints_TemplatePreferences.png)

1. 在 [!UICONTROL 範本偏好設定] 節，指定新模板名稱。
1. 指定下列項目：

   <table style="table-layout:auto">
    <tr>
        <td><strong>[!UICONTROL模板所有者]<strong></td>
        <td>此人會收到範本的[!UICONTROL管理]權限，且當使用範本建立專案時，將成為專案擁有者。</td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL模板發起人]</strong></td>
        <td>此人通常是需要了解專案發生狀況的經理、執行官或利害關係人。 專案發起人不會取得專案的任何其他存取權，但會新增至專案的電子郵件通知中。</td>
    </tr>
    <tr>
        <td><strong>[!UICONTROLPortfolio]</strong></td>
        <td>這是專案建立後所屬的產品組合。</td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL程式]</strong></td>
        <td>這是項目建立後將屬於的項目。</td>
    </tr>
   </table>

1. 選取範本安裝為使用中或非使用中。
1. 如果首選項可用，則選擇是否要使用定義的新問題首選項。

   按一下 **[!UICONTROL 請參閱問題偏好設定]** 查看將與blueprint一起安裝的特定首選項。 從匯入的範本建立的專案，會針對 [!UICONTROL 問題] 區段。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>佇列主題群組</strong></td> 
      <td> <p>佇列主題群組會定義問題或請求的最高層級類別。 使用者在選取要提交請求的位置時，可以選取功能表選項來檢視主題群組。 主題組可以包含多個隊列主題。 如需詳細資訊，請參閱 <a href="../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md" class="MCXref xref">建立主題群組</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>佇列主題</strong></td> 
      <td> <p>排隊主題與路由規則一起工作，以分配問題或請求。 這些功能表選項是使用者在輸入問題或請求時，在選取主題群組後所選取的功能表選項。 如需詳細資訊，請參閱 <a href="../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md" class="MCXref xref">建立佇列主題</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>路由規則</strong></td> 
      <td>路由規則將問題或請求發送給特定作業角色、用戶或團隊。 他們也可以將請求傳送至特定專案，與請求佇列相關聯的專案除外。 如需詳細資訊，請參閱 <a href="../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md" class="MCXref xref">建立路由規則</a>. </td> 
     </tr> 
    </tbody> 
   </table>

   >[!INFO]
   >
   >**範例：** 此Blueprint中的新問題偏好設定提供四個佇列主題。 使用者在建立問題時會選取下列其中一個主題。 （因為只有一個主題組存在，因此會自動應用該主題組，用戶不必選擇它。） 當用戶完成並提交問題時，路由規則將確定分配給哪個作業角色或團隊。
   >![新問題偏好設定範例](assets/Blueprints_IssuePrefsDetails.png)
   >![新問題的排隊主題](assets/blueprints-newissueqtopicsexample-350x204.png)
   >![轉至作業角色的問題](assets/Blueprints_ProjectShowsIssueAssignment.png)

   >[!TIP]
   >
   >* 使用問題偏好設定有助於建立專案上擷取新問題或要求的一致性。
   >* 設定這些偏好設定不會自動將從範本建立的專案放入請求佇列中。 如需設定請求佇列的相關資訊，請參閱 [建立請求佇列](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).
   >* 並非所有藍圖都包含新的問題首選項。



## [!UICONTROL 角色對應] {#role-mapping}

>[!NOTE]
>
>某些藍圖中可能不會顯示此部分。

有些範本包含指定的工作角色。 將模板轉換為項目時，工作角色可幫助您分配正確的人員。 在安裝Blueprint之前，您可以自訂角色的對應方式。 按一下 **[!UICONTROL 請參閱角色說明]** 以進一步了解blueprint中可用的角色。

Blueprint會依角色名稱搜尋，以查看是否有任何現有角色相符。 搜尋會區分大小寫，因此名稱必須完全相符。 如果現有角色不相符，您可以讓Blueprint為您建立這些角色。

![[!UICONTROL 角色對應] 節](assets/Blueprints_RoleMapping.png)

1. 如果角色存在，您可以選擇以下選項之一：

   1. 使用不同名稱建立新角色，然後在文本框中鍵入名稱。
   1. 使用現有角色，然後在選擇框中選擇角色。
   1. 請勿使用已映射的角色。 不建議使用此選項，因為某些任務將不分配角色。

1. 如果角色不存在，您可以選擇以下選項之一：

   1. 建立新角色。 此選項會建立Blueprint建議的角色。
   1. 使用不同名稱建立新角色，然後在文本框中鍵入名稱。
   1. 使用現有角色，然後在選擇框中選擇角色。
   1. 請勿使用已映射的角色。 不建議使用此選項，因為某些任務將不分配角色。

>[!NOTE]
>
>安裝程式不會將角色套用至特定人員。 安裝Blueprint解決方案後，您應驗證這些角色中的人員，並視需要指派人員。 如需詳細資訊，請參閱 [安裝Blueprint後要採取的動作](../../administration-and-setup/blueprints/best-next-actions-after-install.md).

如需中作業角色的詳細資訊，請參閱 [!DNL Workfront]，請參閱 [建立和管理作業角色](../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

## [!UICONTROL 團隊對應] {#team-mapping}

>[!NOTE]
>
>某些藍圖中可能不會顯示此部分。

有些範本包括指定的團隊。 指派給團隊的工作可由團隊的任何成員完成。 在安裝Blueprint之前，您可以自訂團隊的對應方式。 按一下 **[!UICONTROL 請參閱團隊說明]** 以進一步了解blueprint中可用的團隊。

Blueprint會依團隊名稱搜尋，以查看現有團隊是否相符。 搜尋會區分大小寫，因此名稱必須完全相符。 如果現有團隊不相符，您可以讓Blueprint為您建立這些團隊。

![[!UICONTROL 團隊對應] 節](assets/Blueprints_TeamMapping.png)

1. 如果團隊存在，您可以選擇下列其中一個選項：

   1. 使用不同名稱建立新團隊，然後在文本框中鍵入名稱。
   1. 使用 [!UICONTROL 現有團隊]，然後在「選擇」(selection)框中選擇一個組。
   1. 請勿使用已對應的團隊。 不建議使用此選項，因為某些任務不會指派團隊。

1. 如果團隊不存在，您可以選擇下列其中一個選項：

   1. 建立新團隊。 此選項會建立Blueprint建議的團隊。
   1. 使用不同名稱建立新團隊，然後在文本框中鍵入名稱。
   1. 使用 [!UICONTROL 現有團隊]，然後在「選擇」(selection)框中選擇一個組。
   1. 請勿使用已對應的團隊。 不建議使用此選項，因為某些任務不會指派團隊。

>[!NOTE]
>
>安裝程式不會將人員新增至團隊。 安裝Blueprint解決方案後，您應驗證團隊中的人員，並視需要指派人員。 如需詳細資訊，請參閱 [安裝Blueprint後要採取的動作](../../administration-and-setup/blueprints/best-next-actions-after-install.md).

如需團隊在 [!DNL Workfront]，請參閱 [建立和管理團隊](../../people-teams-and-groups/create-and-manage-teams/create-and-mange-teams.md).

## 公司對應 {#company-mapping}

>[!NOTE]
>
>某些藍圖中可能不會顯示此部分。

有些藍圖包括有規定的公司。 公司是一個組織單位，可代表您的組織、組織內的部門或您與其合作的客戶。 在安裝Blueprint之前，您可以自訂公司的對應方式。 按一下 **[!UICONTROL 請參閱公司說明]** 以進一步了解Blueprint中可用的公司。

藍圖會依公司名稱搜尋，以查看現有公司是否相符。 搜尋會區分大小寫，因此名稱必須完全相符。 如果現有公司不相符，您可以讓Blueprint為您建立這些公司。 Blueprint中的主要公司對應至您環境中的主要公司，即使它們沒有相同的名稱亦然。

![[!UICONTROL 公司對應] 節](assets/Blueprints_CompanyMapping.png)

1. 如果公司存在，您可以選擇下列其中一個選項：

   1. 以不同名稱建立新公司，然後在文字方塊中輸入名稱。
   1. 使用現有公司，然後在選取方塊中選取公司。\

      Blueprint中的主要公司對應至您環境中的主要公司，即使它們沒有相同的名稱亦然。
   1. 請勿使用已對應的公司。 不建議使用此選項，因為公司在其他物件中的參考將為空。

1. 如果公司不存在，您可以選擇下列其中一個選項：

   1. 建立新的公司. 此選項會建立Blueprint建議的公司。
   1. 以不同名稱建立新公司，然後在文字方塊中輸入名稱。
   1. 使用現有公司，然後在選取方塊中選取公司。
   1. 請勿使用已對應的公司。 不建議使用此選項，因為公司在其他物件中的參考將為空。

>[!NOTE]
>
>若要在安裝Blueprint後設定公司，請參閱 [安裝Blueprint後要採取的動作](../../administration-and-setup/blueprints/best-next-actions-after-install.md).

如需範本與公司關聯的詳細資訊，請參閱 [編輯專案範本](../../manage-work/projects/create-and-manage-templates/edit-templates.md).

如需關於公司在 [!DNL Workfront]，請參閱 [建立和編輯公司](../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

## [!UICONTROL 群組對應] {#group-mapping}

>[!NOTE]
>
>某些藍圖中可能不會顯示此部分。

有些藍圖包括指定的組。 組是與部門結構一致的一組用戶。 群組類似於Workfront，但與團隊和公司不同。 在安裝Blueprint之前，您可以自訂群組的對應方式。 按一下 **[!UICONTROL 請參閱群組說明]** 以進一步了解Blueprint中可用的群組。

Blueprint會依群組名稱搜尋，以查看是否有任何現有群組相符。 搜尋會區分大小寫，因此名稱必須完全相符。 如果現有的群組不相符，您可以讓Blueprint為您建立這些群組。

![[!UICONTROL 群組對應] 節](assets/Blueprints_GroupMapping.png)

1. 如果群組存在，您可以選取 **[!UICONTROL 重新映射組]** 並選擇以下選項之一：

   1. **[!UICONTROL 以不同名稱建立新群組]**，然後輸入要指派給此群組的名稱。 Blueprint定義中對群組的參考將改為與此新群組相關聯。
   1. **[!UICONTROL 替換為現有組]**，然後搜尋並在選取方塊中選取群組。

      >[!NOTE]
      >
      >無法更名現有組。

1. 如果群組不存在，您可以：

   1. 在文字方塊中輸入建議的群組名稱，以變更該群組名稱。
   1. 選擇 **[!UICONTROL 重新映射組]** 選擇 [!UICONTROL 替換為現有組]，然後搜尋並在選取方塊中選取群組。
   1. 選擇 **[!UICONTROL 重新映射組]** 選擇 **[!UICONTROL 在現有組下插入]**，然後搜尋並在選取方塊中選取群組。 此選項在現有組下建立新的子組。

>[!NOTE]
>
>若要在安裝Blueprint後設定群組，請參閱 [安裝Blueprint後要採取的動作](../../administration-and-setup/blueprints/best-next-actions-after-install.md).

如需在中使用群組的相關資訊 [!DNL Workfront]，請參閱 [群組概觀](../../administration-and-setup/manage-groups/groups-overview/groups.md).
