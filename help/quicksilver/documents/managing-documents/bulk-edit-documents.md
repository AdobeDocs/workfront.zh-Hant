---
content-type: reference
product-area: documents
navigation-topic: documents-navigation-topic
title: 大量編輯檔案
description: 您可以在「檔案」區域中一次編輯多個檔案。
author: Courtney
feature: Digital Content and Documents
recommendations: noDisplay, noCatalog
source-git-commit: 8c1f829eb29d8cd13524814d98ed353add15e881
workflow-type: tm+mt
source-wordcount: '572'
ht-degree: 0%

---


# 大量編輯檔案

<span class="preview">此頁面上的資訊是指尚未普遍提供的功能。 它只能在「預覽Sandbox」環境中使用。</span>

您可以一次編輯多個檔案中的說明、新增自訂表單及編輯自訂表單。

## 編輯自訂表單時的注意事項

大量編輯檔案自訂表單時，請考量下列事項：

* 您正在選取的所有檔案上變更的資訊會覆寫個別檔案的現有資訊。
* 當您為相同欄位選取具有不同值的檔案時，該欄位會顯示「多個值」指示器。 核取方塊、選項按鈕和切換的欄位旁邊會有一個「多個值」指示器。
* 當您在多選項欄位（例如顯示為一組切換或核取方塊的欄位）中更新一個選項時，所選檔案之間的所有其他選項必須相符。

>[!BEGINSHADEBOX]

**範例**
您可能會有包含核取方塊欄位的自訂表單，其中含有三個核取方塊（「選項1」、「選項2」和「選項3」），所有選取的檔案的「選項1」都會取消核取，而某些檔案的「選項2」和「選項3」則會取消核取，其他選取的檔案則會取消核取。 如果您要核取所有檔案的選項1，您還必須使選項2和3符合所有選取的專案，然後才能儲存變更。 因此，您必須選取或取消選取這些專案，以便它們在所有選取的專案上相符。 如果您未變更任何選項，您可以依原樣儲存欄位，檔案會保留其目前對所有選項的選取。

>[!ENDSHADEBOX]

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具備下列條件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p> 任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td><p> 新增：投稿人或更高版本</p> 
   <p> 目前：要求或以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>編輯檔案的存取權</p> <p>注意：如果您還是沒有存取權，請詢問您的Workfront管理員，他們是否在您的存取層級中設定其他限制。 如需Workfront管理員如何修改存取層級的詳細資訊，請參閱<a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理對檔案的存取</p> <p>如需請求其他存取權的資訊，請參閱<a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求物件</a>的存取權。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的Workfront管理員。

+++

## 大量編輯檔案

若要大量編輯檔案：

1. 從主功能表瀏覽至專案的「檔案」標籤或「檔案」區域。
1. 在鍵盤上按ctrl或cmd，然後選取要編輯的檔案。
1. 按一下「編輯」圖示![編輯圖示](assets/edit-icon.png)。
   ![編輯頁面](assets/edit-multiple-documents.png)上的圖示位置
1. （選用）新增或編輯&#x200B;**描述**。 如果每個檔案的描述不同，您會在描述方塊中看到&#x200B;_多個值_。 您可以為所有檔案新增相同的說明，但當您大量編輯時，無法編輯個別檔案說明。
1. 使用自訂表單進行下列變更：

   <table>
    <tr>
    <td><strong>新增表單</strong></td>
    <td>在<strong>新增自訂表單方塊</strong>中，您可以從附加的表單中選擇要新增的表單。 附加的表單位於部分選定檔案上，但不是全部檔案。 附加到所有選定檔案的表單會自動顯示在編輯視窗中。  </td>
    </tr>
    <tr>
    <td><strong>編輯表單</strong></td>
    <td>編輯任何附加的自訂表單。 您變更的資訊會覆寫個別檔案的現有資訊。 跨檔案具有不同值的欄位會顯示為「多個值」。 </td>
    </tr>
    <tr>
    <td><strong>重新排清單單</strong></td>
    <td>按一下並拖曳自訂表單以重新排列。</td>
    </tr>
    </table>
1. 按一下「**儲存**」。


