---
title: Workfront檔案中的存取需求
content-type: reference
product-area: system-administration
keywords: 存取，層級，系統，管理員，供需規劃員，工作者，檢閱者，請求者，外部，使用者
navigation-topic: access-levels
description: Workfront檔案how-to文章包含一個表格，說明該程式所需的存取權和許可權。 本文詳細說明存取需求表格，並包含詳細資訊的連結。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 39ea0d53-ec31-4644-b772-cfe260b8e013
source-git-commit: c1c30696dc9ef324103467f3bdcb83609cf5d1d8
workflow-type: tm+mt
source-wordcount: '1010'
ht-degree: 0%

---

# Workfront檔案中的存取需求

Workfront檔案how-to文章包含一個表格，說明該程式所需的存取和許可權需求。 此存取需求表格可讓您瞭解您是否可以在Workfront中執行特定動作，或為何無法執行。 本文說明存取需求表格的每個元素，並提供疑難排解提示和連結，以取得更深入的資訊。

如果指定文章的「存取需求」表格中沒有列，則該動作就沒有該型別的需求。

>[!NOTE]
>
>如果您對此表格中任何欄位如何套用至您有任何疑問，請聯絡Workfront管理員。

## 存取需求表格

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront套件</td> 
   <td> Adobe Workfront套件是指您的組織已購買的一組功能。 大部分的Workfront功能都可在所有套件中使用，只有少數例外，大多與策略規劃和企業控制項有關。 <p>2022年以前存在的套件未列出。</p>
   <p>Workfront套件分為三個區域。 有些區域提供不同的套件，例如Select、Prime和Ultimate。<p>
   <ul>
   <li><b>Workfront工作流程</b>：包含與作業相關的功能，例如工作管理、核准和時程表。 此套件進一步分為「工作流程選取」、「工作流程Prime」和「工作流程Ultimate」套件。</li>
   <li><b>Workfront規劃</b>：包含與策略規劃相關的功能。 此套件進一步分為Planning Select、Planning Prime和Planning Ultimate套件。</li>
   <li><b>Workfront自動化與整合</b>：包含與自動化程式以及與其他應用程式整合相關的功能。</li>
   </ul>
  <p>您的組織可能在一個或多個上述區域購買了Workfront套件。</p>
  <p>之前，Workfront提供Workfront Select、Workfront Prime和Workfront Ultimate套件，而不區分工作流程、計畫和自動化與整合。 您的組織可能位於這些舊版套件之一。 
   <ul><li>若要瞭解貴組織使用哪個Adobe Workfront套件，包括貴組織使用目前的封裝模式或舊版封裝模式，請聯絡Workfront管理員。</li>
   <li>如需Workfront管理員如何找到您組織的Workfront封裝的說明，請參閱<a href="/help/quicksilver/administration-and-setup/get-started-wf-administration/firewall-overview.md#view-your-organizations-cluster-and-workfront-package" class="MCXref xref">檢視您組織的叢集和Workfront封裝</a>。</li><li>如需Workfront套件的詳細資訊，請參閱<a href="https://business.adobe.com/tw/products/workfront/pricing.html">Adobe Workfront定價與封裝</a>。</li></ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td> Adobe Workfront授權指的是一組Workfront功能，包含在指派給您的授權中。 例如，一位使用者可能擁有將工作專案標籤為完成和記錄時間的授權，而另一位使用者擁有僅允許其核准資產或提交請求的授權。 <p> 
   <ul>
   <li>若要瞭解系統指派給您的授權，請連絡Workfront管理員。</li>
   <li>如需授權的相關資訊，請參閱：
   <ul>
   <li><a href="/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/licenses-overview.md" class="MCXref xref">新授權總覽</a></li>
   <li><a href="/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">授權總覽</a></li></ul></li>
   <li>如果您擁有正確的存取層級，但仍然沒有存取權，請詢問您的Workfront管理員，他們是否對您的存取層級設定其他限制。 如需Workfront管理員如何修改存取層級的詳細資訊，請參閱<a href="/help/quicksilver/administration-and-setup/get-started-wf-administration/firewall-overview.md#view-your-organizations-cluster-and-workfront-package" class="MCXref xref">建立或修改自訂存取層級</a>。
   </ul>
      </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td><p>由於Workfront可與其他Adobe產品密切合作，因此Workfront中的某些程式會直接與這些產品互動。 若要遵循這些程式，您的組織必須已購買該產品。 例如，若要使用可讓Workfront與Adobe Experience Manager Assets互動的功能，您的組織必須已購買Adobe Experience Manager Assets。</p>
   <p>描述使用其他產品執行的程式的文章列出此表格的「產品」系列中所需的產品。</p>
   <p>若要瞭解您的組織是否已購買這些額外產品之一，請聯絡您的Workfront管理員。</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級</td> 
   <td> 存取層級是您可以在Workfront中執行動作的一組許可權，由Workfront管理員設定。 <p>Workfront有與Workfront授權對應的內建存取層級，但您的Workfront管理員可以建立更多存取層級，以更準確地反映組織所需的許可權集。</p>
   <ul>
    <li>如需有關存取層級的資訊，請參閱：
   <ul>
   <li><a href="/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md" class="MCXref xref">新存取層級概觀</a></li>
   <li><a href="/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md" class="MCXref xref">存取層級概觀</a></li></ul></li>
    <li>若要瞭解存取層級的詳細資訊，請聯絡Workfront管理員</li>
    <li>如果您是Workfront管理員，請參閱<a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/configure-access.md" class="MCXref xref">設定Adobe Workfront的存取權</a>，深入瞭解如何授與存取層級中特定物件的存取權。</li>  
   <li>如果您擁有正確的存取層級，但仍然沒有存取權，請詢問您的Workfront管理員，他們是否對您的存取層級設定其他限制。 如需Workfront管理員如何修改存取層級的詳細資訊，請參閱<a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>。</li>
    </td>
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td><p>物件許可權是指當您建立個別Workfront物件或與您共用這些物件時，您對物件擁有的存取權。 例如，您必須擁有特定專案的檢視存取權才能檢視專案，即使您的存取層級允許您檢視專案。 「存取需求」表格的這個段落說明您在文章中執行動作所需的任何特定物件許可權。</p>
   <p>如需請求物件其他存取權的資訊，請參閱<a href="/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求物件的存取權</a>。</p><p>如需共用物件的資訊，請參閱<a href="/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/share-an-object.md" class="MCXref xref">共用物件</a>。</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">版面配置範本</td> 
   <td><p>版面配置範本可控制您在主功能表中看到的內容，並由Workfront管理員設定。 此行會記下您的主要功能表中必須包含的任何特定Workfront區域，才能執行動作。</p><p>一般而言，如果文章指示您按一下主要功能表中的某個區域，但主要功能表中未顯示該區域，請聯絡您的Workfront管理員以判斷該區域是否可供您使用。</p><p>
   如需Workfront管理員如何設定主功能表的資訊，請參閱<a href="/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md" class="MCXref xref">使用版面配置範本自訂主功能表</a>。</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront Fusion授權</td> 
   <td>Adobe Workfront Fusion與Workfront有不同的授權模型。 
   <ul><li>目前的授權模型是以執行的作業數為基礎，對組織可執行的動作沒有限制。 </li>
   <li>舊版授權取決於案例能否連線至協力廠商應用程式，或案例是否僅用於Workfront自動化。 </li>
   </ul>
   如需Fusion授權的詳細資訊，請參閱<a href="https://experienceleague.adobe.com/zh-hant/docs/workfront-fusion/using/set-up-and-manage-fusion/licensing-and-operations-overviews/license-automation-vs-integration" class="MCXref xref">Workfront Fusion授權</a>。
   </td> 
  </tr> 
 </tbody> 
</table>
