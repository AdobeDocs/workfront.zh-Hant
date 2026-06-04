---
title: 品牌化Adobe Workfront執行個體
user-type: administrator
product-area: system-administration
navigation-topic: brand-workfront
description: Adobe Workfront不再提供品牌化功能。 此功能在Workfront上線至Adobe Experience Cloud時已遭取代。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 94603393-bdea-4673-9256-08da14f6916e
TQID: https://experienceleague.adobe.com/kay1VuO1Kk45rqyVRBbMe9xNI-j92rh2thW1IMtsg0Y
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 56
ht-degree: 8%

---

# 為您的 Adobe Workfront 執行個體建立品牌

<!--
**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **
-->

>[!IMPORTANT]
>
>Adobe Workfront不再提供品牌化功能。 此功能在Workfront上線至Adobe Experience Cloud時已遭取代。

<!-- 


>[!IMPORTANT]
>
>The procedure described on this page applies only to organizations that are not yet onboarded to [!DNL Adobe Experience Cloud].
>
> If your organization has been onboarded to [!DNL Adobe Experience Cloud], branding is not available.

As a Workfront administrator, you can brand Workfront with logos in the following places:

* Login screen

  ![Brand in login screen](assets/brand-login-screen-nwe-adobe.jpg)

* Top navigation area

  ![Brand in top navigation](assets/brand-top-nav-area-nwe-adobe.jpg)

* Main Menu

  ![Brand in main menu](assets/brand-main-menu-adobe.jpg)

You can also change the background image and color of the login screen:

![Banner on login screen](assets/wf_banner_on_login_screen-adobe.png)

>[!NOTE]
>
>* Changing the login background image and color is not available if your organization's Workfront instance uses a custom SSO portal. See your network or IT administrator if you need more information.
>
>
>* A Workfront administrator or group administrator can also brand Workfront for certain groups and users using a layout template. Branding in a layout template overrides the system-level branding explained in this article. For instructions on branding in a layout template, see [Brand Adobe Workfront using a layout template](../../../administration-and-setup/customize-workfront/use-layout-templates/brand-wf-using-a-layout-template.md).

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront package</td> 
   <td><p>Any</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront license</td> 
   <td><p>Standard</p>
       <p>Plan</p></td>
  </tr> 
  <tr> 
   <td>Access level configurations</td> 
   <td>System Administrator</td> 
  </tr> 
 </tbody> 
</table>

For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Brand the login screen

{{step-1-to-setup}}

1. Click **System** > **Branding**.

1. Make any of the following changes to customize Workfront with your branding images.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>Brand the Home icon <span style="font-weight: normal;">(displays at the far left of the top navigation area)</span></p> </td> 
      <td> <p>In the <strong>Top navigation area</strong> section, under <strong>Home icon</strong>, click anywhere in the box, then find and select your logo image. Or drag an image to the box.</p> <p>To crop the image, use the scrolling controls and drag the image to the position you want inside the prescribed space.</p> <p>We recommend a 120 x 120 image. It can be in any of the following formats: GIF, JPG, PNG, SVG.</p> <p>This icon also appears in reports, lists, dashboards, and delivered reports that users export as PDF files.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Brand the Main Menu <img src="assets/main-menu-icon.png"> logo <span style="font-weight: normal;">(displays in the upper-right corner of the Main Menu)</span></p> </td> 
      <td> <p>In the <strong>Top navigation area</strong> section, under <strong>Main Menu logo</strong>, click anywhere in the box, then find and select your logo image. Or drag an image to the box.</p> <p>To crop the image, use the scrolling controls and drag the image to the position you want inside the prescribed space.</p> <p>We recommend a 300 x 120 pixel image. It can be in any of the following formats: GIF, JPG, PNG, SVG.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Brand the login screen logo <span style="font-weight: normal;">(displays in the top-left of the box where users type login credentials)</span></td> 
      <td> <p>Under <strong>Login Screen</strong>, click anywhere in the box, then find and select your logo image. To crop the image, use the scrolling controls and drag the image to the position you want inside the prescribed space.</p> <p>We recommend a 300 x 120 pixel image. It can be in any of the following formats: GIF, JPG, PNG, SVG.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Brand the login screen background color <span style="font-weight: normal;">(displays behind the box where users type login credentials)</span></td> 
      <td> <p>Under <strong>Login Screen</strong>, set a <strong>Background Color</strong>. </p> <p>You can use RGB or HEX color codes.</p> <p>The background color is visible only if the login screen background is larger than the login screen background image (see the next row in this table) or if there is any transparency in the image.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Brand the login screen background image <span style="font-weight: normal;">(displays behind the box where users type their login credentials)</span></td> 
      <td> 
       <ol style="list-style-type: lower-alpha;"> 
        <li value="1"> <p> In the <strong>Login Screen</strong> area, under <strong>Background Image</strong>, click the box, then find and select your JPG or PNG image or images (up to 20 ). </p> <p>Multiple background images display in random order, changing each time users refresh their login page. We recommend images no larger than 2 MB.</p> </li> 
        <li value="2"> <p>Hover over each background image you have uploaded, click the Settings (gear) icon, and use any of the following options to specify where and how you want the image to appear in the login screen background:</p> 
         <ul> 
          <li> <p><strong>Fill Screen</strong>: Fits the image to the login screen background, which may enlarge the image. Use a high-resolution image (up to 2 MB) for the best results.</p> <p>When you use this option, the Workfront banner, which is not customizable, obscures part your image.</p> </li> 
          <li> <p><strong>Tile</strong>: Tiles your image across the login screen background area, in its original size. This is useful for creating a pattern. Select a blue alignment option to start the tiling from the top-left corner, top-center, or top-right of the background area.</p> </li> 
          <li> <p><strong>Position</strong>: Places your image in its original size in the position you choose using one of the blue alignment options: the top-left, top-center, or top-right of the login screen background area.</p> <p>The background color fills the rest of the login screen background area. For more about the background color, see the preceding row in this table.</p> </li> 
         </ul> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Reset to the default branding</td> 
      <td> <p>Resetting to the default branding deletes all photos and images that you have uploaded.</p> <p>Click <strong>Reset all branding to Workfront defaults</strong> in the lower-right corner of the screen, then click <strong>Yes</strong>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >This is not available if your organization's Workfront instance uses a custom SSO portal.
   >
   >
   >See your network or IT administrator if you need more information.

1. Click **Save**.

-->