---
title: CustomXMLPrefixMappings.LookupPrefix Method (Office)
keywords: vbaof11.chm290006
f1_keywords:
- vbaof11.chm290006
ms.prod: office
api_name:
- Office.CustomXMLPrefixMappings.LookupPrefix
ms.assetid: 49af8a41-d5d5-58e8-672f-db561c5c7688
ms.date: 06/08/2017
---


# CustomXMLPrefixMappings.LookupPrefix Method (Office)

Allows you to get a prefix corresponding to the specified namespace. 


## Syntax

 _expression_. `LookupPrefix`( `_NamespaceURI_` )

 _expression_ An expression that returns a [CustomXMLPrefixMappings](./Office.CustomXMLPrefixMappings.md) object.


### Parameters



|**Name**|**Required/Optional**|**Data Type**|**Description**|
|:-----|:-----|:-----|:-----|
| _NamespaceURI_|Required|**String**|Contains the namespace URI.|

### Return Value

String


## Remarks

If no prefix is assigned to the requested namespace, the method returns an empty string (""). If there are multiple prefixes specified in the namespace manager, the method returns the first prefix that matches the supplied namespace.


## Example

The following example retrieves the namespace prefix associated with the namespace URI. 


```vb
Dim objCustomPrefixMappings As  CustomPrefixMappings 
Dim strNamespacePrefix As String 
 
' Gets the namespace corresponding to the prefix. 
strNamespacePrefix = objCustomPrefixMappings.LookupPrefix("urn:invoice:namespace") 

```


## See also


[CustomXMLPrefixMappings Object](Office.CustomXMLPrefixMappings.md)
#### Other resources


[CustomXMLPrefixMappings Object Members](./overview/customxmlprefixmappings-members-office.md)
