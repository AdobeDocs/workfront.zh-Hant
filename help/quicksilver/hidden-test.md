---
title: 隱藏的測試檔案
author: Bob
description: 在搜尋和左側導覽中隱藏
hidefromtoc: true
hide: true
exl-id: b6b0f429-b619-4b8e-ab81-ad190dae5a0b
source-git-commit: 1655726151338c47d8f81201db9ef0bb92d9ce9a
workflow-type: tm+mt
source-wordcount: '277'
ht-degree: 1%

---


# 隱藏測試檔案 — 功能分支測試

此檔案在搜索中隱藏(`hide: yes`)和左側導覽列(`hidefromtoc: yes`)。

<span class="preview">此檔案為 **隱藏** 從搜索(`hide: yes`)和左側導覽列(`hidefromtoc: yes`)。</span>

<p class="preview">此檔案在搜**中隱藏**(「隱藏：是」)和左側導覽列(「hidefromtoc:是')。</p>

## 影像測試

![影像測試](assets/get-started.png){width="50" align="center"}

## 預覽醒目提示測試

**對元件區塊使用DIV。**

DIV從下面開始。

<div class="preview">

開始DIV。

>[!NOTE]
>
>這是張紙條。
>
>我要求突顯筆記的背景。

![影像](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/assets/add-admin-1.png)

最後一個突出顯示的項目。

</div>

DIV結尾於上方。

**對段落或短語使用SPAN**

這是段落。 <span class="preview">我是黃色的。</span> 請記得正確關閉語法，否則頁面可能會呈現出奇怪的效果。

DIV和SPAN在HTML表中也很有用。

**其他支援的HTML元素**

您也可以指定 `class="preview"` 語法 `<p>`, `<td>`, `<tr>`等。 請務必在預覽時測試。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr class="preview"> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">Adobe Workfront計畫</a>*</td> 
   <td> <p>Pro或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"></td> 
   <td> <p class="preview">計劃</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">吉拉訪問</td> 
   <td> <p><span class="preview">系統管理員存取</p> <p>重要：建議您在Jira和Workfront中建立個別的系統管理員帳戶，以專門用於此整合，而不是使用可能附加至使用者的現有帳戶。 </span></p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>您必須是Workfront管理員。 如需Workfront管理員的相關資訊，請參閱。</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

畫質的視訊= 12

>[!VIDEO](https://video.tv.adobe.com/v/3413544/?quality=12)

品質為6的視訊

>[!VIDEO](https://video.tv.adobe.com/v/3413544/?quality=6)

HTML表內的視訊

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  </tr> 
  <tr> 
   <td role="rowheader">這段錄像有用嗎？</td> 
   <td>不，不 </td> 
  </tr> 
 </tbody> 
</table>

Markdown表格內的影片

| 欄 1 | 欄 2 |
|---|---|
| 這有用嗎？ | 也否 |
