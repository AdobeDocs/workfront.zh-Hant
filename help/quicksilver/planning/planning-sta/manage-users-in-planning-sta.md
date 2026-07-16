---
title: 在Adobe Workfront Planning中作為獨立產品管理使用者
description: 本文說明將Planning購買為獨立產品時，如何在Adobe Workfront Planning中管理使用者和團隊。
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
source-git-commit: ee260723331ddff4e8d89f7d9ca2b807835d6130
workflow-type: tm+mt
source-wordcount: '835'
ht-degree: 0%

---


# 在Adobe Workfront Planning中作為獨立產品管理使用者

>[!IMPORTANT]
>
>本文資訊是指Adobe Workfront Planning （購買獨立產品時）。 當您的公司購買僅Adobe Workfront Planning套件，但未購買Workfront Workflow套件時，請參閱本文。
>
>如需搭配Adobe Workfront套件一起購買時的Workfront Planning相關資訊，請參閱[開始使用Adobe Workfront Planning](/help/quicksilver/planning/general/planning-overview.md)。

您可以在Adobe Workfront Planning中作為獨立產品管理使用者，其方式與在Adobe Workfront中管理使用者類似。

您可以在Workfront Planning中指派使用者的存取層級有一些限制。

## 存取權要求

+++ 展開以檢視本文中功能的存取需求。 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront規劃套件</p></td> 
   <td> 
<p>任何Workfront Planning作為獨立套件</p>

</td> </tr>
  <tr> 
   <td role="rowheader"><p>Adobe Workfront授權</p></td> 
   <td><p>規劃管理員</p>
   </td> 
  </tr>

</tbody> 
</table>

如需有關以獨立套件形式使用Workfront所需存取權的詳細資訊，請參閱[以獨立產品形式使用Adobe Workfront Planning所需的存取權](/help/quicksilver/planning/planning-sta/access-needed-for-planning-sta.md)。
+++    

## Adobe Workfront Planning中的存取層級

當以獨立產品形式購買時，您可以在Workfront Planning中指派以下存取層級給使用者：

* 規劃管理員
* 規劃標準

如需每次存取所含功能的詳細資訊，請參閱[獨立產品Adobe Workfront Planning所需的](/help/quicksilver/planning/planning-sta/access-needed-for-planning-sta.md)存取。

在Workfront Planning中作為獨立產品使用存取層級時，請考量下列事項：

* 您無法在Workfront Planning中建立或修改存取層級。 已預先設定。

* 當您將使用者新增至Adobe Admin Console並成為Workfront產品的管理員後，系統會自動將使用者指派給Workfront Planning中的此存取層級，且無法在Planning中編輯其存取層級。
* 新增使用者至Admin Console後，您只能將Planning Standard存取層級指派給Planning中的使用者。 這是您可以手動指派給使用者的唯一存取層級。

## 在Workfront Planning中作為獨立產品管理使用者

1. 以Planning管理員的身分，執行下列任一項作業：

   * 如果您是新的Workfront Planning客戶，您會收到Adobe Workfront的電子郵件，提醒您現在在Adobe Workfront擁有帳戶。 使用電子郵件中的連結來登入Admin Console。

   * 如果您是現有的Workfront規劃管理員，並且想要將其他人新增至您的帳戶，請登入Admin Console。

   如需詳細資訊，請參閱[在Adobe Admin Console中管理使用者](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md)。

1. 在Admin Console中，開始在下列其中一個標籤中新增使用者：

   * **管理員**：使用者會自動建立為Planning中的Planning管理員使用者。
   * **使用者**：您必須在Workfront規劃中指派存取層級。

1. （視條件而定）從Adobe CX Enterprise首頁登入Workfront。

   Workfront Planning隨即開啟。
1. 按一下&#x200B;**主功能表** > **使用者** > **新增使用者**。

   ![Planning獨立版中的新使用者方塊](assets/new-user-box-planning-sta.png)

1. 在&#x200B;**新使用者**&#x200B;方塊中，更新下列資訊：

   * **名字**：與您新增至Admin Console的名稱相同。
   * **姓氏**：與您新增至Admin Console的名稱相同。
   * **電子郵件地址（使用者名稱）**：您新增至Admin Console的電子郵件相同。
   * **使用者處於作用中狀態**：若要指出使用者處於作用中狀態，且可以登入Workfront Planning並指派給記錄，請開啟設定。
   * **存取層級**：為非管理員使用者選取Planning標準。 這是唯一的選項。

     >[!TIP]
     >
     >新增已在Admin Console中設定為「管理員」的使用者，會自動將「Planning管理員」存取層級新增至使用者。 無法編輯此專案。

   * **團隊**：從下拉式功能表中，選取要與使用者建立關聯的團隊。 必須先建立團隊，然後才能將團隊指派給使用者。

     如需詳細資訊，請參閱[管理團隊](/help/quicksilver/planning/planning-sta/manage-teams-in-planning-sta.md)。

1. 按一下&#x200B;**立即上傳**&#x200B;以新增個人資料圖片，然後按一下&#x200B;**儲存**。

1. 按一下「**儲存**」或「**新增人員並開始另一個**」以儲存使用者並新增另一個。

   使用者已新增，且將收到登入Workfront Planning的電子郵件。
1. （可選）若要編輯現有使用者，請執行下列任一項作業：

   * 將滑鼠停留在清單中的使用者名稱上，然後按一下&#x200B;**更多**&#x200B;功能表![更多](assets/more-menu.png) > **編輯使用者**
   * 在清單中選取使用者，然後按一下頁面底部藍色工具列上的&#x200B;**編輯使用者**。
1. （選用）若要刪除使用者，請執行下列任一項作業：

   * 將滑鼠停留在清單中的使用者名稱上，然後按一下&#x200B;**更多**&#x200B;功能表![更多](assets/more-menu.png) > **刪除使用者**
   * 在清單中選取團隊，然後按一下頁面底部藍色工具列上的&#x200B;**刪除使用者**
1. 按一下&#x200B;**刪除**&#x200B;以進行確認。
1. （可選）若要停用使用者，請執行下列任一項作業：

   * 將滑鼠停留在清單中的使用者名稱上，然後按一下&#x200B;**更多**&#x200B;功能表![更多](assets/more-menu.png) > **停用**
   * 在清單中選取團隊，然後按一下頁面底部藍色工具列上的&#x200B;**「停用**」
1. 按一下&#x200B;**停用**&#x200B;以確認。

   若要保留您工作的歷程記錄，建議您停用使用者，而非刪除使用者。



