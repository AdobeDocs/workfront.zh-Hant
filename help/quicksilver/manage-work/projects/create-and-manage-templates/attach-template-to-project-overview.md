---
content-type: overview
product-area: templates
keywords: 覆寫，欄位，已覆寫
navigation-topic: templates-navigation-topic
title: 將範本附加至專案的概觀
description: 將範本附加到現有專案時，您會根據範本修改專案上的一些資訊。 專案上的一些資訊維持不變。
author: Alina
feature: Work Management
exl-id: 7f0137b6-ce8e-4b66-ad55-e6dc2aae09d9
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1258'
ht-degree: 5%

---

# 將範本附加至專案的概觀

將範本附加到現有專案時，您會根據範本修改專案上的一些資訊。 專案上的一些資訊維持不變。

如需如何將範本附加到專案的詳細資訊，請參閱[將範本附加到專案](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md)。

## 將範本新增至專案時的注意事項

將範本新增至專案時，請考量下列事項：

* 您只能將作用中的範本附加至專案。
* 當專案處於「完成」、「廢棄」或「未決核准」狀態時，只有當Adobe Workfront管理員或群組管理員在「專案偏好設定」區域中啟用此功能時，您才能將範本附加到專案。 如需有關設定專案偏好設定的資訊，請參閱[設定全系統的專案偏好設定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)。
* 除非您將特定範本任務排除在附件流程中新增外，否則所有範本任務都會新增到現有專案。
* 大部分的範本設定都會新增至專案。 某些專案設定會保留。 如需詳細資訊，請參閱本文[瞭解附加範本](#understand-changes-to-project-fields-when-attaching-a-template)時專案欄位的變更。

## 瞭解附加範本時專案欄位的變更 {#understand-changes-to-project-fields-when-attaching-a-template}

>[!IMPORTANT]
>
>將範本附加到專案與從範本建立專案不同。 從範本建立專案時，所有範本欄位都會轉移到新專案。 附加範本後，部分現有專案欄位保持不變。

有些範本設定會自動轉移至專案，除非您明確將其標示為在範本附加程式期間被排除。 當您將其標籤為要排除時，會保留專案欄位值。

不過，在將範本附加到專案的過程中，並非所有專案欄位都可以管理。 如需詳細資訊，請參閱[將範本附加至專案](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md)。

下表說明附加範本時專案欄位的預設，以及在附加程式期間可以管理哪些欄位以覆寫預設行為：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>欄位</td> 
   <td>依預設，附加範本的程式中會發生什麼事</td> 
   <td>能夠管理附件流程中的欄位更新 </td> 
  </tr> 
  <tr> 
   <td>說明</td> 
   <td>專案資訊會保留</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>狀態</p> </td> 
   <td>專案資訊會保留</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>URL</td> 
   <td>已從範本傳輸，如果專案上的欄位為空</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>優先順序</td> 
   <td>專案資訊會保留</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>條件型別</td> 
   <td>專案資訊會保留</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>排程模式</td> 
   <td>專案資訊會保留</td> 
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
   <td>專案資訊會保留</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>方案</td> 
   <td>專案資訊會保留</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>群組</td> 
   <td>專案資訊會保留</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>公司</td> 
   <td>已從範本傳輸，如果專案上的欄位為空</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>規劃時數</td> 
   <td>可能會根據新增的任務而變更</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>專案所有者</td> 
   <td>已從範本傳輸，如果專案上的欄位為空</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>專案贊助者</td> 
   <td>已從範本傳輸，如果專案上的欄位為空</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>資源管理員</td> 
   <td>已新增至專案中現有的資源管理員清單</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>自訂Forms</td> 
   <td>除了已新增至專案中的表單外，還新增至專案</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>預算</td> 
   <td>專案資訊會保留</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>貨幣</td> 
   <td>專案資訊會保留</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>績效指數方法</td> 
   <td>專案資訊會保留</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>EAC</td> 
   <td>專案資訊會保留</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>規劃收益</td> 
   <td>專案資訊會保留</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>實際收益</td> 
   <td>專案資訊會保留</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>里程碑路徑</td> 
   <td>已從範本傳輸，如果專案上的欄位為空</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>完成模式</td> 
   <td>專案資訊會保留</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>摘要完成模式</td> 
   <td>專案資訊會保留</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>更新類型</td> 
   <td>專案資訊會保留</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>排程</td> 
   <td>專案資訊會保留</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>使用者休假</td> 
   <td>專案資訊會保留</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>資源平準模式</td> 
   <td>專案資訊會保留</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>風險（專案欄位）</td> 
   <td>專案資訊會保留</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>資源集區</td> 
   <td>已新增至專案上現有資源集區的清單</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>小時類型</td> 
   <td> <p>如果在附件程式期間取消選取，專案上的「時數型別」設定將保持不變。 </p> <p>如果選取，範本設定會轉移至專案。 如果專案和範本上的「時數型別」篩選都設為「是」，則範本中的時數型別會新增至專案中的時數型別。</p> </td> 
   <td> <p> </p> <p> </p> <p> </p> <p>✓ (A)</p> </td> 
  </tr> 
  <tr> 
   <td>提醒通知</td> 
   <td> <p>已新增至專案現有提醒的清單。 </p> <p>如果在附件程式期間取消選取，專案提醒通知將維持不變。 </p> </td> 
   <td>✓ (A)</td> 
  </tr> 
  <tr> 
   <td>任務預設核准流程</td> 
   <td>專案資訊會保留</td> 
   <td>✓ (A)</td> 
  </tr> 
  <tr> 
   <td>任務預設自訂Forms</td> 
   <td>專案資訊會保留</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>工作量</td> 
   <td>專案資訊會保留</td> 
   <td> </td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td><span>允許使用者新增內嵌問題</span> </td> 
   <td><span>專案資訊已保留</span> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>所有設定</td> 
   <td>範本設定會覆寫專案的範本設定</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>任務</td> 
   <td>在現有專案任務之外，新增到任務清單底部</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>文件</td> 
   <td>除了現有專案檔案外，已新增至專案</td> 
   <td>✓ (A)</td> 
  </tr> 
  <tr> 
   <td>風險（專案風險區域中的物件）</td> 
   <td>除了現有的專案風險外，已新增至專案 </td> 
   <td>✓ (A)</td> 
  </tr> 
  <tr> 
   <td>核准流程</td> 
   <td>已從範本轉移</td> 
   <td>✓ (A)</td> 
  </tr> 
  <tr> 
   <td>收費率</td> 
   <td> <p>除了專案上現有的收費率之外，已從範本傳輸。 </p> <p>如果專案和範本上相同職務角色有不同的費率，專案上的費率會保持不變。 </p> </td> 
   <td> <p> </p> <p>✓ (A)</p> </td> 
  </tr> 
  <tr> 
   <td>付費記錄</td> 
   <td>專案資訊會保留</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>費用</td> 
   <td>除了專案上的現有費用外，已從範本轉移</td> 
   <td>✓ (A)</td> 
  </tr> 
  <tr> 
   <td>財務資訊</td> 
   <td> <p>在附件程式中選取此專案時，會將下列欄位轉移或新增至專案： </p> 
    <ul> 
     <li> <p>固定成本</p> <p>選取此選項時，會使用下列公式計算更新的專案固定成本：</p> <p><code>Updated Project Fixed Cost = Original Project Fixed Cost + Template Fixed Cost</code> </p> </li> 
     <li> <p>固定收入</p> <p>選取此選項時，會使用下列公式計算更新的專案固定收入：</p> <p><code>Updated Project Fixed Revenue = Original Project Fixed Revenue + Template Fixed Revenue </code> </p> </li> 
     <li> <p>任務的成本型別</p> <p>已從範本轉移</p> </li> 
     <li> <p>任務的收入型別</p> <p>已從範本轉移</p> </li> 
    </ul> <p>如果在附件處理期間取消選取此欄位，將會發生下列情況：</p> 
    <ul> 
     <li> <p>專案上的固定成本和固定收入會保留。</p> </li> 
     <li> <p>從範本新增之任務的「成本」與「收入型態」設定為「無成本」與「不可開立帳單」</p> </li> 
    </ul> </td> 
   <td> <p> </p> <p> </p> <p> </p> <p> </p> <p> </p> <p> </p> <p>✓ (A)</p> </td> 
  </tr> 
  <tr> 
   <td>時數</td> 
   <td>專案資訊會保留</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>佇列詳細資訊、主題群組、佇列主題、路由規則</td> 
   <td> <p>已從範本轉移</p> <p>如果您在附件程式期間選取<strong>佇列屬性和問題設定</strong>選項，範本的佇列詳細資料會覆寫專案的佇列詳細資訊。 在這種情況下，範本的路由規則、佇列主題和主題群組會新增至專案的路由規則、佇列主題和主題群組。 <br>如果專案設定為請求佇列，而您附加至專案的範本未設定為請求佇列，則若您保留<strong>佇列屬性和問題設定</strong>核取方塊，則會移除專案的佇列資訊。 <br>如果您取消選取<strong>佇列屬性和問題設定</strong>方塊，則會保留專案的所有佇列設定設定，且不會附加範本中的佇列設定設定。</p> </td> 
   <td> <p> </p> <p> </p> <p> </p> <p> </p> <p> </p> <p> </p> <p> </p> <p>✓ (A)</p> </td> 
  </tr> 
  <tr> 
   <td>任務限制</td> 
   <td> <p>已從範本轉移 </p> <p>如果在附件處理期間取消選取，則視專案「排程起始日期」設定而定，作業限制會設定為「儘可能早」或「儘可能晚」。 </p> </td> 
   <td> <p> </p> <p> </p> <p style="text-align: center;">✓ (A)</p> </td> 
  </tr> 
  <tr> 
   <td>前置任務</td> 
   <td> <p>已從範本轉移</p> <p>如果在附件程式期間取消選取，則會移除範本任務之間的所有前置任務連線。</p> </td> 
   <td>✓ (A)</td> 
  </tr> 
  <tr> 
   <td>共用選項</td> 
   <td> <p>如果在附加程式期間取消選取，專案許可權將維持不變。</p> <p>如果在附加程式期間選取範本許可權，範本許可權會新增至專案或覆寫專案的許可權。 </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>範例： </b></span></span>如果使用者A擁有專案的檢視許可權，但他們擁有範本的管理許可權，在附加範本後，使用者A將獲得專案的管理存取許可權。</p> </td> 
   <td>✓ (A)</td> 
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

 
