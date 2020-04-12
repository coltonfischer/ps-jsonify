---
title: ToJsonString
parent: JSON Array Methods
grand_parent: JSON Array
nav_order: 160
---

### [](#header-3)Syntax

**ToJsonString**()

### [](#header-3)Description

Use this method to return the String of the JSON Array.

### [](#header-3)Parameters

None.

### [](#header-3)Returns

String.

### [](#header-3)Example

```java
Local PSM_JSON:Array &oArray = create PSM_JSON:Array();
   
/* Populate JSON Array */
   
Local string &sJson = &oArray.ToJsonString();
```
