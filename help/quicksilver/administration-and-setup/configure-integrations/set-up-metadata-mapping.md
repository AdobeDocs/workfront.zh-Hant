---
title: 設定中繼資料對應
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
description: 元資料是與文檔相關聯的描述性資訊。 您可以設定 [!DNL Adobe Workfront] 包括元資料，並將文檔發送到 [!DNL Workfront] 應用程式。
author: Caroline
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
exl-id: 7cf4787d-7cff-489e-bd5b-69db3ff09f6e
source-git-commit: ceda437684f565b91dbb8b02f6b03cbe8d27a70a
workflow-type: tm+mt
source-wordcount: '614'
ht-degree: 0%

---

# 設定中繼資料對應

元資料是與文檔相關聯的描述性資訊。 您可以設定 [!DNL Adobe Workfront] 包括元資料，並將文檔發送到 [!DNL Workfront] 應用程式。

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

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
   <td>[!UICONTROL計畫]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置</td> 
   <td> <p>您必須是 [!DNL Workfront] 管理員。 如需詳細資訊，請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予使用者完整的管理存取權</a>.</p> <p><b>注意</b>:如果您仍無法存取，請詢問您的 [!DNL Workfront] 管理員。 若要了解 [!DNL Workfront] 管理員可修改您的存取層級，請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 關於 [!DNL Workfront] 中繼資料

中文檔的元資料 [!DNL Workfront] 可包括相關項目名稱、任務說明或計畫完成日期等資訊。 As a [!DNL Workfront] 管理員，您可以 [!DNL Workfront] 包括從中發送的文檔的元資料 [!DNL Workfront] 變更為下列項目 [!DNL Workfront] 應用程式：

* [!DNL Workfront DAM]

在可以隨文檔一起發送元資料之前，您必須先指定或映射要包含的元資料。 您可以對應中使用的任何欄位 [!DNL Workfront]. 設定中繼資料對應後，所有上傳至 [!DNL Workfront] 應用程式將包含對應的中繼資料。

當用戶從 [!DNL Workfront] 到 [!DNL Workfront] 應用程式中，映射元資料沿文檔傳輸。 若 [!DNL Workfront] 應用程式連結至 [!DNL Workfront]，對中的文檔元資料所做的更改 [!DNL Workfront] 未反映在 [!DNL Workfront] 應用程式。 若 [!DNL Workfront] 更改後，您必須將包含更新元資料的新文檔版本發送到 [!DNL Workfront] 應用程式。

>[!NOTE]
>
>您只能將中繼資料對應至一個方向：從 [!DNL Workfront] to [!DNL Workfront DAM]. 連結到的文檔的元資料 [!DNL Workfront] 從 [!DNL Workfront DAM] 無法轉移至Workfront。

您可以對應相同的 [!DNL Workfront] 欄位至 [!DNL Workfront DAM]，但您無法在任一應用程式中為多個 [!DNL Workfront] 中繼資料欄位。

配置多個 [!DNL Workfront] 要匯出至 [!DNL Workfront] 應用程式，首先在中建立計算的自訂欄位 [!DNL Workfront] 以顯示物件的所有個別自訂欄位。 然後，映射計算 [!DNL Workfront] 欄位至中繼資料欄位 [!DNL Workfront] 應用程式。 如需計算自訂欄位的詳細資訊，請參閱 [將計算資料新增至自訂表單](../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

您必須先啟用應用程式，才能映射中繼資料對應程式的欄位 [!DNL Workfront]. 如需詳細資訊，請參閱 [配置文檔整合](../../administration-and-setup/configure-integrations/configure-document-integrations.md).

## 設定 [!DNL Workfront] 傳送中繼資料

1. 按一下 **[!UICONTROL 主菜單]** 圖示 ![](assets/main-menu-icon.png) 在 [!DNL Adobe Workfront]，然後按一下 **[!UICONTROL 設定]** ![](assets/gear-icon-settings.png).

1. 在左側面板中，按一下 **[!UICONTROL 檔案]** > **[!UICONTROL 中繼資料對應]**.

   ![](assets/metadata-mapping.png)

1. 在 **[!UICONTROL 選擇要映射的源欄位]** 方塊中，開始輸入您要對應的Workfront欄位名稱 [!DNL Workfront DAM]，然後在清單中看到它時選取它。
1. 在 **[!UICONTROL 選擇映射的目標欄位]** 框中，選擇要在所選欄位中填入資訊的欄位 [!DNL Workfront] 欄位。

1. 按一下 **[!UICONTROL 新增對應]**.

   對應欄位會顯示在頁面底部列出的對應欄位中。

1. 重複步驟5和6，直到您新增所有所需 [!DNL Workfront] 欄位及其對應 [!DNL Workfront DAM] 欄位。

## 刪除映射的欄位

1. 登入 [!DNL Workfront] 管理員。
1. 按一下 **[!UICONTROL 主菜單]** 圖示 ![](assets/main-menu-icon.png) 在 [!DNL Adobe Workfront]，然後按一下 **[!UICONTROL 設定]** ![](assets/gear-icon-settings.png).

1. 在左側面板中，按一下 **[!UICONTROL 檔案]** > **[!UICONTROL 中繼資料對應]**.

1. 在映射欄位清單中，選擇要從元資料映射中刪除的欄位。
1. 按一下 **[!UICONTROL 刪除]**.

   指定的欄位不再對應。 現在，當使用者從 [!DNL Workfront] to [!DNL Workfront DAM]，刪除欄位中包含的中繼資料不會與檔案一併傳輸。

   在您刪除映射欄位之前發送的文檔將保留隨其發送的原始元資料，包括已刪除欄位的元資料。
