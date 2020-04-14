---
title: AddNumber
parent: JSON Object Methods
grand_parent: JSON Object
nav_order: 90
---

### [](#header-3)Syntax

**AddNumber**(_name_, _number_)

### [](#header-3)Description

Use this method to add a Number value to the JSON Object.

### [](#header-3)Parameters

| Name           | Description                                                                      |
|:---------------|:---------------------------------------------------------------------------------|
| name           | Specifies the name of the number that needs to be added as a string.             |
| number         | Specifies the number to add to the JSON Object as a Number type.                 |


### [](#header-3)Returns

None.

### [](#header-3)Example

```java
Local PSM_JSON:Object &oObject = create PSM_JSON:Object();
   
&oObject.AddNumber("MyNbr", 7);
```
