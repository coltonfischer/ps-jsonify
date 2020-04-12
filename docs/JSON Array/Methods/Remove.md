---
title: Remove
parent: JSON Array Methods
grand_parent: JSON Array
nav_order: 140
---

### [](#header-3)Syntax

**Remove**(_index_)

### [](#header-3)Description

Use this method to remove the element at the index location.

### [](#header-3)Parameters

| Name           | Description                                                                    |
|:---------------|:-------------------------------------------------------------------------------|
| index          | Specifies the index as an integer.                                             |


### [](#header-3)Returns

None.

### [](#header-3)Example

```java
Local PSM_JSON:Array &oArray = create PSM_JSON:Array();
   
&oArray.AddString("the");
&oArray.AddString("remove");
&oArray.AddString("test");
   
&oArray.Remove(1);
```
