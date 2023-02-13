---
product-area: projects
navigation-topic: grant-and-request-access-to-objects
title: 請求對對象的訪問
description: Adobe Workfront中物件的可見性取決於您對該類型物件的存取權，以及您對個別物件的權限。
author: Alina
feature: Get Started with Workfront
exl-id: ad1c525c-42a8-4fb7-a2cd-7792e1c280ab
source-git-commit: dd7f61fcd92a43303be356dd3209ec6da6a063dd
workflow-type: tm+mt
source-wordcount: '1424'
ht-degree: 0%

---

# 請求對對象的訪問

Adobe Workfront中物件的可見性取決於您對該類型物件的存取權，以及您對個別物件的權限。

>[!NOTE]
>
>本文介紹如何向除Adobe Workfront方案規劃器中的計畫外的所有對象請求權限。 有關請求訪問計畫的資訊，請參閱 [請求方案計畫員中計畫的訪問權](../../scenario-planner/request-access-to-plan.md). 這需要額外的授權。

您的Workfront管理員會設定您對存取層級中某類型物件的存取權。 如需詳細資訊，請參閱 [存取層級與權限如何搭配運作](../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md).

如果您需要Workfront內特定物件的權限，可以要求存取權。 您不必傳送電子郵件給Workfront管理員或物件擁有者以說明您的需求，而是可以在Workfront內要求額外的存取權（或權限）。

如果某人與您共用了指向對象的連結，則可以請求對對象的初始訪問，或者，您可以請求對至少可以查看的對象的額外訪問。

例如，您可能擁有專案的「檢視」權限，但您需要將工作新增至該專案。 在此情況下，您可以向專案要求Contribute權限。

## 存取需求

<!--drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard</p> 
   Or
   <p>Legacy license: Work or higher</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View access or higher to the objects you request permissions to</p> <p><b>NOTE</b> 
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

-->

您必須具備以下條件才能共用物件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>任何 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>工作或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>查看對您請求權限的對象的訪問或更高</p> <p><b>附註</b>

如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td>
</tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 了解標準共用規則

下列標準共用規則會在Workfront系統中設定為預設選項時自動生效。 

* 指派給任務或問題的使用者有Contribute存取權。 
* 項目、Portfolio和項目群經理對他們擁有的對象具有管理訪問權限。
* 對話中包含的用戶對對話發生的對象具有查看訪問權限。
* 被分配為批准者的用戶對等待批准的對象具有查看訪問權限。
* 共用控制面板時，控制面板上的所有報表也會以相同使用者存取權共用給相同的使用者。 
* 對象所有者無法擴展對對象的訪問權限，超出其對管理員定義的該對象的訪問權限。

## 要求存取

您可以請求對當前無權訪問的對象的初始訪問，也可以請求對您只有有限訪問權限的對象的額外訪問。

* [要求初始存取](#request-initial-access)
* [請求其他訪問](#request-additional-access)

### 要求初始存取  {#request-initial-access}

如果您尚未擁有對象的訪問權限，並且從連結導航到該對象，則會顯示一個螢幕，通知您沒有查看資訊的訪問權限。  

要請求對對象的初始訪問，請執行以下操作：

1. 按一下 **請求存取**.\
   此 **請求存取** 對話框。

1. （條件性）如果一個以上的使用者有權授予您其他存取權，則使用者名稱旁會顯示下拉式箭頭。 
1. 從下拉式清單中選取您要接收存取請求的使用者。\
   下拉式清單中只會顯示10位使用者。 清單按字母順序排序。\
   如需此下拉式功能表中所列使用者順序的詳細資訊，請參閱  [「請求存取」和「請求更多存取」下拉式功能表的階層](#hierarchy-of-the-request-access-and-request-more-access-drop-down-menus).

1. 從下拉式清單中，選取您要求的存取類型。
1. （選用）在 **P.S.** 欄位中，針對您需要其他存取權的原因，為使用者指定附註。

   ![](assets/request-access-dialog-350x314.png)

如果您沒有物件的存取層級權限，且嘗試從連結存取該物件，畫面會隨即顯示，通知您聯絡Workfront管理員。 

例如，如果您沒有產品組合存取權，但您獲得了產品組合的連結，則會看到下列訊息：\
![](assets/permission-request-initial2-350x96.png)

### 請求其他訪問 {#request-additional-access}

要請求對已有有限訪問權限的對象的額外訪問，請執行以下操作：

1. 移至您要要求其他存取權的物件。

1. 按一下 **更多** 內嵌在專案名稱中的功能表，然後按一下 **要求更多存取權**.\
   ![](assets/request-access-in-project-350x201.png)

1. （條件性）如果一個以上的使用者有權授予您其他存取權，則使用者名稱旁會顯示下拉式箭頭。
1. 從下拉式清單中選取您要接收存取請求的使用者。\
   下拉式清單中只會顯示10位使用者。 清單按字母順序排序。\
   如需此下拉式功能表中所列使用者順序的詳細資訊，請參閱  [「請求存取」和「請求更多存取」下拉式功能表的階層](#hierarchy-of-the-request-access-and-request-more-access-drop-down-menus).

1. 從下拉式清單中，選取您要求的存取層級。
1. （選用）在 **P.S.** 欄位中，指定您為何需要其他存取權的附註。
1. 按一下 **請求存取**.\
   ![](assets/request-access-dialog-350x314.png)

## 「請求存取」和「請求更多存取」下拉式功能表的階層 {#hierarchy-of-the-request-access-and-request-more-access-drop-down-menus}

* [了解「請求存取」和「請求更多存取」下拉式功能表中所列的使用者階層](#understand-the-hierarchy-of-users-listed-in-the-request-access-and-request-more-access-drop-down-menus)
* [了解物件的擁有者](#understand-the-owner-of-an-object)

### 了解「請求存取」和「請求更多存取」下拉式功能表中所列的使用者階層 {#understand-the-hierarchy-of-users-listed-in-the-request-access-and-request-more-access-drop-down-menus}

在物件上填入「要求存取」或「要求更多存取」清單時，Workfront會選取最多10個使用者的清單，這些使用者在共用物件時會履行下列說明的各種角色。 這些使用者可將物件的存取權授予要求該物件的使用者。\
然後，產生的清單會依名稱以遞增字母順序排序。\
Workfront會在「請求存取」和「請求更多存取」清單中顯示最多10位使用者。 

「請求存取」或「請求更多存取」下拉式功能表中的使用者順序，由下列規則決定： 

* 清單中的第一個使用者是物件「擁有者」，如 [了解物件的擁有者](#understand-the-owner-of-an-object). 
* 接著，清單會填入個別共用物件的使用者。 按字母順序列出。
* 接著，清單中會進一步填入透過與團隊、群組或公司共用而取得必要存取權的使用者。 按字母順序列出。
* 如果清單空白，系統會新增Workfront管理員，讓一律有人要求存取權。 按字母順序列出。 
* 清單中的每個用戶必須具有請求的對對象的訪問權和共用對象的訪問權限。 

### 了解物件的擁有者 {#understand-the-owner-of-an-object}

對象的所有者定義如下：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>物件</strong> </th> 
   <th><strong>對象所有者的定義</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>專案</td> 
   <td>責任人是項目責任人，或者如果項目責任人丟失或他們沒有必要的訪問權限，則是父產品組合的責任人。 <p>他們可能與專案建立者不同。 </p></td> 
  </tr> 
  <tr> 
   <td>任務</td> 
   <td>責任人是主要受讓人，或者，如果主要受讓人丟失或沒有必要的訪問權限，則是任務所在的項目的責任人，如上所定義。 <p>他們可能與任務建立者不同。 </p></td> 
  </tr> 
  <tr> 
   <td>問題</td> 
   <td> <p>所有者是問題的主要聯繫人，或者，如果缺少問題或他們沒有必要的訪問權限，則是問題所在項目的所有者（如上所定義）。 </p> <p>他們可能與期刊建立者不同。 </p> </td> 
  </tr> 
  <tr> 
   <td>專案組合</td> 
   <td>擁有者是Portfolio擁有者。 <p>他們可能與產品組合建立者不同。 </p></td> 
  </tr> 
  <tr> 
   <td>文件</td> 
   <td>所有者是文檔的所有者（上載文檔的用戶），或者，如果缺少文檔或者他們沒有必要的訪問權限，則是文檔所在對象的所有者。</td> 
  </tr> 
  <tr> 
   <td>報表和控制面板</td> 
   <td>擁有者是建立者、報表或控制面板。 </td> 
  </tr> 
  <tr> 
   <td>行事曆</td> 
   <td>所有者是日曆的建立者。 依預設，所有使用者都會獲派日曆。 它們被視為該日曆的所有者。 </td> 
  </tr> 
  <tr> 
   <td>篩選器、檢視和群組</td> 
   <td>篩選器、檢視或分組的擁有者即為建立者。 </td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td><span>計畫</span> </td> 
   <td> <p><span>所有者是計畫的建立者。</span> </p> <p>這需要額外的授權。 </p> <p><span>有關Workfront方案計畫器的資訊，請參閱</span> <a href="../../scenario-planner/scenario-planner-overview.md" class="MCXref xref">方案計畫員概覽</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td>目標</td> 
   <td> <p>擁有者是指定為擁有者的使用者。 他們可能與目標建立者不同。 </p> <p>這需要額外的授權。 </p> <p>如需Workfront目標的相關資訊，請參閱 <a href="../../workfront-goals/goal-management/wf-goals-overview.md" class="MCXref xref">Adobe Workfront目標概覽</a>. </p> </td> 
  </tr> 
 </tbody> 
</table>

 
