---
title: AddDate
parent: JSON Array Methods
grand_parent: JSON Array
nav_order: 35
---

### [](#header-3)Syntax

**AddDate**(_date_)

### [](#header-3)Description

Use this method to add a Date value to the JSON Array.

### [](#header-3)Parameters

| Name           | Description                                                                    |
|:---------------|:-------------------------------------------------------------------------------|
| date           | Specifies the date to add to the JSON Array as a Date type.                    |


### [](#header-3)Returns

None.

### [](#header-3)Example

```java
Local PSM_JSON:Array &oArray = create PSM_JSON:Array();
   
&oArray.AddDate(%Date);
```
