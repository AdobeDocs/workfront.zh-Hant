---
user-type: administrator
content-type: reference
product-area: system-administration;workfront-integrations
navigation-topic: best-practices-catalog
title: 安裝Blueprint
description: 您可以在生產環境或沙箱環境中安裝Blueprint。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 546e19ab-dc50-4d23-b5f6-31bde1c82b6a
source-git-commit: 5fd855bec596926a4361fd07a1a763c7956e5e61
workflow-type: tm+mt
source-wordcount: '475'
ht-degree: 1%

---

# 安裝Blueprint

<!-- Audited: 5/2025 -->

您可以在生產環境或沙箱環境中安裝Blueprint。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront套件</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td>
   <p>標準</p>
   <p>規劃</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td>Workfront管理員</td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 我該在哪裡安裝Blueprint？ {#where-should-i-install-a-blueprint}

您可以在下列任何環境中安裝套件：

<table style="table-layout:auto">
        <tr>
        <td><strong>生產</strong></td>
        <td>生產環境是您的即時環境。</td>
    </tr>
    <tr>
        <td><strong>Sandbox 預覽</strong></td>
        <td>沙箱預覽是測試環境，可作為即時環境的復本，並在每個週末由Adobe Workfront重新整理。 所有支援套件都可存取「沙箱預覽」。 如需詳細資訊，請參閱<a href="../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md">預覽Sandbox環境[!DNL Adobe Workfront]。</a></td>
    </tr>
    <tr>
        <td><strong>Sandbox 1和2</strong></td>
        <td>自訂重新整理沙箱是獨立的測試環境，由您手動重新整理。 取得自訂重新整理沙箱需要額外付費。 如需詳細資訊，請參閱<a href="../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md">自訂重新整理沙箱環境[!DNL Adobe Workfront]。</a></td>
    </tr>
</table>

>[!TIP]
>
>我們建議先在沙箱環境中安裝Blueprint。 如此一來，您可以測試Blueprint的內容，並確保其非常適合您的組織，無需對即時資料進行變更。

>[!NOTE]
>
>某些Blueprint只能安裝在預覽環境中以進行測試。 如果您在生產環境、沙箱1或沙箱2中存取僅預覽內容，則安裝按鈕不會啟用，並且您可能會看到警告訊息。\
>此外，存取僅限預覽的內容時，即使您是在預覽環境中，環境切換功能也會受到限制。

## 安裝Blueprint

{{step1-to-blueprints}}

1. 尋找您要安裝的Blueprint。 您可以依使用案例、成熟度層級、安裝狀態以及頁面右側的型別來篩選。
1. （選用）按一下「**[!UICONTROL 詳細資料]**」以瞭解Blueprint的運作方式。
1. 按一下&#x200B;**[!UICONTROL 安裝]**。
1. 選擇安裝在您的生產環境或沙箱環境中。\
   如需詳細資訊，請參閱[我該在哪裡安裝Blueprint？本文中的](#where-should-i-install-a-blueprint)節。
1. 在&#x200B;**設定**&#x200B;頁面上，您可以選擇執行下列任一項作業：

   * 依原樣安裝Blueprint。 對於不需要任何設定的Blueprint型別，這是唯一的選項。 對於需要設定的Blueprint型別，您可以選擇現在安裝Blueprint並於稍後進行設定。 按一下[依原樣安裝] ****。
   * 在安裝之前設定藍圖，適用於需要設定的Blueprint。 選擇您的設定，然後按一下&#x200B;**[!UICONTROL 安裝Blueprint]**。

     如需詳細資訊，請參閱[設定藍圖](../../administration-and-setup/blueprints/configure-template-package.md)。

   安裝完成，並顯示已成功與Blueprint一起安裝的特定物件（例如角色、專案團隊或群組）清單，以及任何無法安裝的物件。

安裝Blueprint後，可能需要一些其他動作才能完全部署。 如需詳細資訊，請參閱安裝Blueprint[後要採取的](../../administration-and-setup/blueprints/best-next-actions-after-install.md)動作。
