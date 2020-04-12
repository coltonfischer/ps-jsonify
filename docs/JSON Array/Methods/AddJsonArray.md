---
title: AddJsonArray
parent: JSON Array Methods
grand_parent: JSON Array
nav_order: 65
---

### [](#header-3)Syntax

**AddJsonArray**(_json_array_)

### [](#header-3)Description

Use this method to add a JsonArray to the JSON Array.

### [](#header-3)Parameters

| Name           | Description                                                                  |
|:---------------|:-----------------------------------------------------------------------------|
| json_array     | Specifies the Json array to add to the JSON Array as a JsonArray data type.  |


### [](#header-3)Returns

None.

### [](#header-3)Example

```java
Local JsonArray &jaJson = CreateJsonArray();
   
/* Populate Json Array ... */
   
Local PSM_JSON:Array &oArray = create PSM_JSON:Array();
   
&oArray.AddJsonArray(&jaJson);
```
