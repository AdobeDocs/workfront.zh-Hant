---
product-area: documents
navigation-topic: approvals
title: 建立檔案的核准工作流程範本
description: 您可以建立核准範本以簡化核准流程。
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: c18d6c6d-1a09-47c5-af4e-027f7cc48cd7
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/jsEcIKopi-lJOSXQitDnufu3j0AmkWkPmCXtCR0V6nk
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40cid: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 5e9318366f0dff85591a5d5a752920027f5c9b0e
workflow-type: tm+mt
source-wordcount: 895
ht-degree: 3%

---

# 建立檔案的核准工作流程範本

{{highlighted-preview}}

在Workfront設定區域中，擁有標準授權的使用者可以建立可重複使用的核准範本。 核准範本建立後，即可套用至物件之檔案區域中的資產。
>[!IMPORTANT]
>
>本文內容指的更新檔案核准功能僅適用於特定帳戶。 如需有關標準核准程式的資訊，請參閱[工作核准](/help/quicksilver/review-and-approve-work/manage-approvals/manage-approvals.md)中列出的文章。

## 存取權要求

+++ 展開以檢視這篇文章中所述功能的存取權要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 封裝</td> 
   <td><p>使用舊版Workfront儲存空間管理核准的任何Workfront套件</p>
<p>使用Adobe雲端儲存空間管理核准的任何Workflow套件</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td> <p>標準</p> 
   <p>規劃</p>
   </td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 在生產環境中建立核准範本

{{step-1-to-setup}}

1. 在左側面板中，按一下&#x200B;**檢閱和核准** > **核准範本**。
1. 按一下頁面右側的&#x200B;**新範本**。

1. 填寫以下詳細資料：

   <table>
     <tr>
   <td><strong>範本名稱</strong></td>
   <td>新增範本名稱。 </td>
   </tr>
   <tr>
   <td><strong>階段名稱</strong></td>
   <td>新增階段名稱。 您可以將名稱變更為描述性更強的名稱，例如<em>初始稽核</em>或<em>最終核准</em>。</td>
   </tr>
   <tr>
   <td><strong>新增姓名或電子郵件</strong></td>
   <td>開始輸入使用者或團隊名稱，以新增為核准者或稽核者。 如果您只有稽核者，他們將會收到通知並可以選擇完成稽核，但不需要或做出任何決定。</td>
   </tr>
   <tr>
   <td><strong>需要一項決定（選擇性）</strong></td>
   <td>第一個做出決定的人會完成階段。</td>
   </tr>
   <tr>
   <td><strong>到期日前的工作日數</strong></td>
   <td>選擇階段啟動後核准到期的工作日數。</td>
   </tr>
   </table>

1. （選擇性）重複上一步驟，視需要新增其他階段。

   >[!NOTE]
   >
   >如果您新增多個階段，核准工作流程會依階段列出的順序進行。 完成所有必要的決定後，下一個階段會開始，而上一個階段會鎖定。

   ![檔案詳細資料](assets/new-stage.png)

1. 按一下「**儲存**」。

建立範本後，可將其套用至物件之檔案區域中的檔案，以在Workfront中開始正式的稽核和核准流程。

<div class="preview">

## 在預覽中建立核准範本

核准範本對話方塊一律會在進階模式下開啟。 範本沒有基本模式。 您可以在範本中設定最多30個平行路徑，總共100個階段。 每個路徑會獨立執行，並可包含一或多個循序階段。

若要建立核准範本，請執行下列動作：

{{step-1-to-setup}}

1. 在左側面板中，按一下&#x200B;**檢閱和核准** > **核准範本**。

1. 按一下頁面右側的&#x200B;**新範本**。

1. 新增&#x200B;**範本名稱**。

1. 填寫路徑1中階段1的詳細資訊：

   <table>
   <tr>
   <td><strong>階段名稱</strong></td>
   <td>依預設，階段名為<em>階段1</em>、<em>階段2</em>等。 將階段重新命名為較清楚描述的階段，例如<em>初始稽核</em>或<em>最終核准</em>。</td>
   </tr>
   <tr>
   <td><strong>新增名稱或電子郵件（選擇性）</strong></td>
   <td>開始輸入使用者或團隊名稱，以新增為核准者或稽核者。 範本中的參與者是選用的。 您可以在範本套用至檔案時新增它們。<p>附註：一次只能將檢閱者或核准者指派給相同資產上的一個開啟階段。 如果同時開啟多個平行階段，則無法將同一個使用者新增至多個階段。</p></td>
   </tr>
   <tr>
   <td><strong>只需要一個決定（選擇性）</strong></td>
   <td>第一個做出決定的人會完成階段。</td>
   </tr>
   <tr>
   <td><strong>到期日之前的工作日（選擇性）</strong></td>
   <td>選擇階段開啟後需要多少個工作日才能完成。 每個路徑的第一階段也支援絕對到期日期。 路徑中的每個後續階段僅支援相對到期日。</td>
   </tr>
   <tr>
   <td><strong>新增自訂訊息（選擇性）</strong></td>
   <td>在<strong>新增自訂訊息</strong>文字方塊中輸入訊息。 將範本套用至檔案時，該訊息會顯示在核准電子郵件通知和Workfront的「核准」索引標籤中。<p>新增第二個階段時，預設會選取<strong>在所有階段顯示此訊息</strong>。 將其保留為選取狀態，以便在每個階段中使用相同的訊息。 若要對每個階段使用不同的訊息，請清除<strong>在所有階段顯示此訊息</strong>，然後在每個階段的<strong>新增自訂訊息</strong>文字方塊中輸入階段專屬訊息。</p></td>
   </tr>
   </table>

   ![新增階段](assets/add-stage.png)

1. （選擇性）按一下&#x200B;**新增階段**&#x200B;以新增另一個階段至路徑。 路徑中的階段會依其列出的順序執行。 當一個階段中的所有必要決定都完成時，該路徑中的下一個階段開始，並且上一個階段被鎖定。 您可以在路徑內重新排序階段，但無法將階段從一個路徑移動到另一個路徑。 每個路徑可以有不同的階段數量。

1. （選擇性）在&#x200B;**平行路徑**&#x200B;下，按一下&#x200B;**新增路徑**&#x200B;以新增其他路徑。 新路徑會從一個空白階段開始，成為選取的路徑。 路徑無法重新排序。

   ![新增平行路徑](assets/add-path.png)

1. （選擇性）若要重新命名路徑，請將游標停留在路徑標籤上，按一下鉛筆圖示，然後輸入新名稱。 若要移除路徑，請將滑鼠指標暫留在路徑標籤上，然後按一下垃圾桶圖示。 **無法移除路徑1**，而且只有在路徑中沒有鎖定或完成的階段時，才能移除其他路徑。

1. （選擇性）若要清除所有路徑和階段並重新開始，請按一下右上角的&#x200B;**重設**。

1. 按一下「**儲存**」。

建立範本後，可將其套用至物件之檔案區域中的檔案，以在Workfront中開始正式的稽核和核准流程。

</div>



<!--
 Once a template is created, it can be applied to assets sent from Frame.io to begin the formal review and approval process in Workfront.
![Assign template](assets/assign-template.png)
-->
