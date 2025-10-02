---
product-area: projects
navigation-topic: business-case-and-scorecards
title: 建立及編輯專案的風險
description: 風險是阻礙專案準時完成或在預算內完成的可能事件或因素。 您可以記錄專案風險，作為建立專案業務案例的一部分或使用「風險」頁標。 您可以將風險新增至專案和範本。 您無法將風險與任務或問題建立關聯。
author: Alina
feature: Work Management
exl-id: 6125c477-c0d8-43b4-88d8-35b0c2412468
source-git-commit: fbf902196c9f5b55ddd1e20516e4237309dff2ed
workflow-type: tm+mt
source-wordcount: '1080'
ht-degree: 1%

---

# 建立及編輯專案的風險

<!--Audited: 06/2025-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers after a week from the Preview release. </span>   

<span class="preview">For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md). </span>-->

風險是阻礙專案準時完成或在預算內完成的可能事件或因素。 您可以在建立專案的業務案例時記錄風險，或使用「風險」頁標來記錄風險。

您只能在專案或範本上建立風險。 您無法將風險與任務或問題建立關聯。

風險可與成本相關聯，但實際風險成本不會影響專案的實際成本。

>[!NOTE]
>
>當您在專案的業務案例中定義專案相關的風險，或在專案的「風險」標籤中新增風險時，本文會定義這些風險。
>
>如需編輯專案時可用的風險欄位相關資訊，請參閱[編輯專案](../../../manage-work/projects/manage-projects/edit-projects.md)。

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

+++ 展開以檢視本文中功能的存取需求。 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront計畫*</p></td> 
   <td> <p>目前計畫：</p>
   <ul><li>任何計畫，以在專案的風險區域中新增風險</p></li>
   <li><p>Prime （含）以上版本，在專案的業務案例中新增風險</p></li></ul>
   <p>舊版計畫：任何計畫</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront授權*</p></td> 
   <td> <p>目前：標準 </p>
   <p>舊版：計畫 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>存取層級設定</p></td> 
   <td> <p>編輯專案與財務資料的存取權</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>物件許可權</p></td> 
   <td> <p> 管理許可權，包括管理您要建立或編輯風險的專案財務 </p> </td> 
  </tr> 
 </tbody> 
</table>

*如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 建立並編輯業務案例中的風險

您可以在規劃專案的業務案例時建立風險。 例如，當業務案例的機率、移轉計畫或成本發生變更時，您稍後可以在業務案例中編輯這些專案。 如需建立業務案例的相關資訊，請參閱[為專案建立業務案例](../../../manage-work/projects/define-a-business-case/create-business-case.md)。

您的Workfront管理員或群組管理員必須在「專案偏好設定」區域的業務案例中啟用&#x200B;**風險**&#x200B;區段，您才能在業務案例區段的專案層級檢視該區段。 如需有關設定專案偏好設定的資訊，請參閱[設定全系統的專案偏好設定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)。

在業務案例中建立和編輯風險是相同的。

若要在業務案例中建立或編輯風險：

1. 移至您要建立風險的專案。
1. 按一下左側面板中的&#x200B;**業務案例**。
1. 在&#x200B;**風險**&#x200B;區段中，按一下&#x200B;**編輯風險**。
1. 輸入或編輯下列資訊：

   * **描述：**&#x200B;描述風險。

   * **潛在成本**：如果發生風險，請輸入預估成本。

   * **機率**：輸入風險發生的機率作為百分比值。

   * **型別：**&#x200B;選取風險所屬的類別。
   * **緩解計畫**：更新計畫的描述以降低風險。

   * **移轉成本**：輸入您必須建立的移轉計畫成本，以防止風險發生。

   ![風險](assets/edit-risk.png)

1. （選擇性）按一下&#x200B;**新增其他風險**&#x200B;以新增其他風險。
1. 按一下「**儲存**」。

## 在風險區域中建立和編輯風險

除了在業務案例中建立和編輯風險之外，您還可以使用專案的&#x200B;**風險**&#x200B;區段來執行此操作。

您可以在專案或範本的風險區段中建立和編輯風險。 為範本建立風險與為專案建立風險相同。

### 在風險區域中建立風險 {#create-risks-in-the-risks-area}

1. 移至您要建立風險的專案。
1. 按一下左側面板中的&#x200B;**風險**。

   ![任務的風險區段](assets/risks-section-on-project-2022.png)

1. 按一下&#x200B;**新增更多風險**，並透過內嵌編輯其資訊來建立風險。

   或

   按一下「**新風險**」以開啟「**新風險**」方塊。

   ![新風險方塊](assets/new-risk-box.png)

1. （視條件而定）如果您在&#x200B;**新風險**&#x200B;方塊中新增風險，請輸入下列資訊：

   * **描述**：描述風險。 這是必填欄位。
   * **風險型別**：指出風險所屬的類別。\
     您的Workfront管理員會定義環境中可用的風險型別。 如需定義風險型別的相關資訊，請參閱文章[編輯與建立風險型別](../../../administration-and-setup/set-up-workfront/configure-system-defaults/edit-create-risk-types.md)。

   * **機率**：以百分比值表示風險發生的機率。
   * **潛在成本**：表示如果發生風險，則表示預估成本。
   * **實際成本**：表示風險發生時的實際風險成本。
   * **移轉成本**：表示您必須設定移轉計畫的成本，以防止風險發生。
   * **緩解計畫**：更新計畫的描述以降低風險。

1. 按一下「**儲存**」。

1. （選擇性）針對風險清單套用&#x200B;**標準**&#x200B;檢視時，在&#x200B;**狀態**&#x200B;下拉式功能表中，選取其他&#x200B;**狀態**&#x200B;的風險。

   依預設，風險的&#x200B;**狀態**&#x200B;為&#x200B;**已識別**。

### 編輯風險區域中的風險 {#edit-risks-in-the-risks-area}

您可以在專案存留期間或變更發生時（例如機率、潛在成本或狀態變更）編輯風險。

您可以一次編輯一個風險或大量編輯多個風險。

若要編輯風險，請執行下列步驟：

1. 導覽至您要編輯現有風險的專案。
1. 按一下左側面板中的&#x200B;**風險**。
1. 開始內聯編輯您在清單中看到的風險欄位，一次編輯一個風險。

   或

   選取一或多個風險，然後按一下[編輯] **&#x200B;**&#x200B;以同時編輯多個風險。

   >[!NOTE]
   >
   >當您同時編輯多個風險時，會將相同的資訊套用至所有選取的風險。 在變更前與每個風險相關的資訊會以大量編輯方式覆寫。

1. 如果您已按一下&#x200B;**編輯**，則會開啟&#x200B;**編輯風險**&#x200B;或&#x200B;**編輯風險**&#x200B;方塊。

   更新下列欄位：

   * **描述**：編輯風險的描述。
   * **風險型別**：更新風險所屬的類別。
   * **機率**：以百分比值表示風險發生的機率。
   * **潛在成本**：表示如果發生風險，則表示預估成本。
   * **實際成本**：表示風險發生時的實際風險成本。
   * **移轉成本**：表示您必須設定移轉計畫的成本，以防止風險發生。
   * **緩解計畫**：更新計畫的描述以降低風險。

1. 按一下「**儲存**」。
1. （選擇性）套用風險清單的&#x200B;**標準**&#x200B;檢視時，在&#x200B;**狀態**&#x200B;下拉式功能表中編輯風險的&#x200B;**狀態**。

   >[!NOTE]
   >
   >您無法在&#x200B;**編輯風險**&#x200B;對話方塊中編輯風險的&#x200B;**狀態**。 您只能在內嵌編輯中執行此操作。
