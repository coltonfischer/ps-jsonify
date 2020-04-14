---
title: AddString
parent: JSON Object Methods
grand_parent: JSON Object
nav_order: 125
---

### [](#header-3)Syntax

**AddString**(_name_, _value_)

### [](#header-3)Description

Use this method to add a String value to the JSON Object.

### [](#header-3)Parameters

| Name           | Description                                                                      |
|:---------------|:---------------------------------------------------------------------------------|
| name           | Specifies the name of the string that needs to be added as a string.             |
| value          | Specifies the string to add to the JSON Object as a String type.                 |


### [](#header-3)Returns

None.

### [](#header-3)Example

```java
Local PSM_JSON:Object &oObject = create PSM_JSON:Object();
   
&oObject.AddString("MyString", "hello");
```
