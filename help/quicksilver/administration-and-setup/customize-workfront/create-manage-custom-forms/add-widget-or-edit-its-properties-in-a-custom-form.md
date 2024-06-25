---
title: 使用舊版表單產生器，在自訂表單中新增或編輯影像或其他資產Widget
description: 您可以新增或編輯以下任何資產Widget的屬性，例如自訂表單中的影像、影片、PDF檔案和Adobe XD檔案。 若您需要納入品牌化影像、教學影片，或您設計之應用程式的互動式原型等視覺內容，這個選項相當實用。
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 62a2f9a1-80de-40e7-9d8b-46ed9df083c1
source-git-commit: d32f274390f6ffc5fdd01c2c9b4b2abd99d7cb10
workflow-type: tm+mt
source-wordcount: '1345'
ht-degree: 1%

---

# 使用舊版表單產生器，在自訂表單中新增或編輯影像或其他資產Widget

{{form-designer-default}}

您可以在自訂表單中新增或編輯以下任何資產Widget的屬性：

* 影像
* 影片
* PDF檔案
* Adobe XD檔案

若您需要納入品牌化影像、教學影片，或您設計之應用程式的互動式原型等視覺內容，這個選項相當實用。

將包含Widget的自訂表單附加到物件時，使用物件的使用者可在下列區域看到它：

* 物件的「詳細資訊」區域（例如，專案的「詳細資訊」區域）
* 物件的「編輯」方塊(如果它具有新的Adobe Workfront體驗外觀) （例如「編輯專案」和「編輯任務」方塊）

目前，使用者無法在下列區域看到Widget&#x200B;：

* 清單與報告
* 首頁和摘要
* 物件的「編輯」方塊(如果它沒有新的Adobe Workfront體驗外觀) （例如「編輯費用」方塊）
* Workfront行動應用程式


## 存取需求

您必須具備下列專案才能執行本文所述的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront計畫*</p> </td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td>計劃</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>管理自訂表單的存取權</p> <p>如需Workfront管理員如何授予此存取許可權的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">授予使用者管理特定區域的存取權</a>.</p> </td> 
  </tr>  
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取層級設定，請聯絡Workfront管理員。

## 在自訂表單中新增或編輯資產Widget

1. 開始使用自訂表單，如所述 [建立或編輯自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).
1. 使用 **新增欄位** 標籤開啟，執行下列任一項作業：

   * 如果您要新增一個Widget，請選取 **影像**， **PDF**，或 **視訊** 將其新增至表單底部，或將其拖曳至表單上您想要的位置。

     ![](assets/add-widget.png)


   * 如果您想要新增已新增至其他自訂表單的Widget，請按一下 **欄位程式庫**，然後按一下顯示清單中Widget的名稱。 如需詳細資訊，請參閱 [在自訂表單中重複使用自訂欄位或Widget](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md).

   * 如果您正在編輯已新增至自訂表單的Widget，請選取它。

1. 為Widget輸入或編輯下列任一屬性：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">標籤</td> 
      <td> <p>（必要）輸入要顯示在Widget上方的描述性標籤。 您可以隨時變更標籤。</p> <p><b>重要</b>：請避免在此標籤中使用特殊字元。 它們在報表中無法正確顯示。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">姓名</td> 
      <td> <p>（必要）此名稱是系統識別Widget的方式。</p> <p>當您第一次設定Widget且輸入標籤時，「名稱」欄位會自動填入以和相符。 但是「標籤」和「名稱」欄位不同步，這可讓您自由地變更使用者看到的標籤，而不必變更系統看到的名稱。</p> <p><b>重要</b>：雖然可以這樣做，但建議您不要在您或其他使用者開始在Widget中使用自訂表單後變更此名稱。 如果這樣做，系統將無法再辨識Widget，而此時它可能會在Workfront的其他區域中被參照。 </p> <p>每個Widget名稱在貴組織的Workfront例項中必須是唯一的。 如此一來，您便可重複使用已針對其他自訂表單建立的表單。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">URL</td> 
      <td> <p>（必要）輸入或貼上儲存於網際網路之Widget的URL。</p> 
       <p><strong>重要</strong>：的URL必須是公用URL。 </p>
      <p>如果您新增視訊Widget，目前可在URL方塊中新增下列內容來完成此操作：</p> 
      <ul> 
      <li> <p>YouTube或Vimeo連結</p> </li> 
      <li> <p>Google Drive影片連結</p> </li> 
      <li> <p>使用MP4和MOV擴充功能的視訊連結</p> </li> 
      <li> <p>視訊連結已上傳至Workfront執行個體中的檔案區域。 如需指示，請參閱 <a href="#add-a-video-widget-to-a-custom-form-from-the-documents-area" class="MCXref xref">從檔案區域新增視訊Widget至自訂表單</a> 本文章內容。</p> 
      </li> 
      </ul> 
       </td> 
     </tr> 
     <tr> 
      <td role="rowheader">指示</td> 
      <td> <p>輸入有關Widget的任何其他資訊。 當使用者填寫自訂表單時，可以將滑鼠指標暫留在問號圖示上，以檢視包含您在此處輸入資訊的工具提示。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">大小</td> 
      <td>視需要變更Widget的顯示大小。</td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下 **套用**.
1. 如果您想以其他方式繼續建置自訂表單，請繼續閱讀下列其中一篇文章：

   * [在自訂表單中定位自訂欄位和Widget](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [新增自訂欄位至自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md)
   * [在自訂表單中重複使用自訂欄位或Widget](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md)
   * [新增計算資料至自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)
   * [在自訂表單中重複使用現有的計算自訂欄位](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md)
   * [新增顯示邏輯和略過邏輯至自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)
   * [預覽並完成自訂表格](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/preview-and-complete-a-custom-form.md)


## 將XD檔案新增至自訂表單

1. 開始使用自訂表單，如所述 [建立或編輯自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).
1. 使用 **新增欄位** 標籤開啟，選取 **Adobe XD**.
1. 為Widget輸入或編輯下列任一屬性：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">標籤</td> 
      <td> <p>（必要）輸入要顯示在Widget上方的描述性標籤。 您可以隨時變更標籤。</p> <p><b>重要</b>：請避免在此標籤中使用特殊字元。 它們在報表中無法正確顯示。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">姓名</td> 
      <td> <p>（必要）此名稱是系統識別Widget的方式。</p> <p>當您第一次設定Widget且輸入標籤時，「名稱」欄位會自動填入以和相符。 但是「標籤」和「名稱」欄位不同步，這可讓您自由地變更使用者看到的標籤，而不必變更系統看到的名稱。</p> <p><b>重要</b>：雖然可以這樣做，但建議您不要在您或其他使用者開始在Widget中使用自訂表單後變更此名稱。 如果這樣做，系統將無法再辨識Widget，而此時它可能會在Workfront的其他區域中被參照。 </p> <p>每個Widget名稱在貴組織的Workfront例項中必須是唯一的。 如此一來，您便可重複使用已針對其他自訂表單建立的表單。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">URL</td> 
      <td> <p>（必要）輸入或貼上有效的XD原型連結。</p> 
      <p>注意：在Adobe XD中，共用標籤上的連結存取設定必須設定為具有連結的任何人。 否則，使用者將無法檢視原型。 
   </td> 
     </tr> 
     <tr> 
      <td role="rowheader">指示</td> 
      <td> <p>（選用）輸入有關Widget的任何其他資訊。 當使用者填寫自訂表單時，可以將滑鼠指標暫留在問號圖示上，以檢視包含您在此處輸入資訊的工具提示。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">大小</td> 
      <td>（選用）視需要變更Widget的顯示大小。</td> 
     </tr> 
    </tbody> 
   </table>

1. 如果您想以其他方式繼續建置自訂表單，請繼續閱讀下列其中一篇文章：

   * [在自訂表單中定位自訂欄位和Widget](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [新增自訂欄位至自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md)
   * [在自訂表單中重複使用自訂欄位或Widget](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md)
   * [新增計算資料至自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)
   * [在自訂表單中重複使用現有的計算自訂欄位](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md)
   * [新增顯示邏輯和略過邏輯至自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)
   * [預覽並完成自訂表格](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/preview-and-complete-a-custom-form.md)

## 從檔案區域新增視訊Widget至自訂表單 {#add-a-video-widget-to-a-custom-form-from-the-documents-area}

>[!IMPORTANT]
>
>以這種方式將視訊新增至自訂表單時，當使用者存取物件上的表單時，只有針對自訂表單設定的許可權會套用至視訊，而不是檔案區域中為視訊設定的許可權。

1. 前往檔案區域中的影片，並為其產生校樣，如中所述 [為網站或其他網頁內容建立互動式校樣](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-interactive-proof-for-website-or-other-web-content.md).
1. 開啟校訂。
1. 以滑鼠右鍵按一下視訊上的任何位置，然後選取「 」 **複製視訊位址**.
1. 在您新增視訊Widget的自訂表單中，將複製的地址貼到 **URL** 方塊。
