---
author: swapnil1993
ms.date: 08/30/2020
title: "Create a columnDefinition in a site"
description: "Create a site column."
localization_priority: Normal
doc_type: apiPageType
ms.prod: "sites-and-lists"
---

# Create a columnDefinition in a site
Namespace: microsoft.graph

Create a column for a [site][site] with a request that specifies a [columnDefinition][columnDefinition].

## Permissions

One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/concepts/permissions_reference.md).

  

|Permission type | Permissions (from least to most privileged) |
|:--------------------|:---------------------------------------------------------|
|Delegated (work or school account) | Sites.Manage.All, Sites.FullControl.All |
|Delegated (personal Microsoft account) | Not supported. |
|Application | Sites.Manage.All, Sites.FullControl.All |

  

## HTTP request

<!-- { "blockType": "ignored" } -->
```http
POST /sites/{site-id}/columns
```

## Request body

In the request body, supply a JSON representation of the [columnDefinition][] resource to add.  

## Response

If successful, this method returns a `201 Created` response code and [columnDefinition][] object in the response body.

## Example

### Request
<!-- { "blockType": "request", "name": "site_post_columns" } -->
```http
POST https://graph.microsoft.com/v1.0/sites/{site-id}/columns
Content-Type: application/json

{
   "description":"test",
   "enforceUniqueValues":false,
   "hidden":false,
   "indexed":false,
   "name":"Title",
   "text":{
      "allowMultipleLines":false,
      "appendChangesToExistingText":false,
      "linesForEditing":0,
      "maxLength":255
   }
}
```

### Response

<!-- { "blockType": "response", "@type": "microsoft.graph.columnDefinition", "truncated": true } -->

  

```http
HTTP/1.1 201 Created
Content-type: application/json

{
   "description":"test",
   "displayName":"Title",
   "enforceUniqueValues":false,
   "hidden":false,
   "id":"99ddcf45-e2f7-4f17-82b0-6fba34445103",
   "indexed":false,
   "name":"Title",
   "text":{
      "allowMultipleLines":false,
      "appendChangesToExistingText":false,
      "linesForEditing":0,
      "maxLength":255
   }
}
```

  

[columnDefinition]: ../resources/columnDefinition.md
[site]: ../resources/site.md
  

