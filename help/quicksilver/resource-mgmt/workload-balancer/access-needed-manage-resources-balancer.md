---
product-area: resource-management
navigation-topic: the-workload-balancer
title: 管理工作負載平衡工具中的資源所需的存取權
description: 沒有正確的存取權或許可權，您可能無法在工作負載平衡器中檢視或管理您的工作指派。
author: Lisa
feature: Resource Management
exl-id: b3da9a62-481e-4503-8f27-136d6513262e
source-git-commit: 2c4fe48ef969741ba792e37c28adba86ffdcba9a
workflow-type: tm+mt
source-wordcount: '533'
ht-degree: 0%

---

# 管理工作負載平衡工具中的資源所需的存取權

如果沒有正確的存取權或許可權，您可能無法在「工作負載平衡器」中檢視或管理您的工作指派。

您必須有權檢視您要在工作負載平衡器中檢視或管理其工作負載的使用者。 除此之外，您必須在與工作關聯的專案上擁有正確的存取層級和正確的許可權。

## Adobe Workfront計畫需要在不同的區域使用工作負載平衡器

下表說明貴公司擁有的Workfront計畫與系統中可使用工作負載平衡器的位置之間的連線：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><p><b>Workfront 計畫</b></p></td> 
   <td> <p><b>您可以存取工作負載平衡器的區域</b></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">團隊或以上 </td> 
   <td>團隊或專案的工作負載平衡器</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Pro或更高</td> 
   <td>系統層級多個專案的工作負載平衡器</td> 
  </tr> 
 </tbody> 
</table>

如需Workfront計畫的相關資訊，請參閱 [我們的計畫](https://www.workfront.com/plans).

如需有關在Workfront中可找到工作負載平衡器的資訊，請參閱 [找到工作負載平衡器](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

## 檢視工作負載平衡器所需的存取權

您必須具有下列存取權才能檢視工作負載平衡器：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>規劃在資源區域中檢視工作負載平衡器</p>
   <p>工作以檢視團隊或專案的工作負載平衡器</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>檢視或更高的資源管理存取許可權</p> <p>如需有關資源管理存取層級的資訊，請參閱文章 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md" class="MCXref xref">授與資源管理的存取權</a>.</p> <p><b>附註</b>

如果您還是沒有存取權，請詢問您的Workfront管理員，他們是否在您的存取層級中設定其他限制。 如需有關Workfront管理員如何修改您的存取層級的資訊，請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>您對想要檢視其指派的專案具有檢視許可權。 </p> <p>如需有關專案許可權的資訊，請參閱文章 <a href="../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">在Adobe Workfront中共用專案</a>.</p> <p>如需請求其他存取許可權的詳細資訊，請參閱 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">要求物件的存取權 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的Workfront管理員。

## 管理工作負載平衡器中指派所需的存取權

您必須具有下列存取權才能管理工作負載平衡器：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>規劃以管理在資源區域的工作負載平衡器指派</p>
   <p>致力於管理團隊或專案的工作負載平衡器中的指派</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>編輯對資源管理的存取權</p> 
     <p>如需有關資源管理存取層級的資訊，請參閱文章 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md" class="MCXref xref">授與資源管理的存取權</a>.</p>
     <p><b>附註</b>

如果您還是沒有存取權，請詢問您的Workfront管理員，他們是否在您的存取層級中設定其他限制。 如需有關Workfront管理員如何修改您的存取層級的資訊，請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p> 您想要管理其指派的專案的Contribute或更高許可權，包括進行指派的許可權。 </p> <p>如需有關專案許可權的資訊，請參閱文章 <a href="../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">在Adobe Workfront中共用專案</a>.</p> <p>如需請求其他存取許可權的詳細資訊，請參閱 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">要求物件的存取權 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的Workfront管理員。

<!--these notes were inside the table: for the Edit access to Res Management
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">View or higher access to Financial Data, if you want to view information by cost (NOTE: this is not possible yet!)</p>    
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about the Financial Data access level, see the article<a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">Grant access to financial data</a>. (NOTE: this is not possible yet!)</p>
    -->