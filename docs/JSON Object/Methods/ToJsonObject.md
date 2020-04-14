---
title: ToJsonObject
parent: JSON Object Methods
grand_parent: JSON Object
nav_order: 175
---

### [](#header-3)Syntax

**ToJsonObject**()

### [](#header-3)Description

Use this method to return the JsonObject of the JSON Object.

### [](#header-3)Parameters

None.

### [](#header-3)Returns

JsonObject.

### [](#header-3)Example

```java
Local PSM_JSON:Object &oObject = create PSM_JSON:Object();
   
/* Populate JSON Object */
   
Local JsonObject &jaJson = &oObject.ToJsonObject();
```
