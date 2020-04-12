---
title: AddFloat
parent: JSON Array Methods
grand_parent: JSON Array
nav_order: 50
---

### [](#header-3)Syntax

**AddFloat**(_value_)

### [](#header-3)Description

Use this method to add a Float value to the JSON Array.

### [](#header-3)Parameters

| Name           | Description                                                                    |
|:---------------|:-------------------------------------------------------------------------------|
| value          | Specifies the float to add to the JSON Array as a Float type.                    |


### [](#header-3)Returns

None.

### [](#header-3)Example

```java
Local PSM_JSON:Array &oArray = create PSM_JSON:Array();
   
&oArray.AddFloat(5.1234567);
```
