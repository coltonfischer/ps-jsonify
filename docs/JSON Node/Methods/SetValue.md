---
title: SetValue
parent: JSON Node Methods
grand_parent: JSON Node
nav_order: 55
---

### [](#header-3)Syntax

**SetValue**(_value_)

### [](#header-3)Description

Use this method to set the value of the JSON Node.

### [](#header-3)Parameters

| Name            | Description                                                                    |
|:----------------|:-------------------------------------------------------------------------------|
| value           | Specifies the value of the JSON Node as an Any type.                           |


### [](#header-3)Returns

None.

### [](#header-3)Example

```java
Local any &aValue = %Request;
   
If Int(Rand() * 10) > 5 Then
    &aValue = True;
End-If;
   
Local PSM_JSON:Node &oNode = create PSM_JSON:Node();
   
&oNode.SetValue(&aValue);
```
