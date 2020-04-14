---
title: AddDateTime
parent: JSON Object Methods
grand_parent: JSON Object
nav_order: 40
---

### [](#header-3)Syntax

**AddDateTime**(_name_, _date_time_)

### [](#header-3)Description

Use this method to add a Datetime value to the JSON Object.

### [](#header-3)Parameters

| Name                | Description                                                                          |
|:--------------------|:-------------------------------------------------------------------------------------|
| name                | Specifies the name of the datetime that needs to be added as a string.               |
| date_time           | Specifies the datetime to add to the JSON Object as a Datetime type.                 |


### [](#header-3)Returns

None.

### [](#header-3)Example

```java
Local PSM_JSON:Object &oObject = create PSM_JSON:Object();
   
&oObject.AddDateTime("CurrentDate", %Datetime);
```
