---
title: AddBoolean
parent: JSON Array Methods
grand_parent: JSON Array
nav_order: 20
---

### [](#header-3)Syntax

**AddBoolean**(_bool_)

### [](#header-3)Description

Use this method to add a Boolean to the JSON Array.

### [](#header-3)Parameters

| Name           | Description                                                              |
|:---------------|:-------------------------------------------------------------------------|
| bool           | Specifies the boolean to add to the JSON Array as a Boolean data type.   |


### [](#header-3)Returns

None.

### [](#header-3)Example

```java
Local boolean &bIsBool = True;
   
Local PSM_JSON:Array &oArray = create PSM_JSON:Array();
   
&oArray.AddBoolean(&bIsBool);
```
