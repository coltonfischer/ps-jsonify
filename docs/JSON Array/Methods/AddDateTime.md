---
title: AddDateTime
parent: JSON Array Methods
grand_parent: JSON Array
nav_order: 40
---

### [](#header-3)Syntax

**AddDateTime**(_date_time_)

### [](#header-3)Description

Use this method to add a Datetime value to the JSON Array.

### [](#header-3)Parameters

| Name           | Description                                                                    |
|:---------------|:-------------------------------------------------------------------------------|
| date_time      | Specifies the date time to add to the JSON Array as a Datetime type.           |


### [](#header-3)Returns

None.

### [](#header-3)Example

```java
Local PSM_JSON:Array &oArray = create PSM_JSON:Array();
   
&oArray.AddDateTime(%Datetime);
```
