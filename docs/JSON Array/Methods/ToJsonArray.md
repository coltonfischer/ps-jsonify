---
title: ToJsonArray
parent: JSON Array Methods
grand_parent: JSON Array
nav_order: 155
---

### [](#header-3)Syntax

**ToJsonArray**()

### [](#header-3)Description

Use this method to return the JsonArray of the JSON Array.

### [](#header-3)Parameters

None.

### [](#header-3)Returns

JsonArray.

### [](#header-3)Example

```java
Local PSM_JSON:Array &oArray = create PSM_JSON:Array();
   
/* Populate JSON Array */
   
Local JsonArray &jaJson = &oArray.ToJsonArray();
```
