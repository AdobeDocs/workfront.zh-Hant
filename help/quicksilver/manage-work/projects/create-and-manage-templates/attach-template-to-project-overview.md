---
content-type: overview
product-area: templates
keywords: 覆蓋，欄位，覆蓋
navigation-topic: templates-navigation-topic
title: 將範本附加至專案的概觀
description: 將模板附加到現有項目時，您將根據模板的模板修改有關項目的某些資訊。 項目的一些資訊保持不變。
author: Alina
feature: Work Management
exl-id: 7f0137b6-ce8e-4b66-ad55-e6dc2aae09d9
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1247'
ht-degree: 5%

---

# 將範本附加至專案的概觀

將模板附加到現有項目時，您將根據模板的模板修改有關項目的某些資訊。 項目的一些資訊保持不變。

如需如何將範本附加至專案的詳細資訊，請參閱 [將範本附加至專案](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

## 將範本新增至專案時的考量事項

將範本新增至專案時，請考量下列事項：

* 您只能將作用中的範本附加至專案。
* 當項目處於「完成」、「無效」或「待批准」狀態時，您只能在您的Adobe Workfront管理員或組管理員已在「項目首選項」區域中啟用此功能時，將模板附加到項目。 有關設定項目首選項的資訊，請參閱 [配置系統範圍的項目首選項](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).
* 除非您排除特定範本任務，否則不會在附件程式中新增，否則所有範本任務都會新增至現有專案。
* 大部分的範本設定都會新增至專案。 某些專案設定會保留。 如需詳細資訊，請參閱 [了解附加範本時對專案欄位的變更](#understand-changes-to-project-fields-when-attaching-a-template) 這篇文章。

## 了解附加範本時對專案欄位的變更 {#understand-changes-to-project-fields-when-attaching-a-template}

>[!IMPORTANT]
>
>將範本附加至專案，與從範本建立專案不同。 從範本建立專案時，所有範本欄位都會轉移至新專案。 附加範本會維持部分現有專案欄位不變。

某些範本設定會自動轉移至專案，除非您在範本附件處理期間特別將其標示為要排除。 將項目標籤為要排除時，將保留項目欄位值。

不過，並非所有專案欄位都可在將範本附加至專案的過程中加以管理。 如需詳細資訊，請參閱 [將範本附加至專案](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

下表說明附加範本時專案欄位的預設值，以及在附加程式期間可管理哪些欄位以覆寫預設行為：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>欄位</td> 
   <td>依預設，附加範本的程式會發生什麼事</td> 
   <td>管理附件流程中欄位更新的功能 </td> 
  </tr> 
  <tr> 
   <td>說明</td> 
   <td>保留專案資訊</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>狀態</p> </td> 
   <td>保留專案資訊</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>URL</td> 
   <td>從範本轉移，如果專案上的欄位空白</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>優先順序</td> 
   <td>保留專案資訊</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>條件類型</td> 
   <td>保留專案資訊</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>時程表模式</td> 
   <td>保留專案資訊</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>計畫日期</td> 
   <td>可能會根據新增的任務而變更</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>實際日期</td> 
   <td>可能會根據新增的任務而變更</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>專案組合</td> 
   <td>保留專案資訊</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>方案</td> 
   <td>保留專案資訊</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>群組</td> 
   <td>保留專案資訊</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>公司</td> 
   <td>從範本轉移，如果專案上的欄位空白</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>計畫小時</td> 
   <td>可能會根據新增的任務而變更</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>專案所有者</td> 
   <td>從範本轉移，如果專案上的欄位空白</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>專案贊助者</td> 
   <td>從範本轉移，如果專案上的欄位空白</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>資源管理員</td> 
   <td>已添加到項目上現有資源管理器清單中</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>自訂Forms</td> 
   <td>新增至專案，以及專案中已有的表單</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>預算</td> 
   <td>保留專案資訊</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>貨幣</td> 
   <td>保留專案資訊</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>績效指數方法</td> 
   <td>保留專案資訊</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>EAC</td> 
   <td>保留專案資訊</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>計畫收益</td> 
   <td>保留專案資訊</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>實際收益</td> 
   <td>保留專案資訊</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>里程碑路徑</td> 
   <td>從範本轉移，如果專案上的欄位空白</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>完成模式</td> 
   <td>保留專案資訊</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>摘要完成模式</td> 
   <td>保留專案資訊</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>更新類型</td> 
   <td>保留專案資訊</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>排程</td> 
   <td>保留專案資訊</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>用戶關閉時間</td> 
   <td>保留專案資訊</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>資源平準模式</td> 
   <td>保留專案資訊</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>風險（項目欄位）</td> 
   <td>保留專案資訊</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>資源集區</td> 
   <td>已添加到項目上現有資源池的清單中</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>小時類型</td> 
   <td> <p>如果在附件處理期間取消選中，則項目上的「小時類型」設定保持不變。 </p> <p>如果選取，範本設定會轉移至專案。 如果項目和模板上的「小時類型」(Hour Type)篩選均設定為「是」(Yes)，則模板中的小時類型將添加到項目上的小時類型。</p> </td> 
   <td> <p> </p> <p> </p> <p> </p> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td>提醒通知</td> 
   <td> <p>新增至專案上現有提醒的清單。 </p> <p>如果在附件處理期間取消選取，專案提醒通知將維持不變。 </p> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>任務預設核准流程</td> 
   <td>保留專案資訊</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>任務預設自定義Forms</td> 
   <td>保留專案資訊</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>工作量</td> 
   <td>保留專案資訊</td> 
   <td> </td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td><span>允許使用者內嵌新增問題</span> </td> 
   <td><span>保留專案資訊</span> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>所有設定</td> 
   <td>範本設定會覆寫專案的設定</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>任務</td> 
   <td>除了現有項目任務外，還添加到任務清單的底部</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>文件</td> 
   <td>新增至專案，以及現有專案檔案</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>風險（項目風險區域中的對象）</td> 
   <td>除了現有項目風險外，還添加到項目中 </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>核准流程</td> 
   <td>從模板轉移</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>收費率</td> 
   <td> <p>除了項目的現有開單費率外，還從模板中轉移。 </p> <p>如果項目和模板上同一職務角色的費率不同，則項目費率保持不變。 </p> </td> 
   <td> <p> </p> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td>付費記錄</td> 
   <td>保留專案資訊</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>費用</td> 
   <td>除項目現有費用外，從模板轉移</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>財務資訊</td> 
   <td> <p>在附件流程中選取此選項時，會將下列欄位轉移或新增至專案： </p> 
    <ul> 
     <li> <p>固定成本</p> <p>選擇該選項後，將使用以下公式計算項目的更新固定成本：</p> <p><code>Updated Project Fixed Cost = Original Project Fixed Cost + Template Fixed Cost</code> </p> </li> 
     <li> <p>固定收入</p> <p>選取選項後，專案的更新固定收入會使用下列公式計算：</p> <p><code>Updated Project Fixed Revenue = Original Project Fixed Revenue + Template Fixed Revenue </code> </p> </li> 
     <li> <p>任務成本類型</p> <p>從模板轉移</p> </li> 
     <li> <p>任務上的收入類型</p> <p>從模板轉移</p> </li> 
    </ul> <p>如果在附件過程中取消選擇此欄位，將發生以下情況：</p> 
    <ul> 
     <li> <p>項目上的固定成本和固定收入將保留。</p> </li> 
     <li> <p>從模板添加的任務的「成本」和「收入類型」設定為「無成本」和「不可開單」</p> </li> 
    </ul> </td> 
   <td> <p> </p> <p> </p> <p> </p> <p> </p> <p> </p> <p> </p> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td>時數</td> 
   <td>保留專案資訊</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>隊列詳細資訊、主題組、隊列主題、路由規則</td> 
   <td> <p>從模板轉移</p> <p>如果您選取 <strong>隊列屬性和問題設定</strong> 選項，則範本的「佇列詳細資料」會覆寫專案的「佇列詳細資料」。 在這種情況下，模板的「路由規則」、「隊列主題」和「主題組」將添加到項目的「路由規則」、「隊列主題」和「主題組」。 <br>如果將項目設定為請求隊列，而您附加到項目的模板未設定為請求隊列，則如果您離開 <strong>隊列屬性和問題設定</strong> 框。 <br>如果您取消選取 <strong>隊列屬性和問題設定</strong> 框中，將保留項目的所有「隊列設定」設定，並且不附加模板中的「隊列設定」設定。</p> </td> 
   <td> <p> </p> <p> </p> <p> </p> <p> </p> <p> </p> <p> </p> <p> </p> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td>任務約束</td> 
   <td> <p>從模板轉移 </p> <p>如果在附件處理過程中取消選擇，則根據項目計畫自設定，任務約束將設定為「盡快」或「盡可能晚」。 </p> </td> 
   <td> <p> </p> <p> </p> <p style="text-align: center;">✓</p> </td> 
  </tr> 
  <tr> 
   <td>前置任務</td> 
   <td> <p>從模板轉移</p> <p>如果在附件過程中取消選中，則模板任務之間的所有前置連接都將被刪除。</p> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>共用選項</td> 
   <td> <p>如果在附件處理期間取消選取，專案權限將維持不變。</p> <p>如果在附件處理期間選取，則會將範本權限新增至或覆寫專案的權限。 </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>範例： </b></span></span>如果使用者A擁有專案的「檢視」權限，但他們擁有範本的「管理」權限，則附加範本後，使用者A將獲得專案的「管理」存取權。</p> </td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

 

<!--WRITER
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<div>
<h2> </h2>
<h2>Understand changes to project fields when attaching a template</h2> 
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: drafted and replaced with the table above, per Anna)</p>
-->
<!--
<p>Some template settings automatically transfer to the project, unless you specifically mark them to be excluded during the template attachment process. When you mark them to be excluded, the project field values are preserved. </p> <note type="important">
Not all project fields are available to manage in the process of attaching a template to a project. For information, see
<a href="../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md" class="MCXref xref">Attach a template to a project</a>.
</note>
<p>The following scenarios exist when attaching a template to an existing project: </p>
<ul>
<li> <p><a href="#project-fields-that-are-empty-and-the-template-information-updates-them" class="MCXref xref">Project fields that are empty and the template information updates them</a> </p> </li>
<li> <p><a href="#project-fields-that-are-populated-and-the-template-information-overwrites-them" class="MCXref xref">Project fields that are populated and the template information overwrites them</a> </p> </li>
<li> <p><a href="#project-fields-that-are-populated-and-they-remain-unchanged-after-attaching-the-template" class="MCXref xref">Project fields that are populated and they remain unchanged after attaching the template</a> </p> </li>
</ul> <note type="important">
Attaching a template to a project is not the same as creating a project from a template. When you create a project from a template all template fields transfer to the new project. Attaching a template leaves some of the existing project's fields unchanged.
</note>
<p><strong>Project fields that are empty and the template information updates them</strong></p>
<p>Most project fields that are empty are populated with template information when attaching the template to an existing project. </p>
<p><strong>Project fields that are populated and the template information overwrites them</strong></p>
<p>The following fields always overwrite or update existing project information with template information when you attach a template to the project and they cannot be managed during attaching the template: </p>
<ul>
<li> <p><b>Resource manager</b>: The template Resource Managers are added to the list of existing resource managers on the project.</p> </li>
</ul>
<ul>
<li> <p><b>Financial Information</b>: You can indicate whether you want financial information to transfer from the template or to keep the existing financial information on the project in the process of attaching a template. However, when the Financial Information option is selected to indicate that you intend to keep the information from the template, the following fields are updated on the project: </p>
<ul>
<li> <p> The updated Fixed Cost of the project is calculated using the following formula:</p> <p><code>Updated Project Fixed Cost = Original Project Fixed Cost + Template Fixed Cost</code> </p> </li>
<li> <p>The updated Fixed Revenue of the project is calculated using the following formula:</p> <p><code>Updated Project Fixed Revenue = Original Project Fixed Revenue + Template Fixed Revenue </code> </p> </li>
</ul> </li>
</ul>
<ul>
<li> <p><b>Filter Hour Types</b> </p> </li>
</ul>
<ul>
<li> <p><b>Access settings</b> </p> </li>
</ul>
<ul>
<li> <p><b>Custom&nbsp;Forms</b>:&nbsp;Template custom forms are added to the project, in addition to existing project custom forms. If the fields from the template custom forms already exist on the project and contain information, they preserve the information already on the project. You cannot edit them during attaching the template. </p> </li>
</ul>
<ul>
<li> <p><b>Start&nbsp;From</b> </p> </li>
</ul>
<p><strong>Project fields that are populated and they remain unchanged after attaching the template</strong></p>
<p>The following fields remain unchanged on the project, even if they are also populated on the template, and they cannot be managed during attaching the template: </p>
<ul>
<li> <p style="font-weight: bold;">URL</p> </li>
<li> <p style="font-weight: bold;">Project Owner</p> </li>
<li> <p style="font-weight: bold;">Project&nbsp;Sponsor</p> </li>
<li> <p style="font-weight: bold;">Group</p> </li>
<li> <p style="font-weight: bold;">Company</p> </li>
<li> <p style="font-weight: bold;">Currency</p> </li>
<li> <p style="font-weight: bold;">Milestone Path</p> </li>
<li> <p><b>Completion Mode</b> </p> </li>
<li> <p style="font-weight: bold;">Resource Pool</p> </li>
<li> <p style="font-weight: bold;">Tasks Settings fields</p> </li>
<li class="preview" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p style="font-weight: bold;">Issue Settings fields</p> </li>
</ul>
</div>
<p>&nbsp;</p>
</div>
-->

 
