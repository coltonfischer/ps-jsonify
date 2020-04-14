---
title: AddBoolean
parent: JSON Object Methods
grand_parent: JSON Object
nav_order: 20
---

### [](#header-3)Syntax

**AddBoolean**(_name_, _bool_)

### [](#header-3)Description

Use this method to add a Boolean to the JSON Object.

### [](#header-3)Parameters

| Name           | Description                                                                      |
|:---------------|:---------------------------------------------------------------------------------|
| name           | Specifies the name of the boolean that needs to be added as a string.            |
| bool           | Specifies the boolean to add to the JSON Object as a Boolean data type.          |


### [](#header-3)Returns

None.

### [](#header-3)Example

```java
Local boolean &bIsBool = True;
   
Local PSM_JSON:Object &oObject = create PSM_JSON:Object();
   
&oObject.AddBoolean("MyBool", &bIsBool);
```
