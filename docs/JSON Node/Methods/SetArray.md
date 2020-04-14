---
title: SetArray
parent: JSON Node Methods
grand_parent: JSON Node
nav_order: 10
---

### [](#header-3)Syntax

**SetArray**(_array_value_)

### [](#header-3)Description

Use this method to set the array value of the JSON Node.

### [](#header-3)Parameters

| Name           | Description                                                                    |
|:---------------|:-------------------------------------------------------------------------------|
| array_value    | Specifies the array value of the JSON Node as an Array object.                 |


### [](#header-3)Returns

None.

### [](#header-3)Example

```java
Local array of any &aaMyArray;
   
&aaMyArray = CreateArrayAny("test", True, 6, Null);
Local PSM_JSON:Node &oNode = create PSM_JSON:Node();
   
&oNode.SetArray(&aaMyArray);
```
