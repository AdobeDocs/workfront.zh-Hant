---
product-area: resource-management
navigation-topic: the-workload-balancer
title: 管理工作負載平衡工具中的資源所需的存取權
description: 沒有正確的存取權或許可權，您可能無法在工作負載平衡器中檢視或管理您的工作指派。
author: Lisa
feature: Resource Management
exl-id: b3da9a62-481e-4503-8f27-136d6513262e
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/qokl32bOcjAvfU4OmQHDVaKtf09q6iXdLKtWxgpr9bE
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aadid: e14a7f57-c82c-4874-a495-5d036cbbdc3d
subfeature_v2: id: c33d85a1-be85-4290-854c-87408c10aa80
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 375
ht-degree: 2%

---

# 管理工作負載平衡工具中的資源所需的存取權

沒有正確的存取權或許可權，您可能無法在工作負載平衡器中檢視或管理您的工作指派。

您必須有權檢視您要在工作負載平衡器中檢視或管理其工作負載的使用者。 除此之外，您必須在與工作關聯的專案上擁有正確的存取層級和正確的許可權。

<!--
## Adobe Workfront package needed to use the Workload Balancer for different areas

The following table illustrates the connection between the Workfront plan your company has and where in the system you can use the Workload Balancer:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><p><b>Workfront Plan (Current)</b></p></td> 
   <td> <p><b>Areas where you can access the Workload Balancer</b></p> </td> 
  </tr> 
  <tr> 
   <td>Team or higher </td> 
   <td>Workload Balancer for a team or a project</td> 
  </tr> 
  <tr> 
   <td>Pro or higher</td> 
   <td>Workload Balancer for multiple projects, at the system level</td> 
  </tr> 
  <tr> 
   <td><p><b>Workfront Plan (New)</b></p></td> 
   <td> <p><b>Areas where you can access the Workload Balancer</b></p> </td> 
  </tr>
  <tr> 
   <td>Any </td> 
   <td>Access the Workload Balancer anywhere in Workfront</td> 
  </tr> 
 </tbody> 
</table>

For information about the Workfront plans, see [Our Plans](https://business.adobe.com/products/workfront/pricing.html).

For information about where you can locate the Workload Balancer in Workfront, see [Locate the Workload Balancer](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).
-->

## 檢視工作負載平衡器所需的存取權

您必須具有下列存取權才能檢視工作負載平衡器：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody>
  <tr> 
   <td>Adobe Workfront 封裝</td> 
   <td><p>任何</p></td>
  </tr>
  <tr> 
   <td>Adobe Workfront授權</td> 
   <td><p>標準</p>
       <p>計畫：在資源區域中檢視工作負載平衡器；工作：檢視團隊或專案的工作負載平衡器</p></td>
  </tr>  
  <tr> 
   <td>存取層級設定</td> 
   <td> <p>檢視或更高的資源管理存取許可權</p> <p>如需有關資源管理存取層級的資訊，請參閱文章<a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md">授予資源管理的存取權</a>。</p></td> 
  </tr> 
  <tr> 
   <td>物件許可權</td> 
   <td> <p>您必須擁有專案的檢視許可權，才能檢視您要檢視的工作總攬。 </p> <p>如需有關專案許可權的資訊，請參閱文章<a href="../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md">在Adobe Workfront中共用專案</a>。</p></td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

所有使用者都有權在其個人設定檔上檢視工作負載平衡器。 這不受授權或存取層級的限制。 請注意，使用者設定檔上的工作負載平衡器是唯讀的，指派和配置無法變更。

## 管理工作負載平衡器中指派所需的存取權

您必須具有下列存取權才能管理工作負載平衡器：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody>
  <tr> 
   <td>Adobe Workfront 封裝</td> 
   <td><p>任何</p></td>
  </tr>
  <tr> 
  <tr> 
   <td>Adobe Workfront授權</td> 
   <td><p>標準</p>
       <p>計畫，在資源區域的工作負載平衡器中管理指派；工作，在團隊或專案的工作負載平衡器中管理指派</p></td>
  </tr> 
  <tr> 
   <td>存取層級設定</td>
   <td> <p>編輯對資源管理的存取權</p>
     <p>如需有關資源管理存取層級的資訊，請參閱文章<a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md" >授予資源管理的存取權</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>物件許可權</td> 
   <td> <p> 您想要管理其指派的專案的Contribute或更高許可權，包括進行指派的許可權。 </p> <p>如需有關專案許可權的資訊，請參閱文章<a href="../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md">在Adobe Workfront中共用專案</a>。</p></td>
  </tr> 
 </tbody>
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。


