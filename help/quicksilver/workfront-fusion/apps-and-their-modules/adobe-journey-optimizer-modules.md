---
filename: adobe-journey-optimizer-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Adobe Journey Optimizer模組
description: 在 [!DNL Adobe Workfront Fusion] 情境中，您可以使用自動化工作流程 [!DNL Adobe Journey Optimizer]，並連結至多個協力廠商應用程式和服務。
author: Becky
feature: Workfront Fusion
exl-id: 2c1aea46-edbf-42a3-a6e9-f8aea042a48d
hide: true
hidefromtoc: true
source-git-commit: 35c4043c40a374006e0023be5a1e942e95a63863
workflow-type: tm+mt
source-wordcount: '59'
ht-degree: 0%

---

# [!DNL Adobe Journey Optimizer] 模組

>[!IMPORTANT]
>
>此聯結器已淘汰，因為它是根據現在已淘汰的Adobe Journey Optimizer API。
>
>我們目前正在開發以新Adobe Journey Optimizer API為基礎的新聯結器。

<!--

In an [!DNL Adobe Workfront Fusion] scenario, you can automate workflows that use [!DNL Adobe Journey Optimizer], as well as connect it to multiple third-party applications and services. [!DNL Adobe Journey Optimizer] modules allow you to create, read, update, or delete records, or perform a custom API call to the [!DNL Adobe Journey Optimizer] API.


If you need instructions on creating a scenario, see [Create a scenario](../../workfront-fusion/scenarios/create-a-scenario.md).

For information about modules, see [Modules in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## Access requirements

You must have the following access to use the functionality in this article:

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] plan*</td>
      <td>
        <p>[!UICONTROL Pro] or higher</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] license*</td>
      <td>
        <p>[!UICONTROL Plan], [!UICONTROL Work]</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront Fusion] license**</td>
      <td>
   <p>Current license requirement: No [!DNL Workfront Fusion] license requirement.</p>
   <p>Or</p>
   <p>Legacy license requirement: [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td>
    </tr>
    <tr>
      <td role="rowheader">Product</td>
      <td>
   <p>Current product requirement: If you have the [!UICONTROL Select] or [!UICONTROL Prime] [!DNL Adobe Workfront] Plan, your organization must purchase [!DNL Adobe Workfront Fusion] as well as [!DNL Adobe Workfront] to use functionality described in this article. [!DNL Workfront Fusion] is included in the [!UICONTROL Ultimate] [!DNL Workfront] plan.</p>
   <p>Or</p>
   <p>Legacy product requirement: Your organization must purchase [!DNL Adobe Workfront Fusion] as well as [!DNL Adobe Workfront] to use functionality described in this article.</p>
   </td>
    </tr>
  </tbody>
</table>


To find out what plan, license type, or access you have, contact your [!DNL Workfront] administrator.

For information on [!DNL Adobe Workfront Fusion] licenses, see [[!DNL Adobe Workfront Fusion] licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Prerequisites

Before you can use the [!DNL Adobe Journey Optimizer] connector, you must ensure that the following prerequisites are met:

* You must have an active [!DNL Adobe Journey Optimizer] account.

## Create a connection to [!DNL Adobe Journey Optimizer]

To create a connection for your [!DNL Adobe Journey Optimizer] modules:

1. In any [!DNL Adobe Journey Optimizer] module, click **[!UICONTROL Add]** next to the Connection box.

1. Fill in the following fields:

   <table style="table-layout:auto"> 
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
      </col>
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
      </col>
      <tbody>
        <tr>
          <td role="rowheader">[!UICONTROL Connection name]</td>
          <td>
            <p>Enter a name for this connection.</p>
          </td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Client ID]</td>
          <td>Enter your [!DNL Adobe] [!UICONTROL Client ID]. This can be found in the [!UICONTROL Credentials details] section of the [!DNL Adobe Developer Console].</td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Client Secret]</td>
          <td>Enter your [!DNL Adobe] [!UICONTROL Client Secret]. This can be found in the [!UICONTROL Credentials details] section of the [!DNL Adobe Developer Console].
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Technical account ID]</td>
          <td>Enter your [!DNL Adobe] [!UICONTROL Technical account ID]. This can be found in the [!UICONTROL Credentials details] section of the [!DNL Adobe Developer Console].
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Organization ID]</td>
          <td>Enter your [!DNL Adobe] [!UICONTROL Organization ID]. This can be found in the [!UICONTROL Credentials details] section of the [!DNL Adobe Developer Console].
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Meta scopes]</td>
          <td>
            Enter any meta scopes needed for the connection.
          </td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Private key]</td>
          <td>
            <p>Enter the private key that was generated when your credentials were created in the [!DNL Adobe Developer Console]. </p>
            <p>To extract your private key or certificate:</p>
            <ol>
              <li value="1">
                <p>Click <b>[!UICONTROL Extract]</b>.</p>
              </li>
              <li value="2">
                <p>Select the type of file you are extracting.</p>
              </li>
              <li value="3">
                <p>Select the file that contains the private key or certificate.</p>
              </li>
              <li value="4">
                <p>Enter the password for the file.</p>
              </li>
              <li value="5">
                <p>Click <b>[!UICONTROL Save]</b> to extract the file and return to the connection setup.</p>
              </li>
            </ol>
          </td>
        </tr>
      </tbody>
    </table>
1. Click **[!UICONTROL Continue]** to save the connection and return to the module.

## [!DNL Adobe Journey Optimizer] modules and their fields

When you configure [!DNL Adobe Journey Optimizer] modules, [!DNL Workfront Fusion] displays the fields listed below. Along with these, additional [!DNL Adobe Journey Optimizer] fields might display, depending on factors such as your access level in the app or service. A bolded title in a module indicates a required field.

If you see the map button above a field or function, you can use it to set variables and functions for that field. For more information, see [Map information from one module to another in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Actions](#actions)
* [Searches](#searches)

### Actions

* [[!UICONTROL Create a record]](#create-a-record)
* [[!UICONTROL Make a custom API call]](#make-a-custom-api-call)
* [[!UICONTROL Delete a record]](#delete-a-record)
* [[!UICONTROL Update a record]](#update-a-record)

#### [!UICONTROL Create a record]

This action module creates a placement, decision rule, tag, personalized offer, collection, or fallback offer.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
     <td>For instructions on creating a connection to [!DNL Adobe Journey Optimizer], see <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Create a connection to [!DNL Adobe Journey Optimizer]</a> in this article.</td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Record type]
      </td>
      <td>
        Select the type of record that you want to create
        <ul>
        <li><b>[!UICONTROL Placement]</b>: Continue to <a href="#placement-fields" >[!UICONTROL Placement] fields</a>.</li>
        <li><b>[!UICONTROL Decision rule]</b>: Continue to <a href="#decision-rule-fields" >[!UICONTROL Decision rule] fields</a>.</li>
        <li><b>[!UICONTROL Decision]</b>: Continue to <a href="#decision-fields" >[!UICONTROL Decision] fields</a>.</li>
        <li><b>[!UICONTROL Tag]</b>: Continue to <a href="#tag-fields" >[!UICONTROL Tag] fields</a>.</li>
        <li><b>[!UICONTROL Collection]</b>: Continue to <a href="#collection-fields" >[!UICONTROL Collection] fields</a>.</li>
        <li><b>[!UICONTROL Fallback offer]</b>: Continue to <a href="#fallback-offer-fields" >[!UICONTROL Fallback offer] fields</a>.</li>
        <li><b>[!UICONTROL Personalized offer]</b>: Continue to <a href="#personalized-offer-fields" >[!UICONTROL Personalized offer] fields</a>.</li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

##### [!UICONTROL Placement] fields

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
     <td>Enter or map a name for the placement.</td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Description]
      </td>
      <td>Enter or map a description for the placement.
      </td>
    </tr>
  </tbody>
</table>


##### [!UICONTROL Decision rule] fields

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
     <td>Enter or map a name for the description rule.</td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Description]
      </td>
      <td>Enter or map a description for the decision rule.
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Condition]
      </td>
      <td>Enter or map the condition the decision rule.
      </td>
    </tr>
  </tbody>
</table>

##### [!UICONTROL Decision] fields

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
     <td>Enter or map a name for the description rule.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Status]</td>
      <td>Select the status for the decision.
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Start date]</td>
      <td><p>Enter or map the start date for the decision.</p><p>For a list of supported date formats, see <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Type coercion in [!DNL Adobe Workfront Fusion]</a>.</p>
      </td>
    </tr>
   <tr>
      <td role="rowheader">[!UICONTROL End date]</td>
      <td><p>Enter or map the end date for the decision.</p><p>For a list of supported date formats, see <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Type coercion in [!DNL Adobe Workfront Fusion]</a>.</p>
      </td>
    </tr>
   <tr>
      <td role="rowheader">[!UICONTROL Placements]</td>
      <td>Select the placements to add to this decision
      </td>
    </tr>
   <tr>
      <td role="rowheader">[!UICONTROL Collection]</td>
      <td>Select the offer collection that contains the offers that this decision will consider.
      </td>
    </tr>
   <tr>
      <td role="rowheader">[!UICONTROL Fallback offer]</td>
      <td>Select the fallback offer that will be presented to customers that do not match the rules for this decision.
      </td>
    </tr>
  </tbody>
</table>

##### [!UICONTROL Tag] fields

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
     <td>Enter or map a name for the tag.</td>
    </tr>
  </tbody>
</table>

##### [!UICONTROL Collection] fields

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
     <td>Enter or map a name for the collection.</td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Filter Type]
      </td>
      <td>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Elements]
      </td>
      <td>Select the tags to include in the colelction.
      </td>
    </tr>
  </tbody>
</table>

##### [!UICONTROL Fallback offer] fields

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
     <td>Enter or map a name for the fallback offer.</td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Status]
      </td>
      <td> Select the status of the fallback offer.
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Placement]
      </td>
      <td>Enter or map the placement for the fallback offer.
      </td>
    </tr>
  </tbody>
</table>

##### [!UICONTROL Personalized offer] fields

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
     <td>Enter or map a name for the description rule.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Status]</td>
      <td>Select the status for the decision.
      </td>
    </tr>
    <tr>
      <td role="rowheader">Placement</td>
      <td>Select the placement for the personalized offer.
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Start date]</td>
      <td><p>Enter or map the start date for the personalized offer.</p><p>For a list of supported date formats, see <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Type coercion in [!DNL Adobe Workfront Fusion]</a>.</p>
      </td>
    </tr>
   <tr>
      <td role="rowheader">[!UICONTROL End date]</td>
      <td><p>Enter or map the end date for the personalized offer.</p><p>For a list of supported date formats, see <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Type coercion in [!DNL Adobe Workfront Fusion]</a>.</p>
      </td>
    </tr>
   <tr>
      <td role="rowheader">[!UICONTROL Decision rules]</td>
      <td>Select the decision rules to add to this personalized offer.
      </td>
    </tr>
   <tr>
      <td role="rowheader">[!UICONTROL Priority]</td>
      <td>Select the priority of this offer. Priority affects whether this offer will be presented rather than another offer.
      </td>
    </tr>
   <tr>
      <td role="rowheader">[!UICONTROL Capping constraint]</td>
      <td>Enter or map the number of times this offer will be presented.
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Delete a record]

This action module deletes a single record in [!DNL Adobe Journey Optimizer].

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
     <td>For instructions on creating a connection to [!DNL Adobe Journey Optimizer], see <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Create a connection to [!DNL Adobe Journey Optimizer]</a> in this article.</td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Record type]
      </td>
      <td>
        Select the type of record that you want to delete
        <ul>
        <li>[!UICONTROL Placement]</li>
        <li>[!UICONTROL Decision rule]</li>
        <li>[!UICONTROL Decision]</li>
        <li>[!UICONTROL Tag]</li>
        <li>[!UICONTROL Collection]</li>
        <li>[!UICONTROL Fallback offer]</li>
        <li>[!UICONTROL Personalized offer]</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Placement]/[!UICONTROL Decision rule]/[!UICONTROL Decision]/[!UICONTROL Tag]/[!UICONTROL Collection]/[!UICONTROL Fallback offer]/[!UICONTROL Personalized offer]
      </td>
      <td>
        Select the record that you want to delete.
      </td>
    </tr>

</tbody>
</table>

#### [!UICONTROL Make a custom API call]

This module makes a custom API call to the [!DNL Adobe Journey Optimizer] API

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
     <td role="rowheader">[!UICONTROL Connection]</td>
     <td>For instructions on creating a connection to [!DNL Adobe Journey Optimizer], see <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Create a connection to [!DNL Adobe Journey Optimizer]</a> in this article.</td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Path]</p>
      </td>
      <td>
        <p>Enter a path relative to {baseURL} starting with<code>/</code></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Method]</p>
      </td>
   <td> <p>Select the HTTP request method you need to configure the API call. For more information, see <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP request methods in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Headers]</td>
      <td>
        <p>Add the headers of the request in the form of a standard JSON object.</p>
        <p>For example, <code>{"Content-type":"application/json"}</code></p>
        <p>Workfront Fusion adds authorization headers and x-api-key headers automatically.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Query String]  </td>
      <td>
        <p>Enter the request query string.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Body]</td>
   <td> <p>Add the body content for the API call in the form of a standard JSON object.</p> <p>Note:  <p>When using conditional statements such as <code>if</code> in your JSON, put the quotation marks outside of the conditional statement.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
     <tr>
      <td role="rowheader">[!UICONTROL Limit]  </td>
      <td>
        <p>Enter the maximum number of results that you want the module to return in one execution cycle.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Delete a Record]

This action module deletes a single record in [!DNL Adobe Journey Optimizer].

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
     <td role="rowheader">[!UICONTROL Connection]</td>
     <td>For instructions on creating a connection to [!DNL Adobe Journey Optimizer], see <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Create a connection to [!DNL Adobe Journey Optimizer]</a> in this article.</td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Record Type]
      </td>
      <td>
        Select the type of record that you want to delete
        <ul>
        <li>[!UICONTROL Placement]</li>
        <li>[!UICONTROL Decision rule]</li>
        <li>[!UICONTROL Decision]</li>
        <li>[!UICONTROL Tag]</li>
        <li>[!UICONTROL Collection]</li>
        <li>[!UICONTROL Fallback offer]</li>
        <li>[!UICONTROL Personalized offer]</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Placement]/[!UICONTROL Decision rule]/[!UICONTROL Decision]/[!UICONTROL Tag]/[!UICONTROL Collection]/[!UICONTROL Fallback offer]/[!UICONTROL Personalized offer]
      </td>
      <td>
        Select the record that you want to delete.
      </td>
    </tr>

</tbody>
</table>

#### [!UICONTROL Update a record]

This action module creates a placement, decision, decision rule, tag, personalized offer, collection, or fallback offer.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
     <td role="rowheader">[!UICONTROL Connection]</td>
     <td>For instructions on creating a connection to [!DNL Adobe Journey Optimizer], see <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Create a connection to [!DNL Adobe Journey Optimizer]</a> in this article.</td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Record type]
      </td>
      <td>
        Select the type of record that you want to update
        <ul>
        <li>[!UICONTROL Placement]</li>
        <li>[!UICONTROL Decision rule]</li>
        <li>[!UICONTROL Decision]</li>
        <li>[!UICONTROL Tag]</li>
        <li>[!UICONTROL Collection]</li>
        <li>[!UICONTROL Fallback offer]</li>
        <li>[!UICONTROL Personalized offer]</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Placement]/[!UICONTROL Decision rule]/[!UICONTROL Decision]/[!UICONTROL Tag]/[!UICONTROL Collection]/[!UICONTROL Fallback offer]/[!UICONTROL Personalized offer]
      </td>
      <td>
        Select the record that you want to update.
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Fields]
      </td>
      <td>For each field that you want to update:
      <ol>
      <li>Click <b>[!UICONTROL Add]</b>.</li>
      <li>Select whether you want to add, replace, or remove values.</li>
      <li>Enter the field that you want to update.</li>
      <li>Enter the new value for the field.</li>
      </td>
    </tr>

</tbody>
</table>


### Searches

#### [!UICONTROL List records]

This search module lists records of the selected type, returning results based on criteria you specify.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
     <td role="rowheader">[!UICONTROL Connection]</td>
     <td>For instructions on creating a connection to [!DNL Adobe Journey Optimizer], see <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Create a connection to [!DNL Adobe Journey Optimizer]</a> in this article.</td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Record type]</p>
      </td>
      <td>
        <p>Select the type of record that you want to list.</p>
        <ul>
        <li>[!UICONTROL Placement]</li>
        <li>[!UICONTROL Decision rule]</li>
        <li>[!UICONTROL Decision]</li>
        <li>[!UICONTROL Tag]</li>
        <li>[!UICONTROL Collection]</li>
        <li>[!UICONTROL Fallback offer]</li>
        <li>[!UICONTROL Personalized offer]</li>
       </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Query operator]</p>
      </td>
      <td>
        <p>Select an operator to apply to parameters in the query</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Fields]</td>
      <td><p>If you want to limit the search to specific fields, enter the fields. For each field that you want to limit the search to, click [!UICONTROL Add item] and enter the name of the field.</p><p>Path expressions are in the form of dot separated paths such as <code>_instance.xdm:name</code>.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Order by] </td>
      <td>Enter or map the property by which you want to order results.
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Order direction]</td>
   <td>Select whether you want to order results by ascending or descending direction.
    </td>
     </tr>
  </tbody>
</table>

-->
