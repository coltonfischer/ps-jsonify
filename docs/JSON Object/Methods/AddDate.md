---
title: AddDate
parent: JSON Object Methods
grand_parent: JSON Object
nav_order: 35
---

### [](#header-3)Syntax

**AddDate**(_name_, _date_)

### [](#header-3)Description

Use this method to add a Date value to the JSON Object.

### [](#header-3)Parameters

| Name           | Description                                                                      |
|:---------------|:---------------------------------------------------------------------------------|
| name           | Specifies the name of the date that needs to be added as a string.               |
| date           | Specifies the date to add to the JSON Object as a Date type.                     |


### [](#header-3)Returns

None.

### [](#header-3)Example

```java
Local PSM_JSON:Object &oObject = create PSM_JSON:Object();
   
&oObject.AddDate("CurrentDate", %Date);
```
