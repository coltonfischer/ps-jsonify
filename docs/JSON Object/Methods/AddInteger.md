---
title: AddInteger
parent: JSON Object Methods
grand_parent: JSON Object
nav_order: 60
---

### [](#header-3)Syntax

**AddInteger**(_name_, _value_)

### [](#header-3)Description

Use this method to add an Integer to the JSON Object.

### [](#header-3)Parameters

| Name           | Description                                                                      |
|:---------------|:---------------------------------------------------------------------------------|
| name           | Specifies the name of the integer that needs to be added as a string.            |
| value          | Specifies the integer to add to the JSON Object as an Integer data type.         |


### [](#header-3)Returns

None.

### [](#header-3)Example

```java
Local PSM_JSON:Object &oObject = create PSM_JSON:Object();
   
&oObject.AddInteger("MyInt", 2);
```
