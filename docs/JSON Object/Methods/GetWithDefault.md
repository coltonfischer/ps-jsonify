---
title: GetWithDefault
parent: JSON Object Methods
grand_parent: JSON Object
nav_order: 150
---

### [](#header-3)Syntax

**GetWithDefault**(_name_, _default_)

### [](#header-3)Description

Use this method to return the property value mentioned by the name parameter from the JSON Object.  If no property is found by the given name, then this method will return the value provided in the default parameter.

### [](#header-3)Parameters

| Name           | Description                                                                    |
|:---------------|:-------------------------------------------------------------------------------|
| name           | Specifies the name of the property value as a string.                          |
| default        | Specifies the fallback value to return as a string.                            |


### [](#header-3)Returns

Any.

### [](#header-3)Example

```java
Local PSM_JSON:Object &oObject = create PSM_JSON:Object();
   
&oObject.AddString("user", "PS");

Local string &sUser = &oObject.GetWithDefault("user", %OperatorId);
```
