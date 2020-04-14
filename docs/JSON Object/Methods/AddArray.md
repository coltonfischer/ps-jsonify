---
title: AddObject
parent: JSON Object Methods
grand_parent: JSON Object
nav_order: 15
---

### [](#header-3)Syntax

**AddArray**(_name_, _array_)

### [](#header-3)Description

Use this method to add an Array object to the JSON Object.

### [](#header-3)Parameters

| Name           | Description                                                                      |
|:---------------|:---------------------------------------------------------------------------------|
| name           | Specifies the name of the array that needs to be added as a string.              |
| array          | Specifies the array to add to the JSON Object as an Array object.                |


### [](#header-3)Returns

None.

### [](#header-3)Example

```java
Local array of any &aaMyArray;
   
&aaMyArray = CreateArrayAny("test", True, 6, Null);
Local PSM_JSON:Object &oObject = create PSM_JSON:Object();
   
&oObject.AddArray("MyArray", &aaMyArray);
```
