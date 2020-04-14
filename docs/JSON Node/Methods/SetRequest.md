---
title: SetRequest
parent: JSON Node Methods
grand_parent: JSON Node
nav_order: 45
---

### [](#header-3)Syntax

**SetRequest**(_request_value_)

### [](#header-3)Description

Use this method to set the request value of the JSON Node.

### [](#header-3)Parameters

| Name            | Description                                                                    |
|:----------------|:-------------------------------------------------------------------------------|
| request_value   | Specifies the request value of the JSON Node as a Request object.              |


### [](#header-3)Returns

None.

### [](#header-3)Example

```java
Local PSM_JSON:Node &oNode = create PSM_JSON:Node();
   
&oNode.SetRequest(%Request);
```
