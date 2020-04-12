---
title: Pop
parent: JSON Array Methods
grand_parent: JSON Array
nav_order: 135
---

### [](#header-3)Syntax

**Pop**()

### [](#header-3)Description

Use this method to remove the last element in the JSON Array.

### [](#header-3)Parameters

None.

### [](#header-3)Returns

None.

### [](#header-3)Example

```java
Local PSM_JSON:Array &oArray = create PSM_JSON:Array();
   
&oArray.AddString("pop");
&oArray.AddString("test");
   
&oArray.Pop();
```
