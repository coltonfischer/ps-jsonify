---
title: AddArray
parent: JSON Array Methods
grand_parent: JSON Array
nav_order: 15
---

### [](#header-3)Syntax

**AddArray**(_array_)

### [](#header-3)Description

Use this method to add an Array object to the JSON Array.

### [](#header-3)Parameters

| Name           | Description                                                        |
|:---------------|:-------------------------------------------------------------------|
| array          | Specifies the array to add to the JSON Array as an Array object.   |


### [](#header-3)Returns

None.

### [](#header-3)Example

```java
Local array of any &aaMyArray;
   
&aaMyArray = CreateArrayAny("test", True, 6, Null);
Local PSM_JSON:Array &oArray = create PSM_JSON:Array();
   
&oArray.AddArray(&aaMyArray);
```
