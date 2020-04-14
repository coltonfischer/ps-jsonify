---
title: SetException
parent: JSON Node Methods
grand_parent: JSON Node
nav_order: 20
---

### [](#header-3)Syntax

**SetException**(_exception_value_)

### [](#header-3)Description

Use this method to set the exception value of the JSON Node.

### [](#header-3)Parameters

| Name            | Description                                                                    |
|:----------------|:-------------------------------------------------------------------------------|
| exception_value | Specifies the exception value of the JSON Node as an Exception object.         |


### [](#header-3)Returns

None.

### [](#header-3)Example

```java
Local Exception &oException;
&oException = CreateException(0, 0, "An Error Occured");
   
Local PSM_JSON:Node &oNode = create PSM_JSON:Node();
   
&oNode.SetException(&oException);
```
