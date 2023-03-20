---
product-area: resource-management
navigation-topic: the-workload-balancer
title: 在工作負載平衡器中管理資源所需的訪問
description: 如果沒有正確的訪問權限或權限，您可能無法在工作負載平衡器中查看或管理您的工作分配。
author: Alina
feature: Resource Management
exl-id: b3da9a62-481e-4503-8f27-136d6513262e
source-git-commit: bbd99435bb07d68bf9058bcd3e8c6ef5d9df75a9
workflow-type: tm+mt
source-wordcount: '535'
ht-degree: 0%

---

# 在工作負載平衡器中管理資源所需的訪問

如果沒有正確的訪問權限或權限，您可能無法在工作負載平衡器中查看或管理您的工作分配。

您必須有權查看要在工作負載平衡器中查看或管理其工作負載的用戶。 除此之外，您必須對與工作相關聯的專案擁有正確的存取層級和正確的權限。

## Adobe Workfront計畫需要針對不同領域使用工作負載平衡器

下表說明了貴公司擁有的Workfront計畫與系統中可使用工作負載平衡器的位置之間的連接：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><p><b>Workfront 計畫</b></p></td> 
   <td> <p><b>可以訪問工作負載平衡器的區域</b></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">團隊或更高 </td> 
   <td>團隊或項目的工作負載平衡器</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Pro或更高版本</td> 
   <td>系統級多個項目的工作負載平衡器</td> 
  </tr> 
 </tbody> 
</table>

如需Workfront計畫的相關資訊，請參閱 [我們的計畫](https://www.workfront.com/plans).

有關可以在Workfront中找到工作負載平衡器的位置的資訊，請參見 [找到工作負載平衡器](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

## 查看工作負載平衡器所需的訪問

要查看工作負載平衡器，您必須具有以下訪問權限：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>計畫在資源區中查看工作負載平衡器</p>
   <p>工作以查看團隊或項目的工作負載平衡器</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>查看或更高程度地訪問資源管理</p> <p>有關資源管理訪問級別的資訊，請參見文章 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md" class="MCXref xref">授予資源管理的訪問權限</a>.</p> <p><b>附註</b>

如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>您對要查看其分配的項目具有「查看」權限。 </p> <p>如需專案權限的相關資訊，請參閱文章 <a href="../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">在Adobe Workfront中共用專案</a>.</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 在工作負載平衡器中管理分配所需的訪問

要管理工作負載平衡器，您必須具有以下訪問權限：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>計畫在資源區的工作負載平衡器中管理分配</p>
   <p>在團隊或項目的工作負載平衡器中管理分配</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯對資源管理的訪問</p> 
     <p>有關資源管理訪問級別的資訊，請參見文章 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md" class="MCXref xref">授予資源管理的訪問權限</a>.</p>
     <p><b>附註</b>

如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p> 對要管理其分配的項目貢獻或更高權限，包括進行分配的權限。 </p> <p>如需專案權限的相關資訊，請參閱文章 <a href="../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">在Adobe Workfront中共用專案</a>.</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

<!--these notes were inside the table: for the Edit access to Res Management
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">View or higher access to Financial Data, if you want to view information by cost (NOTE: this is not possible yet!)</p>    
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about the Financial Data access level, see the article<a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">Grant access to financial data</a>. (NOTE: this is not possible yet!)</p>
    -->