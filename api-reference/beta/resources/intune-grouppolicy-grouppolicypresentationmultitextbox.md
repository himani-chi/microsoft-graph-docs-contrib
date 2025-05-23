---
title: "groupPolicyPresentationMultiTextBox resource type"
description: "Represents an ADMX multiTextBox element and an ADMX multiText element."
author: "jaiprakashmb"
ms.localizationpriority: medium
ms.subservice: "intune"
doc_type: resourcePageType
ms.date: 08/01/2024
---

# groupPolicyPresentationMultiTextBox resource type

Namespace: microsoft.graph

> **Important:** APIs under the /beta version in Microsoft Graph are subject to change which could break your applications. While Intune /beta APIs are supported by Microsoft, you should use these at your own discretion. In general, /beta APIs are not recommended for use in production applications. To determine whether an API is available in v1.0, use the Version selector

> **Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.

Represents an ADMX multiTextBox element and an ADMX multiText element.


Inherits from [groupPolicyUploadedPresentation](../resources/intune-grouppolicy-grouppolicyuploadedpresentation.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List groupPolicyPresentationMultiTextBoxes](../api/intune-grouppolicy-grouppolicypresentationmultitextbox-list.md)|[groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) collection|List properties and relationships of the [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) objects.|
|[Get groupPolicyPresentationMultiTextBox](../api/intune-grouppolicy-grouppolicypresentationmultitextbox-get.md)|[groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md)|Read properties and relationships of the [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) object.|
|[Create groupPolicyPresentationMultiTextBox](../api/intune-grouppolicy-grouppolicypresentationmultitextbox-create.md)|[groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md)|Create a new [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) object.|
|[Delete groupPolicyPresentationMultiTextBox](../api/intune-grouppolicy-grouppolicypresentationmultitextbox-delete.md)|None|Deletes a [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md).|
|[Update groupPolicyPresentationMultiTextBox](../api/intune-grouppolicy-grouppolicypresentationmultitextbox-update.md)|[groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md)|Update the properties of a [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|label|String|Localized text label for any presentation entity. The default value is empty. Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|id|String|Key of the entity. Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|lastModifiedDateTime|DateTimeOffset|The date and time the entity was last modified. Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|required|Boolean|Requirement to enter a value in the text box. Default value is false.|
|maxLength|Int64|An unsigned integer that specifies the maximum number of text characters. Default value is 1023.|
|maxStrings|Int64|An unsigned integer that specifies the maximum number of strings. Default value is 0.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|definition|[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|The group policy definition associated with the presentation. Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyPresentationMultiTextBox"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationMultiTextBox",
  "label": "String",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "required": true,
  "maxLength": 1024,
  "maxStrings": 1024
}
```