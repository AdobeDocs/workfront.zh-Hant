---
title: 存取層級需求
content-type: reference
product-area: system-administration
keywords: 存取，層級，系統，管理員，供需規劃員，工作者，檢閱者，請求者，外部，使用者
navigation-topic: access-levels
description: Workfront檔案how-to文章包含一個表格，說明該程式所需的存取權和許可權。 本文詳細說明存取需求表格，並包含詳細資訊的連結。
author: Becky
feature: System Setup and Administration
role: Admin
hide: true
hidefromtoc: true
source-git-commit: 66957a8bb24538fd302fe0ff7612b266da18118f
workflow-type: tm+mt
source-wordcount: '869'
ht-degree: 0%

---

# Workfront檔案中的存取層級要求

Workfront檔案how-to文章包含一個表格，說明該程式所需的存取和許可權需求。 此存取需求表格可讓您瞭解您是否可以在Workfront中執行特定動作，或為何無法執行。 本文說明存取需求表格的每個元素，並提供疑難排解提示和連結，以取得更深入的資訊。

如果指定文章的「存取需求」表格中沒有列，則該動作就沒有該型別的需求。

某些列包含標示為「新」和「目前」的資訊。 這是因為Workfront正在轉換到新的定價和封裝模式，有些組織會在新模式下運作，有些組織則仍在使用目前的模式。 若要瞭解您的組織使用哪種模型，請聯絡您的Workfront管理員。 您可以在以下連結中找到詳細資訊和資訊連結： [存取需求表格](#the-access-requirements-table) 一節。

>[!NOTE]
>
>如果您對此表格中任何欄位如何套用至您有任何疑問，請聯絡Workfront管理員。

## 存取需求表格

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td> Adobe Workfront計畫會參考貴組織已購買的一組功能。 大部分的Workfront功能都可在所有計畫中使用，只有少數例外，大多與策略規劃及企業控制有關。 
   <ul><li>若需瞭解貴組織使用哪種Adobe Workfront計畫，包括貴組織使用的新封裝模式或目前封裝模式，請聯絡您的Workfront管理員。</li>
   <li>如需Workfront管理員如何找出貴組織Workfront計畫的指示，請參閱 <a href="/help/quicksilver/administration-and-setup/get-started-wf-administration/firewall-overview.md#view-your-organizations-cluster-and-workfront-plan" class="MCXref xref">檢視貴組織的叢集和Workfront計畫</a>.</li></ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td> Adobe Workfront授權指的是一組Workfront功能，包含在指派給您的授權中。 例如，一位使用者可能擁有將工作專案標籤為完成和記錄時間的授權，而另一位使用者擁有僅允許其核准資產或提交請求的授權。 <p> 
   <ul>
   <li>若要瞭解系統指派給您的授權，請連絡Workfront管理員。</li>
   <li>Adobe Workfront正在轉換至新的定價與封裝模式。 如需授權的相關資訊，請參閱：
   <ul>
   <li>新增： <a href="/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/licenses-overview.md" class="MCXref xref">新授權總覽</a></li>
   <li>目前： <a href="/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">授權總覽</a></li></ul></li>
   <li>如果您擁有正確的存取層級，但仍然沒有存取權，請詢問您的Workfront管理員，他們是否對您的存取層級設定其他限制。 如需有關Workfront管理員如何修改您的存取層級的資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.
   </ul>
      </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>除了Workfront之外，Workfront還提供一些可以購買的產品。
   <p>說明在這些其他產品內執行的程式的文章在此處列出了所需的產品。</p>
   <ul>
   <li>Adobe Experience Manager Assets或Assets Essentials </li>
   <li>Workfront Fusion</li>
   <li>Workfront Goals</li>
   <li>Workfront情境規劃工具</li>
   </ul>
   <p>若要瞭解您的組織是否已購買這些額外產品之一，請聯絡您的Workfront管理員。</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級</td> 
   <td> 存取層級是您可以在Workfront中執行動作的一組許可權，由Workfront管理員設定。 <p>Workfront有與Workfront授權對應的內建存取層級，但您的Workfront管理員可以建立更多存取層級，以更準確地反映組織所需的許可權集。</p>
   <ul>
    <li>Adobe Workfront正在轉換至新的定價與封裝模式。 如需每個模型的存取層級相關資訊，請參閱：
   <ul>
   <li>新增： <a href="/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md" class="MCXref xref">新存取層級概觀</a></li>
   <li>目前： <a href="/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md" class="MCXref xref">存取層級概觀</a></li></ul></li>
    <li>若要瞭解存取層級的詳細資訊，請聯絡Workfront管理員</li>
    <li>如果您是Workfront管理員，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md" class="MCXref xref">設定Adobe Workfront的存取權</a> 以進一步瞭解在存取層級中授與特定物件的存取權。</li>  
   <li>如果您擁有正確的存取層級，但仍然沒有存取權，請詢問您的Workfront管理員，他們是否對您的存取層級設定其他限制。 如需有關Workfront管理員如何修改您的存取層級的資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</li>
    </td>
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td><p>物件許可權是指當您建立個別Workfront物件或與您共用這些物件時，您對物件擁有的存取權。 例如，您必須擁有特定專案的檢視存取權才能檢視專案，即使您的存取層級允許您檢視專案。 「存取需求」表格的這個段落說明您在文章中執行動作所需的任何特定物件許可權。</p>
   <p>如需請求物件的其他存取許可權的相關資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">要求物件的存取權</a>.</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>除了Workfront之外，Workfront還提供一些可以購買的產品。
   <p>說明在這些其他產品內執行的程式的文章在此處列出了所需的產品。</p>
   <ul>
   <li>Adobe Experience Manager Assets或Assets Essentials </li>
   <li>Workfront Fusion</li>
   <li>Workfront Goals</li>
   <li>Workfront情境規劃工具</li>
   </ul>
   <p>若要瞭解您的組織是否已購買這些額外產品之一，請聯絡您的Workfront管理員。</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront Fusion授權</td> 
   <td>Adobe Workfront Fusion與Workfront有不同的授權模型。 
   <ul><li>目前：目前的許可證模型是以執行的作業數為基礎，對組織可執行的動作沒有限制。 </li>
   <li>舊版：舊版授權取決於案例能否連線至協力廠商應用程式，或案例是否僅用於Workfront自動化。 </li>
   </ul>
   如需Fusion授權的相關資訊，請參閱 <a href="/help/quicksilver/workfront-fusion/get-started/license-automation-vs-integration.md" class="MCXref xref">Workfront Fusion授權</a>.
   </td> 
  </tr> 
 </tbody> 
</table>


