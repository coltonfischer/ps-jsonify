---
title: AddFloat
parent: JSON Object Methods
grand_parent: JSON Object
nav_order: 50
---

### [](#header-3)Syntax

**AddFloat**(_name_, _value_)

### [](#header-3)Description

Use this method to add a Float value to the JSON Object.

### [](#header-3)Parameters

| Name           | Description                                                                      |
|:---------------|:---------------------------------------------------------------------------------|
| name           | Specifies the name of the float that needs to be added as a string.              |
| value          | Specifies the float to add to the JSON Object as a Float type.                   |


### [](#header-3)Returns

None.

### [](#header-3)Example

```java
Local PSM_JSON:Object &oObject = create PSM_JSON:Object();
   
&oObject.AddFloat("MyFloat", 5.1234567);
```
