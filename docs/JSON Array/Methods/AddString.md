---
title: AddString
parent: JSON Array Methods
grand_parent: JSON Array
nav_order: 125
---

### [](#header-3)Syntax

**AddString**(_value_)

### [](#header-3)Description

Use this method to add a String value to the JSON Array.

### [](#header-3)Parameters

| Name           | Description                                                                    |
|:---------------|:-------------------------------------------------------------------------------|
| value          | Specifies the string to add to the JSON Array as a String type.                |


### [](#header-3)Returns

None.

### [](#header-3)Example

```java
Local PSM_JSON:Array &oArray = create PSM_JSON:Array();
   
&oArray.AddString("hello");
```
