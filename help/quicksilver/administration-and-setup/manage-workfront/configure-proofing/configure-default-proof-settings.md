---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-proofing-functionality
title: 配置預設校樣設定
description: 這些設定可讓您設定套用至使用者建立之所有新校樣的預設值。 不過，使用者在建立校樣時可以覆寫其中大部分的設定。
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: cfccb120-8759-49f2-8b7b-dabcd57d4fda
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '513'
ht-degree: 7%

---

# 配置預設校樣設定

這些設定可讓您設定套用至使用者建立之所有新校樣的預設值。 不過，使用者在建立校樣時可以覆寫其中大部分的設定。

## 配置新的校樣預設設定

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **設定**.
1. 在左側面板中，按一下 **校樣** > **校樣設定**.
1. 在 **新校樣預設值** 區段，配置下列設定：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader" colspan="2"><b>收件者</b></td> 
     </tr> 
     <tr> 
      <td role="rowheader">需要登入</td> 
      <td> <p>審核者必須先使用其電子郵件和密碼登入，才能檢視在您組織帳戶中建立的校樣。 啟用後，用戶無法與來賓審核者共用校樣。</p> <p><b>重要</b>:啟用後，所有新建立的校樣都需登入。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">從原始校訂中複製所有者以取得新版本</td> 
      <td> <p>第一個版本的擁有者也是所有連續版本的驗證的擁有者，無論是誰建立這些版本。 預設會啟用此設定。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">允許使用者刪除他們的校訂評論</td> 
      <td>使用者可以刪除自己的留言。 預設會啟用此設定。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">需要以電子方式簽署決策 </td> 
      <td> <p>決策者在決定證明時，系統會提示他們輸入其Workfront登入憑證。</p> <p><b>重要</b>:啟用後，使用者無法與沒有登入憑證的訪客審核者共用校樣。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader" colspan="2"><b>期限</b></td> 
     </tr> 
     <tr> 
      <td role="rowheader">設定預設期限</td> 
      <td> <p>系統會將此截止日期套用至帳戶中沒有自動化工作流程的所有新校樣。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">在舉證有風險前通知收件者</td> 
      <td>收件者會透過電子郵件收到通知，之後會根據上述指定的期限，將校樣視為有風險。</td> 
     </tr> 
     <tr> 
      <td role="rowheader" colspan="2"><b>電子郵件通知</b></td> 
     </tr> 
     <tr> 
      <td role="rowheader">當收件者被新增至校訂時通知他們</td> 
      <td>收件者新增至校樣時，會透過電子郵件收到通知。</td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下&#x200B;**儲存**。

## 配置校樣決策

使用者可使用校樣決策，在審核後指出校樣的狀態。

>[!NOTE]
>
>如果有多個不同層級的決策，則證明決策背後的邏輯用於計算證明工作流的整體狀態。 「已核准」和「已核准且變更」決策會觸發自動工作流程的下一個階段。

要配置校樣決策：

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **設定**.
1. 在左側面板中，按一下 **校樣** > **校樣設定**.
1. 在 **決策**&#x200B;區段，您可以

   1. **更名決策**:按一下決策方塊內的文字，然後開始輸入新的決策標籤。

      >[!TIP]
      >
      >重新命名決策時，請保留該邏輯。 例如，預設決策「已拒絕」可變更為 *需要新版本*，但不應變更為 *發送到打印機*.

      ![](assets/rename-decision-350x109.png)

   1. **重新排列決策順序**:依照您希望決策方塊在校對檢視器中的顯示順序來拖曳決策方塊。

      ![](assets/move-decision-350x110.png)

   1. **隱藏決策**:將滑鼠指標暫留在決策方塊上，然後按一下右上角的隱藏圖示。

      ![](assets/hide-decision-350x109.png)

1. （選用）若要回復Workfront預設值，請按一下 **還原預設值**.
1. 按一下&#x200B;**儲存**。
