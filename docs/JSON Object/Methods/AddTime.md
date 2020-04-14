---
title: AddTime
parent: JSON Object Methods
grand_parent: JSON Object
nav_order: 130
---

### [](#header-3)Syntax

**AddTime**(_name_, _time_)

### [](#header-3)Description

Use this method to add a Time value to the JSON Object.

### [](#header-3)Parameters

| Name           | Description                                                                      |
|:---------------|:---------------------------------------------------------------------------------|
| name           | Specifies the name of the time that needs to be added as a string.               |
| time           | Specifies the time to add to the JSON Object as a Time type.                     |


### [](#header-3)Returns

None.

### [](#header-3)Example

```java
Local PSM_JSON:Object &oObject = create PSM_JSON:Object();
   
&oObject.AddTime("CurrentTime", %Time);
```
