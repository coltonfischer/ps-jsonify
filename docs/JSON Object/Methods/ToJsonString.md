---
title: ToJsonString
parent: JSON Object Methods
grand_parent: JSON Object
nav_order: 180
---

### [](#header-3)Syntax

**ToJsonString**()

### [](#header-3)Description

Use this method to return the String of the JSON Object.

### [](#header-3)Parameters

None.

### [](#header-3)Returns

String.

### [](#header-3)Example

```java
Local PSM_JSON:Object &oObject = create PSM_JSON:Object();
   
/* Populate JSON Object */
   
Local string &sJson = &oObject.ToJsonString();
```
