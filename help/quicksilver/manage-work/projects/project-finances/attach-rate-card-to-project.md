---
title: 將費率卡附加至專案
description: 當您附加費率卡至專案時，所有角色都會依地點及其相關帳單費率新增至專案。
author: Lisa
feature: Work Management
role: User
source-git-commit: 8dbb48e6aa2df874caa816468cf2e3ad408ebf7e
workflow-type: tm+mt
source-wordcount: '449'
ht-degree: 0%

---

# 將費率卡附加至專案

{{highlighted-preview-article-level}}

費率卡會根據位置儲存每個工作角色的多個收費率。 您可以讓位於巴黎的設計師擔任工作角色，讓位於紐約的設計師擔任第二個工作角色，每個角色都有不同的收費率。 不過，費率卡上的職務角色不需要位置。 費率卡上工作角色（可能還有地點）的計費費率也可包含有效日期。

當您附加費率卡至專案時，所有角色都會依地點及其相關帳單費率新增至專案。

>[!NOTE]
>
>附加費率卡會覆寫專案上任何現有的計費費率。

您可以直接在專案中編輯費率卡的計費費率。 這不會影響預設費率卡上儲存的費率。

如需建立費率卡的相關資訊，請參閱 [管理費率卡](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/manage-rate-cards.md).

如需有關覆寫專案的工作角色收費率以及計算專案收入的一般資訊，請參閱 [覆寫工作角色帳單費率與計算專案收入的概要](/help/quicksilver/manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>目前計畫：標準</p><p>或</p><p>舊版計畫：計畫 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>編輯對專案和財務資料的存取權</p> <p>職位角色的管理存取權</p> <p>注意：如果您仍然沒有存取權，請詢問您的Workfront管理員是否對您的存取層級設定了其他限制。 如需有關Workfront管理員如何修改您的存取層級的資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理具有管理財務許可權之專案的許可權</p> <p>如需請求其他存取許可權的詳細資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">要求物件的存取權 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的Workfront管理員。

## 將費率卡附加至專案

1. 前往專案。
1. 按一下 **收費率** 在左側面板中。 您可能需要先按一下 **顯示更多**.
1. 按一下 **新增帳單費率>附加費率卡**.

   「附加費率卡」頁面隨即開啟。 如需詳細資訊，請參閱 [管理費率卡](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/manage-rate-cards.md).

1. 選取要新增至專案的費率卡，然後按一下 **附加**.

   費率卡及其所有工作角色費率會新增至計費費率清單。

   ![將評等卡新增至專案](assets/billing-rates-added-from-rate-card.png)

   >[!NOTE]
   >
   >在計費費率清單上，您可以移除一或多個來自費率卡的工作角色。 從專案移除工作角色收費率時，並不會將其從預設費率卡中移除。

