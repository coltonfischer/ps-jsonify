---
title: HasKey
parent: JSON Object Methods
grand_parent: JSON Object
nav_order: 185
---

### [](#header-3)Syntax

**HasKey**(_name_)

### [](#header-3)Description

Use this method to check whether a property exists.

### [](#header-3)Parameters

| Name           | Description                                                                    |
|:---------------|:-------------------------------------------------------------------------------|
| name           | Specifies the name of the property that needs to be checked as a string.       |


### [](#header-3)Returns

Boolean.

### [](#header-3)Example

```java
Local PSM_JSON:Object &oObject = create PSM_JSON:Object();
   
&oObject.AddString("one", "test");
   
Local boolean &bExist = &oObject.HasKey("one");
```
