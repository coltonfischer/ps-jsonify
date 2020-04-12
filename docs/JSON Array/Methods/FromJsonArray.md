---
title: FromJsonArray
parent: JSON Array Methods
grand_parent: JSON Array
nav_order: 5
---

### [](#header-3)Syntax

**FromJsonArray**(_json_array_)

### [](#header-3)Description

Use this method to populate the JSON Array from an existing JsonArray object.

### [](#header-3)Parameters

| Name           | Description                                              |
|:---------------|:---------------------------------------------------------|
| json_array     | Specifies the Json array as a JsonArray object.          |


### [](#header-3)Returns

None.

### [](#header-3)Example

```java
Local JsonArray &jaJson = CreateJsonArray();
   
/* Populate JsonArray ... */
   
Local PSM_JSON:Array &oArray = create PSM_JSON:Array();
&oArray.FromJsonArray(&jaJson);
```
