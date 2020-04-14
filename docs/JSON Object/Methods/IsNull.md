---
title: IsNull
parent: JSON Object Methods
grand_parent: JSON Object
nav_order: 165
---

### [](#header-3)Syntax

**IsNull**(_name_)

### [](#header-3)Description

Use this method to check whether a property is null or not.

Unexpected Results
{: .label .label-red }

### [](#header-3)Parameters

| Name           | Description                                                                    |
|:---------------|:-------------------------------------------------------------------------------|
| name           | Specifies the name of the property that needs to be checked as a string.       |


### [](#header-3)Returns

Boolean.

### [](#header-3)Example

```java
Local PSM_JSON:Object &oObject = create PSM_JSON:Object();
   
&oObject.AddString("test", "val");
   
Local boolean &bIsNull = &oObject.IsNull("test"); /* Expected: False - Actual: True */
```
