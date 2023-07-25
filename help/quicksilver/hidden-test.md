---
title: 隱藏的測試檔案
author: Bob
description: 在搜尋和左側導覽中隱藏
hidefromtoc: true
hide: true
exl-id: b6b0f429-b619-4b8e-ab81-ad190dae5a0b
source-git-commit: 5c47b09550c54b7ea4f8319bb42e93572e06324b
workflow-type: tm+mt
source-wordcount: '277'
ht-degree: 1%

---


# 隱藏測試檔案 — 功能分支測試

此檔案在搜尋中隱藏(`hide: yes`)並從左側導覽(`hidefromtoc: yes`)。

<span class="preview">此檔案為 **隱藏** 從搜尋(`hide: yes`)並從左側導覽(`hidefromtoc: yes`)。</span>

<p class="preview">此檔案在搜尋中**隱藏** ('hide： yes')和在左側導覽中('hidefromtoc： yes')。</p>

## 影像測試

![影像測試](assets/get-started.png){width="50" align="center"}

## 預覽醒目提示測試

**對元件區塊使用DIV。**

DIV會從下方開始。

<div class="preview">

DIV的開頭。

>[!NOTE]
>
>這是備註。
>
>我要求反白標示附註的背景。

![影像](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/assets/add-admin-1.png)

最後一個反白專案。

</div>

DIV結尾在上方。

**對段落或短語使用SPAN**

這是段落。 <span class="preview">我是黃色文字。</span> 請記得正確關閉您的語法，否則頁面可能會呈現異常。

DIV和SPAN在HTML表格中也很實用。

**其他支援的HTML元素**

您也可以指定 `class="preview"` 中的語法 `<p>`， `<td>`， `<tr>`、等等。 請務必在預覽時測試。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr class="preview"> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">Adobe Workfront計畫</a>*</td> 
   <td> <p>Pro或以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"></td> 
   <td> <p class="preview">計劃</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Jira存取</td> 
   <td> <p><span class="preview">系統管理員存取權</p> <p>重要：建議您在Jira和Workfront中建立個別的系統管理員帳戶，以專門用於此整合，而不使用可能附加至使用者的現有帳戶。 </span></p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>您必須是Workfront管理員。 如需Workfront管理員的相關資訊，請參閱。</p> <p>注意：如果您仍然沒有存取權，請詢問您的Workfront管理員是否對您的存取層級設定了其他限制。 如需有關Workfront管理員如何修改您的存取層級的資訊，請參閱 <a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

高品質視訊= 12

>[!VIDEO](https://video.tv.adobe.com/v/3413544/?quality=12)

視訊品質= 6

>[!VIDEO](https://video.tv.adobe.com/v/3413544/?quality=6)

HTML表格內的影片

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  </tr> 
  <tr> 
   <td role="rowheader">此影片是否有效？</td> 
   <td>不，它不會 </td> 
  </tr> 
 </tbody> 
</table>

Markdown表格內的影片

| 欄 1 | 欄 2 |
|---|---|
| 這個功能可以運作嗎？ | 也否 |


