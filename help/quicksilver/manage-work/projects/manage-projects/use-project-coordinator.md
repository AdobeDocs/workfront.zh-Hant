---
title: 使用專案協調員共同作業人員
content-type: reference
description: 瞭解如何使用專案協調器，這個現成的AI共同作業程式可監控專案狀態並追蹤逾期任務。
author: Becky
feature: Work Management, Projects
source-git-commit: 13403cc11448a0611ad0996ed21e1745277e9c05
workflow-type: tm+mt
source-wordcount: '513'
ht-degree: 4%

---
# 使用專案協調員共同作業人員

{{highlighted-preview-article-level}}

專案協調員是現成的AI共同作業人員，可監視您的專案並通知利害關係人重要狀態資訊。

使用專案協調員不需要在Workfront外部設定代理程式。

如需設定專案協調器的說明，請參閱「設定AI共同作業人員」一文中的[「設定專案協調器」](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md#configure-a-project-coordinator)。

如需一般的AI共同作業人員資訊，請參閱[設定AI共同作業人員](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md)。

## 存取權要求

+++ 展開以檢視這篇文章中所述功能的存取權要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] 封裝</td> 
   <td><p>選取、Prime或Ultimate</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] 授權</td> 
   <td><p>[!UICONTROL 標準]</p></td>
  </tr> 
  <tr> 
   <td>物件許可權</td> 
   <td>您必須擁有專案的管理許可權才能指派專案協調員。</td> 
  </tr>
  </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 專案協調員概觀

專案協調員會監視您的專案，並協助您順利完成工作。 當指派給專案時，會依管理員設定的排程傳送專案更新。 更新可包括：

* 進度摘要
* 專案健康情況
* 逾期或存在風險的任務或核准
* 遺失欄位或指派

專案協調員也可以評論專案及其任務。

您的管理員會設定傳送更新的頻率、傳送時間以及誰會收到更新。

您也可以在專案的更新中提及「專案協調器」，以隨選執行。 當提到專案協調器時，即使沒有排程在該時間執行，它也會執行。

>[!NOTE]
>
>專案協調員行為可能會在一般可用性之前變更。

## 將專案協調員新增至專案

管理員必須先建立專案協調器，並將&#x200B;**專案協調器**&#x200B;欄位新增到版面配置範本中的專案標題。 然後欄位會出現在專案標題中。

如需詳細資訊，請參閱[使用配置範本自訂物件標頭](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md)。

若要將專案協調員指派給專案：

1. 移至您要為其指派專案協調器的專案。
1. 在專案標題中，按一下&#x200B;**專案協調員**&#x200B;欄位。
1. 選取您要指派的專案協調器。

   此視窗會顯示所選「專案協調器」的描述，以及「專案協調器」執行的動作。
1. 按一下「**套用**」。

## 透過提及專案協調員來執行它

除了其排定的更新外，您可以隨時透過在專案上@mentioning入更新來觸發專案協調員。 專案協調員一經提及，就會執行，即使當時並未排定該協調員執行。

提及專案協調員：

1. 移至已指派專案協調器的專案。
1. 開啟專案的&#x200B;**更新**&#x200B;區域。
1. 在更新欄位中，輸入&#x200B;**@**&#x200B;並選取專案協調員。
1. 新增您的訊息，然後張貼更新。

   專案協調員執行並張貼其回應。

>[!NOTE]
>
>您必須先將專案協調員指派給專案，才能使用@mention案觸發專案。

## 設定專案協調員

如需設定專案協調器的說明，請參閱「設定AI共同作業人員」一文中的[「設定專案協調器」](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md#configure-a-project-coordinator)。
