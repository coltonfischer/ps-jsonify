---
title: AddJsonArray
parent: JSON Object Methods
grand_parent: JSON Object
nav_order: 65
---

### [](#header-3)Syntax

**AddJsonArray**(_name_, _json_array_)

### [](#header-3)Description

Use this method to add a JsonArray to the JSON Object.

### [](#header-3)Parameters

| Name           | Description                                                                      |
|:---------------|:---------------------------------------------------------------------------------|
| name           | Specifies the name of the Json array that needs to be added as a string.         |
| json_array     | Specifies the Json array to add to the JSON Object as a JsonArray object type.   |


### [](#header-3)Returns

None.

### [](#header-3)Example

```java
Local JsonArray &jaJson = CreateJsonArray();
   
/* Populate Json Array ... */
   
Local PSM_JSON:Object &oObject = create PSM_JSON:Object();
   
&oObject.AddJsonArray("MyJsonArray", &jaJson);
```
