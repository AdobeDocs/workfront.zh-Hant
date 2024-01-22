---
product-area: user-management;portfolios
navigation-topic: grant-and-request-access-to-objects
title: 移除物件的許可權
description: 您可以移除其他使用者對您有權共用之物件的許可權。 從物件中移除許可權對於所有可共用的物件來說都是相同的。
author: Alina
feature: Get Started with Workfront
exl-id: 8e191b5e-31df-4291-8b9d-9ca69be27561
source-git-commit: 71d5e15c38b26b9a833ac2418d5782afd249a24c
workflow-type: tm+mt
source-wordcount: '1144'
ht-degree: 0%

---

# 移除物件的許可權

<!--Audited: 01/2024-->

您可以移除其他使用者對您有權共用之物件的許可權。 從物件中移除許可權對於所有可共用的物件來說都是相同的。

與共用物件類似的考量適用於從物件移除許可權。 如需詳細資訊，請參閱區段 [關於共用物件的考量事項](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md#consider) 在文章中 [物件許可權共用概觀](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)

## 存取需求

您必須具備下列專案才能共用物件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td> <p>任何 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Workfront授權*</td> 
   <td> <p>新授權：投稿人或以上版本</p>
   或  
   <p>目前授權：要求或以上</p>
   <p><b>附註</b></p>

<p>某些物件需要比請求更高的存取權。 </p>

<p>例如，對於新授權，貢獻者可以共用問題，但只有Standard授權使用者可以共用專案。</p>

<p>就目前的授權而言，請求者可以共用問題，但只有工作或計畫人員可以共用專案。</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>檢視您要共用之物件的存取許可權或以上許可權</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>檢視您要共用之物件的許可權或更高的許可權</p> <p>管理移除物件繼承許可權的許可權</p>  </td> 
  </tr> 
 </tbody> 
</table>

*若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的Workfront管理員。 如需詳細資訊，請參閱 [Workfront檔案的存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## 從物件的共用清單中移除實體 {#remove-entities-from-the-sharing-list-of-an-object}

您可以從物件的共用清單中移除實體（使用者、工作角色、團隊、群組、公司）。 這會移除使用者對物件的許可權。

1. 移至您要移除許可權的物件。

   如需哪些物件可以共用的資訊，請參閱 [物件許可權共用概觀](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

1. （視條件而定）針對計畫、投資組合和檔案，執行下列動作：

   1. 按一下 **更多** 圖示 ![](assets/more-icon.png)在物件名稱旁，然後按一下 **共用** 或 **共用。**

      ![](assets/share-a-document-350x160.png)

   1. 按一下 **x** 在物件存取方塊中，位於使用者、專案團隊、群組、公司、工作角色名稱旁，以移除這些專案。

      ![](assets/remove-permissions-on-portfolio.png)

   1. 在 **&lt;使用者名稱>的Workfront存取權將從此移除** 下拉式功能表，選取您是否要從選取的物件移除其存取權，或是從與其關聯的所有子物件移除其存取權。

1. （視條件而定）對於專案、任務和問題，請執行以下作業：

   1. 按一下 **共用** 物件名稱右側。

      ![](assets/new-share-button.png)
   1. 尋找要從物件中移除的使用者、角色、團隊、群組或公司。
   1. 按一下 **移除**.
在 **移除「&lt;使用者名稱>」，從** 下拉式功能表，選取您是否要從選取的物件移除其存取權，或是從與其關聯的所有子物件移除其存取權。

      ![](assets/remove-permissions-on-project-nwe-350x479.png)

   存在下列情況：

   * 如果您只從物件中移除實體，則該實體會失去其對物件的許可權，以及其對子物件的繼承許可權。 如果先前已個別授予子專案的許可權，當您選取此選項時，它們會保留與其相關聯之所有子物件的相同許可權。
   * 如果您將實體從物件及所有子物件中移除，該實體會失去其對該物件及所有子物件的許可權，即使先前已授予他們個別對各個子物件的許可權。

1. 按一下「**儲存**」。

## 大量移除數個物件的許可權

當您在清單中大量選取實體（使用者、工作角色、團隊、群組、公司）時，可以一次從數個物件中移除這些實體。

>[!NOTE]
>
>當您大量選取物件時，無法檢視所有選取物件的存取實體。 在移除物件的許可權之前，您必須知道要從選取物件的共用中移除哪個實體。

1. 移至您要共用的物件清單。

   如需哪些物件可以共用的資訊，請參閱 [物件許可權共用概觀](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

1. 在清單中選取數個物件，然後按一下 **共用** 圖示 ![](assets/share-icon.png)在清單頂端。
1. 輸入您要移除其存取許可權的使用者、角色、團隊、群組或公司名稱。 **編輯 `<Object Name>` 存取目標** 欄位。
1. 從存取下拉式功能表中，選取 **無存取權**.

   ![](assets/no-access-option-removing-permissions-bulk-tasks-nwe-350x166.png)

1. 在 `<User Name>`的Workfront存取權會從此下拉式選單中移除，請選取是否要僅從您選取的物件移除其存取權，或是從與其關聯的所有其他子物件移除其存取權。\
   存在下列情況：

   * 如果您只從物件中移除實體，則該實體會失去其對物件的許可權，以及其對子物件的繼承許可權。 如果先前已個別授予子專案的許可權，當您選取此選項時，它們會保留與其相關聯之所有子物件的相同許可權。 
   * 如果您將實體從物件及所有子物件中移除，該實體會失去其對該物件及所有子物件的許可權，即使先前已授予他們個別對各個子物件的許可權。

   **範例：** 選擇是否僅移除您在清單中選取之任務的許可權，或移除附加到任務的問題和檔案的許可權。

   ![](assets/remove-permissions-bulk-drop-down-for-attached-objects-nwe-350x96.png)

1. （可選）若要大量變更數個物件的許可權，請為選取的實體選取另一個共用層級。

   例如，如果他們有「管理」許可權，請改為選取「貢獻」或「檢視」。

1. 按一下「**儲存**」。

## 移除繼承的許可權

繼承的許可權可以從物件中移除，讓擁有者能夠明確識別誰將取得子物件的存取權，無論使用者是否取得父物件的存取權。

>[!IMPORTANT]
>
>只有具有「管理」許可權的使用者才能移除繼承的許可權。

若要移除繼承的許可權：

1. 移至您擁有管理許可權的物件。 例如，前往任務。
1. 移至物件存取方塊，如 [從物件的共用清單中移除實體](#remove-entities-from-the-sharing-list-of-an-object) 一節。
1. 選取 **x** 旁邊 **繼承的許可權** ，移除此處列出的任何使用者。

   ![](assets/remove-inherited-permissions-on-project-nwe-350x475.png)

   這可確保授予父系物件（例如專案）許可權的任何人都不會預設擁有此任務的許可權。 您必須在任務共用清單中列出個別實體，才能授與任務許可權。

   >[!TIP]
   >
   >您無法從繼承的許可權清單中移除個別實體。 您只能對列出的所有實體停用繼承許可權。

1. 按一下 **儲存**. 

## 將物件設為私人

如果您已在系統範圍內共用物件，或透過將其設為公開而與外部使用者共用物件，則可移除系統範圍或公開許可權，使其再次成為私人物件。 

如需有關讓物件在整個系統內或公開可用的詳細資訊，請參閱 [共用物件](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).

將物件設為私人：

1. 移至您要設為私用的物件。\
   例如，導覽至報表。
1. 按一下 **報表動作**，然後 **共用**.

   ![](assets/report-permissions-make-private-nwe-350x477.png)

1. 按一下 **移除公開存取權** 移除外部使用者檢視報表的存取權。
1. 按一下 **移除系統範圍存取許可權** 以停止與所有Workfront使用者共用。 
1. 按一下「**儲存**」。
