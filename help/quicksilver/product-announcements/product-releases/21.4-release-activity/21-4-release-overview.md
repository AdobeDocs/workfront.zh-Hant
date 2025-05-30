---
content-type: release-notes
keywords: 備註，每季，更新
navigation-topic: 2021-4-release-activity
title: 21.4版本總覽
description: 本頁提供Adobe Workfront Classic功能和21.4版所含新Adobe Workfront體驗的相關資訊。 協助您釋放生產力和協同合作。[此發行版本的行銷單一版面]
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 0897b269-c6f3-4b63-8956-b7f9fbe0a553
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '4718'
ht-degree: 0%

---

# 21.4版本總覽

本頁提供Adobe Workfront Classic功能和21.4版所含新Adobe Workfront體驗的相關資訊。

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
to help you unlock productivity and collaboration.
</MadCap:conditionalText>
-->

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
[Marketing one-liner for the release]
</MadCap:conditionalText>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">These enhancements are currently available in the Preview environment. As the 21.4 release nears its planned Production release the week of October 4, 2021
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in October 2021
</MadCap:conditionalText>
, this page will be updated with all functionality included with 21.4.</p>
-->

這些增強功能已在2021年10月4日當週的生產環境中推出。

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
These enhancements are currently available in the Preview environment and will be made available in the Production environment the week of October 4, 2021
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
,
</MadCap:conditionalText>
</MadCap:conditionalText>
-->

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
unless otherwise specifiedthe week of May 10, 2021.
</MadCap:conditionalText>


For specific release dates and times for each cluster, see the [Adobe Workfront status page](https://status.adobe.com/en/products/5943) on [status.adobe.com](http://status.adobe.com/). You must log in to see specific release times.

-->

## Adobe Workfront增強功能

* [管理員增強功能](#administrator-enhancements)
* [敏捷增強功能](#agile-enhancements)
* [專案增強功能](#project-enhancements)
* [資源管理增強功能](#resource-management-enhancements)
* [報告增強功能](#reporting-enhancements)
* [要求增強功能](#requests-enhancements)
* [校訂增強功能](#proofing-enhancements)
* [整合增強功能](#integration-enhancements)
* [行動裝置增強功能](#mobile-enhancements)
* [其他增強功能](#other-enhancements)

### 管理員增強功能 {#administrator-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>功能</strong> </p> </td> 
   <td> <p><strong>發行日期與環境</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-admin-enhancements.md#for" class="MCXref xref" xrefformat="{para}">對於管理員：檢視哪些群組與核准程式相關聯</a> </p> <p>為協助您找出哪些群組與系統中的核准流程相關聯，我們在「設定」的「核准」頁面上，將「群組名稱」欄新增至「標準」檢視。 現在，您無需建立自訂檢視即可檢視此資訊。</p> </td> 
   <td> <p><b>在以下日期可用：</b> </p> <p>預覽版本： 2021年9月9日<br></p> <p>生產版本：第21.4發行版本</p> <p><strong>在以下環境中可用：</strong> </p> <p>全新Adobe Workfront體驗 </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-admin-enhancements.md#new" class="MCXref xref" xrefformat="{para}">管理員的新設定：群組可以設定自己的時程表和小時喜好設定</a> </p> <p>在大型組織中，某些群組可能需要單獨設定時程表和小時偏好設定以符合其獨特的工作流程，而不是繼承系統管理員在系統層級設定的偏好設定。 現在，Workfront管理員可以解鎖系統中所有群組的時程表和小時偏好設定，以便他們能夠自行設定。</p> <p>此功能最近也針對專案偏好設定以及任務和問題偏好設定新增。</p> </td> 
   <td> <p><b>在以下日期可用：</b> </p> <p>預覽版本： 2021年9月9日<br></p> <p>生產版本：使用21.4版本<span style="color: #ff0000;"> （最初僅在生產環境中提供給叢集4上的客戶）</span></p> <p><strong>在以下環境中可用：</strong> </p> <p>全新Adobe Workfront體驗 </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-admin-enhancements.md#new2" class="MCXref xref" xrefformat="{para}">Workfront管理員的新功能：為新Workfront體驗中自動布建的使用者設定版面配置範本</a> </p> <p>現在您可以在新的Workfront體驗中設定版面配置範本，供自動布建的使用者使用。 在對應使用者屬性的Workfront「使用者屬性」下拉式功能表中（「設定」&gt;「系統」&gt;「單一登入」），新的「全新配置範本」功能表專案現在可用於進行此設定。 之前，您只能在Workfront Classic中為自動布建的使用者設定版面範本。</p> </td> 
   <td> <p><b>在以下日期可用：</b> </p> <p>預覽版本： 2021年9月9日<br></p> <p>生產版本：第21.4發行版本</p> <p><strong>在以下環境中可用：</strong> </p> <p>全新Adobe Workfront體驗 </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-admin-enhancements.md#new3" class="MCXref xref" xrefformat="{para}">新欄位顯示您的使用者所屬的群組</a> </p> <p>現在，您可輕鬆瞭解使用者屬於哪些群組。 在列出使用者的報表或檢視中，您可以使用新的「其他群組」欄位來建立欄。 此欄位會列出每個使用者所屬的群組。</p> </td> 
   <td> <p><b>在以下日期可用：</b> </p> <p>預覽版本： 2021年9月9日<br></p> <p>生產版本：第21.4發行版本</p> <p><strong>在以下環境中可用：</strong> </p> <p>全新Adobe Workfront體驗 </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-admin-enhancements.md#blueprin" class="MCXref xref" xrefformat="{para}">藍圖詳細資訊頁面現在會顯示影像</a> </p> <p>現在，每個Blueprint的詳細資訊頁面都會顯示與Blueprint一起安裝的專案範本影像。 此影像提供Blueprint內容的預覽，讓您知道要安裝的內容。 您可以選擇在瀏覽器中預覽完整影像或下載影像。</p> </td> 
   <td><strong>在以下日期可用：</strong> <p>預覽版本： 2021年9月9日<br></p> <p>生產版本：第21.4發行版本</p> <p><strong>在以下環境中可用：</strong> </p> <p>全新Adobe Workfront體驗 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-admin-enhancements.md#blueprin2" class="MCXref xref" xrefformat="{para}">新問題的Blueprint偏好設定</a> </p> <p>某些Blueprint現在提供新的問題偏好設定。 預設會安裝偏好設定，但當您設定安裝詳細資訊時，可以選擇退出安裝偏好設定。</p> <p>偏好設定包括佇列主題群組、佇列主題和路由規則，可在提交問題或請求時收集正確資訊，並將問題或請求傳送給正確的工作角色或團隊。 使用偏好設定有助於在專案上擷取新問題或請求的方式建立一致性。</p> <p>請注意，使用這些偏好設定不會將從範本建立的專案放入請求佇列。</p> </td> 
   <td><strong>在以下日期可用：</strong> <p>預覽版本： 2021年9月9日<br></p> <p>生產版本：第21.4發行版本</p> <p><strong>在以下環境中可用：</strong> </p> <p>全新Adobe Workfront體驗 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-admin-enhancements.md#new4" class="MCXref xref" xrefformat="{para}">群組管理員的新專案：檢視及管理群組最近刪除及還原的專案</a> </p> <p>我們持續讓您更輕鬆地集中管理群組及其相關物件。 現在，您可以從「群組」區域檢視和使用群組最近刪除和還原的專案。 這可讓您無須前往「設定」中的「最近刪除」或「最近還原」區域來管理這些專案。 而且它會將您正在使用的群組專案清單與系統中其他已刪除和還原的專案分開。</p> </td> 
   <td><strong>在以下日期可用：</strong> <p>預覽版本： 2021年8月26日<br></p> <p>生產版本：第21.4發行版本</p> <p><strong>在以下環境中可用：</strong> </p> <p>全新Adobe Workfront體驗 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-admin-enhancements.md#new5" class="MCXref xref" xrefformat="{para}">群組管理員的新設定：群組偏好設定現在會影響群組範本</a> </p> <p>現在，可以更輕鬆確定您群組的專案範本符合您群組的需求。 當您在建立群組時將新專案範本指派給群組時，範本會繼承群組的專案和任務偏好設定中的各種設定。</p> <p>當您在與群組相關聯的專案範本中建立新範本任務時，範本任務會繼承群組任務偏好設定的各種設定。</p> <p>以前，專案範本和專案範本任務從系統層級設定的專案和任務偏好設定繼承這些設定。</p> <p>如果您建立沒有群組的範本或範本任務（例如，從主「範本」頁面），則上述設定會繼承自系統層級的專案和任務偏好設定。 但是，如果您稍後將群組指派給範本或範本任務，群組的偏好設定不會影響它。</p> </td> 
   <td> <p>預覽版本： 2021年8月26日<br></p> <p>生產版本：第21.4發行版本</p> <p><strong>在以下環境中可用：</strong> </p> <p>全新Adobe Workfront體驗 </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-admin-enhancements.md#new6" class="MCXref xref" xrefformat="{para}">管理員的新功能：瞭解哪些自訂表單正在使用自訂欄位</a> </p> <p>現在變更自訂表單中的自訂欄位更容易。 只要在自訂表單中按一下，您就可以找到有關也使用該欄位的任何其他自訂表單。 請務必評估這些表單是否需要調整，以便在您進行變更後能夠繼續正常運作。</p> </td> 
   <td><strong>在以下日期可用：</strong> <p>預覽版本： 2021年8月19日<br></p> <p>生產版本：第21.4發行版本</p> <p><strong>在以下環境中可用：</strong> </p> <p>全新Adobe Workfront體驗 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-admin-enhancements.md#new7" class="MCXref xref" xrefformat="{para}">群組管理員的新功能：鎖定並解除鎖定群組的專案、任務和問題偏好設定</a> </p> <p>現在您可以確保群組及其子群組中的每個人都針對專案、任務或問題偏好設定使用相同的設定。 Workfront管理員在系統層級解除鎖定偏好設定後，您就可以進行設定，然後為群組鎖定它。 雖然您仍可重新設定鎖定的群組偏好設定，但較低子群組的管理員無法為其群組分別執行此操作。</p> </td> 
   <td><strong>在以下日期可用：</strong> <p>預覽版本： 2021年8月12日<br></p> <p>生產版本：第21.4發行版本</p> <p><strong>在以下環境中可用：</strong> </p> <p>全新Adobe Workfront體驗 </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-admin-enhancements.md#new8" class="MCXref xref" xrefformat="{para}">群組管理員的新功能：從群組區域建立和編輯範本</a> </p> <p>我們持續讓您更輕鬆地在一個位置管理群組及其關聯的物件。 現在您可以從「設定」的「群組」區域檢視和使用群組的範本。 這可讓您無須前往「範本」區域來管理群組的範本。 而且它會將您正在處理的群組範本清單與整個系統中的其他群組範本清單分開。</p> </td> 
   <td><strong>在以下日期可用：</strong> <p>預覽版本： 2021年8月12日<br></p> <p>生產版本：第21.4發行版本</p> <p><strong>在以下環境中可用：</strong> </p> <p>全新Adobe Workfront體驗 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-admin-enhancements.md#enter" class="MCXref xref" xrefformat="{para}">一次在一個附加的自訂表單中輸入並儲存資訊</a> </p> <p>現在，在物件的詳細資訊區段中提供資訊變得更加容易：在單一自訂欄位或可展開區域（例如Overview和Finance）中輸入並儲存資訊，即使物件上其他自訂表單中的必填欄位尚未填寫。</p> <p>先前，當您在一個自訂表單或物件的可展開區域中輸入資訊時，附加到物件的所有自訂表單都會進入編輯模式，而且您必須先完成其所有必填欄位，然後才能儲存變更。 如果您因為某個必填欄位是提供給其他使用者而無法完成，則會發生問題。</p> </td> 
   <td><strong>在以下日期可用：</strong> <p>預覽版本： 2021年7月22日<br></p> <p>生產版本：第21.4發行版本</p> <p><strong>在以下環境中可用：</strong> </p> <p>全新Adobe Workfront體驗 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-admin-enhancements.md#new9" class="MCXref xref" xrefformat="{para}">群組管理員的新增：建立和管理任何層級群組的狀態</a> </p> <p>為了更方便組織的所有層級獨立管理和控制其工作流程，我們引進了建立和管理子群組狀態的功能。 </p> </td> 
   <td><strong>在以下日期可用：</strong> <p>預覽版本：2021年6月3日（21.3版本週期內）<br></p> <p>生產版本： 2021年7月22日</p> <p><strong>在以下環境中可用：</strong> </p> <p>全新Adobe Workfront體驗 </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-admin-enhancements.md#new10" class="MCXref xref" xrefformat="{para}">Workfront管理員的新功能：自行將版面配置範本從Workfront Classic移轉到新的Workfront體驗</a> </p> <p>為協助您在使用者切換使用新Workfront體驗時管理版面範本，我們已建立按鈕，您可以使用它將版面範本從Workfront Classic移轉到新體驗，而不依賴Workfront客戶支援。</p> <p>之前，只有Workfront客戶支援可將您的版面配置範本從Workfront Classic移轉到新的Workfront體驗。</p> </td> 
   <td><strong>在以下日期可用：</strong> <p>預覽版本： 2021年7月1日<br></p> <p>生產版本： 2021年7月15日</p> <p><strong>在以下環境中可用：</strong> </p> <p>全新Adobe Workfront體驗 </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-admin-enhancements.md#when" class="MCXref xref" xrefformat="{para}">將範本與群組建立關聯時，請在佇列詳細資料和佇列主題</a>中選取群組核准程式 </p> <p>我們在建立範本與群組的關聯程式中，新增了一個選項。 現在，您可以在範本的「佇列詳細資訊」或其中一個佇列主題中，為問題選取群組特定的核准流程。</p> <p>在21.3中，當我們新增將群組範本與群組建立關聯的功能時，您可以在範本中選取群組特定的核准程式，但您無法在範本的「佇列詳細資訊」或「佇列主題」中執行此操作。</p> </td> 
   <td><strong>在以下日期可用：</strong> <p>預覽版本： 2021年7月1日<br></p> <p>生產版本：第21.4發行版本</p> <p><strong>在以下環境中可用：</strong> </p> <p>全新Adobe Workfront體驗 </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
 </tbody> 
</table>

### 專案增強功能 {#project-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>功能</strong> </p> </td> 
   <td> <p><strong>發行日期與環境</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-project-enhancements.md#include" class="MCXref xref" xrefformat="{para}">在更新中包含影像</a> </p> <p>在物件的「更新」標籤上，您現在可以按一下工具列上的「影像」圖示來新增影像。 您也可以將影像拖放至更新區域。 請注意，您必須先啟用Workfront管理員新增影像，才能看到影像圖示。</p> <p>您可以在更新與回覆中新增影像。 更新中的影像縮圖表示收件者可以在瀏覽器中預覽或下載影像，而電子郵件和應用程式內通知會顯示影像已附加至更新。</p> <p>之前，在Workfront中共用影像的唯一方式是將影像作為檔案附加至物件。 在「更新」標籤上新增的影像只能在該標籤上使用，不能在「檔案」標籤上使用。</p> <p>在Workfront使用者能在更新中包含影像之前，此功能必須先由Adobe Workfront管理員啟用。</p> </td> 
   <td><strong>在以下日期可用：</strong> <p>預覽版本： 2021年9月9日<br></p> <p>生產版本：第21.4發行版本</p> <p><strong>在以下環境中可用：</strong> </p> <p>全新Adobe Workfront體驗 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-project-enhancements.md#updated" class="MCXref xref" xrefformat="{para}">已更新智慧指派的演演算法</a> </p> <p>我們已改善進行智慧型指派時使用的演演算法。 透過新的改進，Workfront會檢視登入使用者最近進行的30個指派，以在他們指派任務和問題時提供建議。 建議清單最多可包含50位使用者。 </p> <p>在此增強功能之前，Workfront在建議使用者時，會考慮父系任務上的指派以及與這些指派相關的其他使用者屬性。</p> </td> 
   <td><strong>在以下日期可用：</strong> <p>預覽版本： 2021年9月9日<br></p> <p>生產版本：第21.4發行版本</p> <p><strong>在以下環境中可用：</strong> </p> <p>全新Adobe Workfront體驗 </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-project-enhancements.md#new" class="MCXref xref" xrefformat="{para}">從範本建立專案時的新體驗</a> </p> <p>為了讓您使用Workfront與新的Workfront體驗一致，我們重新設計了介面，用於從範本建立專案。 使用範本建立專案的功能並未變更。 不過，這個全新重新設計的介面有以下幾項改善專案：</p> 
    <ul> 
     <li> <p>附加範本資訊之前先預覽範本資訊</p> </li> 
     <li> <p>在專案建立過程中將範本新增至我的最愛清單</p> </li> 
    </ul> <p>當您從專案和範本區域建立專案時，我們已更新用於建立專案的介面。</p> </td> 
   <td><strong>在以下日期可用：</strong> <p>預覽版本： 2021年9月9日<br></p> <p>生產版本：第21.4發行版本</p> <p><strong>在以下環境中可用：</strong> </p> <p>全新Adobe Workfront體驗 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-project-enhancements.md#new2" class="MCXref xref" xrefformat="{para}">將範本附加到專案時的新體驗</a> </p> <p>為了讓您使用Workfront與新的Workfront體驗一致，我們重新設計了介面以將範本附加到專案。 附加範本的功能未變更。 不過，這個全新重新設計的介面有一些改良功能，包括下列專案：</p> 
    <ul> 
     <li> <p>附加範本資訊之前先預覽範本資訊</p> </li> 
     <li> <p>在附件程式期間將範本新增至我的最愛清單</p> </li> 
     <li> <p>在一個連續頁面中檢視用於管理範本和專案設定的所有選項</p> </li> 
    </ul> </td> 
   <td><strong>在以下日期可用：</strong> <p>預覽版本： 2021年8月26日<br></p> <p>生產版本：第21.4發行版本</p> <p><strong>在以下環境中可用：</strong> </p> <p>全新Adobe Workfront體驗 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-project-enhancements.md#unified" class="MCXref xref" xrefformat="{para}">任務的統一期間和期間單位值</a> </p> <p>為了提供更乾淨且更精簡的使用者體驗，我們已將「持續時間」欄位的值與持續時間單位合併。 在此增強功能之前，時間單位會顯示在持續時間欄位後面的個別下拉式欄位中。</p> <p>除了「任務詳細資訊」、「編輯任務」和「新任務」方塊中的「工期」欄位外，我們也會更新下列欄位以符合此體驗：</p> 
    <ul> 
     <li> <p>進行進階指派時的期間欄位</p> </li> 
     <li> <p>建立或編輯任務時平準延遲欄位</p> </li> 
     <li> <p>建立週期性任務時的頻率欄位（即將推出）</p> </li> 
     <li> <p>新增前置任務時的延遲欄位（即將推出）</p> </li> 
    </ul> </td> 
   <td><strong>在以下日期可用：</strong> <p>預覽版本： 2021年8月19日<br></p> <p>生產版本：第21.4發行版本</p> <p><strong>在以下環境中可用：</strong> </p> <p>全新Adobe Workfront體驗 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-project-enhancements.md#disable" class="MCXref xref" xrefformat="{para}">停用在專案上新增內嵌問題</a> </p> <p>為確保使用者完成問題表單以將問題新增至專案時可提供準確資訊，我們引入了一項新設定，可讓您管理使用者是否可以將問題新增至專案或其內嵌任務。 此設定預設在編輯專案方塊的新問題設定區域中啟用。 若停用此專案，專案問題區段中的新增更多問題選項會變暗，因此使用者無法在清單中新增任何其他問題。 使用者仍然可以透過使用問題區段中的新問題選項或使用請求佇列（如果為專案配置了請求佇列）將問題新增到專案。</p> </td> 
   <td><strong>在以下日期可用：</strong> <p>預覽版本： 2021年8月5日<br></p> <p>生產版本：第21.4發行版本</p> <p><strong>在以下環境中可用：</strong> </p> <p>全新Adobe Workfront體驗 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-project-enhancements.md#custom" class="MCXref xref" xrefformat="{para}">核取方塊和選項按鈕的自訂欄位顯示改善</a> </p> <p>在自訂表單中檢視及選取核取方塊和選項按鈕選項變得更加容易 — 包含許多核取方塊或選項按鈕選項的自訂欄位現在顯示在頁面的多個欄中。 以前，它們會顯示在單一欄中，使用者填寫表單時需要進行額外的捲動。</p> <p>這取決於您在自訂表單中放置欄位的方式 — 如果您將另一個欄位與核取方塊或選項按鈕欄位放在同一列，則選項可能只有足夠的水準空間可顯示在單一欄中。</p> </td> 
   <td><strong>在以下日期可用：</strong> <p>預覽版本： 2021年7月29日<br></p> <p>生產版本：第21.4發行版本</p> <p><strong>在以下環境中可用：</strong> </p> <p>全新Adobe Workfront體驗 </p> </td> 
  </tr> 
 </tbody> 
</table>

### 資源管理增強功能 {#resource-management-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>功能</strong> </p> </td> 
   <td> <p><strong>發行日期與環境</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-resource-management-enhancements.md#make" class="MCXref xref" xrefformat="{para}">在工作負載平衡器</a>中進行快速指派 </p> <p>您現在可以透過從未指派區域拖曳專案並將其放置在已指派區域中的使用者行上，以最少點按次數有效平衡工作負載平衡器中的資源。 您也可以使用拖放功能從使用者中取消指派專案，並將它們移回「未指派」區域，以及將它們移動給其他使用者。 </p> <p>在此增強功能之前，您只能透過按一下任務或問題的更多選單，然後使用指派選項來指派專案。 現在，分配給使用者的計畫時數在拖曳任務時即時更新。</p> </td> 
   <td><strong>在以下日期可用：</strong> <p>預覽版本： 2021年9月9日<br></p> <p>生產版本：第21.4發行版本</p> <p><strong>在以下環境中可用：</strong> </p> <p>全新Adobe Workfront體驗 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-resource-management-enhancements.md#new" class="MCXref xref" xrefformat="{para}">工作負載平衡器的新預設選項</a> </p> <p>為了淘汰排程並改用工作負載平衡器Workfront的主要資源指派工具，我們已將Workfront平衡器設為所有新使用者的預設選項。 目前，排程是預設選項。 此變更適用於您可從中存取排程的所有區域，包括「資源」區域(在新的Adobe Workfront體驗中)或「人員」區域(在Adobe Workfront Classic中)，以及專案和團隊層級。</p> </td> 
   <td><strong>在以下日期可用：</strong> <p>預覽版本： 2021年9月9日<br></p> <p>生產版本：第21.4發行版本</p> <p><strong>在以下環境中可用：</strong> </p> <p>全新Adobe Workfront體驗 </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-resource-management-enhancements.md#new2" class="MCXref xref" xrefformat="{para}">工作負載平衡器的新篩選器體驗</a> </p> <p>我們重新設計了工作負載平衡器的篩選器體驗，以包含以下附加功能：</p> 
    <ul> 
     <li> <p>更簡單、更精簡的使用者介面，符合新的Workfront體驗</p> </li> 
     <li> <p>可篩選的其他欄位</p> </li> 
     <li> <p>複製篩選器的功能</p> </li> 
     <li> <p>與其他使用者共用篩選器</p> </li> 
    </ul> </td> 
   <td><strong>在以下日期可用：</strong> <p>預覽版本： 2021年9月16日<br></p> <p>生產版本：第21.4發行版本</p> <p><strong>在以下環境中可用：</strong> </p> <p>全新Adobe Workfront體驗 </p> </td> 
  </tr> 
 </tbody> 
</table>

### 敏捷增強功能 {#agile-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>功能</strong> </p> </td> 
   <td> <p><strong>發行日期與環境</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-agile-enhancements.md#user" class="MCXref xref" xrefformat="{para}">Kanban和Scrum展示板上的使用者指派</a> </p> <p>我們已更新Kanban和Scrum面板上的劇本卡片，以便更輕鬆地將使用者指派給劇本。 現在當您展開本文卡片時，可以按一下團隊或使用者頭像來新增指派。 之前，您必須找到並按一下個別的加號圖示。</p> </td> 
   <td> <p>預覽版本： 2021年9月9日 <br></p> <p>生產版本：第21.4發行版本</p> <p><strong>在以下環境中可用：</strong> </p> <p>全新Adobe Workfront體驗 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-agile-enhancements.md#configur" class="MCXref xref" xrefformat="{para}">設定將工作專案新增到Scrum反複專案時如何套用日期</a> </p> <p>根據預設，當您將工作專案新增到反複專案時，會修改工作專案上的計劃開始日期和計畫完成日期，以符合反複專案的開始和日期。 現在您可以選擇保留團隊所有工作專案上的原始計劃開始日期和計畫完成日期。</p> <p>此選項僅適用於Scrum團隊，不適用於Kanban團隊。</p> </td> 
   <td><strong>在以下日期可用：</strong> <p>預覽版本： 2021年9月9日<br></p> <p>生產版本：第21.4發行版本</p> <p><strong>在以下環境中可用：</strong> </p> <p>全新Adobe Workfront體驗 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-agile-enhancements.md#changes" class="MCXref xref" xrefformat="{para}">專案上敏捷檢視的變更</a> </p> <p>在21.3版中，我們改良了敏捷卡片和故事板（請參閱<a href="../../../product-announcements/product-releases/21.3-release-activity/21-3-project-enhancements.md#agile" class="MCXref xref" xrefformat="{para}">敏捷卡片和故事板更新</a>）。 這些更新套用至疊代以及專案的敏捷檢視。</p> <p>在21.4版中，我們正在針對專案的敏捷檢視恢復這些增強功能。 未對敏捷反複專案進行任何變更。</p> <p>以下是關於專案的敏捷檢視正在還原的變更：</p> 
    <ul> 
     <li> <p>故事卡和板欄的寬度可調整。</p> </li> 
     <li> <p>欄沒有背景陰影。</p> </li> 
     <li> <p>卡片沒有識別碼標籤（父內文、子任務、內文、任務或問題）。</p> </li> 
     <li> <p>「父級劇本」欄已重新命名為「劇本」。</p> </li> 
    </ul> </td> 
   <td><strong>在以下日期可用：</strong> <p>預覽版本： 2021年9月16日<br></p> <p>生產版本：第21.4發行版本</p> <p><strong>在以下環境中可用：</strong> </p> <p>全新Adobe Workfront體驗 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-agile-enhancements.md#add" class="MCXref xref" xrefformat="{para}">從Kanban面板新增劇本和問題</a> </p> <p>您現在可以直接從Kanban面板建立新劇本或問題。 這可讓您更輕鬆地快速新增內文，而無需前往專案、報告或儀表板來建立任務。</p> </td> 
   <td><strong>在以下日期可用：</strong> <p>預覽版本： 2021年7月22日<br></p> <p>生產版本：第21.4發行版本</p> <p><strong>在以下環境中可用：</strong> </p> <p>全新Adobe Workfront體驗 </p> </td> 
  </tr> 
 </tbody> 
</table>

### 報告增強功能 {#reporting-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>功能</strong> </p> </td> 
   <td> <p><strong>發行日期與環境</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-reporting-enhancements.md#new" class="MCXref xref" xrefformat="{para}">更新清單和報告中[工作總攬]欄位的新外觀</a> </p> <p>為了與新Workfront體驗中其他區域的現代外觀相符，已變更更新清單和報告中「工作總攬」欄位的樣式。 重新設計包括新的工作角色圖示、進階指派的新「人員」圖示、新「限制存取」圖示等。</p> </td> 
   <td><strong>在以下日期可用：</strong> <p>Beta預覽版本： 2021年4月8日（21.2版本）<br></p> <p>生產版本： 2021年7月15日<span class="uitext" style="color: #dc143c;"> （最初於21.2版本發佈至生產環境）</span></p> <p><strong>在以下環境中可用：</strong> </p> <p>全新Adobe Workfront體驗 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-reporting-enhancements.md#new2" class="MCXref xref" xrefformat="{para}">更新清單和報告中預先輸入欄位的新外觀</a> </p> <p>為了與新Workfront體驗中其他區域的現代外觀相符，已變更更新清單和報告中預先輸入欄位的樣式。 這些變更包含各種增強功能。</p> </td> 
   <td><strong>在以下日期可用：</strong> <p>Beta預覽版本： 2021年4月8日（21.2版本）<br></p> <p>生產版本： 2021年7月15日<span class="uitext" style="color: #dc143c;"> （最初於21.2版本發佈至生產環境）</span></p> <p><strong>在以下環境中可用：</strong> </p> <p>全新Adobe Workfront體驗 </p> </td> 
  </tr> 
 </tbody> 
</table>

### 要求增強功能 {#requests-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>功能</strong> </p> </td> 
   <td> <p><strong>發行日期與環境</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-requests-enhancements.md#improved" class="MCXref xref" xrefformat="{para}">已改善的請求搜尋現在包含特殊字元</a> </p> <p>為了讓提交請求時更快更輕鬆地尋找請求佇列，我們已改善搜尋演演算法，現在可尋找可能包含任何特殊字元的佇列。</p> <p>例如，您可以在請求型別欄位中輸入「*Workfront」或「Workfront」，尋找名為「*Workfront」的請求佇列。</p> <p>支援所有特殊字元。</p> </td> 
   <td><strong>在以下日期可用：</strong> <p>預覽版本： 2021年9月9日<br></p> <p>生產版本：第21.4發行版本</p> <p><strong>在以下環境中可用：</strong> </p> <p>全新Adobe Workfront體驗 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-requests-enhancements.md#new" class="MCXref xref" xrefformat="{para}">新Workfront體驗中內嵌請求佇列的新外觀</a> </p> <p>為了讓提交請求的外觀與感覺在新的Workfront體驗中保持相同，我們重新設計了介面，以將請求新增至內嵌請求佇列。 在此增強功能之前，從控制面板新增請求的介面與Workfront Classic環境相符。</p> </td> 
   <td><strong>在以下日期可用：</strong> <p>預覽版本： 2021年8月26日<br></p> <p>生產版本：第21.4發行版本</p> <p><strong>在以下環境中可用：</strong> </p> <p>全新Adobe Workfront體驗 </p> </td> 
  </tr> 
 </tbody> 
</table>

### 校訂增強功能 {#proofing-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>功能</strong> </p> </td> 
   <td> <p><strong>發行日期與環境</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-proofing-enhancements.md#improved" class="MCXref xref" xrefformat="{para}">已改善檢閱者和要求者的校訂功能</a> </p> <p>為了在Workfront和Proof之間提供更整合的體驗，我們針對檢閱者和請求者的校訂功能做了幾項改進：</p> 
    <ul> 
     <li> <p>您可以在Workfront中將「版主」或「作者」角色授與任何使用者，不論他們是否具備「校訂」授權，授予他們額外的許可權，例如套用動作或解決評論。</p> </li> 
     <li> <p>您可以將檢閱者和請求者新增至需要登入或需要以電子方式簽署的校訂。</p> </li> 
     <li> <p>所有使用者都能從Workfront和Proof之間更佳的連線能力中獲益。 現在，停用使用者或更新使用者的電子郵件地址時，在Workfront中變更時校訂中會正確反映您的更新。</p> </li> 
    </ul> </td> 
   <td><strong>在以下日期可用：</strong> <p>預覽版本： 2021年8月5日 <br></p> <p>生產版本： 21.4版本<span class="uitext" style="color: #dc143c;">（於2021年10月20日從預覽和生產中移除）。 最初僅向完全整合的EMEA客戶發行。 稍後會將此功能重新介紹給所有客戶。)</span></p> <p><strong>在以下環境中可用：</strong> </p> <p>全新Adobe Workfront體驗 </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
 </tbody> 
</table>

### 整合增強功能 {#integration-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>功能</strong> </p> </td> 
   <td> <p><strong>發行日期與環境</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-integration-enhancements.md#link" class="MCXref xref" xrefformat="{para}">從Dropbox Business連結檔案</a> </p> <p>我們已將Dropbox商務新增為可用的檔案整合。 現在，您可以直接從Workfront內部存取儲存在Dropbox Business中的檔案。</p> <p>Dropbox Business可讓您連結共用檔案，並將檔案上傳至共用資料夾。 Dropbox (非Dropbox Business)僅允許檔案擁有者在Workfront中檢視檔案。</p> <p>您的Workfront管理員可為貴組織啟用此整合。</p> </td> 
   <td> <p><b>在以下日期可用：</b> </p> <p>預覽版本：不適用<br></p> <p>生產版本：第21.4發行版本</p> <p><strong>在以下環境中可用：</strong> </p> <p>全新Adobe Workfront體驗 </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-integration-enhancements.md#updates" class="MCXref xref" xrefformat="{para}">Slack的Workfront更新</a> </p> <p>用於Slack整合的Workfront現在會顯示下列更新：</p> <p>適用於Slack的Workfront整合現在提供全新的外觀。 此外，您現在會即時收到Slack的Workfront通知。 </p> <p>例如，如果您被指派給任務，您會在被指派後立即收到該通知。 </p> <p>之前，通知出現在Slack中可能會有延遲。</p> </td> 
   <td><strong>在以下日期可用：</strong> <p>預覽版本： 2021年7月29日<br></p> <p>生產版本： 2021年7月29日</p> <p><strong>在以下環境中可用：</strong> </p> <p>全新Adobe Workfront體驗 </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-integration-enhancements.md#more" class="MCXref xref" xrefformat="{para}">在同意Adobe Workfront整合時，可更清楚檢視帳戶存取的詳細資料</a> </p> <p>Adobe Workfront整合的同意畫面現已更新。 現在，您可以檢視整合功能可存取的特定動作和區域，以便更清楚瞭解您允許整合或應用程式存取的內容。</p> <p>這個新的同意畫面適用於使用OAuth 2.0的任何Adobe Workfront整合。 </p> </td> 
   <td><strong>在以下日期可用：</strong> <p>預覽版本： 2021年7月29日<br></p> <p>生產版本： 2021年7月29日</p> <p><strong>在以下環境中可用：</strong> </p> <p>全新Adobe Workfront體驗 </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-integration-enhancements.md#api" class="MCXref xref" xrefformat="{para}">整合不再需要API金鑰驗證</a> </p> <p>Workfront整合最近開始使用OAuth2來提高安全性和可用性。 在此移動中，Workfront不再需要API金鑰以進行整合驗證。</p> </td> 
   <td><strong>在以下日期可用：</strong> <p>預覽版本： 2021年8月5日<br></p> <p>生產版本： 2021年8月5日</p> <p><strong>在以下環境中可用：</strong> </p> <p>全新Adobe Workfront體驗 </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
 </tbody> 
</table>

### 行動裝置增強功能 {#mobile-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>功能</strong> </p> </td> 
   <td> <p><strong>發行日期與環境</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-mobile-enhancements.md#review" class="MCXref xref" xrefformat="{para}">在行動應用程式中檢閱及核准校樣</a> </p> <p>Adobe Workfront行動應用程式現在會在我的工作中的核准清單中，顯示指派給您的所有校訂核准。 您可以直接在應用程式中檢閱校訂檔案，並做出決定。</p> </td> 
   <td><strong>在以下日期可用：</strong> <p>預覽版本：不適用<br></p> <p>生產版本： 2021年10月11日當週</p> <p><strong>在以下環境中可用：</strong> </p> 
    <ul> 
     <li> <p>iOS應用程式商店</p> </li> 
     <li> <p>Android應用程式商店</p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-mobile-enhancements.md#create" class="MCXref xref" xrefformat="{para}">從行動應用程式首頁區域建立新要求</a> </p> <p>您現在可以從Adobe Workfront行動應用程式的首頁區域建立新請求。 點選浮動導覽列中的「新增」按鈕，會顯示「請求」和「任務」的選項。 之前，您必須導覽至「請求」頁面才能建立請求。</p> </td> 
   <td><strong>在以下日期可用：</strong> <p>預覽版本：不適用<br></p> <p>生產版本： 2021年8月4日</p> <p><strong>在以下環境中可用：</strong> </p> 
    <ul> 
     <li> <p>iOS應用程式商店</p> </li> 
     <li> <p>Android應用程式商店</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 其他增強功能 {#other-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>功能</strong> </p> </td> 
   <td> <p><strong>發行日期與環境</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-other-enhancements.md#new" class="MCXref xref" xrefformat="{para}">新的鍵盤快速鍵可在清單中縮排及凸排</a> </p> <p>為了為所有系統使用者提供無障礙的體驗，並遵循標準的鍵盤導覽原則，縮排/凸排鍵盤指令已改變。 </p> <p>針對Mac，按下Option + &gt;以縮排清單專案，並按下Option + &lt;以縮排。 </p> <p>若是Windows，請按Alt + &gt;以縮排清單專案，然後按Alt + &lt;以縮排。</p> <p>之前，在清單中縮排的鍵盤快速鍵是Tab，而縮排是Shift + Tab。 但是，使用Tab鍵來縮排和凸排表示無法透過介面中的所有作用中欄位使用Tab鍵。</p> <p>此變更僅適用於更新的清單，不適用於舊版清單。 </p> </td> 
   <td><strong>在以下日期可用：</strong> <p>預覽版本： 2021年8月12日<br></p> <p>生產版本：第21.4發行版本</p> <p><strong>在以下環境中可用：</strong> </p> 
    <ul> 
     <li> <p>全新Adobe Workfront體驗 </p> </li> 
     <li> <p>Adobe Workfront Classic </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Workfront Fusion增強功能

Workfront Fusion中的新功能可在21.4發行排程之外的步調中用於生產環境。 如需最新功能的詳細資訊，請參閱[Adobe Workfront Fusion發行活動](https://experienceleague.adobe.com/zh-hant/docs/workfront-fusion/using/fusion-release-activity/fusion-release-activity)。

## Workfront Scenario Planner增強功能

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">There are no Scenario Planner updates at this point in the release. This area will be updated when updates are available.</p>
-->

Workfront Scenario Planner第21.4發行版本將推出新功能。 如需這些現在可在「預覽」中取得的新功能的相關資訊，請參閱[Adobe Workfront情境規劃工具發行活動](../../../product-announcements/product-releases/scenario-planner-release-activity/sp-release-activity.md)。

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Workfront Proof enhancements</h2>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">New features in Workfront Proof are now available. For more information, see <a href="../../../product-announcements/product-releases/workfront-proof-release-activity/wp-release-may-17.md" class="MCXref xref" xrefformat="{para}">Workfront Proof release activity:&nbsp;Week of May 17, 2021</a>.</p>
-->

## Workfront目標增強功能

此版本中目前沒有Workfront目標更新。 在有更新可用時，此區域將會更新。

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Most new features coming to Workfront Goals release with the 21.2 release. For information about these new features now available in Preview, see <a href="../../../product-announcements/product-releases/goals-release-activity/goals-21.2-release/goals-release-21-2.md" class="MCXref xref" xrefformat="{para}" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Adobe Workfront Goals with the 21.2 release</a>.</p>
-->

## API 14版

針對API版本14，我們已修改一些資源和端點。 有些變更支援新功能，有些則讓您更輕鬆地透過API使用可用資訊。

如需新增和更新的詳細資訊，請參閱[ API 14](../../../wf-api/api/new-api-version-14.md)版的新增功能。

如需API版本的資訊，請參閱[API版本設定與支援排程](../../../wf-api/api/api-version-support-schedule.md)。

## 21.4版本網路研討會

Workfront 21.4版本網路研討會已於2021年9月23日推出。 您可以從Workfront One[&#128279;](https://one.workfront.com/s/event)上的活動頁面檢視網路研討會影片。

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Functionality being removed from Production</h2>
<h3>Feature rollback: Carry over the existing proof workflow when generating a new version</h3>
<p>Due to customer feedback, <b>Workfront is removing this change from Preview environments on March 30, 2021 and from Production environments on March 31, 2021</b>.</p>
<p>On March 11, 2021, Workfront released a change to existing proof workflows in both Workfront Classic and the new Workfront experience. The change allowed for an existing workflow to carry over to any new proof versions created by a user, regardless of the method used to generate them.</p>
<p>In the new Workfront experience after this change is removed, proofs created with the Simple proof selection will not include any preset proofing settings, and new versions will not carry over existing workflows or proof settings. A user can adjust settings after proof generation.</p>
<p>In Workfront Classic after this change is removed, the option to Generate Proof will not include any preset proofing settings, and new versions will not carry over existing workflows or proof settings. A user can adjust settings after proof generation.</p>
<p>Similar functionality to easily copy existing workflows might be added to Production at a future time.</p>
</div>
-->

## 訓練更新

探索每個Adobe Workfront產品版本的學習計畫、學習路徑、影片和指南的最新更新。 如需詳細資訊，請參閱[訓練版本更新頁面](https://experienceleague.adobe.com/zh-hant/docs/workfront-learn/tutorials-workfront/home)。

## 不再支援的功能

### Internet Explorer 11

隨著移除對Internet Explorer的支援，Workfront現在正式支援Microsoft Edge。

如需支援瀏覽器的詳細資訊，請參閱[Adobe Workfront瀏覽器需求](../../../workfront-basics/workfront-browser-requirements.md)。
