---
title: GetPropertyNameAt
parent: JSON Object Methods
grand_parent: JSON Object
nav_order: 160
---

### [](#header-3)Syntax

**GetPropertyNameAt**(_index_)

### [](#header-3)Description

Use this method to return the name of the property at the specified index in the JSON Object.

### [](#header-3)Parameters

| Name           | Description                                                                    |
|:---------------|:-------------------------------------------------------------------------------|
| index          | Specifies the index in the JSON Object as an Integer.                          |


### [](#header-3)Returns

String.

### [](#header-3)Example

```java
Local PSM_JSON:Object &oObject = create PSM_JSON:Object();
   
&oObject.AddString("one", "test");
   
Local string &sName = &oObject.GetPropertyNameAt(1);
```
