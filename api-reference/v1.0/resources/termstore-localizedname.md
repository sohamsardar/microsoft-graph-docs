---
title: "localizedName resource type"
description: "Represents the localized name used in the term store, which identifies the name in the localized language."
author: vishriv
localization_priority: Normal
ms.prod: "taxonomy"
doc_type: resourcePageType
---

# localizedName resource type

Namespace: microsoft.graph.termStore

Represents the localized name used in the term [store], which identifies the name in the localized language. For more information, see [localizedLabel].

## Properties
|Property|Type|Description|
|:---|:---|:---|
|languageTag|String|The language tag for the label.|
|name|String|The name in the localized language.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.termStore.localizedName"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.termStore.localizedName",
  "name": "String",
  "languageTag": "String"
}
```

[microsoft.graph.termStore.localizedLabel]: termstore-localizedlabel.md
[microsoft.graph.termstore.store]: termstore-store.md
[store]: ../resources/termstore-store.md
[localizedLabel]: ../resources/termstore-localizedlabel.md

<!--
{
  "type": "#page.annotation",
  "description": "TermLocalizedName is the facet for containing the name of termGroup",
  "keywords": "termLocalizedLNameFacet,facet,resource",
  "section": "documentation",
  "tocPath": "TermLocalizedNameFacet",
  "tocBookmarks": {
    "Resources/termStore.termLocalizedName": "#"
  },
  "suppressions": []
}
-->


