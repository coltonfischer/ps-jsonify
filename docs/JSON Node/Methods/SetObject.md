---
title: SetObject
parent: JSON Node Methods
grand_parent: JSON Node
nav_order: 30
---

### [](#header-3)Syntax

**SetObject**(_object_)

### [](#header-3)Description

Use this method to set the object of the JSON Node.

### [](#header-3)Parameters

| Name            | Description                                                                    |
|:----------------|:-------------------------------------------------------------------------------|
| object          | Specifies the object of the JSON Node as an Object.                            |


### [](#header-3)Returns

None.

### [](#header-3)Example

```java
Local object &oValue = %Request;
   
If Int(Rand() * 10) > 5 Then
    &oValue = CreateArrayAny("test", True, 6, Null);
End-If;
   
Local PSM_JSON:Node &oNode = create PSM_JSON:Node();
   
&oNode.SetObject(&oValue);
```
