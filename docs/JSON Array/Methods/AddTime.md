---
title: AddTime
parent: JSON Array Methods
grand_parent: JSON Array
nav_order: 130
---

### [](#header-3)Syntax

**AddTime**(_time_)

### [](#header-3)Description

Use this method to add a Time value to the JSON Array.

### [](#header-3)Parameters

| Name           | Description                                                                    |
|:---------------|:-------------------------------------------------------------------------------|
| time           | Specifies the time to add to the JSON Array as a Time type.                    |


### [](#header-3)Returns

None.

### [](#header-3)Example

```java
Local PSM_JSON:Array &oArray = create PSM_JSON:Array();
   
&oArray.AddTime(%Time);
```
