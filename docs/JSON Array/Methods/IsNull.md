---
title: IsNull
parent: JSON Array Methods
grand_parent: JSON Array
nav_order: 165
---

### [](#header-3)Syntax

**IsNull**(_index_)

### [](#header-3)Description

Use this method to check whether the JSON Array element at the index location is null.

Unexpected Results
{: .label .label-red }

### [](#header-3)Parameters

| Name           | Description                                                                    |
|:---------------|:-------------------------------------------------------------------------------|
| index          | Specifies the index in the JSON Array as an integer.                           |


### [](#header-3)Returns

Boolean.

### [](#header-3)Example

```java
Local PSM_JSON:Array &oArray = create PSM_JSON:Array();
   
&oArray.AddString("test");
   
Local boolean &bIsNull = &oArray.IsNull(1); /* Expected: False - Actual: True */
```
