---
title: AddNull
parent: JSON Object Methods
grand_parent: JSON Object
nav_order: 85
---

### [](#header-3)Syntax

**AddNull**(_name_)

### [](#header-3)Description

Use this method to add a Null object to the JSON Object.

### [](#header-3)Parameters

| Name           | Description                                                                      |
|:---------------|:---------------------------------------------------------------------------------|
| name           | Specifies the name of the null object that needs to be added as a string.        |

### [](#header-3)Returns

None.

### [](#header-3)Example

```java
Local PSM_JSON:Object &oObject = create PSM_JSON:Object();
   
&oObject.AddNull("MyNull");
```
